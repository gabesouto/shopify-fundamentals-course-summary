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


# O Ecossistema de apps da Shopify

- [O que são apps?](#o-que-são-apps)
- [Tipos de apps](#tipos-de-apps)
  - [Public apps](#public-apps)
  - [Custom apps](#custom-apps)
- [Como os apps funcionam na Shopify](#entendendo-como-apps-funcionam-no-contexto-shopify)
  - [Áreas de Extensão de Funcionalidade](#áreas-de-extensão-de-funcionalidade)
- [Categorias e funções comuns de apps Shopify](#categorias-e-funções-comuns-de-apps-shopify)
- [Apps by Shopify](#apps-by-shopify)
- [Recursos úteis](#recursos-úteis)

## O que são apps?

Apps no contexto da Shopify são aplicações que estendem as funcionalidades da plataforma, permitindo que lojistas personalizem e melhorem suas lojas virtuais. Eles podem ser usados para adicionar novos recursos, integrar com serviços de terceiros, otimizar processos e muito mais.

A Shopify possui um ecossistema robusto de apps, que podem ser encontrados na Shopify App Store. Esses apps são desenvolvidos por parceiros da Shopify e podem ser instalados diretamente nas lojas dos lojistas.

Também é possível desenvolver apps personalizados para atender necessidades específicas de um negócio. Esses apps podem ser integrados à loja através da Shopify API, permitindo acesso a dados e funcionalidades da plataforma.

- Exemplo de  um app Shopify: app de **Wishlist**, ainda que seja totalmente possível criar uma wishlist com código customizado, o app pode facilitar e muito a implementação muitas vezes com um custo de recursos menor do que o código customizado exigiria.

> **importante**: Enquanto desenvolvedor é de EXTREMA importância saber avaliar quando utilizar um app ou código customizado, esse é um dos pontos que mais impacta o tempo de entrega e a qualidade do projeto. Sempre que possível utilize apps prontos, mas sempre avalie o custo de cada opção.

---

## Tipos de apps

### Public apps

Public apps são aplicativos desenvolvidos para serem usados por qualquer lojista na Shopify. Eles podem ser encontrados na Shopify App Store e são projetados para atender a uma ampla gama de necessidades.

### Custom apps

Custom apps são aplicativos desenvolvidos especificamente para uma loja ou cliente. Eles são criados para atender a necessidades específicas e podem ser personalizados de acordo com os requisitos do negócio.

---

## Entendendo como apps funcionam no contexto Shopify

Como dito antes um app no contexto Shopify é uma aplicação que estende as funcionalidades da plataforma, apps podem estender quase que qualquer funcionalidade da plataforma, desde a criação de um produto até o checkout.

Um app pode ser um simples script que roda em um servidor e se comunica com a Shopify API, ou uma aplicação complexa com front-end e back-end próprios.

### Áreas de Extensão de Funcionalidade

- **Admin do Shopify:** Apps podem ser incorporados ao Admin para integrações consistentes.
- **Loja Online:** Extensões de apps para adicionar elementos dinâmicos sem alterar código de tema.
- **Checkout:** Extensões de UI para customizar a experiência de checkout.
- **Contas de Clientes:** Adicionar elementos e páginas específicas às contas.
- **Ponto de Venda (POS):** Personalizações para vendas presenciais.
- **Apps Apenas no Servidor:** Sincronização e funcionalidade backend adicionais.

---

## Categorias e funções comuns de apps Shopify

- **Finding products**: Aplicativos relacionados à busca e fornecimento de produtos para a loja. Aqui, você encontrará aplicativos relacionados a encontrar fornecedores, dropshipping, print-on-demand (POD) e compra no atacado.

- **Selling products**: Aplicativos relacionados à exibição e venda de produtos. Subcategorias incluem métodos de venda, como varejo, exibição de produtos, precificação, opções de compra como assinaturas, presentes, produtos digitais e blockchain.

- **Orders and shipping**: Aplicativos relacionados ao gerenciamento e processamento de pedidos. Subcategorias incluem gestão de pedidos, cumprimento de pedidos, gerenciamento de inventário, além de entrega e retirada.

- **Store design**: Aplicativos relacionados à personalização da aparência e sensação de uma loja. Subcategorias incluem páginas da loja, navegação e busca, imagens e mídia, notificações, alertas da loja, internacionalização, aprimoramentos de página e prova social.

- **Marketing and conversion**: Aplicativos relacionados a atrair, engajar e converter clientes. Recursos incluem ferramentas para marketing por e-mail, publicidade em mídias sociais, otimização para SEO, retenção de clientes e testes A/B.

---

## Apps by Shopify

Shopify oferece uma variedade de aplicativos próprios que são integrados à plataforma. Esses aplicativos são projetados para melhorar a experiência do usuário e otimizar o desempenho da loja. Alguns dos principais aplicativos da Shopify incluem:

- **Bundles**: Permite que as empresas vendam vários produtos juntos com desconto.

- **Shopify Audiences:** Ajuda as empresas a encontrar novos clientes gerando uma lista de público para plataformas de publicidade.

- **Shopify Flow:** Cria fluxos de trabalho para automatizar tarefas comuns na sua loja.

- **Translate & Adapt:** Adiciona traduções à sua loja para produtos, coleções, postagens de blog, políticas e páginas.

## Recursos úteis

- [Shopify App Store](https://apps.shopify.com/) - Loja de aplicativos da Shopify
- [Shopify App Bridge](https://shopify.dev/tools/app-bridge) - Biblioteca para integrar apps com o Shopify Admin
- [Shopify Polaris](https://polaris.shopify.com/) - Biblioteca de componentes para criar interfaces de usuário consistentes
- [Shopify CLI](https://shopify.dev/cli) - Ferramenta de linha de comando para criar e gerenciar apps Shopify
- [Shopify API Reference](https://shopify.dev/api/admin-rest) - Referência completa das APIs da Shopify
