---
title: Estilos de componentes no Microsoft Graph Toolkit
description: Use as propriedades personalizadas de CSS para modificar os estilos de componente do Microsoft Graph Toolkit.
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 33ccc02f182731d494820976632b7cec2425d077
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663922"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>Estilos de componentes no Microsoft Graph Toolkit

Cada componente do kit de ferramentas do Microsoft Graph documenta um conjunto de [Propriedades personalizadas de CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) que você pode usar para alterar a aparência de determinados elementos. Você pode encontrar as propriedades CSS personalizadas disponíveis em cada um dos documentos do componente. Por exemplo:

```css
mgt-person {
  --avatar-size: 34px;
}
```

Você não pode estilizar elementos internos de um componente, a menos que forneça uma propriedade personalizada de CSS. Os elementos filho do componente estão hospedados em um [dom de sombra](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).

Para obter mais flexibilidade, considere o uso de [modelos personalizados](./templates.md).

## <a name="apply-themes"></a>Aplicar temas

Dois temas estão disponíveis-claro e escuro. Por padrão, todos os componentes são estilizados com tema claro. Para mudar para o tema escuro, você pode simplesmente aplicar `class="mgt-dark"` à seção da página HTML. Os componentes dentro dessa seção terão temas escuros aplicados. Os exemplos a seguir mostram como os temas serão aplicados com base na forma como você estrutura o HTML.

Exemplo 1: tema global

```html
<body class="mgt-light">
    <!-- light theme will apply to all components in this section -->
    <header><mgt-login></mgt-login></header>
    <article><mgt-agenda></mgt-agend></article>
    <footer></footer>
</body>
```

Exemplo 2: tema de componente individual

```html
<mgt-person-card class="mgt-dark"></mgt-person-card>
```

Exemplo 3: tema regional

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

Exemplo 4: personalizar o CSS com o tema

```html
<mgt-people-picker class="mgt-dark custom-class"></mgt-people-picker>
```
```css
mgt-people-picker.custom-class {
    --input-background-color: $custom-background-color;
    --input-border: $custom-input-border;
}
```
