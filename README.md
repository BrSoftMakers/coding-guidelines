# Coding Guidelines - Softmakers

[![NPM](https://img.shields.io/npm/v/docsify-themeable.svg?style=flat-square)](https://www.npmjs.com/package/docsify-themeable)
[![Codacy grade](https://img.shields.io/codacy/grade/860d40719cbd4e0f91e145b87ec7c29a.svg?style=flat-square)](https://www.codacy.com/app/jhildenbiddle/docsify-themeable?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jhildenbiddle/docsify-themeable&amp;utm_campaign=Badge_Grade)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://github.com/jhildenbiddle/docsify-themeable/blob/master/LICENSE)
[![jsDelivr](https://data.jsdelivr.com/v1/package/npm/docsify-themeable/badge)](https://www.jsdelivr.com/package/npm/docsify-themeable)

## Sobre o projeto

A ideia geral e buscar definir padrões para as equipes. Seja padrões de estilos de código, arquitetura de determinado framework, ou soluções para problemas comuns nas línguagens e/ou frameworks.

### Sobre o tema

O tema Docsify é um sistema de tema simples para [docsify.js](docsify.js.org). Apresenta vários temas com opções de personalização ricas, uma experiência de desktop e móvel aprimorada e suporte a navegador legado (IE10 +).

> Links abaixo da página do tema e um preview

- [Homepage](https://jhildenbiddle.github.io/docsify-themeable) - Live demo, documentation, and theme previews
- [Demo Sandbox](https://codesandbox.io/s/xv36w4695o) - Online editor with demo docsify-themeable site

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

Exemplo: `docs/NODEJS/introduction.md`

Após criado o arquivo, deve ser adicionado no header lateral do projeto, que fica no arquivo:

`docs/sidebar.md`

Após feita a alteração, solicitar pull request, para a branch main.

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte a [LICENSE](https://github.com/BrSoftMakers/coding-guidelines/blob/main/LICENSE) para obter detalhes.

Projeto criado baseado no docsify do Copyright (c) John Hildenbiddle ([@jhildenbiddle](https://twitter.com/jhildenbiddle))

