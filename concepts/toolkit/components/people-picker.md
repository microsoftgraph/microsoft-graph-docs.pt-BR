---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 175370b3c00ebaef0db85912c032898e2dacb5e7
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144300"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="61d5c-103">Componente de seletor de pessoas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="61d5c-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="61d5c-104">Você pode usar a `mgt-people-picker` pesquisa de componente da Web para um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="61d5c-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="61d5c-105">Por padrão, o componente pesquisará todas as pessoas; Você também pode definir uma propriedade de grupo para filtrar os resultados.</span><span class="sxs-lookup"><span data-stu-id="61d5c-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="61d5c-106">Se o número de pessoas a serem exibidas exceder o `show-max` valor, nem todas as pessoas retornadas serão exibidas na lista de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="61d5c-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="61d5c-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61d5c-107">Example</span></span>

<span data-ttu-id="61d5c-108">O exemplo a seguir mostra `mgt-people-picker` o componente.</span><span class="sxs-lookup"><span data-stu-id="61d5c-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="61d5c-109">Comece a pesquisar um nome para ver os resultados renderizar e usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="61d5c-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="61d5c-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="61d5c-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="61d5c-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61d5c-111">Properties</span></span>

<span data-ttu-id="61d5c-112">Por padrão, o `mgt-people-picker` componente busca eventos do `/me/people` ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="61d5c-112">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="61d5c-113">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="61d5c-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="61d5c-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="61d5c-114">Attribute</span></span> | <span data-ttu-id="61d5c-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61d5c-115">Property</span></span> | <span data-ttu-id="61d5c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d5c-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="61d5c-117">show-Max</span><span class="sxs-lookup"><span data-stu-id="61d5c-117">show-max</span></span> | <span data-ttu-id="61d5c-118">showMax</span><span class="sxs-lookup"><span data-stu-id="61d5c-118">showMax</span></span>   | <span data-ttu-id="61d5c-119">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="61d5c-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="61d5c-120">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="61d5c-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="61d5c-121">people</span><span class="sxs-lookup"><span data-stu-id="61d5c-121">people</span></span>   | <span data-ttu-id="61d5c-122">people</span><span class="sxs-lookup"><span data-stu-id="61d5c-122">people</span></span>    | <span data-ttu-id="61d5c-123">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="61d5c-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="61d5c-124">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="61d5c-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="61d5c-125">Defina esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="61d5c-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="61d5c-126">group</span><span class="sxs-lookup"><span data-stu-id="61d5c-126">group</span></span>    | <span data-ttu-id="61d5c-127">group</span><span class="sxs-lookup"><span data-stu-id="61d5c-127">group</span></span>     | <span data-ttu-id="61d5c-128">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="61d5c-128">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="61d5c-129">selecionado-pessoas</span><span class="sxs-lookup"><span data-stu-id="61d5c-129">selected-people</span></span>  | <span data-ttu-id="61d5c-130">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="61d5c-130">selectedPeople</span></span>     | <span data-ttu-id="61d5c-131">Uma matriz do tipo `person`, representando pessoas selecionadas no componente.</span><span class="sxs-lookup"><span data-stu-id="61d5c-131">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="61d5c-132">Defina esse valor para escolher as pessoas selecionadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="61d5c-132">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="61d5c-133">Este é um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="61d5c-133">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="61d5c-134">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="61d5c-134">Selected people</span></span>

<span data-ttu-id="61d5c-135">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="61d5c-135">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

<span data-ttu-id="61d5c-137">Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="61d5c-137">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="61d5c-138">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="61d5c-138">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="61d5c-139">Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.</span><span class="sxs-lookup"><span data-stu-id="61d5c-139">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="61d5c-140">**Observação:** Se nenhum usuário for localizado para um `id`, nenhum dado será renderizado para isso `id`.</span><span class="sxs-lookup"><span data-stu-id="61d5c-140">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="61d5c-141">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="61d5c-141">CSS custom properties</span></span>

<span data-ttu-id="61d5c-142">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="61d5c-142">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="61d5c-143">Modelos</span><span class="sxs-lookup"><span data-stu-id="61d5c-143">Templates</span></span>

 <span data-ttu-id="61d5c-144">`mgt-people-picker`o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="61d5c-144">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="61d5c-145">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="61d5c-145">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="61d5c-146">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="61d5c-146">Data type</span></span> | <span data-ttu-id="61d5c-147">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="61d5c-147">Data context</span></span> | <span data-ttu-id="61d5c-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d5c-148">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="61d5c-149">Padrão.</span><span class="sxs-lookup"><span data-stu-id="61d5c-149">default</span></span> | <span data-ttu-id="61d5c-150">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="61d5c-150">null: no data</span></span> | <span data-ttu-id="61d5c-151">O modelo usado para substituir a renderização de todo o componente.</span><span class="sxs-lookup"><span data-stu-id="61d5c-151">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="61d5c-152">carregando</span><span class="sxs-lookup"><span data-stu-id="61d5c-152">loading</span></span> | <span data-ttu-id="61d5c-153">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="61d5c-153">null: no data</span></span> | <span data-ttu-id="61d5c-154">O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="61d5c-154">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="61d5c-155">erro</span><span class="sxs-lookup"><span data-stu-id="61d5c-155">error</span></span> | <span data-ttu-id="61d5c-156">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="61d5c-156">null: no data</span></span> | <span data-ttu-id="61d5c-157">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="61d5c-157">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="61d5c-158">sem dados</span><span class="sxs-lookup"><span data-stu-id="61d5c-158">no-data</span></span> | <span data-ttu-id="61d5c-159">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="61d5c-159">null: no data</span></span> | <span data-ttu-id="61d5c-160">Um modelo alternativo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="61d5c-160">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="61d5c-161">selecionado-pessoa</span><span class="sxs-lookup"><span data-stu-id="61d5c-161">selected-person</span></span> | <span data-ttu-id="61d5c-162">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="61d5c-162">person: The person details object</span></span> | <span data-ttu-id="61d5c-163">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="61d5c-163">The template to render selected people.</span></span> |
