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

# Shopify Themes

- [O que são temas no Shopify?](#o-que-são-temas-no-shopify)
- [Tipos de temas](#tipos-de-temas)
- [Theme Architecture no Shopify](#theme-architecture-no-shopify)
- [Tema Dawn: O padrão ouro](#tema-dawn-o-padrão-ouro)
- [Customização com o Theme Editor](#customização-com-o-theme-editor)
- [Estrutura de arquivos de um tema](#estrutura-de-arquivos-de-um-tema)
- [Páginas importantes em qualquer tema](#páginas-importantes-em-qualquer-tema)
- [Recursos úteis](#recursos-úteis)

## O que são temas no Shopify?

Temas são modelos personalizáveis que definem o layout, design e funcionalidades do **frontend** de uma loja Shopify. Eles determinam como os produtos, coleções, páginas e conteúdo são apresentados aos clientes.

## Tipos de temas

1. **Temas pré-construídos (prebuilt)**  
   - Disponíveis na [Shopify Theme Store](https://themes.shopify.com)  
   - Incluem opções gratuitas e pagas  
   - Personalizáveis com **Liquid**, HTML, CSS e JavaScript

2. **Temas customizados**  
   - Criados do zero ou baseados em temas existentes  
   - Utilizados por marcas com necessidades específicas  
   - Exigem conhecimento técnico (Liquid, JSON templates, APIs)

---

## Theme Architecture no Shopify

A arquitetura de temas no Shopify é baseada em uma estrutura modular que permite personalização visual e funcional através de arquivos e configurações bem organizadas. Essa arquitetura é a base para qualquer loja que utiliza o **Online Store 2.0**.

### Componentes da arquitetura de um tema

| Nº | Componente                        | Descrição                                                                                                                                     |
|----|-----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| 1  | **Layout**                        | Arquivo principal (`layout/theme.liquid`) que contém elementos persistentes em todas as páginas, como o `<head>`, cabeçalho e rodapé.        |
| 2  | **Template**                      | Define a estrutura para páginas específicas (`templates/*.json` ou `.liquid`). Ex: `product.json`, `collection.json`, `index.json`.         |
| 3  | **Section Groups**                | Contêineres que agrupam seções e blocos de aplicativos reutilizáveis, com suas configurações. Ex: grupo de seções no rodapé.                |
| 4  | **Sections**                      | Componentes reutilizáveis com lógica própria. Ex: banner, lista de produtos, formulário de contato (`sections/*.liquid`).                    |
| 5  | **Blocks**                        | Módulos dentro das seções. Os usuários podem adicionar, remover ou reorganizar blocos dentro de uma seção. Ex: um bloco de imagem + texto.   |

> 💡 **Dica**: Use o esquema JSON para definir a estrutura e os blocos disponíveis nas seções — isso permite flexibilidade e personalização via editor visual.

---

## Tema Dawn: O padrão ouro

**Dawn** é o tema de referência criado pela Shopify, que incorpora as melhores práticas de desenvolvimento de temas com foco em performance, acessibilidade e design moderno.

### Características do Dawn

- **Compatível com Online Store 2.0**
- **Mobile-first** e com uso mínimo de JavaScript
- Totalmente **customizável via editor visual**
- Estrutura leve com alta **performance de carregamento**
- Projetado com foco em **acessibilidade e usabilidade**

---

## Customização com o Theme Editor

O **Theme Editor** permite que você personalize facilmente um tema como o Dawn, usando a interface visual (no-code). Você pode:

- Adicionar / remover seções e blocos
- Reorganizar elementos da página
- Alterar cores, fontes e logos
- Adicionar links de redes sociais e configurar o menu

### Caminho de acesso

- Acesse **Online Store > Themes > Customize**
- Edite por página (Home, Product, Contact, etc.)
- Use a aba “**Theme Settings**” para configurações globais de marca

---

## Estrutura de arquivos de um tema

```bash
my-theme/
│
├── assets/            # CSS, JS, imagens
├── config/            # settings_schema.json e settings_data.json
├── layout/            # Arquivos base (ex: theme.liquid)
├── locales/           # Traduções
├── sections/          # Componentes independentes da UI
├── snippets/          # Trechos reutilizáveis de código
├── templates/         # JSON ou Liquid (ex: product.json)
└── templates/customers/ # Templates para páginas de clientes (ex: login, register)
```

## Páginas importantes em qualquer tema

- **Página Inicial (home)**: Apresenta produtos em destaque, coleções e banners. Use o template `index`.

- **Página de Coleção (collection)**: Lista produtos de uma coleção com o template `collection`.

- **Página de Produto (PDP)**: Detalhes específicos dos produtos. Utiliza o template `product`.

- **Página de Carrinho(cart)**: Visão geral do carrinho do cliente. Utiliza o template `cart`.

- **Conta do Cliente**: Histórico de pedidos e perfis. Utiliza o template `customers/account`.

- **Página de Pesquisa**: Incluir com o template `search`.

- **Blog**: Artigos e postagens. Utiliza o template `blog`.

- **Artigo**: Detalhes de um blog post específico. Utiliza o template `article`.

## Recursos úteis

- [Shopify Theme Store](https://themes.shopify.com)
- [Shopify Theme Development](https://shopify.dev/themes)
- [Shopify Liquid](https://shopify.dev/api/liquid)
