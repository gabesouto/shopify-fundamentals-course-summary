<div align="center">

<table>
  <tr>
    <td><a href="https://github.com/gabesouto/shopify-fundamentals-course-summary/blob/main/themes.md">Themes</a></td>
    <td><a href="https://github.com/gabesouto/shopify-fundamentals-course-summary/blob/main/storefront.md">Storefront API</a></td>
    <td><a href="https://github.com/gabesouto/shopify-fundamentals-course-summary/blob/main/shopify-apps.md">Apps Shopify</a></td>
    <td><a href="https://github.com/gabesouto/shopify-fundamentals-course-summary/blob/main/shopify-data-model.md">Shopify data model</a></td>
    <td><a href="https://github.com/gabesouto/shopify-fundamentals-course-summary/blob/main/shopify-graphql.md">Graphql</a></td>
    <td><a href="https://github.com/gabesouto/shopify-fundamentals-course-summary/blob/main/shopify-api.md">Shopify APIs</a></td>
    <td><a href="https://github.com/gabesouto/shopify-fundamentals-course-summary/blob/main/shopify-tools.md">Shopify Tools</a></td>
  </tr>
</table>

</div>


# Shopify APIs

- [APIs da Shopify](#apis-da-shopify)
- [APIs vs Webhooks](#apis-vs-webhooks)
- [APIs](#apis)
- [Webhooks](#webhooks)
- [API ou Webhook?](#api-ou-webhook)
- [Recursos úteis](#recursos-úteis)

A Shopify oferece uma variedade de APIs para desenvolvedores, permitindo que eles criem aplicativos personalizados, integrem sistemas externos e estendam a funcionalidade da plataforma. Aqui estão algumas das principais APIs disponíveis:

- **Admin API**: A Admin API é a principal interface para interagir com os dados da loja, como produtos, pedidos, clientes e muito mais. Ela permite que os desenvolvedores criem, leiam, atualizem e excluam dados na loja.

- **Storefront API**: A Storefront API é projetada para criar experiências de compra personalizadas em qualquer plataforma, como aplicativos móveis, sites personalizados e muito mais. Ela permite que os desenvolvedores acessem dados de produtos, coleções, carrinhos e checkout.
- **Customer account API**: A Customer account API permite que os desenvolvedores criem e gerenciem contas de clientes, incluindo autenticação, recuperação de senha e gerenciamento de informações do cliente.

## APIs X Webhooks

### APIs

APIs são interfaces que permitem que diferentes sistemas se comuniquem entre si. Elas permitem que os desenvolvedores acessem e manipulem dados em tempo real. As APIs da Shopify são baseadas em REST ou GraphQL, dependendo da API específica.

As APIs permitem que os desenvolvedores criem, leiam, atualizem e excluam dados na loja, como produtos, pedidos e clientes.

### Webhooks

Webhooks são uma maneira de receber notificações em tempo real quando eventos específicos ocorrem na loja. Eles permitem que os desenvolvedores configurem URLs de callback que serão acionados quando um evento ocorrer, como a criação de um novo pedido ou a atualização de um produto.

### API ou Webhook?

No ecossistema Shopify, APIs e webhooks não são mutuamente exclusivos, mas complementares. As APIs são ideais para operações sob demanda e consultas complexas, enquanto os webhooks são perfeitos para reações em tempo real a eventos da plataforma. Uma estratégia de integração bem-sucedida geralmente combina ambos para maximizar a eficiência, mantendo os sistemas sincronizados com o mínimo de latência e uso de recursos.

A escolha entre APIs e webhooks (ou uma combinação dos dois) deve ser baseada nos requisitos específicos da sua aplicação, considerando fatores como necessidade de dados em tempo real, volume de dados, frequência de atualizações e recursos disponíveis.

## Recursos úteis

- [Documentação oficial da Shopify](https://shopify.dev/docs)
- [Shopify API Reference](https://shopify.dev/api/admin-rest) - Referência completa das APIs da Shopify
