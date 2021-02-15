# Formulários

> Boas práticas para validação de formulários.

Uma das boas praticas para criar formulários sólidos é o uso das máscaras. As máscaras induzem os usuários a inputar tipos e formatos de dados.

## Máscaras

Usamos o [**jquery.mask.min.js**](https://github.com/igorescobar/jQuery-Mask-Plugin/tree/master/dist) para criar máscaras nos formulários de _aplicações web_. Um exemplo simples é a máscara de input do CPF:

```html
<input type="text" class="input-cpf">
```

```javascript
<script>
    $(document).ready(function(){
        $(".input-cpf").mask("000.000.000-00");
    });
</script>
```

É válido notar que usamos o **seletor CSS** para criar essa máscara. Pois, em alguns casos, o mesmo fomulário é renderizado **diversas vezes em uma mesma página**.

Pra mais, veja [jQuery-Mask-Plugin/docs](https://igorescobar.github.io/jQuery-Mask-Plugin/docs.html).
