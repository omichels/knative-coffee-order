# knative-coffee-order

the docker image for the coffee-order shop is available from public docker hub

- docker.io/olivermichelsbechtle/coffee-order:v1

and

- docker.io/olivermichelsbechtle/coffee-order:v2


once correctly deployed you can use curl to interact with the REST API of the shop

```bash
 curl -s -H "Host: coffee-order.default.example.com" 172.19.0.3/menu | jq .
```

http routes available:

- /menu GET
- /orders POST
- /orders GET
- /orders/{id} GET
- /orders/{id} PUT
- /orders/{id} DELETE

