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
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="9a548-103">Estilos de componentes no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="9a548-103">Styling components in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9a548-104">Cada componente do kit de ferramentas do Microsoft Graph documenta um conjunto de [Propriedades personalizadas de CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) que você pode usar para alterar a aparência de determinados elementos.</span><span class="sxs-lookup"><span data-stu-id="9a548-104">Each Microsoft Graph Toolkit component documents a set of [CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) that you can use to change the look and feel of certain elements.</span></span> <span data-ttu-id="9a548-105">Você pode encontrar as propriedades CSS personalizadas disponíveis em cada um dos documentos do componente. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9a548-105">You can find the available custom CSS properties in each component docs. For example:</span></span>

```css
mgt-person {
  --avatar-size: 34px;
}
```

<span data-ttu-id="9a548-106">Você não pode estilizar elementos internos de um componente, a menos que forneça uma propriedade personalizada de CSS.</span><span class="sxs-lookup"><span data-stu-id="9a548-106">You can't style internal elements of a component unless you provide a CSS custom property.</span></span> <span data-ttu-id="9a548-107">Os elementos filho do componente estão hospedados em um [dom de sombra](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span><span class="sxs-lookup"><span data-stu-id="9a548-107">The component child elements are hosted in a [shadow dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span></span>

<span data-ttu-id="9a548-108">Para obter mais flexibilidade, considere o uso de [modelos personalizados](./templates.md).</span><span class="sxs-lookup"><span data-stu-id="9a548-108">For more flexibility, consider using [custom templates](./templates.md).</span></span>

## <a name="apply-themes"></a><span data-ttu-id="9a548-109">Aplicar temas</span><span class="sxs-lookup"><span data-stu-id="9a548-109">Apply themes</span></span>

<span data-ttu-id="9a548-110">Dois temas estão disponíveis-claro e escuro.</span><span class="sxs-lookup"><span data-stu-id="9a548-110">Two themes are available - light and dark.</span></span> <span data-ttu-id="9a548-111">Por padrão, todos os componentes são estilizados com tema claro.</span><span class="sxs-lookup"><span data-stu-id="9a548-111">By default, all components are styled with light theme.</span></span> <span data-ttu-id="9a548-112">Para mudar para o tema escuro, você pode simplesmente aplicar `class="mgt-dark"` à seção da página HTML.</span><span class="sxs-lookup"><span data-stu-id="9a548-112">To switch to dark theme, you can simply apply `class="mgt-dark"` to the  section of your HTML page.</span></span> <span data-ttu-id="9a548-113">Os componentes dentro dessa seção terão temas escuros aplicados.</span><span class="sxs-lookup"><span data-stu-id="9a548-113">The components inside that section will have dark theme applied.</span></span> <span data-ttu-id="9a548-114">Os exemplos a seguir mostram como os temas serão aplicados com base na forma como você estrutura o HTML.</span><span class="sxs-lookup"><span data-stu-id="9a548-114">The following examples show how themes will apply based on how you structure your HTML.</span></span>

<span data-ttu-id="9a548-115">Exemplo 1: tema global</span><span class="sxs-lookup"><span data-stu-id="9a548-115">Example 1: Global theme</span></span>

```html
<body class="mgt-light">
    <!-- light theme will apply to all components in this section -->
    <header><mgt-login></mgt-login></header>
    <article><mgt-agenda></mgt-agend></article>
    <footer></footer>
</body>
```

<span data-ttu-id="9a548-116">Exemplo 2: tema de componente individual</span><span class="sxs-lookup"><span data-stu-id="9a548-116">Example 2: Individual component theme</span></span>

```html
<mgt-person-card class="mgt-dark"></mgt-person-card>
```

<span data-ttu-id="9a548-117">Exemplo 3: tema regional</span><span class="sxs-lookup"><span data-stu-id="9a548-117">Example 3: Regional theme</span></span>

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

<span data-ttu-id="9a548-118">Exemplo 4: personalizar o CSS com o tema</span><span class="sxs-lookup"><span data-stu-id="9a548-118">Example 4: Customize CSS with theme</span></span>

```html
<mgt-people-picker class="mgt-dark custom-class"></mgt-people-picker>
```
```css
mgt-people-picker.custom-class {
    --input-background-color: $custom-background-color;
    --input-border: $custom-input-border;
}
```
