---
title: Estilizando o Microsoft Graph Toolkit
description: Usar propriedades personalizadas de CSS para modificar os estilos de componente
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 41262c4e58973d84f4fec56a6d5abe8dfaf555ef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242932"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="6044c-103">Estilos de componentes no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="6044c-103">Styling components in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="6044c-104">Use Propriedades personalizadas de CSS para modificar os estilos de componente.</span><span class="sxs-lookup"><span data-stu-id="6044c-104">Use CSS custom properties to modify the component styles.</span></span>

<span data-ttu-id="6044c-105">Cada componente documenta um conjunto de [Propriedades personalizadas de CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) que você pode usar para alterar a aparência de determinados elementos.</span><span class="sxs-lookup"><span data-stu-id="6044c-105">Each component documents a set of [CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) that you can use to change the look and feel of certain elements.</span></span> <span data-ttu-id="6044c-106">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="6044c-106">For example:</span></span>

```css
mgt-person {
  --avatar-size: 34px;
}
```

<span data-ttu-id="6044c-107">Você não pode estilizar elementos internos de um componente, a menos que forneça uma propriedade personalizada de CSS.</span><span class="sxs-lookup"><span data-stu-id="6044c-107">You can't style internal elements of a component unless you provide a CSS custom property.</span></span> <span data-ttu-id="6044c-108">Os elementos filho do componente estão hospedados em um [dom de sombra](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span><span class="sxs-lookup"><span data-stu-id="6044c-108">The component child elements are hosted in a [shadow dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span></span>

<span data-ttu-id="6044c-109">Para obter mais flexibilidade, considere o uso de [modelos personalizados](./templates.md).</span><span class="sxs-lookup"><span data-stu-id="6044c-109">For more flexibility, consider using [custom templates](./templates.md).</span></span>

## <a name="disable-the-shadow-dom-experimental"></a><span data-ttu-id="6044c-110">Desabilitar o dom de sombra (experimental)</span><span class="sxs-lookup"><span data-stu-id="6044c-110">Disable the shadow dom (experimental)</span></span>

<span data-ttu-id="6044c-111">Você pode desabilitar o dom de sombra e estilizar diretamente elementos internos usando folhas de estilo normais do navegador, definindo a `useShadowDom` propriedade estática `MgtBaseComponent` da classe como false antes de usar qualquer marca de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="6044c-111">You can disable the shadow dom, and directly style internal elements using normal browser stylesheets, by setting the static property `useShadowDom` of the `MgtBaseComponent` class to false before using any MGT tags.</span></span>


```html
<script type="module">
  import { MgtBaseComponent } from './dist/es6/components/baseComponent.js';
   MgtBaseComponent.useShadowRoot = false;
</script>

<script type="module" src="./dist/es6/components/mgt-tasks/mgt-tasks.js"></script>
````
