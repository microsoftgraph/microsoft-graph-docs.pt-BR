---
title: Componentes de estilo no microsoft Graph Toolkit
description: Use propriedades personalizadas CSS para modificar os estilos de componente Graph Toolkit Microsoft.
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 437bad7f8a8e76d04f277f0796e7b44b98cac0b8f3f32e7787352d7c3cd9c8f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54221072"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>Componentes de estilo no microsoft Graph Toolkit

Cada componente Graph Toolkit Microsoft documenta um conjunto de [propriedades personalizadas CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) que você pode usar para alterar a aparência de determinados elementos. Você pode encontrar as propriedades CSS personalizadas disponíveis em cada documento de componente. Por exemplo:

```css
mgt-person {
  --avatar-size: 34px;
}
```

Não é possível estilização de elementos internos de um componente, a menos que você forneça uma propriedade personalizada CSS. Os elementos filho do componente são hospedados em um [dom de sombra.](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)

Para obter mais flexibilidade, considere o uso [de modelos personalizados.](./templates.md)

## <a name="apply-themes"></a>Aplicar temas

Dois temas estão disponíveis - claro e escuro. Por padrão, todos os componentes são estilados com tema claro. Para alternar para o tema escuro, você pode simplesmente `class="mgt-dark"` aplicar à seção da sua página HTML. Os componentes dentro dessa seção terão o tema escuro aplicado. Os exemplos a seguir mostram como os temas serão aplicados com base em como você estrutura seu HTML.

Exemplo 1: Tema global

```html
<body class="mgt-light">
    <!-- light theme will apply to all components in this section -->
    <header><mgt-login></mgt-login></header>
    <article><mgt-agenda></mgt-agend></article>
    <footer></footer>
</body>
```

Exemplo 2: Tema de componente individual

```html
<mgt-person-card class="mgt-dark"></mgt-person-card>
```

Exemplo 3: Tema regional

```html
<div class="mgt-light">
    <header class="mgt-dark">
        // login component will have dark theme
        <mgt-login></mgt-login>
    </header>
    <article>
        // agenda component will have light theme
        <mgt-agenda></mgt-agenda>
    </article>
</div>
```

Exemplo 4: Personalizar CSS com tema

```html
<mgt-people-picker class="mgt-dark custom-class"></mgt-people-picker>
```
```css
mgt-people-picker.custom-class {
    --input-background-color: $custom-background-color;
    --input-border: $custom-input-border;
}
```