| <span data-ttu-id="61d5c-164">person</span><span class="sxs-lookup"><span data-stu-id="61d5c-164">person</span></span> | <span data-ttu-id="61d5c-165">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="61d5c-165">person: The person details object</span></span> | <span data-ttu-id="61d5c-166">O modelo para renderizar pessoas na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="61d5c-166">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="61d5c-167">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="61d5c-167">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="61d5c-168">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="61d5c-168">Microsoft Graph permissions</span></span>

<span data-ttu-id="61d5c-169">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="61d5c-169">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="61d5c-170">API</span><span class="sxs-lookup"><span data-stu-id="61d5c-170">API</span></span>                                                                                                              | <span data-ttu-id="61d5c-171">Permissão</span><span class="sxs-lookup"><span data-stu-id="61d5c-171">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="61d5c-172">/me/people</span><span class="sxs-lookup"><span data-stu-id="61d5c-172">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="61d5c-173">People.Read</span><span class="sxs-lookup"><span data-stu-id="61d5c-173">People.Read</span></span>        |
| [<span data-ttu-id="61d5c-174">/groups/\${GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="61d5c-174">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="61d5c-175">People.Read</span><span class="sxs-lookup"><span data-stu-id="61d5c-175">People.Read</span></span>        |
| [<span data-ttu-id="61d5c-176">/Users/$ {userprincípioname}</span><span class="sxs-lookup"><span data-stu-id="61d5c-176">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="61d5c-177">User. Readbasic. All</span><span class="sxs-lookup"><span data-stu-id="61d5c-177">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="61d5c-178">Autenticação</span><span class="sxs-lookup"><span data-stu-id="61d5c-178">Authentication</span></span>

<span data-ttu-id="61d5c-179">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="61d5c-179">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="61d5c-180">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="61d5c-180">Extend for more control</span></span>

<span data-ttu-id="61d5c-181">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="61d5c-181">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="61d5c-182">Método</span><span class="sxs-lookup"><span data-stu-id="61d5c-182">Method</span></span> | <span data-ttu-id="61d5c-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d5c-183">Description</span></span> |
| - | - |
| <span data-ttu-id="61d5c-184">renderInput</span><span class="sxs-lookup"><span data-stu-id="61d5c-184">renderInput</span></span> | <span data-ttu-id="61d5c-185">Renderiza a caixa de texto de entrada.</span><span class="sxs-lookup"><span data-stu-id="61d5c-185">Renders the input text box.</span></span> |
| <span data-ttu-id="61d5c-186">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="61d5c-186">renderSelectedPeople</span></span> | <span data-ttu-id="61d5c-187">Renderiza os tokens de pessoas selecionados.</span><span class="sxs-lookup"><span data-stu-id="61d5c-187">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="61d5c-188">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="61d5c-188">renderSelectedPerson</span></span> | <span data-ttu-id="61d5c-189">Renderiza um token de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="61d5c-189">Renders an individual person token.</span></span> |
| <span data-ttu-id="61d5c-190">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="61d5c-190">renderFlyout</span></span> | <span data-ttu-id="61d5c-191">Renderiza o cromo domenu.</span><span class="sxs-lookup"><span data-stu-id="61d5c-191">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="61d5c-192">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="61d5c-192">renderFlyoutContent</span></span> | <span data-ttu-id="61d5c-193">Processa o estado apropriado no submenu de resultados.</span><span class="sxs-lookup"><span data-stu-id="61d5c-193">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="61d5c-194">renderLoading</span><span class="sxs-lookup"><span data-stu-id="61d5c-194">renderLoading</span></span> | <span data-ttu-id="61d5c-195">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="61d5c-195">Renders the loading state.</span></span> |
| <span data-ttu-id="61d5c-196">renderNoData</span><span class="sxs-lookup"><span data-stu-id="61d5c-196">renderNoData</span></span> | <span data-ttu-id="61d5c-197">Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="61d5c-197">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="61d5c-198">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="61d5c-198">renderSearchResults</span></span> | <span data-ttu-id="61d5c-199">Renderiza a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="61d5c-199">Renders the list of search results.</span></span> |
| <span data-ttu-id="61d5c-200">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="61d5c-200">renderPersonResult</span></span> | <span data-ttu-id="61d5c-201">Renderiza um resultado de pesquisa de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="61d5c-201">Renders an individual person search result.</span></span> |
