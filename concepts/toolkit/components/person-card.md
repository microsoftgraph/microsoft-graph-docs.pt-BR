---
title: Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph
description: Um componente de cartão de pessoa é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 336e6beabc227a2574e41cf6a658d38fdabfcdcf
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639923"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="56f9c-103">Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="56f9c-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="56f9c-104">Um componente de cartão de pessoa é um componente responsivo para exibir mais informações relacionadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="56f9c-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="56f9c-105">Geralmente, é usado como um submenu do `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="56f9c-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="56f9c-106">Para obter mais informações sobre `mgt-person` o componente, consulte [docs-Person docs](./person.md).</span><span class="sxs-lookup"><span data-stu-id="56f9c-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="56f9c-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56f9c-107">Example</span></span>

<span data-ttu-id="56f9c-108">O exemplo a seguir mostra o uso do `mgt-person-card` componente com um `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="56f9c-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="56f9c-109">Passe o mouse sobre a pessoa para ver o cartão Person e use o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="56f9c-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="56f9c-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="56f9c-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="properties"></a><span data-ttu-id="56f9c-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56f9c-111">Properties</span></span>

<span data-ttu-id="56f9c-112">O componente usa o Microsoft Graph para fornecer detalhes adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="56f9c-112">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="56f9c-113">Para definir um usuário, você deve usar a propriedade **Person-Query** de `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="56f9c-113">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="56f9c-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="56f9c-114">Attribute</span></span>         | <span data-ttu-id="56f9c-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="56f9c-115">Type</span></span>                     | <span data-ttu-id="56f9c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="56f9c-116">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="56f9c-117">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="56f9c-117">person-details</span></span> | <span data-ttu-id="56f9c-118">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="56f9c-118">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="56f9c-119">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="56f9c-119">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="56f9c-120">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="56f9c-120">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="56f9c-121">Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="56f9c-121">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="56f9c-122">pessoa-imagem</span><span class="sxs-lookup"><span data-stu-id="56f9c-122">person-image</span></span>   | <span data-ttu-id="56f9c-123">png/jpg/SVG</span><span class="sxs-lookup"><span data-stu-id="56f9c-123">png/jpg/svg</span></span>                    | <span data-ttu-id="56f9c-124">Imagem relacionada à pessoa exibida no cartão.</span><span class="sxs-lookup"><span data-stu-id="56f9c-124">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="56f9c-125">Inherit-detalhes</span><span class="sxs-lookup"><span data-stu-id="56f9c-125">inherit-details</span></span>   | <span data-ttu-id="56f9c-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="56f9c-126">None.</span></span>                  | <span data-ttu-id="56f9c-127">Permite que o cartão de pessoa percorra a `mgt-person` árvore pai para que o `person-details` componente `person-image` use o mesmo e os dados.</span><span class="sxs-lookup"><span data-stu-id="56f9c-127">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="56f9c-128">Modelos</span><span class="sxs-lookup"><span data-stu-id="56f9c-128">Templates</span></span>

<span data-ttu-id="56f9c-129">O componente de cartão de pessoa usa [modelos](../templates.md) que permitem que você adicione ou substitua partes do componente.</span><span class="sxs-lookup"><span data-stu-id="56f9c-129">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="56f9c-130">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="56f9c-130">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="56f9c-131">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="56f9c-131">Data type</span></span> | <span data-ttu-id="56f9c-132">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="56f9c-132">Data context</span></span> | <span data-ttu-id="56f9c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="56f9c-133">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="56f9c-134">Padrão.</span><span class="sxs-lookup"><span data-stu-id="56f9c-134">default</span></span> | <span data-ttu-id="56f9c-135">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="56f9c-135">`person`: The person details object</span></span> <br> <span data-ttu-id="56f9c-136">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="56f9c-136">`personImage`: The URL of the image</span></span> | <span data-ttu-id="56f9c-137">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="56f9c-137">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="56f9c-138">adicional-detalhes</span><span class="sxs-lookup"><span data-stu-id="56f9c-138">additional-details</span></span> | <span data-ttu-id="56f9c-139">`person`: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="56f9c-139">`person`: The person details object</span></span> <br> <span data-ttu-id="56f9c-140">`personImage`: a URL da imagem</span><span class="sxs-lookup"><span data-stu-id="56f9c-140">`personImage`: the URL of the image</span></span> | <span data-ttu-id="56f9c-141">O modelo usado para adicionar conteúdo adicional ao cartão.</span><span class="sxs-lookup"><span data-stu-id="56f9c-141">The template used to add additional content to the card.</span></span> |

<span data-ttu-id="56f9c-142">Por exemplo, você pode usar um modelo para personalizar o componente anexado ao `mgt-person` componente e um modelo para adicionar mais detalhes no cartão.</span><span class="sxs-lookup"><span data-stu-id="56f9c-142">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="css-custom-properties"></a><span data-ttu-id="56f9c-143">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="56f9c-143">CSS custom properties</span></span>

<span data-ttu-id="56f9c-144">O `mgt-person-card` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="56f9c-144">The `mgt-person-card` component defines the following CSS custom properties.</span></span>

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

<span data-ttu-id="56f9c-145">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="56f9c-145">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="56f9c-146">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="56f9c-146">Microsoft Graph permissions</span></span>

<span data-ttu-id="56f9c-147">Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="56f9c-147">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="56f9c-148">Autenticação</span><span class="sxs-lookup"><span data-stu-id="56f9c-148">Authentication</span></span>

<span data-ttu-id="56f9c-149">O controle de cartão de pessoa usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="56f9c-149">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
