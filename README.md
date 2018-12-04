# Node - Desafio 1

![GitHub last commit](https://img.shields.io/github/last-commit/google/skia.svg)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/badges/shields.svg)
![GitHub repo size in bytes](https://img.shields.io/github/repo-size/badges/shields.svg)
![GitHub top language](https://img.shields.io/github/languages/top/badges/shields.svg)
![GitHub language count](https://img.shields.io/github/languages/count/badges/shields.svg)
![David](https://img.shields.io/david/osvaldokalvaitir/node-desafio1.svg)

Nesse desafio vamos construir uma aplicação que aceita a entrada de um campo do usuário por um formulário e o redireciona para a página correta baseado em sua idade.

Configure uma aplicação utilizando **ExpressJS, Nunjucks, EditorConfig e ESLint**.

## Rotas

- `/`: Rota inicial que renderiza uma página com um formulário com um único campo `age` que representa a idade do usuário;
- `/check`: Rota chamada pelo formulário da página inicial via método POST que checa se a idade do usuário é maior que 18 e o redireciona para a rota `/major`, caso contrário o redireciona para a rota `/minor` (Lembre de enviar a idade como Query Param no redirecionamento);
- `/major`: Rota que renderiza uma página com o texto: `Você é maior de idade e possui x anos`, onde `x` deve ser o valor informado no input do formulário;
- `/minor`: Rota que renderiza uma página com o texto: `Você é menor de idade e possui x anos`, onde `x` deve ser o valor informado no input do formulário;

## Middlewares

Deve haver um middleware que é chamado nas rotas `/major` e `/minor` e checa se a informação de idade não está presente nos Query Params. Se essa informação não existir deve redirecionar o usuário para a página inicial com o formulário, caso contrário o middleware deve apenas continuar com o fluxo normal.
