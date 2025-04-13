# Introdução ao GraphQL (no contexto da Shopify)

- [O que é GraphQL?](#o-que-é-graphql)
- [GraphQL vs REST](#graphql-vs-rest)
- [Por que a Shopify prefere GraphQL?](#por-que-a-shopify-prefere-graphql)
- [Consultas (Queries) vs Mutations](#consultas-queries-vs-mutations)
- [Objetos e campos em GraphQL](#objetos-e-campos-em-graphql)
- [Exemplo de consulta (Query)](#exemplo-de-consulta-query)
- [Exemplo de mutation](#exemplo-de-mutation)
- [Error handling in GraphQL](#error-handling-in-graphql)
- [Recursos úteis](#recursos-úteis)

## O que é GraphQL?

**GraphQL** é uma linguagem para consultar e manipular APIs de forma precisa, retornando **somente os dados solicitados**. Foi criada pelo Facebook e é hoje a **tecnologia preferida da Shopify** para desenvolvimento de APIs.

---

## GraphQL vs REST

| Característica         | GraphQL                            | REST                                 |
|------------------------|------------------------------------|--------------------------------------|
| Tipo de chamada        | Único endpoint (POST)              | Múltiplos endpoints (GET, POST etc.) |
| Volume de dados        | Apenas o que é solicitado          | Retorna todos os dados disponíveis   |
| Requisições            | Uma única chamada pode retornar dados de vários recursos | Requer múltiplas chamadas separadas |
| Autocompletar e tipagem| Fortemente tipado + introspectivo  | Depende de documentação externa      |
| Flexibilidade          | Alta                               | Limitada pela estrutura do endpoint  |

---

## Por que a Shopify prefere GraphQL?

- **Menor sobrecarga de dados**: retorna apenas o que foi requisitado
- **Alta performance**: menos chamadas à rede
- **Facilidade de uso com autocompletion e validação**
- **Documentação embutida** via introspecção
- **Maior controle sobre o uso dos dados pelos apps**

---

## Consultas (Queries) vs Mutations

- **Query**: usada para **buscar dados**, equivalente ao GET no REST.
- **Mutation**: usada para **criar ou modificar dados**, equivalente ao POST/PUT/DELETE no REST.

Ambas usam o método HTTP **POST** e são enviadas a um único endpoint.

---

## Objetos e campos em GraphQL

Em GraphQL, tudo gira em torno de **objetos**. Cada objeto tem campos que podem ser de tipos primitivos (String, Int, Boolean) ou outros objetos.

### Exemplo

```graphql
type User {
  id: ID!
  name: String!
  age: Int
  email: String
}
```

- User é o tipo de objeto.

- ! indica que o campo é obrigatório (non-nullable).

- Os tipos podem ser escalares ou objetos personalizados.

### Exemplo de consulta (Query)

```graphql
query {
  user(id: "123") {
    name
    age
  }
}
```

- Retorna o nome e a idade do usuário com ID 123.
- Se o campo `age` não estiver disponível, a consulta falhará, pois é um campo opcional.
- Se o campo `name` não estiver disponível, a consulta falhará, pois é um campo obrigatório.

### Exemplo de mutation

```graphql
mutation {
  createUser(name: "John Doe", age: 30) {
    id
    name
  }
}
```

- Cria um novo usuário com nome "John Doe" e idade 30.
- Retorna o ID e o nome do usuário criado.

### Error handling in GraphQL

Para lidar com erros em GraphQL você pode usar o campo `errors` na resposta. Se houver erros, eles serão retornados nesse campo, enquanto os dados válidos serão retornados no campo `data`.

```graphql

mutation {
  customerCreate(input: 
    { firstName: "Ayumu", 
      lastName: "Hirano", 
      email: "ayumu@example.com" }) {
    customer {
      id
    }
    userErrors{
      field
      message
    }
  }
}


{
  "data": {
    "customerCreate": {
      "customer": null,
      "userErrors": [
        {
          "field": [
            "email"
          ],
          "message": "Email has already been taken"
        }
      ]
    }
  }
}


```

- O campo `userErrors` contém uma lista de erros, cada um com um campo e uma mensagem.
- O campo `customer` é nulo, pois a criação do cliente falhou devido ao erro de email duplicado.

## Recursos úteis

- [GraphQL Docs](https://graphql.org/learn/)
- [Shopify GraphQL API](https://shopify.dev/api/admin-graphql)
