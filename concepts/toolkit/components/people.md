---
title: Componente pessoas no Microsoft Graph Toolkit
description: Você pode usar o `mgt-people` componente da Web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9e19636c6f69784984d7438d53f57bac78fc6675
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660055"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d5d00-103">Componente pessoas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d5d00-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d5d00-104">Você pode usar o `mgt-people` componente da Web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais.</span><span class="sxs-lookup"><span data-stu-id="d5d00-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="d5d00-105">Por padrão, ele exibirá os contatos mais frequentes para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d5d00-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="d5d00-106">Este componente usa vários controles de [pessoal de gerenciamento](./person.md) , mas pode ser vinculado a um conjunto de descritores de pessoas.</span><span class="sxs-lookup"><span data-stu-id="d5d00-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="d5d00-107">Se houver mais pessoas para exibir o `show-max` valor, um número será adicionado para indicar o número de contatos adicionais.</span><span class="sxs-lookup"><span data-stu-id="d5d00-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="d5d00-108">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5d00-108">Example</span></span>

<span data-ttu-id="d5d00-109">O exemplo a seguir mostra um grupo de pessoas exibidas usando o `mgt-people` componente.</span><span class="sxs-lookup"><span data-stu-id="d5d00-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="d5d00-110">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="d5d00-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="d5d00-111">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="d5d00-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="d5d00-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5d00-112">Properties</span></span>

<span data-ttu-id="d5d00-113">Por padrão, o `mgt-people` componente busca eventos do ponto de `/me/people` extremidade com o `personType/class eq 'Person'` filtro para exibir os usuários contatados com frequência.</span><span class="sxs-lookup"><span data-stu-id="d5d00-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="d5d00-114">Você pode usar várias propriedades para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="d5d00-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="d5d00-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="d5d00-115">Attribute</span></span> | <span data-ttu-id="d5d00-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5d00-116">Property</span></span> | <span data-ttu-id="d5d00-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5d00-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d5d00-118">show-Max</span><span class="sxs-lookup"><span data-stu-id="d5d00-118">show-max</span></span> | <span data-ttu-id="d5d00-119">showMax</span><span class="sxs-lookup"><span data-stu-id="d5d00-119">showMax</span></span> | <span data-ttu-id="d5d00-120">Indica o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="d5d00-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="d5d00-121">O valor padrão é 3.</span><span class="sxs-lookup"><span data-stu-id="d5d00-121">Default value is 3.</span></span> |
| <span data-ttu-id="d5d00-122">people</span><span class="sxs-lookup"><span data-stu-id="d5d00-122">people</span></span> | <span data-ttu-id="d5d00-123">people</span><span class="sxs-lookup"><span data-stu-id="d5d00-123">people</span></span> | <span data-ttu-id="d5d00-124">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="d5d00-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="d5d00-125">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="d5d00-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="d5d00-126">Defina esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="d5d00-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="d5d00-127">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="d5d00-127">group-id</span></span> | <span data-ttu-id="d5d00-128">groupId</span><span class="sxs-lookup"><span data-stu-id="d5d00-128">groupId</span></span> | <span data-ttu-id="d5d00-129">Recupera pessoas de um Microsoft Graph específico da respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="d5d00-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="d5d00-130">User-IDs</span><span class="sxs-lookup"><span data-stu-id="d5d00-130">user-ids</span></span> | <span data-ttu-id="d5d00-131">userIds</span><span class="sxs-lookup"><span data-stu-id="d5d00-131">userIds</span></span> | <span data-ttu-id="d5d00-132">Dada uma matriz de usuário do Microsoft Graph `ids` , o componente renderizará esses usuários.</span><span class="sxs-lookup"><span data-stu-id="d5d00-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="d5d00-133">pessoas – consultas</span><span class="sxs-lookup"><span data-stu-id="d5d00-133">people-queries</span></span> | <span data-ttu-id="d5d00-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="d5d00-134">peopleQueries</span></span> | <span data-ttu-id="d5d00-135">Dada uma matriz de consultas de pessoa (nomes, UPNs, emails), o componente renderiza esses usuários.</span><span class="sxs-lookup"><span data-stu-id="d5d00-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="d5d00-136">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="d5d00-136">person-card</span></span> | <span data-ttu-id="d5d00-137">personCard</span><span class="sxs-lookup"><span data-stu-id="d5d00-137">personCard</span></span> | <span data-ttu-id="d5d00-138">Uma enumeração para determinar a ação do usuário necessária para ativar o painel ou o menu suspenso `hover` `click` .</span><span class="sxs-lookup"><span data-stu-id="d5d00-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="d5d00-139">O valor padrão é `none`.</span><span class="sxs-lookup"><span data-stu-id="d5d00-139">Default value is `none`.</span></span> |
| <span data-ttu-id="d5d00-140">show-Presence</span><span class="sxs-lookup"><span data-stu-id="d5d00-140">show-presence</span></span> | <span data-ttu-id="d5d00-141">a presença</span><span class="sxs-lookup"><span data-stu-id="d5d00-141">showPresence</span></span> | <span data-ttu-id="d5d00-142">Um booliano para determinar se deve mostrar o crachá de presença de pessoa na imagem de pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5d00-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="d5d00-143">O exemplo a seguir define o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="d5d00-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="d5d00-144">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="d5d00-144">CSS custom properties</span></span>

<span data-ttu-id="d5d00-145">O `mgt-people` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="d5d00-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="d5d00-146">Modelos</span><span class="sxs-lookup"><span data-stu-id="d5d00-146">Templates</span></span>

