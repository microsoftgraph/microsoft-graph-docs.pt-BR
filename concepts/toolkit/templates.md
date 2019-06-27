---
title: Modelos no Microsoft Graph Toolkit
description: Use modelos personalizados para modificar o conteúdo de um componente.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: f0648d0ac1348fbadad6cebe8a022f9445fcf1e3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242929"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="bd09e-103">Modelos no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bd09e-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bd09e-104">Use modelos personalizados para modificar o conteúdo de um componente.</span><span class="sxs-lookup"><span data-stu-id="bd09e-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="bd09e-105">Todos os componentes Web oferecem suporte a `<template>` modelos baseados no elemento.</span><span class="sxs-lookup"><span data-stu-id="bd09e-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="bd09e-106">Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.</span><span class="sxs-lookup"><span data-stu-id="bd09e-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

```html
<mgt-agenda>
  <template data-type="event">
      <div>{{event.subject}}</div>
      <div data-for='attendee in event.attendees'>
          <mgt-person person-query="{{attendee.emailAddress.name}}">
            <template>
              <div data-if="person.image">
                <img src="{{person.image}}" />
              </div>
              <div data-else>
                {{person.displayName}}
              </div>
            </template>
          </mgt-person>
      </div>
  </template>
</mgt-agenda>
```

<span data-ttu-id="bd09e-107">Há suporte para os seguintes recursos de modelo:</span><span class="sxs-lookup"><span data-stu-id="bd09e-107">The following template features are supported:</span></span>

- <span data-ttu-id="bd09e-108">Use as chaves duplas (`{{expression}}`) para expandir uma expressão.</span><span class="sxs-lookup"><span data-stu-id="bd09e-108">Use the double curly brackets (`{{expression}}`) to expand an expression.</span></span> <span data-ttu-id="bd09e-109">No exemplo anterior, o `<mgt-person>` passa um `person` objeto que você pode usar no modelo.</span><span class="sxs-lookup"><span data-stu-id="bd09e-109">In the previous example, the `<mgt-person>` passes a `person` object that you can use in the template.</span></span>
- <span data-ttu-id="bd09e-110">Use os `data-if` atributos `data-else` e para a renderização condicional.</span><span class="sxs-lookup"><span data-stu-id="bd09e-110">Use the `data-if` and `data-else` attributes for conditional rendering.</span></span> <span data-ttu-id="bd09e-111">Expressões condicionais como `event.attendees.length > 2` são suportadas.</span><span class="sxs-lookup"><span data-stu-id="bd09e-111">Conditional expressions such as `event.attendees.length > 2` are supported.</span></span>
- <span data-ttu-id="bd09e-112">Use o `data-for` para repetir um elemento.</span><span class="sxs-lookup"><span data-stu-id="bd09e-112">Use the `data-for` to repeat an element.</span></span>
- <span data-ttu-id="bd09e-113">Use o `data-type` para especificar de que parte do componente será o modelo.</span><span class="sxs-lookup"><span data-stu-id="bd09e-113">Use the `data-type` to specify what part of the component to template.</span></span> <span data-ttu-id="bd09e-114">Não especificar o tipo aplicará o modelo a todo o componente.</span><span class="sxs-lookup"><span data-stu-id="bd09e-114">Not specifying the type will apply the template to the entire component.</span></span>

<span data-ttu-id="bd09e-115">Cada componente documenta os valores `data-type` com suporte e qual contexto de dados é passado para cada modelo.</span><span class="sxs-lookup"><span data-stu-id="bd09e-115">Each component documents the supported `data-type` values and what data context is passed down to each template.</span></span>

<span data-ttu-id="bd09e-116">Os modelos podem ser estilizados normalmente, já que são renderizados fora do dom de sombra.</span><span class="sxs-lookup"><span data-stu-id="bd09e-116">The templates can be styled normally as they are rendered outside of the shadow dom.</span></span>
