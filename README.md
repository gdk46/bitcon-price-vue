<h1 align="center">
    <a href="#"> Bitcon price vue</a>
</h1>
<p align="center">:money_with_wings: Acompanhe a cotação do bitcon </p>
<p align="center">
<img src="https://img.shields.io/static/v1?label=framework&message=Vue&color=4FC08D&style=for-the-badge&logo=vue.js"/>
</p>
<p align="center">
<img src="https://img.shields.io/badge/license-MIT-blue"/>
<img src="https://img.shields.io/badge/npm-v16.13.1-blue"/>
<img src="https://img.shields.io/badge/contribution-welcome-green"/>
<img src="https://img.shields.io/badge/status project-close-red"/>
</p>

Índice
=================
<!--ts-->
* [Sobre](#sobre)
* [Screens](#screens)
* [Estrutura de pasta](#estrutura-de-pasta)
    * [Camadas da arquitetura](#camadas-da-arquitetura)
* [Instalação](#instalacao)
* [Como usar](#como-usar)
    * [Pre Requisitos](#pre-requisitos)
* [Tecnologias](#tecnologias)
* [Features](#features)
* [License](#license)
<!--te-->


## 🏁Sobre
Este aplicativo foi desenvolvido com Vue 3 com intuito de apredizagem.

## :framed_picture: Screens
<p align="center">
<img src="./preview.png"/>
</p>

## Estrutura de pastas
<pre>
Projeto/
├── app/
│   └── src
│       ├── router
│       ├── view
│       ├── components
│       └── assets
└── *
</pre>

### Camadas da arquitetura
pasta | camada | responsabilidade
------ | ------ | ------
router | view controller | caminhos para views
view | views | camada de visão
components | views | camada por agrupar todos pequenos components usados no sistema
assets | resources | camadas por agrupar recursos como css, img, fontes etc.

## 🧰 Instalação
Utilize esse comando para clonar o repositório:
```GIT
git clone https://github.com/gleissonneves/bitcon-price-vue
```
Caso não deseje clonar baixe o [código fonte](https://github.com/gleissonneves/bitcon-price-vue/archive/refs/heads/master.zip).

*Acesse ao diretório:*
```shell
cd bitcon-price-vue
```

*Instale as dependências:*
```shell
npm i ou npm update
```
*ou ainda*
```shell
yarn install ou yarn update
```

*inicie o servidor*
```shell
npm run server
```
*ou configure uma porta específica*
```shell
npm run server --port 8080
```
## Como usar
### 🚧 Pre Requisitos 🚧

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com), [Vue.js CLI](https://cli.vuejs.org/).
Além disto é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/)

## :computer: Tecnologias
* [Vue.js](https://cli.vuejs.org/)

## :heavy_check_mark: Features

- [x] consumo de API rest


## Licença
Este projeto esta sobe a licença MIT.

Feito com :heart: por Gleisson Neves 👋🏽
