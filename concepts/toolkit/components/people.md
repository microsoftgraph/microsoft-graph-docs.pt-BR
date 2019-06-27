---
title: Componente pessoas no Microsoft Graph Toolkit
description: Você pode usar o `mgt-people` componente da Web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: fcc44262f807d3f10f42e8af8e476975ad262cda
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242950"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c4e87-103">Componente pessoas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="c4e87-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c4e87-104">Você pode usar o `mgt-people` componente da Web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais.</span><span class="sxs-lookup"><span data-stu-id="c4e87-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="c4e87-105">Por padrão, ele exibirá os contatos mais frequentes para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c4e87-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="c4e87-106">Este componente usa vários controles de [pessoal de gerenciamento](./person.md) , mas pode ser vinculado a um conjunto de descritores de pessoas.</span><span class="sxs-lookup"><span data-stu-id="c4e87-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="c4e87-107">Se houver mais pessoas para exibir o `show-max` valor, um número será adicionado para indicar o número de contatos adicionais.</span><span class="sxs-lookup"><span data-stu-id="c4e87-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="c4e87-108">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4e87-108">Example</span></span>

[<span data-ttu-id="c4e87-109">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="c4e87-109">jsfiddle example</span></span>](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![gerenciamento-pessoas](./images/mgt-people.png)

## <a name="properties"></a><span data-ttu-id="c4e87-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4e87-111">Properties</span></span>

<span data-ttu-id="c4e87-112">Por padrão, o `mgt-people` componente busca eventos do `/me/people` ponto de extremidade com o `personType/class eq 'Person'` filtro para exibir os usuários contatados com frequência.</span><span class="sxs-lookup"><span data-stu-id="c4e87-112">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="c4e87-113">Você pode usar várias propriedades para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="c4e87-113">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="c4e87-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4e87-114">Property</span></span> | <span data-ttu-id="c4e87-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="c4e87-115">Attribute</span></span> | <span data-ttu-id="c4e87-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4e87-116">Description</span></span> |
| --- | --- | --- |
| `showMax` | `show-max` | <span data-ttu-id="c4e87-117">Indica o número máximo de pessoas a serem exibidas.</span><span class="sxs-lookup"><span data-stu-id="c4e87-117">Indicate the maximum number of people to show.</span></span> <span data-ttu-id="c4e87-118">O valor padrão é 3.</span><span class="sxs-lookup"><span data-stu-id="c4e87-118">Default value is 3.</span></span> |
| `people` | `people` | <span data-ttu-id="c4e87-119">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="c4e87-119">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="c4e87-120">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="c4e87-120">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="c4e87-121">Defina esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="c4e87-121">Set this value to load your own people.</span></span> |

<span data-ttu-id="c4e87-122">O exemplo a seguir define o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="c4e87-122">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="c4e87-123">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="c4e87-123">CSS custom properties</span></span>

<span data-ttu-id="c4e87-124">O `mgt-people` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="c4e87-124">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="c4e87-125">Modelos</span><span class="sxs-lookup"><span data-stu-id="c4e87-125">Templates</span></span>

<span data-ttu-id="c4e87-126">O `mgt-people` dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="c4e87-126">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="c4e87-127">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="c4e87-127">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="c4e87-128">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="c4e87-128">Data type</span></span> | <span data-ttu-id="c4e87-129">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="c4e87-129">Data context</span></span> | <span data-ttu-id="c4e87-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4e87-130">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="c4e87-131">`people`: lista de objetos Person</span><span class="sxs-lookup"><span data-stu-id="c4e87-131">`people`: list of person objects</span></span> | <span data-ttu-id="c4e87-132">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="c4e87-132">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="c4e87-133">`person`: objeto Person</span><span class="sxs-lookup"><span data-stu-id="c4e87-133">`person`: person object</span></span> | <span data-ttu-id="c4e87-134">O modelo usado para renderizar cada pessoa.</span><span class="sxs-lookup"><span data-stu-id="c4e87-134">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="c4e87-135">`people`: lista de objetos Person</span><span class="sxs-lookup"><span data-stu-id="c4e87-135">`people`: list of person objects</span></span> <br> <span data-ttu-id="c4e87-136">`max`: número de pessoas mostradas</span><span class="sxs-lookup"><span data-stu-id="c4e87-136">`max`: number of shown people</span></span> <br> <span data-ttu-id="c4e87-137">`extra`: número de pessoas extras</span><span class="sxs-lookup"><span data-stu-id="c4e87-137">`extra`: number of extra people</span></span> | <span data-ttu-id="c4e87-138">O modelo usado para renderizar o número além do máximo à direita da lista de pessoas.</span><span class="sxs-lookup"><span data-stu-id="c4e87-138">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="c4e87-139">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="c4e87-139">No data context is passed</span></span> | <span data-ttu-id="c4e87-140">O modelo usado quando nenhuma pessoa está disponível.</span><span class="sxs-lookup"><span data-stu-id="c4e87-140">The template used when no people are available.</span></span> |

<span data-ttu-id="c4e87-141">Os exemplos a seguir mostram como usar o `person` modelo.</span><span class="sxs-lookup"><span data-stu-id="c4e87-141">The following examples shows how to use the `person` template.</span></span>

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="c4e87-142">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c4e87-142">Microsoft Graph permissions</span></span>

<span data-ttu-id="c4e87-143">Este componente usa as seguintes APIs e permissões do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="c4e87-143">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="c4e87-144">Resource</span><span class="sxs-lookup"><span data-stu-id="c4e87-144">Resource</span></span> | <span data-ttu-id="c4e87-145">Permissão/escopo</span><span class="sxs-lookup"><span data-stu-id="c4e87-145">Permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="c4e87-146">/me/people</span><span class="sxs-lookup"><span data-stu-id="c4e87-146">/me/people</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="c4e87-147">Autenticação</span><span class="sxs-lookup"><span data-stu-id="c4e87-147">Authentication</span></span>

<span data-ttu-id="c4e87-148">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="c4e87-148">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
