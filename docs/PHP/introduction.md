# PHP

> Guia de estilos de código para PHP e seus frameworks.

## Geral

### Laravel Error - Specified key was too long error

#### Problema

Quando rodando versões antigas do Maria ou do MySql - antes da versão 5.7.7 -, o erro é disparado no console do Laravel na tentativa de popular o banco com migration.

```php
   [Illuminate\Database\QueryException]
   SQLSTATE[42000]: Syntax error or access violation: 1071 Specified key was too long; max key length is 767 bytes (SQL: alter table users add unique users_email_unique(email))

   [PDOException]
   SQLSTATE[42000]: Syntax error or access violation: 1071 Specified key was too long; max key length is 767 bytes
```

#### Solução

Para solucionar, deve ser editado o arquivo de boot dos serviços do laravel, dentro da pasta provider, *AppServiceProvider.php*, na função *boot()*.

```php
  use Illuminate\Support\Facades\Schema;

  public function boot()
  {
      Schema::defaultStringLength(191);
  }
```

Onde é determinado o tamanho padrão dos tipos string do banco de dados.

## Laravel

### Como definir nome de rotas?

Segue exemplo abaixo, para uma rota chamada **users**.

- [GET] - users/
- [GET] - users/create
- [GET] - users/{id}
- [GET] - users/{id}/edit
- [POST] - users/
- [PUT] - users/{id}
