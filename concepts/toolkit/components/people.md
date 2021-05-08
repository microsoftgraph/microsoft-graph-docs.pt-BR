---
title: Componente Pessoas no microsoft graph Toolkit
description: Você pode usar o componente web para exibir um grupo de pessoas ou contatos usando `mgt-people` suas fotos ou iniciais.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0cdade8720112dc623e617514f31ab63151b80ff
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266847"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="5bef1-103">Componente Pessoas no microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="5bef1-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="5bef1-104">Você pode usar o componente web para exibir um grupo de pessoas ou contatos usando `mgt-people` suas fotos ou iniciais.</span><span class="sxs-lookup"><span data-stu-id="5bef1-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="5bef1-105">Por padrão, ele exibirá os contatos mais frequentes para o usuário que entrou.</span><span class="sxs-lookup"><span data-stu-id="5bef1-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="5bef1-106">Esse componente usa vários [controles mgt-person,](./person.md) mas pode ser vinculado a um conjunto de descritores de pessoas.</span><span class="sxs-lookup"><span data-stu-id="5bef1-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="5bef1-107">Se houver mais pessoas para exibir do que o valor, um número será adicionado para indicar o `show-max` número de contatos adicionais.</span><span class="sxs-lookup"><span data-stu-id="5bef1-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="5bef1-108">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bef1-108">Example</span></span>

<span data-ttu-id="5bef1-109">O exemplo a seguir mostra um grupo de pessoas exibidas usando o `mgt-people` componente.</span><span class="sxs-lookup"><span data-stu-id="5bef1-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="5bef1-110">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="5bef1-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="5bef1-111">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="5bef1-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="5bef1-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5bef1-112">Properties</span></span>

<span data-ttu-id="5bef1-113">Por padrão, o componente busca eventos do ponto de extremidade com o filtro para `mgt-people` `/me/people` exibir usuários `personType/class eq 'Person'` contatados com frequência.</span><span class="sxs-lookup"><span data-stu-id="5bef1-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="5bef1-114">Você pode usar várias propriedades para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="5bef1-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="5bef1-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="5bef1-115">Attribute</span></span> | <span data-ttu-id="5bef1-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bef1-116">Property</span></span> | <span data-ttu-id="5bef1-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bef1-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="5bef1-118">show-max</span><span class="sxs-lookup"><span data-stu-id="5bef1-118">show-max</span></span> | <span data-ttu-id="5bef1-119">showMax</span><span class="sxs-lookup"><span data-stu-id="5bef1-119">showMax</span></span> | <span data-ttu-id="5bef1-120">Indica o número máximo de pessoas a mostrar.</span><span class="sxs-lookup"><span data-stu-id="5bef1-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="5bef1-121">O valor padrão é 3.</span><span class="sxs-lookup"><span data-stu-id="5bef1-121">Default value is 3.</span></span> |
| <span data-ttu-id="5bef1-122">people</span><span class="sxs-lookup"><span data-stu-id="5bef1-122">people</span></span> | <span data-ttu-id="5bef1-123">people</span><span class="sxs-lookup"><span data-stu-id="5bef1-123">people</span></span> | <span data-ttu-id="5bef1-124">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="5bef1-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="5bef1-125">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="5bef1-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="5bef1-126">De definir esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="5bef1-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="5bef1-127">group-id</span><span class="sxs-lookup"><span data-stu-id="5bef1-127">group-id</span></span> | <span data-ttu-id="5bef1-128">groupId</span><span class="sxs-lookup"><span data-stu-id="5bef1-128">groupId</span></span> | <span data-ttu-id="5bef1-129">Recupera pessoas de um Microsoft Graph específico da respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="5bef1-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="5bef1-130">user-ids</span><span class="sxs-lookup"><span data-stu-id="5bef1-130">user-ids</span></span> | <span data-ttu-id="5bef1-131">userIds</span><span class="sxs-lookup"><span data-stu-id="5bef1-131">userIds</span></span> | <span data-ttu-id="5bef1-132">Devido a uma matriz de usuário do Microsoft `ids` Graph, o componente renderizará esses usuários.</span><span class="sxs-lookup"><span data-stu-id="5bef1-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="5bef1-133">people-queries</span><span class="sxs-lookup"><span data-stu-id="5bef1-133">people-queries</span></span> | <span data-ttu-id="5bef1-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="5bef1-134">peopleQueries</span></span> | <span data-ttu-id="5bef1-135">Devido a uma matriz de consultas de pessoas (nomes, upns, emails), o componente renderizará esses usuários.</span><span class="sxs-lookup"><span data-stu-id="5bef1-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="5bef1-136">person-card</span><span class="sxs-lookup"><span data-stu-id="5bef1-136">person-card</span></span> | <span data-ttu-id="5bef1-137">personCard</span><span class="sxs-lookup"><span data-stu-id="5bef1-137">personCard</span></span> | <span data-ttu-id="5bef1-138">Uma enumeração para determinar a ação do usuário necessária para ativar o painel do sub-sub-plano - `hover` ou `click` .</span><span class="sxs-lookup"><span data-stu-id="5bef1-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="5bef1-139">O valor padrão é `none`.</span><span class="sxs-lookup"><span data-stu-id="5bef1-139">Default value is `none`.</span></span> |
| <span data-ttu-id="5bef1-140">show-presence</span><span class="sxs-lookup"><span data-stu-id="5bef1-140">show-presence</span></span> | <span data-ttu-id="5bef1-141">showPresence</span><span class="sxs-lookup"><span data-stu-id="5bef1-141">showPresence</span></span> | <span data-ttu-id="5bef1-142">Um booleano para determinar se deve mostrar o selo de presença da pessoa na imagem da pessoa.</span><span class="sxs-lookup"><span data-stu-id="5bef1-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="5bef1-143">O exemplo a seguir define o número máximo de pessoas a mostrar.</span><span class="sxs-lookup"><span data-stu-id="5bef1-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="5bef1-144">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="5bef1-144">CSS custom properties</span></span>

