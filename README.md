# api-games-nodejs

## Projeto de estudo do nodeJS

Esta API é utilizada para manipular uma Lista de Games utilizando REST.

### Endpoints:
#### GET /games
Este ENDPoint retorna a listagem de todos os games cadastrados no BD.
##### Param: 
Nenhum
##### Respostas
Status 200 - Ok: Retorna a lista de games
Exemplo de respostas:
```
{
    "games": [
        {
            "id": 123,
            "title": "Doom",
            "year": 2000,
            "price": 68
        },
        {
            "id": 4,
            "title": "Top Gear",
            "year": 2008,
            "price": 80
        },
        {
            "id": 6,
            "title": "Minecraft",
            "year": 2010,
            "price": 800
        }
    ]
}
```
Status 401 - Falha: Usuário não autenticado

#### GET /game/{id}
Este EndPoint recebe o parametro ID e retorna um game
#### POST /game