<span data-ttu-id="d5d00-147">O `mgt-people` dá suporte a vários [modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="d5d00-147">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="d5d00-148">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="d5d00-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="d5d00-149">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="d5d00-149">Data type</span></span> | <span data-ttu-id="d5d00-150">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="d5d00-150">Data context</span></span> | <span data-ttu-id="d5d00-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5d00-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="d5d00-152">`people`: lista de objetos Person</span><span class="sxs-lookup"><span data-stu-id="d5d00-152">`people`: list of person objects</span></span> | <span data-ttu-id="d5d00-153">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="d5d00-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="d5d00-154">`person`: objeto Person</span><span class="sxs-lookup"><span data-stu-id="d5d00-154">`person`: person object</span></span> | <span data-ttu-id="d5d00-155">O modelo usado para renderizar cada pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5d00-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="d5d00-156">`people`: lista de objetos Person</span><span class="sxs-lookup"><span data-stu-id="d5d00-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="d5d00-157">`max`: número de pessoas mostradas</span><span class="sxs-lookup"><span data-stu-id="d5d00-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="d5d00-158">`extra`: número de pessoas extras</span><span class="sxs-lookup"><span data-stu-id="d5d00-158">`extra`: number of extra people</span></span> | <span data-ttu-id="d5d00-159">O modelo usado para renderizar o número além do máximo à direita da lista de pessoas.</span><span class="sxs-lookup"><span data-stu-id="d5d00-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="d5d00-160">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="d5d00-160">No data context is passed</span></span> | <span data-ttu-id="d5d00-161">O modelo usado quando não há dados disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d5d00-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="d5d00-162">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="d5d00-162">No data context is passed</span></span> | <span data-ttu-id="d5d00-163">O modelo usado enquanto o componente carrega o estado.</span><span class="sxs-lookup"><span data-stu-id="d5d00-163">The template used while the component loads state.</span></span>

<span data-ttu-id="d5d00-164">Os exemplos a seguir mostram como usar o `person` modelo.</span><span class="sxs-lookup"><span data-stu-id="d5d00-164">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d5d00-165">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d5d00-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="d5d00-166">Este componente usa as seguintes APIs e permissões do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="d5d00-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="d5d00-167">Recurso</span><span class="sxs-lookup"><span data-stu-id="d5d00-167">Resource</span></span> | <span data-ttu-id="d5d00-168">Permissão</span><span class="sxs-lookup"><span data-stu-id="d5d00-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="d5d00-169">/me/people</span><span class="sxs-lookup"><span data-stu-id="d5d00-169">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="d5d00-170">Ao usar os modelos padrão, são necessárias APIs e permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="d5d00-170">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="d5d00-171">O modelo padrão para este componente usa um componente de [pessoa de gerenciamento](person.md) , que requer o seguinte.</span><span class="sxs-lookup"><span data-stu-id="d5d00-171">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="d5d00-172">Recurso</span><span class="sxs-lookup"><span data-stu-id="d5d00-172">Resource</span></span> | <span data-ttu-id="d5d00-173">Permissão</span><span class="sxs-lookup"><span data-stu-id="d5d00-173">Permission</span></span> |
| - | - |
| [<span data-ttu-id="d5d00-174">/Users</span><span class="sxs-lookup"><span data-stu-id="d5d00-174">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="d5d00-175">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d5d00-175">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="d5d00-176">Autenticação</span><span class="sxs-lookup"><span data-stu-id="d5d00-176">Authentication</span></span>

<span data-ttu-id="d5d00-177">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="d5d00-177">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="d5d00-178">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="d5d00-178">Extend for more control</span></span>

<span data-ttu-id="d5d00-179">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="d5d00-179">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="d5d00-180">Método</span><span class="sxs-lookup"><span data-stu-id="d5d00-180">Method</span></span> | <span data-ttu-id="d5d00-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5d00-181">Description</span></span> |
| - | - |
| <span data-ttu-id="d5d00-182">renderLoading</span><span class="sxs-lookup"><span data-stu-id="d5d00-182">renderLoading</span></span> | <span data-ttu-id="d5d00-183">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="d5d00-183">Renders the loading state.</span></span> |
| <span data-ttu-id="d5d00-184">renderNoData</span><span class="sxs-lookup"><span data-stu-id="d5d00-184">renderNoData</span></span> | <span data-ttu-id="d5d00-185">Renderiza o estado de dados vazio.</span><span class="sxs-lookup"><span data-stu-id="d5d00-185">Renders the empty data state.</span></span> |
| <span data-ttu-id="d5d00-186">renderPeople</span><span class="sxs-lookup"><span data-stu-id="d5d00-186">renderPeople</span></span> | <span data-ttu-id="d5d00-187">Renderiza uma lista de pessoas, até o `show-max` valor.</span><span class="sxs-lookup"><span data-stu-id="d5d00-187">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="d5d00-188">renderPerson</span><span class="sxs-lookup"><span data-stu-id="d5d00-188">renderPerson</span></span> | <span data-ttu-id="d5d00-189">Renderiza uma pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="d5d00-189">Renders an individual person.</span></span> |
| <span data-ttu-id="d5d00-190">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="d5d00-190">renderOverflow</span></span> | <span data-ttu-id="d5d00-191">Renderiza uma representação de pessoas restantes além do `show-max` valor.</span><span class="sxs-lookup"><span data-stu-id="d5d00-191">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
