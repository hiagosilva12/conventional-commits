# GitFlow

O GitFlow é uma metodologia de gerenciamento de branch que ajuda a equipe a gerenciar o desenvolvimento de software de maneira organizada e eficiente. Ele define as seguintes branches:

## Branches principais

- `master`: branch principal que contém a versão mais estável do software.

- `develop`: branch de desenvolvimento principal que contém o código em desenvolvimento.

## Branches secundárias

- `feat`: branches usadas para desenvolver novas funcionalidades.

- `release`: branches usadas para preparar uma versão para liberação.

- `hotfix`: branches usadas para corrigir problemas críticos na versão mais recente do software.

- `fix`: branches usadas para corrigir problemas não críticos na versão mais recente do software.

## Fluxo de trabalho

- Crie uma nova branch de feat a partir da branch develop.

- Desenvolva e teste a nova funcionalidade na branch de feat.

- Mescle a branch de feat de volta para a branch develop.

- Crie uma nova branch de release a partir da branch develop quando estiver pronto para lançar uma nova versão.

- Teste a nova versão na branch de release e corrija quaisquer problemas encontrados.

- Mescle a branch de release de volta para a branch develop e master.

- Crie uma nova branch de hotfix a partir da branch master se for necessário corrigir um problema crítico.

- Corrija o problema na branch de hotfix e mescle de volta para as branches develop e master.

## Coventional Commits

O Conventional Commits é um padrão para mensagens de commit que ajuda a equipe a entender o que foi feito em cada commit. Ele define as seguintes mensagens de commit:

Para implementar um novo recurso, usa-se o prefixo feat:

```html
git commit -m "feat: msg do que vc implementou"
```

Para corrigir um BUG, usa-se o prefixo fix:

```html
git commit -m "fix: msg do bug que vc corrigiu"
```

Para situações de refatoração, usa-se o prefixo refactor:

```html
git commit -m "refactor: msg explicando sua refatoração"
```

Para melhorar o desempenho, usa-se o prefixo perf:

```html
git commit -m "perf: msg explicando sua melhoria de desempenho"
```

Para trabalhar na parte visual, usa-se o prefixo style:

```html
git commit -m "style: msg explicando sua alteração visual"
```

Para implementar testes, usa-se o prefixo test:

```html
git commit -m "test: msg referente aos testes implementados"
```

Para documentar, usa-se o prefixo docs:

```html
git commit -m "docs: msg refertente a sua documentação"
```

Para tudo que envolve compilação, usa-se o prefixo build:

```html
git commit -m "build: msg sobre a situação de compilação abordada"
```

Para tudo que envolve o ambiente operacional, usa-se o prefixo ops:

```html
git commit -m "ops: msg abordando a situação de ambiente"
```

Para situações extras, por exemplo, alteração de .gitignore, usa-se o prefixo chore:

```html
git commit -m "chore: msg explicando a situação extra modificada"
```

Para indicar uma reversão de um commit anterior, usa-se o prefixo revert:

```html
git commit -m "revert: msg explicando a reversão"
```

Para alteração de arquivo de configuração, usa-se o prefixo ci:

```html
git commit -m "ci: msg explicando a alteração de configuração"
```
