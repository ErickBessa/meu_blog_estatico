---
url: "/como-gerencio-meus-projetos-no-github/"
summary: "Como gerencio meus projetos no github"
author: Erick Bessa
draft: False
title: "Como gerencio meus projetos no github"
date: 2023-01-30T19:40:30-03:00
---

Olá, galera.

Sou desenvolvedor backend com mais de 3 anos de experiência.

Em boa parte da minha carreira, sempre procurei manter meus códigos no github de forma organizada e bem documentada, seja para recapitulação/reprodução futura ou por uma necessidade de negócios (projetos freelances). Pois bem, durante esse processo além de documentar, fui aprendendo as formas de gerenciar um projeto, pessoal ou não, pequeno ou grande, e nesse artigo vou compartilhar um pouco desses aprendizados com vocês.


## Como inicío o projeto

No início do projeto, costumo fazer a quantidade mínima de código na máquina para depois criar um repo no github. Esse mínimo pode ser um `HelloWorld` em qualquer linguagem. 

No projeto adiciono os arquivos `.gitignore`, `REAME.md` e `LICENSE.md` (caso for um projeto para comunidade), 
logo em seguida crio meu repositório no github e sincronizo com o projeto da minha máquina local.


## Como gerencio branchs

Uma boa prática para a se considerar é não fazer commit direto na branch `master/main`, portanto crio uma branch `develop` e trabalho sempre nela, pedindo _merge request_ da `develop` para a `master` a cada alteração importante de código.

Outra maneira de gerenciar branchs é criar uma para cada `fix`,`feat` ou `issue` que adicionarmos ao projetos. Por exemplo:

- adicionar botão na homepage - 
`branch: <feat> add button in homepage`

Depois que essa funcionalidade está pronta, peço o _merge request_ da branch `<feat> add button in homepage` para a `master`.

## Como gerencio tarefas
Para as tarefas a serem feitas, gosto de criar uma _issue_ com _checkbox_ para cada tarefa, sempre em ordem de prioridade para facilitar:

![Minhas issues](./images/3/issues.png#center)

Dessa forma consigo controlar o que tem que ser feito, principalmente quando é um projeto _freelancer_ que tem muita demanda.

Quando encontro um _bug_ ou preciso criar uma nova _feature_, cadastro uma _issue_ e atríbuo uma identificação à ela do tipo `warning`, `bug` ou `feat`:

![Minhas issues](./images/3/labels.png#center)

Obs.: Podemos criar uma _branch_ para resolver cada _issue_.

## Como escrevo minhas mensagens de commits
Gosto de seguir a [convenção de commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/) para ter commits mais padronizados.

- Para commit de incremento de _feature_: `<feat> commit message`.

- Para correção de _bug_:  `<fix> commit message`.

- Para refatoração: `<refactor> commit message`.

# Conclusão
Minha intenção aqui era passar uma idéia básica de como pode ser feito o gerenciamento de projetos pessoais/profissionais no gitub com base na minha experiência. Elas podem ser adaptadas a cada necessidade.

Obrigado por ter lido até aqui, abraços.
