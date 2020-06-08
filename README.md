<h3 align="center">
    <img alt="Logo" title="#logo" width="300px" src=".github/logo.png">
    <br><br>
    <b>Recicle! ajude o meio ambiente!</b>  
    <br>
</h3>

<p align="center">
  <a href="https://rocketseat.com.br">
    <img alt="Made by Rocketseat" src="https://img.shields.io/badge/made%20by-Rocketseat-%237519C1">
  </a>
  <a>
  <img alt="License" src="https://img.shields.io/github/license/vitorserrano/ecoleta?color=%237519C1">
  <br><br>
  <a href="https://insomnia.rest/run/?label=Ecoleta&uri=https%3A%2F%2Fraw.githubusercontent.com%2Fvitorserrano%2Fecoleta%2Fmaster%2F.github%2FInsomnia_2020-06-05.json" target="_blank"><img src="https://insomnia.rest/images/run.svg" alt="Run in Insomnia"></a>
</p>

# Índice

- [Sobre](#sobre)
- [Documentação](#documentacao)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Como Usar](#como-usar)
- [Como Contribuir](#como-contribuir)

<a id="sobre"></a>

## :bookmark: Sobre

O <strong>Ecoleta</strong> é uma aplicação Web e Mobile para ajudar pessoas a encontrarem pontos de coleta para reciclagem.

Essa aplicação foi construída na trilha <strong>Booster</strong> da <strong>Next Level Week</strong> distribuída pela [Rocketseat](https://rocketseat.com.br/). A ideia de criar uma aplicação voltada ao meio ambiente surgiu da coincidência da data do curso e a data da <strong>semana do meio ambiente</strong>.

<a id="documentacao"></a>

## :books: Documentação

Para reforçar alguns conceitos e registrar comandos que são dificeis de se lembrar, segue uma pequena **[DOCUMENTAÇÃO](DOCUMENTATION.md)** feita por [Vitor Serrano](https://github.com/vitorserrano) para ajudar quem está iniciando com **TypeScript**, **Node**, **ReactJS** e **React Native**.

<a id="tecnologias-utilizadas"></a>

## :rocket: Tecnologias Utilizadas

O projeto foi desenvolvido utilizando as seguintes tecnologias:

- [TypeScript](https://www.typescriptlang.org/)
- [Node.js](https://nodejs.org/en/)
- [ReactJS](https://reactjs.org/)
- [React Native](https://reactnative.dev/)

## :heavy_check_mark: :computer: Resultado Web

- O layout está disponível no **[Figma](https://www.figma.com/file/1SxgOMojOB2zYT0Mdk28lB/)**.

<h1 align="center">
    <img alt="Web" src=".github/Video.gif" width="900px">
</h1>

## :heavy_check_mark: :iphone: Resultado Mobile

<h1 align="center">
    <img alt="Mobile Home" src=".github/Home.png" width="300px">
    <img alt="Mobile Detail" src=".github/Detail.svg" width="300px">
</h1>

<a id="como-usar"></a>

## :fire: Como usar

- ### **Pré-requisitos**

  - É **necessário** possuir o **[Node.js](https://nodejs.org/en/)** instalado na máquina;
  - É **preciso** ter um gerenciador de pacotes, seja o **[NPM](https://www.npmjs.com/)** ou **[Yarn](https://yarnpkg.com/)**. Lembrando que o NPM já vem instalado com o Node.js;
  - Por fim, é **essencial** ter o **[Expo](https://expo.io/)** instalado de forma global na máquina e o cliente dele instalado em seu celular ou emulador **[iOS App](https://itunes.apple.com/app/apple-store/id982107779)** ou **[Android App](https://play.google.com/store/apps/details?id=host.exp.exponent&referrer=www)**.

1. Faça um clone :

```sh
  $ git clone https://github.com/prenato84/ecoleta-nlw-01
```

2. Executando a Aplicação:

```sh
  # Instale as dependências
  $ npm install

  ## Crie o banco de dados
  $ cd server
  $ npm run knex:migrate
  $ npm run knex:seed

  # Inicie a API
  $ npm run dev

  # Inicie a aplicação web
  $ cd web
  $ npm start

  # Inicie a aplicação mobile
  $ cd mobile
  $ npm start
```

:exclamation: **OBS:** para que o frontend mobile consiga se comunicar corretamente com o backend (server), é preciso substituir **localhost** pelo IP local de sua máquina nas duas controllers:

1. Acesse a pasta **server/src/controllers**;
2. Em **ItemsController.ts** e utilizando como exemplo o IP 192.168.0.10, altere a propriedade **image_url**:

```javascript
image_url: `http://192.168.0.10:3333/uploads/...`;
```

3. Em **PointsController.ts** e utilizando como exemplo o IP 192.168.0.10, altere a propriedade **image_url**:

```javascript
image_url: `http://192.168.0.10:3333/uploads/...`;
```

<a id="como-contribuir"></a>

## :recycle: Como contribuir

- Faça um Fork desse repositório,
- Crie uma branch com a sua feature: `git checkout -b my-feature`
- Commit suas mudanças: `git commit -m 'feat: My new feature'`
- Push a sua branch: `git push origin my-feature`

## :mortar_board: Quem ministrou?

As aulas foram ministradas pelo CTO da Rocketseat **[Diego Fernandes](https://github.com/diego3g)** nas aulas da **Next Level Week**.

## :memo: License

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

---

<h4 align="center">
    Feito com 💜 by <a href="https://www.linkedin.com/in/prenato84/" target="_blank">Paulo Castro</a>
</h4>
