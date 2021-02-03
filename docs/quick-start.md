# Quick Start

## Como rodar o projeto?

A visualização de seu site localmente requer veicular seus arquivos de um servidor da web.

O guia de início rápido do docsify recomenda docsify-cli para criar e visualizar seu site:

**instale docsify-cli globalmente**

```bash
npm install -g docsify-cli
```

**Serve diretório atual**

```bash
docsify serve
```

**Serve o diretório ./docs**

```bash
docsify serve docs
```

### Como contribuir?

Deve ser criado uma nova branch a partir da develop. E depois adicinar a feature da sessão que quer ser criada, por exemplo, `feature/nodejs#1`.

Dentro da pasta `docs`, estão todos os guides criados atualmente. Com cada pasta com seu devido título.
Deve ser criada a pasta - ou se já existir, ignorar este passo -, depois criar o arquivo markdown dentro do mesmo.

Exemplo: `docs/NODEJS/index.md`

Após criado o arquivo, deve ser adicionado no header lateral do projeto, que fica no arquivo:

`docs/sidebar.md`

Após feita a alteração, solicitar pull request, para a branch main.
