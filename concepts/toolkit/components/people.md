---
title: Componente pessoas no Microsoft Graph Toolkit
description: Você pode usar o `mgt-people` componente da Web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5f85f0a72e8658a8fc734728ae76d79157da39de
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955873"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="a4f0f-103">Componente pessoas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="a4f0f-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a4f0f-104">Você pode usar o `mgt-people` componente da Web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="a4f0f-105">Por padrão, ele exibirá os contatos mais frequentes para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="a4f0f-106">Este componente usa vários controles de [pessoal de gerenciamento](./person.md) , mas pode ser vinculado a um conjunto de descritores de pessoas.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="a4f0f-107">Se houver mais pessoas para exibir o `show-max` valor, um número será adicionado para indicar o número de contatos adicionais.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="a4f0f-108">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4f0f-108">Example</span></span>

[<span data-ttu-id="a4f0f-109">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="a4f0f-109">jsfiddle example</span></span>](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![gerenciamento-pessoas](./images/mgt-people.png)

## <a name="properties"></a><span data-ttu-id="a4f0f-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4f0f-111">Properties</span></span>

<span data-ttu-id="a4f0f-112">Por padrão, o `mgt-people` componente busca eventos do `/me/people` ponto de extremidade com o `personType/class eq 'Person'` filtro para exibir os usuários contatados com frequência.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-112">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="a4f0f-113">Você pode usar várias propriedades para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-113">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="a4f0f-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="a4f0f-114">Attribute</span></span> | <span data-ttu-id="a4f0f-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4f0f-115">Property</span></span> | <span data-ttu-id="a4f0f-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4f0f-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a4f0f-117">show-Max</span><span class="sxs-lookup"><span data-stu-id="a4f0f-117">show-max</span></span> | <span data-ttu-id="a4f0f-118">showMax</span><span class="sxs-lookup"><span data-stu-id="a4f0f-118">showMax</span></span> | <span data-ttu-id="a4f0f-119">Indica o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-119">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="a4f0f-120">O valor padrão é 3.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-120">Default value is 3.</span></span> |
| <span data-ttu-id="a4f0f-121">people</span><span class="sxs-lookup"><span data-stu-id="a4f0f-121">people</span></span> | <span data-ttu-id="a4f0f-122">people</span><span class="sxs-lookup"><span data-stu-id="a4f0f-122">people</span></span> | <span data-ttu-id="a4f0f-123">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="a4f0f-124">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="a4f0f-125">Defina esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="a4f0f-126">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="a4f0f-126">group-id</span></span> | <span data-ttu-id="a4f0f-127">groupId</span><span class="sxs-lookup"><span data-stu-id="a4f0f-127">groupId</span></span> | <span data-ttu-id="a4f0f-128">Recupera pessoas de um Microsoft Graph específico da respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-128">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="a4f0f-129">User-IDs</span><span class="sxs-lookup"><span data-stu-id="a4f0f-129">user-ids</span></span> | <span data-ttu-id="a4f0f-130">userIds</span><span class="sxs-lookup"><span data-stu-id="a4f0f-130">userIds</span></span> | <span data-ttu-id="a4f0f-131">Dada uma matriz de usuário `ids`do Microsoft Graph, o componente renderizará esses usuários.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-131">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="a4f0f-132">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="a4f0f-132">person-card</span></span> | <span data-ttu-id="a4f0f-133">personCard</span><span class="sxs-lookup"><span data-stu-id="a4f0f-133">personCard</span></span> | <span data-ttu-id="a4f0f-134">Uma enumeração para determinar a ação do usuário necessária para ativar o `hover` painel `click`ou o menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-134">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="a4f0f-135">O valor padrão é `none`.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-135">Default value is `none`.</span></span> |


<span data-ttu-id="a4f0f-136">O exemplo a seguir define o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-136">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="a4f0f-137">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="a4f0f-137">CSS custom properties</span></span>

<span data-ttu-id="a4f0f-138">O `mgt-people` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-138">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="a4f0f-139">Modelos</span><span class="sxs-lookup"><span data-stu-id="a4f0f-139">Templates</span></span>

<span data-ttu-id="a4f0f-140">O `mgt-people` dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-140">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="a4f0f-141">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-141">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="a4f0f-142">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="a4f0f-142">Data type</span></span> | <span data-ttu-id="a4f0f-143">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="a4f0f-143">Data context</span></span> | <span data-ttu-id="a4f0f-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4f0f-144">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="a4f0f-145">`people`: lista de objetos Person</span><span class="sxs-lookup"><span data-stu-id="a4f0f-145">`people`: list of person objects</span></span> | <span data-ttu-id="a4f0f-146">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-146">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="a4f0f-147">`person`: objeto Person</span><span class="sxs-lookup"><span data-stu-id="a4f0f-147">`person`: person object</span></span> | <span data-ttu-id="a4f0f-148">O modelo usado para renderizar cada pessoa.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-148">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="a4f0f-149">`people`: lista de objetos Person</span><span class="sxs-lookup"><span data-stu-id="a4f0f-149">`people`: list of person objects</span></span> <br> <span data-ttu-id="a4f0f-150">`max`: número de pessoas mostradas</span><span class="sxs-lookup"><span data-stu-id="a4f0f-150">`max`: number of shown people</span></span> <br> <span data-ttu-id="a4f0f-151">`extra`: número de pessoas extras</span><span class="sxs-lookup"><span data-stu-id="a4f0f-151">`extra`: number of extra people</span></span> | <span data-ttu-id="a4f0f-152">O modelo usado para renderizar o número além do máximo à direita da lista de pessoas.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-152">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="a4f0f-153">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="a4f0f-153">No data context is passed</span></span> | <span data-ttu-id="a4f0f-154">O modelo usado quando não há dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-154">The template used when no data is available.</span></span> |

<span data-ttu-id="a4f0f-155">Os exemplos a seguir mostram como usar o `person` modelo.</span><span class="sxs-lookup"><span data-stu-id="a4f0f-155">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="a4f0f-156">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a4f0f-156">Microsoft Graph permissions</span></span>

<span data-ttu-id="a4f0f-157">Este componente usa as seguintes APIs e permissões do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="a4f0f-157">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="a4f0f-158">Resource</span><span class="sxs-lookup"><span data-stu-id="a4f0f-158">Resource</span></span> | <span data-ttu-id="a4f0f-159">Permissão</span><span class="sxs-lookup"><span data-stu-id="a4f0f-159">Permission</span></span> |
| - | - |
| [<span data-ttu-id="a4f0f-160">/me/people</span><span class="sxs-lookup"><span data-stu-id="a4f0f-160">/me/people</span></span>](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="a4f0f-161">People.Read</span><span class="sxs-lookup"><span data-stu-id="a4f0f-161">People.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="a4f0f-162">Autenticação</span><span class="sxs-lookup"><span data-stu-id="a4f0f-162">Authentication</span></span>

<span data-ttu-id="a4f0f-163">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="a4f0f-163">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
