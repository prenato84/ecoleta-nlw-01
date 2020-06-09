<h3 align="center">
    <img alt="Logo" title="#logo" width="300px" src="logo.png">
    <br><br>
    <b>Recycle! Help the environment!</b>  
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

# Index

- [About](#sobre)
- [Technologies Used](#tecnologias-utilizadas)
- [How to Run](#como-usar)
- [How to Contribute](#como-contribuir)

<a id="sobre"></a>

## :bookmark: About

O <strong>Ecoleta</strong> é uma aplicação Web e Mobile para ajudar pessoas a encontrarem pontos de coleta para reciclagem.

Essa aplicação foi construída na trilha <strong>Booster</strong> da <strong>Next Level Week</strong> distribuída pela [Rocketseat](https://rocketseat.com.br/). A ideia de criar uma aplicação voltada ao meio ambiente surgiu da coincidência da data do curso e a data da <strong>semana do meio ambiente</strong>.

<a id="tecnologias-utilizadas"></a>

## :rocket: Technologies Used

The project was developed with the following technologies:

- [TypeScript](https://www.typescriptlang.org/)
- [Node.js](https://nodejs.org/en/)
- [ReactJS](https://reactjs.org/)
- [React Native](https://reactnative.dev/)

## :heavy_check_mark: :computer: Web Frontend

- The layout is avaiable at **[Figma](https://www.figma.com/file/1SxgOMojOB2zYT0Mdk28lB/)**.

<h1 align="center">
    <img alt="Web" src="Video.gif" width="900px">
</h1>

## :heavy_check_mark: :iphone: Mobile App

<h1 align="center">
    <img alt="Mobile Home" src="Home.png" width="300px">
    <img alt="Mobile Detail" src="Detail.svg" width="300px">
</h1>

<a id="como-usar"></a>

## :fire: How to Run

- ### **Requirements**

  - You **must have** **[Node.js](https://nodejs.org/en/)** installed on your machine;
  - You **must have** a package manager, either **[NPM](https://www.npmjs.com/)** or **[Yarn](https://yarnpkg.com/)**. Quick note: NPM is already installed with Node.js;
  - Finally, it is **essential** to have **[Expo](https://expo.io/)** installed globally on the machine and its client installed on your cell phone or emulator **[iOS App](https://itunes.apple.com/app/apple-store/id982107779)** or **[Android App](https://play.google.com/store/apps/details?id=host.exp.exponent&referrer=www)**.

1. Clone this repository :

```sh
  $ git clone https://github.com/prenato84/ecoleta-nlw-01
```

2. Running the Application:

```sh
  # Install the dependencies
  $ npm install

  ## Create the database
  $ cd server
  $ npm run knex:migrate
  $ npm run knex:seed

  # Start the API
  $ npm run dev

  # Start the Web Frontend
  $ cd web
  $ npm start

  # Start the Mobile Frontend
  $ cd mobile
  $ npm start
```

:exclamation: **NOTE:** for the mobile frontend to be able to communicate correctly with the backend (server), it is necessary to replace **localhost** with the local IP of your machine on both controllers:

1. Access the folder **server/src/controllers**;
2. In **ItemsController.ts** and using IP 192.168.0.10 as an example, change the **image_url** property:

```javascript
image_url: `http://192.168.0.10:3333/uploads/...`;
```

3. In **PointsController.ts** and using IP 192.168.0.10 as an example, change the **image_url** property:

```javascript
image_url: `http://192.168.0.10:3333/uploads/...`;
```

<a id="como-contribuir"></a>

## :recycle: How to Contribute

- Fork this repository,
- Make a new branch with your feature: `git checkout -b my-feature`
- Commit your changes: `git commit -m 'feat: My new feature'`
- Push your branch: `git push origin my-feature`

## :mortar_board: Who was the instructor?

The classes were taught by Rocketseat's CTO **[Diego Fernandes](https://github.com/diego3g)** during **Next Level Week**.

## :memo: License

This project is under MIT License. Check this file [LICENSE](LICENSE.md) for more information.

---

<h4 align="center">
    Made with love 💜 by <a href="https://www.linkedin.com/in/prenato84/" target="_blank">Paulo Castro</a>
</h4>
