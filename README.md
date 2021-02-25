# React Marvel

![ReactMarvel](./docs/react-marvel.png)

Este é um exemplo de aplicativo React que demonstra como usar a API da Marvel com Redux e sagas para mostrar uma lista de personagens da Marvel e uma lista de quadrinhos para cada personagem.

Como a API da Marvel limita nossa solicitação a ** 3000 solicitações ** por dia, talvez a página de demonstração não funcione dependendo de quanto os usuários estão tentando executar, se você pode executar esta demonstração, instale este projeto em sua máquina e use [seu próprias chaves de API] (https://developer.marvel.com/documentation/getting_started) da marvel

`./src/config/config.js`

```
export const marvelApi = {
  publicKey: 'YOUR_PUBLIC_KEY',
  privateKey: 'YOUR_PRIVATE_KEY',
  baseUrl: `${window.location.protocol || 'http'}//gateway.marvel.com:80`,
}
```

## Libs

- [Redux](http://redux.js.org/)
- [Moment](https://momentjs.com/)
- [ReduxSaga](https://github.com/redux-saga/redux-saga)
- [Material UI](https://material-ui-1dab0.firebaseapp.com)

## O que faz?

Esta exemplo deve fornecer as seguintes funcionalidades:

- Uma lista de personagens carregadas da API da Marvel
- Cada cartão abre um diálogo com uma coleção de histórias em quadrinhos
- Rolagem infinita integrada com paginação API

## Possíveis implementações

- Lista de eventos
- Mais detalhes para cada história em quadrinhos
- Criar a aplicação responsiva;
- Criar um filtro por letra inicial do nome do personagem que ao clicar, exiba todos os itens correspondentes;
- Criar uma funcionalidade que permita que o usuário favorite os personagens;
- Armazenar a data em que o item foi favoritado;
- Depois de favoritar, é preciso ter uma página para visualizar os itens favoritos, ordenados por nome ou por data em que foi favoritado (com a seguinte rota: /comics/favorites);
- Opção de remover um personagem de favoritos;
- Opção para limpar todos os itens favoritados;
- Hospedar sua aplicação em algum servidor cloud (se o fizer, envie o link da aplicação hospedada junto com o link do repositório);

# Iniciar

```
$ git clone https://github.com/ctoigo/react-marvel
$ cd react-marvel
$ yarn install
$ yarn start
```
