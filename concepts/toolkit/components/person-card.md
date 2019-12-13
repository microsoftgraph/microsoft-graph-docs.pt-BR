---
title: Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph
description: Um componente de cartão de pessoa é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 7f4f20773b152db037d3b57481aa5e8638866f52
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955866"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="0287f-103">Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0287f-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0287f-104">Um componente de cartão de pessoa é um componente responsivo para exibir mais informações relacionadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="0287f-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="0287f-105">Geralmente, é usado como um submenu do `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="0287f-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="0287f-106">Para obter mais informações sobre `mgt-person` o componente, consulte [docs-Person docs](./person.md).</span><span class="sxs-lookup"><span data-stu-id="0287f-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>
  
## <a name="example"></a><span data-ttu-id="0287f-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0287f-107">Example</span></span>

```html
<mgt-person-card person-details="{personObject}" person-image="imgUrl"></mgt-person-card>
```

## <a name="properties"></a><span data-ttu-id="0287f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0287f-108">Properties</span></span>

<span data-ttu-id="0287f-109">O componente usa o Microsoft Graph para fornecer detalhes adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="0287f-109">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="0287f-110">Para definir um usuário, você deve usar a propriedade **Person-Query** de `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="0287f-110">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="0287f-111">Atributo</span><span class="sxs-lookup"><span data-stu-id="0287f-111">Attribute</span></span>         | <span data-ttu-id="0287f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="0287f-112">Type</span></span>                     | <span data-ttu-id="0287f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0287f-113">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="0287f-114">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="0287f-114">person-details</span></span> | <span data-ttu-id="0287f-115">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="0287f-115">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="0287f-116">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="0287f-116">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="0287f-117">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="0287f-117">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="0287f-118">Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="0287f-118">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="0287f-119">pessoa-imagem</span><span class="sxs-lookup"><span data-stu-id="0287f-119">person-image</span></span>   | <span data-ttu-id="0287f-120">png/jpg/SVG</span><span class="sxs-lookup"><span data-stu-id="0287f-120">png/jpg/svg</span></span>                    | <span data-ttu-id="0287f-121">Imagem relacionada à pessoa exibida no cartão.</span><span class="sxs-lookup"><span data-stu-id="0287f-121">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="0287f-122">Inherit-detalhes</span><span class="sxs-lookup"><span data-stu-id="0287f-122">inherit-details</span></span>   | <span data-ttu-id="0287f-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0287f-123">None.</span></span>                  | <span data-ttu-id="0287f-124">Permite que o cartão de pessoa percorra a `mgt-person` árvore pai para que o `person-details` componente `person-image` use o mesmo e os dados.</span><span class="sxs-lookup"><span data-stu-id="0287f-124">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="0287f-125">Modelos</span><span class="sxs-lookup"><span data-stu-id="0287f-125">Templates</span></span>

<span data-ttu-id="0287f-126">O componente de cartão de pessoa usa [modelos](../templates.md) que permitem que você adicione ou substitua partes do componente.</span><span class="sxs-lookup"><span data-stu-id="0287f-126">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="0287f-127">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="0287f-127">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="0287f-128">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="0287f-128">Data type</span></span> | <span data-ttu-id="0287f-129">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="0287f-129">Data context</span></span> | <span data-ttu-id="0287f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0287f-130">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="0287f-131">Padrão.</span><span class="sxs-lookup"><span data-stu-id="0287f-131">default</span></span> | <span data-ttu-id="0287f-132">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="0287f-132">`person`: The person details object</span></span> <br> <span data-ttu-id="0287f-133">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="0287f-133">`personImage`: The URL of the image</span></span> | <span data-ttu-id="0287f-134">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="0287f-134">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="0287f-135">adicional-detalhes</span><span class="sxs-lookup"><span data-stu-id="0287f-135">additional-details</span></span> | <span data-ttu-id="0287f-136">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="0287f-136">`person`: The person details object</span></span> <br> <span data-ttu-id="0287f-137">`personImage`: a URL da imagem</span><span class="sxs-lookup"><span data-stu-id="0287f-137">`personImage`: the URL of the image</span></span> | <span data-ttu-id="0287f-138">O modelo usado para adicionar conteúdo adicional ao cartão.</span><span class="sxs-lookup"><span data-stu-id="0287f-138">The template used to add additional content to the card.</span></span> |

<span data-ttu-id="0287f-139">Por exemplo, você pode usar um modelo para personalizar o componente anexado ao `mgt-person` componente e um modelo para adicionar mais detalhes no cartão.</span><span class="sxs-lookup"><span data-stu-id="0287f-139">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card inherit-details>
          <template data-type="additional-details">
            <h3>Stuffed Animal Friends:</h3>
            <ul>
              <li>Giraffe</li>
              <li>lion</li>
              <li>Rabbit</li>
            </ul>
          </template>
        </mgt-person-card>
      </template>
    </mgt-person>

```

## <a name="css-custom-properties"></a><span data-ttu-id="0287f-140">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="0287f-140">CSS custom properties</span></span>

<span data-ttu-id="0287f-141">O `mgt-person-card` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="0287f-141">The `mgt-person-card` component defines the following CSS custom properties.</span></span>

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

<span data-ttu-id="0287f-142">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="0287f-142">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="0287f-143">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0287f-143">Microsoft Graph permissions</span></span>

<span data-ttu-id="0287f-144">Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="0287f-144">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="0287f-145">Autenticação</span><span class="sxs-lookup"><span data-stu-id="0287f-145">Authentication</span></span>

<span data-ttu-id="0287f-146">O controle de cartão de pessoa usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="0287f-146">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
