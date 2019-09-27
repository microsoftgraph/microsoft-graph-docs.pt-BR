---
title: Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph
description: Um componente de cartão de pessoa é um componente para exibir mais informações relacionadas a uma pessoa.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: f4d8c975fe91d91658f512cea708ee104d4fd906
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275854"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d1e92-103">Componente de cartão de pessoa no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d1e92-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d1e92-104">Um componente de cartão de pessoa é um componente responsivo para exibir mais informações relacionadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="d1e92-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="d1e92-105">Geralmente, é usado como um submenu do `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="d1e92-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="d1e92-106">Para obter mais informações sobre `mgt-person` o componente, consulte [docs-Person docs](./person.md).</span><span class="sxs-lookup"><span data-stu-id="d1e92-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>
  
## <a name="example"></a><span data-ttu-id="d1e92-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1e92-107">Example</span></span>

```html
<mgt-person-card person-details="{personObject}" person-image="imgUrl"></mgt-person-card>
```

## <a name="properties"></a><span data-ttu-id="d1e92-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1e92-108">Properties</span></span>

<span data-ttu-id="d1e92-109">O componente usa o Microsoft Graph para fornecer detalhes adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="d1e92-109">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="d1e92-110">Para definir um usuário, você deve usar a propriedade **Person-Query** de `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="d1e92-110">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="d1e92-111">Atributo</span><span class="sxs-lookup"><span data-stu-id="d1e92-111">Attribute</span></span>         | <span data-ttu-id="d1e92-112">type</span><span class="sxs-lookup"><span data-stu-id="d1e92-112">type</span></span>                     | <span data-ttu-id="d1e92-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1e92-113">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="d1e92-114">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="d1e92-114">person-details</span></span> | <span data-ttu-id="d1e92-115">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="d1e92-115">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="d1e92-116">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="d1e92-116">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="d1e92-117">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="d1e92-117">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="d1e92-118">Objeto Person conforme definido pelo Microsoft Graph, contendo detalhes relacionados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d1e92-118">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="d1e92-119">pessoa-imagem</span><span class="sxs-lookup"><span data-stu-id="d1e92-119">person-image</span></span>   | <span data-ttu-id="d1e92-120">png/jpg/SVG</span><span class="sxs-lookup"><span data-stu-id="d1e92-120">png/jpg/svg</span></span>                    | <span data-ttu-id="d1e92-121">Imagem relacionada à pessoa exibida no cartão.</span><span class="sxs-lookup"><span data-stu-id="d1e92-121">Image related to the person displayed in the card.</span></span>                                   |



## <a name="templates"></a><span data-ttu-id="d1e92-122">Modelos</span><span class="sxs-lookup"><span data-stu-id="d1e92-122">Templates</span></span>

<span data-ttu-id="d1e92-123">O componente de cartão de pessoa usa [modelos](../templates.md) que permitem que você adicione ou substitua partes do componente.</span><span class="sxs-lookup"><span data-stu-id="d1e92-123">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="d1e92-124">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="d1e92-124">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="d1e92-125">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="d1e92-125">Data type</span></span> | <span data-ttu-id="d1e92-126">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="d1e92-126">Data context</span></span> | <span data-ttu-id="d1e92-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1e92-127">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d1e92-128">Padrão.</span><span class="sxs-lookup"><span data-stu-id="d1e92-128">default</span></span> | <span data-ttu-id="d1e92-129">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="d1e92-129">person: The person details object</span></span> <br> <span data-ttu-id="d1e92-130">personImage: a URL da imagem</span><span class="sxs-lookup"><span data-stu-id="d1e92-130">personImage: The URL of the image</span></span> | <span data-ttu-id="d1e92-131">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="d1e92-131">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="d1e92-132">adicional-detalhes</span><span class="sxs-lookup"><span data-stu-id="d1e92-132">additional-details</span></span> | <span data-ttu-id="d1e92-133">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="d1e92-133">person: The person details object</span></span> <br> <span data-ttu-id="d1e92-134">personImage: a URL da imagem</span><span class="sxs-lookup"><span data-stu-id="d1e92-134">personImage: the URL of the image</span></span> | <span data-ttu-id="d1e92-135">O modelo usado para adicionar conteúdo adicional ao cartão.</span><span class="sxs-lookup"><span data-stu-id="d1e92-135">The template used to add additional content to the card.</span></span> |

<span data-ttu-id="d1e92-136">Por exemplo, você pode usar um modelo para personalizar o componente anexado ao `mgt-person` componente e um modelo para adicionar mais detalhes no cartão.</span><span class="sxs-lookup"><span data-stu-id="d1e92-136">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card person-details="{{person}}" 
            person-image="{{personImage}}">
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

## <a name="css-custom-properties"></a><span data-ttu-id="d1e92-137">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="d1e92-137">CSS custom properties</span></span>

<span data-ttu-id="d1e92-138">O `mgt-person-card` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="d1e92-138">The `mgt-person-card` component defines the following CSS custom properties.</span></span>

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

<span data-ttu-id="d1e92-139">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="d1e92-139">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d1e92-140">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d1e92-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="d1e92-141">Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="d1e92-141">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="d1e92-142">Autenticação</span><span class="sxs-lookup"><span data-stu-id="d1e92-142">Authentication</span></span>

<span data-ttu-id="d1e92-143">O controle de cartão de pessoa usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="d1e92-143">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
