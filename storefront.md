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

# Shopify Storefront API

- [O que é a Storefront API?](#o-que-é-a-storefront-api)
- [Principais usos](#principais-usos)
- [Recursos acessíveis via API](#recursos-acessíveis-via-api)
- [Autenticação](#autenticação)
- [Recursos úteis](#recursos-úteis)

## O que é a Storefront API?

A **Storefront API** é uma API GraphQL pública oferecida pela Shopify, projetada para **desenvolver experiências de compra personalizadas** em qualquer plataforma – websites, aplicativos mobile, videogames, dispositivos IoT, entre outros.

---

## Principais usos

- **Criar storefronts headless** com total liberdade de front-end (React, Vue, Next.js, etc.)
- **Desenvolver apps mobile** (iOS/Android) com acesso em tempo real aos dados da loja
- **Customizar experiências** em realidade aumentada, displays interativos, e muito mais

---

## Recursos acessíveis via API

Você pode consultar, criar ou modificar os seguintes dados:

- Produtos e variantes
- Coleções
- Carrinhos (Cart API)
- Checkout
- Clientes (login, criação, recuperação)
- Metafields (dados personalizados)
- Disponibilidade de estoque
- Preços com suporte a múltiplas moedas e idiomas
- Recomendações de produtos
- Banners, conteúdo estático, e mais (via metadados)

---

## Autenticação

- Uso público: token de Storefront Access Token

- Criado no Admin da loja → Apps → Gerar chave para canal customizado

- Tokens são limitados à leitura/gravação permitida para uso cliente-side

## Recursos úteis

- [Documentação oficial da Storefront API](https://shopify.dev/docs/api/storefront)
- [Exemplos de uso da Storefront API](https://shopify.dev/docs/storefront-api/examples)
