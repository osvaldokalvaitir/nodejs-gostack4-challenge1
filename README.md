# Node - Desafio 1

Aplicação usando Node.js, Express, Nunjucks, EditorConfig e ESLint.

## Desafio

Nesse desafio vamos construir uma aplicação que aceita a entrada de um campo do usuário por um formulário e o redireciona para a página correta baseado em sua idade.

Configure uma aplicação utilizando **ExpressJS, Nunjucks, EditorConfig e ESLint**.

### Rotas

- `/`: Rota inicial que renderiza uma página com um formulário com um único campo `age` que representa a idade do usuário;
- `/check`: Rota chamada pelo formulário da página inicial via método POST que checa se a idade do usuário é maior que 18 e o redireciona para a rota `/major`, caso contrário o redireciona para a rota `/minor` (Lembre de enviar a idade como Query Param no redirecionamento);
- `/major`: Rota que renderiza uma página com o texto: `Você é maior de idade e possui x anos`, onde `x` deve ser o valor informado no input do formulário;
- `/minor`: Rota que renderiza uma página com o texto: `Você é menor de idade e possui x anos`, onde `x` deve ser o valor informado no input do formulário;

### Middlewares

Deve haver um middleware que é chamado nas rotas `/major` e `/minor` e checa se a informação de idade não está presente nos Query Params. Se essa informação não existir deve redirecionar o usuário para a página inicial com o formulário, caso contrário o middleware deve apenas continuar com o fluxo normal.

## Resumo

Esta aplicação foi desenvolvida para realizar a checagem de idade informada pelo usuário.

## Índice

- [Telas](#telas)

  - [Principal](#main)

  - [Maior](#major)

  - [Minor](#minor)

- [Desenvolvimento](#desenvolvimento)

  - [Configurações Iniciais](#configurações-iniciais)

  - [Instalação do Projeto](#instalação-do-projeto)

  - [Execução do Projeto](#execução-do-projeto)

  - [Bibliotecas](#bibliotecas)

## Telas

### Principal

![Screenshoot Main](https://github.com/osvaldokalvaitir/node-desafio1/blob/master/screenshots/Main.png)
Esta é a tela principal onde o usuário informa a idade para a checagem.

### Maior

![Screenshoot Major](https://github.com/osvaldokalvaitir/node-desafio1/blob/master/screenshots/Major.png)
Esta tela aparecerá se a idade informada for maior que 18 anos.

### Menor

![Screenshoot Minor](https://github.com/osvaldokalvaitir/node-desafio1/blob/master/screenshots/Minor.png)
Esta tela aparecerá se a idade informada for menor ou igual à 18 anos.

## Desenvolvimento

### Configurações Iniciais

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/README.md) e siga as Configurações Iniciais.

### Instalação do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga a Instalação de Projeto.

### Execução do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga a Execução de Projeto.

### Bibliotecas

- [ESLint](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/eslint.md)

- [Express](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express.md)

- [Nodemon](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemon.md)

- [Nunjucks](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nunjucks.md)
