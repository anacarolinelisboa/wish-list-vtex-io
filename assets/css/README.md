# Implementando a Wishlist em VTEX IO

Este guia irá te ajudar a adicionar a funcionalidade de Wishlist ao seu tema VTEX IO. Botão de coração no produto e visulização no painel do cliente.

## Adicionando o Botão de Wishlist ao Tema

Para adicionar o botão de Wishlist na página do produto ou product summary, insira:
\```json
"add-to-list-btn"
\``` 

Inserindo no product summary:
\```json
"product-summary.shelf": {
    "children": [ 
      "add-to-list-btn", 
    ]
},
\``` 


## Configuração no Manifest

No arquivo `manifest.json` do seu projeto, adicione a dependência do aplicativo `vtex.wish-list` inserindo o seguinte código:

\```json
"peerDependencies": {
  "vtex.wish-list": "1.x"
}
\```


Documentações: 
- [Documentação do VTEX Wish List App](https://apps.vtex.com/vtex-wish-list/p)
- [Guia de Desenvolvimento VTEX - Wish List](https://developers.vtex.com/docs/apps/vtex-wish-list)