<span data-ttu-id="5bef1-145">O `mgt-people` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="5bef1-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="5bef1-146">Modelos</span><span class="sxs-lookup"><span data-stu-id="5bef1-146">Templates</span></span>

<span data-ttu-id="5bef1-147">O `mgt-people` suporte a vários modelos [que](../customize-components/templates.md) você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="5bef1-147">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="5bef1-148">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.</span><span class="sxs-lookup"><span data-stu-id="5bef1-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="5bef1-149">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="5bef1-149">Data type</span></span> | <span data-ttu-id="5bef1-150">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="5bef1-150">Data context</span></span> | <span data-ttu-id="5bef1-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bef1-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="5bef1-152">`people`: lista de objetos de pessoa</span><span class="sxs-lookup"><span data-stu-id="5bef1-152">`people`: list of person objects</span></span> | <span data-ttu-id="5bef1-153">O modelo padrão substitui todo o componente por seu próprio.</span><span class="sxs-lookup"><span data-stu-id="5bef1-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="5bef1-154">`person`: objeto person</span><span class="sxs-lookup"><span data-stu-id="5bef1-154">`person`: person object</span></span> | <span data-ttu-id="5bef1-155">O modelo usado para renderizar cada pessoa.</span><span class="sxs-lookup"><span data-stu-id="5bef1-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="5bef1-156">`people`: lista de objetos de pessoa</span><span class="sxs-lookup"><span data-stu-id="5bef1-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="5bef1-157">`max`: número de pessoas mostradas</span><span class="sxs-lookup"><span data-stu-id="5bef1-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="5bef1-158">`extra`: número de pessoas extras</span><span class="sxs-lookup"><span data-stu-id="5bef1-158">`extra`: number of extra people</span></span> | <span data-ttu-id="5bef1-159">O modelo usado para renderizar o número além do máximo à direita da lista de pessoas.</span><span class="sxs-lookup"><span data-stu-id="5bef1-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="5bef1-160">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="5bef1-160">No data context is passed</span></span> | <span data-ttu-id="5bef1-161">O modelo usado quando nenhum dado está disponível.</span><span class="sxs-lookup"><span data-stu-id="5bef1-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="5bef1-162">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="5bef1-162">No data context is passed</span></span> | <span data-ttu-id="5bef1-163">O modelo usado enquanto o componente carrega o estado.</span><span class="sxs-lookup"><span data-stu-id="5bef1-163">The template used while the component loads state.</span></span>

