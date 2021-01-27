# GIT

## Como usar git flow?

![Git flow](https://i2.wp.com/lanziani.com/slides/gitflow/images/gitflow_1.png)

O GitFlow é uma ideia abstrata para gerenciamento de branches utilizando Git. Ele auxilia a como deve ser criada as branches, e como mergea-las.
No windows, a instalação base do Git vem com o comando *git flow*, que permite determinar o fluxo no repositório. A única diferença dele para o git init, é que ele cria e delimita nomes para branches específicas.
Em sistemas OSX, ele pode ser instalado via brew, com o comando *brew install git-flow*

### Como funciona

#### Master e Develop branches

A combinação entre as duas branches, permite manter um histórico de versões. A master é a branch de produção, e onde é lançada as tags de versões. A develop é uma branch de integração com as features, ela é criada a partir da master, e todas as próximas features são mergeadas nela.

#### Feature Branches

Uma branch feature é criada a partir da última develop, e quando é finalizada, é mergeada novamente na develop e deletada. Feature branches nunca interagem diretamente com a master.

#### Release Branches

Quando a develop está pronta para ir para homologação, é criada uma release a partir dela. Na branch release criada, é realizada conserto de bugs, documentação, melhorias, qualquer solicitação nos testes realizados pelo QA.
Após finalizada e testada, é mergeada com a master e a develop, criando uma nova tag de versão na master e depois deletada.

#### Hotfix Branches

A hotfix branch são para resolver erros ocorridos em produção, ela é criada diretamente a partir da master, assim que resolvido, é mergeado a master e develop (ou release se estiver ativa ainda). Adicionando também uma nova tag de versão a master.

### Resumo geral

O fluxo geral do Gitflow é:

- develop branch é criada a partir do master
- release branch é criada a partir de develop
- feature branches são criadas a partir da develop
- Quando uma release é concluída, ela é mesclado com a develop branch
- Quando a release é concluída, ele é mesclado com o develop e a master
- Se um problema na master for detectado, um branch de hotfix é criado a partir da master
- Assim que o hotfix for concluído, ele é mesclada para develop e master

### Links

- [Atlassian gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)
- [Git flow repo](https://danielkummer.github.io/git-flow-cheatsheet/index.pt_BR.html)
- [Git flow na pratica](https://www.youtube.com/watch?v=wzxBR4pOTTs&t=82s)

## Como escrever commit?

| Commit Type | Title                    | Description                                                                                                 | Emoji  |
| ----------- | ------------------------ | ----------------------------------------------------------------------------------------------------------- |:------:|
| `feat`      | Features                 | A new feature                                                                                               | ✨     |
| `fix`       | Bug Fixes                | A bug Fix                                                                                                   | 🐛     |
| `docs`      | Documentation            | Documentation only changes                                                                                  | 📚     |
| `style`     | Styles                   | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)      | 💎     |
| `refactor`  | Code Refactoring         | A code change that neither fixes a bug nor adds a feature                                                   | 📦     |
| `perf`      | Performance Improvements | A code change that improves performance                                                                     | 🚀     |
| `test`      | Tests                    | Adding missing tests or correcting existing tests                                                           | 🚨     |
| `build`     | Builds                   | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)         | 🛠     |
| `ci`        | Continuous Integrations  | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) | ⚙️     |
| `chore`     | Chores                   | Other changes that don't modify src or test files                                                           | ♻️     |
| `revert`    | Reverts                  | Reverts a previous commit                                                                                   | 🗑