<span data-ttu-id="5bef1-164">Os exemplos a seguir mostram como usar o `person` modelo.</span><span class="sxs-lookup"><span data-stu-id="5bef1-164">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="5bef1-165">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5bef1-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="5bef1-166">Este componente usa as seguintes APIs e permissões do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="5bef1-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="5bef1-167">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bef1-167">Resource</span></span> | <span data-ttu-id="5bef1-168">Permissão</span><span class="sxs-lookup"><span data-stu-id="5bef1-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="5bef1-169">/me/people</span><span class="sxs-lookup"><span data-stu-id="5bef1-169">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="5bef1-170">Ao usar os modelos padrão, APIs e permissões adicionais são necessárias.</span><span class="sxs-lookup"><span data-stu-id="5bef1-170">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="5bef1-171">O modelo padrão para esse componente usa um [componente mgt-person,](person.md) que exige o seguinte.</span><span class="sxs-lookup"><span data-stu-id="5bef1-171">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="5bef1-172">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bef1-172">Resource</span></span> | <span data-ttu-id="5bef1-173">Permissão</span><span class="sxs-lookup"><span data-stu-id="5bef1-173">Permission</span></span> |
| - | - |
| [<span data-ttu-id="5bef1-174">/users</span><span class="sxs-lookup"><span data-stu-id="5bef1-174">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="5bef1-175">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="5bef1-175">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="5bef1-176">Autenticação</span><span class="sxs-lookup"><span data-stu-id="5bef1-176">Authentication</span></span>

<span data-ttu-id="5bef1-177">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="5bef1-177">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="5bef1-178">Cache</span><span class="sxs-lookup"><span data-stu-id="5bef1-178">Cache</span></span>

|<span data-ttu-id="5bef1-179">Armazenamento de objetos</span><span class="sxs-lookup"><span data-stu-id="5bef1-179">Object store</span></span>|<span data-ttu-id="5bef1-180">Dados armazenados em cache</span><span class="sxs-lookup"><span data-stu-id="5bef1-180">Cached data</span></span>|<span data-ttu-id="5bef1-181">Comentários</span><span class="sxs-lookup"><span data-stu-id="5bef1-181">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="5bef1-182">Informações sobre pessoas que coincidem com a consulta</span><span class="sxs-lookup"><span data-stu-id="5bef1-182">Information about people matching the query</span></span>|<span data-ttu-id="5bef1-183">Usado quando `resource` especificado</span><span class="sxs-lookup"><span data-stu-id="5bef1-183">Used when `resource` specified</span></span>|
|`users`|<span data-ttu-id="5bef1-184">Informações sobre usuários correspondentes à consulta</span><span class="sxs-lookup"><span data-stu-id="5bef1-184">Information about users matching the query</span></span>|<span data-ttu-id="5bef1-185">Usado quando `groupId` , ou nenhuma propriedade `userIds` `peopleQueries` especificada</span><span class="sxs-lookup"><span data-stu-id="5bef1-185">Used when `groupId`, `userIds`, `peopleQueries` or no properties specified</span></span>|
|`presence`|<span data-ttu-id="5bef1-186">Presença para o conjunto especificado de pessoas</span><span class="sxs-lookup"><span data-stu-id="5bef1-186">Presence for the specified set of people</span></span>|<span data-ttu-id="5bef1-187">Usado quando `showPresence` definido como `true`</span><span class="sxs-lookup"><span data-stu-id="5bef1-187">Used when `showPresence` set to `true`</span></span>|

> [!NOTE]
> <span data-ttu-id="5bef1-188">Por padrão, o `mgt-people` componente usa o componente para exibir informações sobre [`mgt-person`](./person.md) pessoas.</span><span class="sxs-lookup"><span data-stu-id="5bef1-188">By default, the `mgt-people` component uses the [`mgt-person`](./person.md) component to display information about people.</span></span> <span data-ttu-id="5bef1-189">O `mgt-person` componente baixa automaticamente e armazena em cache a foto para cada pessoa.</span><span class="sxs-lookup"><span data-stu-id="5bef1-189">The `mgt-person` component automatically downloads and caches the photo for each person.</span></span>

<span data-ttu-id="5bef1-190">Consulte [Cache para](../customize-components/cache.md) obter mais detalhes sobre como configurar o cache.</span><span class="sxs-lookup"><span data-stu-id="5bef1-190">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="5bef1-191">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="5bef1-191">Extend for more control</span></span>

<span data-ttu-id="5bef1-192">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.</span><span class="sxs-lookup"><span data-stu-id="5bef1-192">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="5bef1-193">Método</span><span class="sxs-lookup"><span data-stu-id="5bef1-193">Method</span></span> | <span data-ttu-id="5bef1-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bef1-194">Description</span></span> |
| - | - |
| <span data-ttu-id="5bef1-195">renderLoading</span><span class="sxs-lookup"><span data-stu-id="5bef1-195">renderLoading</span></span> | <span data-ttu-id="5bef1-196">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="5bef1-196">Renders the loading state.</span></span> |
| <span data-ttu-id="5bef1-197">renderNoData</span><span class="sxs-lookup"><span data-stu-id="5bef1-197">renderNoData</span></span> | <span data-ttu-id="5bef1-198">Renderiza o estado de dados vazio.</span><span class="sxs-lookup"><span data-stu-id="5bef1-198">Renders the empty data state.</span></span> |
| <span data-ttu-id="5bef1-199">renderPeople</span><span class="sxs-lookup"><span data-stu-id="5bef1-199">renderPeople</span></span> | <span data-ttu-id="5bef1-200">Renderiza uma lista de pessoas, até o `show-max` valor.</span><span class="sxs-lookup"><span data-stu-id="5bef1-200">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="5bef1-201">renderPerson</span><span class="sxs-lookup"><span data-stu-id="5bef1-201">renderPerson</span></span> | <span data-ttu-id="5bef1-202">Renderiza uma pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="5bef1-202">Renders an individual person.</span></span> |
| <span data-ttu-id="5bef1-203">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="5bef1-203">renderOverflow</span></span> | <span data-ttu-id="5bef1-204">Renderiza uma representação de pessoas restantes além do `show-max` valor.</span><span class="sxs-lookup"><span data-stu-id="5bef1-204">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
