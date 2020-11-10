---
title: People-Picker componente
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 9f47824d62ee5ffcf57884af5e68b255756d5478
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975774"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="eaa5e-103">People-Picker componente no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="eaa5e-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="eaa5e-104">Você pode usar o `mgt-people-picker` componente da Web para procurar pessoas e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="eaa5e-105">Por padrão, o componente pesquisará todas as pessoas e usuários da organização, mas você pode alterar o comportamento para também pesquisar grupos ou apenas grupos.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="eaa5e-106">Você também pode filtrar a pesquisa para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="eaa5e-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaa5e-107">Example</span></span>

<span data-ttu-id="eaa5e-108">O exemplo a seguir mostra o `mgt-people-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="eaa5e-109">Comece a pesquisar um nome para ver os resultados renderizar e usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="eaa5e-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="eaa5e-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="eaa5e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eaa5e-111">Properties</span></span>

<span data-ttu-id="eaa5e-112">Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos de `/me/people` `/users` extremidade e.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="eaa5e-113">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="eaa5e-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="eaa5e-114">Attribute</span></span> | <span data-ttu-id="eaa5e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaa5e-115">Property</span></span> | <span data-ttu-id="eaa5e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa5e-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="eaa5e-117">show-Max</span><span class="sxs-lookup"><span data-stu-id="eaa5e-117">show-max</span></span> | <span data-ttu-id="eaa5e-118">showMax</span><span class="sxs-lookup"><span data-stu-id="eaa5e-118">showMax</span></span>   | <span data-ttu-id="eaa5e-119">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="eaa5e-120">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="eaa5e-121">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="eaa5e-121">group-id</span></span>    | <span data-ttu-id="eaa5e-122">groupId</span><span class="sxs-lookup"><span data-stu-id="eaa5e-122">groupId</span></span>     | <span data-ttu-id="eaa5e-123">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="eaa5e-124">tipo</span><span class="sxs-lookup"><span data-stu-id="eaa5e-124">type</span></span>     | <span data-ttu-id="eaa5e-125">tipo</span><span class="sxs-lookup"><span data-stu-id="eaa5e-125">type</span></span>      | <span data-ttu-id="eaa5e-126">O tipo de entidades a serem pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-126">The type of entities to search for.</span></span> <span data-ttu-id="eaa5e-127">As opções disponíveis são: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="eaa5e-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="eaa5e-128">O valor padrão é `person`.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-128">Default value is `person`.</span></span> <span data-ttu-id="eaa5e-129">Este atributo não terá efeito se a `group-id` propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-129">This attribute has no effect if `group-id` property is set.</span></span>                                                                            |
| <span data-ttu-id="eaa5e-130">tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="eaa5e-130">group-type</span></span>     | <span data-ttu-id="eaa5e-131">groupType</span><span class="sxs-lookup"><span data-stu-id="eaa5e-131">groupType</span></span>      | <span data-ttu-id="eaa5e-132">O tipo de grupo a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-132">The group type to search for.</span></span> <span data-ttu-id="eaa5e-133">As opções disponíveis são: `unified` , `security` , `mailenabledsecurity` , `distribution` , `any` .</span><span class="sxs-lookup"><span data-stu-id="eaa5e-133">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="eaa5e-134">O valor padrão é `any`.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-134">Default value is `any`.</span></span> <span data-ttu-id="eaa5e-135">Este atributo não terá efeito se a `type` propriedade for definida como `person` .</span><span class="sxs-lookup"><span data-stu-id="eaa5e-135">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="eaa5e-136">selecionado-pessoas</span><span class="sxs-lookup"><span data-stu-id="eaa5e-136">selected-people</span></span>  | <span data-ttu-id="eaa5e-137">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="eaa5e-137">selectedPeople</span></span>     | <span data-ttu-id="eaa5e-138">Uma matriz de pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-138">An array of selected people.</span></span> <span data-ttu-id="eaa5e-139">Defina esse valor para selecionar pessoas de forma programática.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-139">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="eaa5e-140">people</span><span class="sxs-lookup"><span data-stu-id="eaa5e-140">people</span></span>   | <span data-ttu-id="eaa5e-141">people</span><span class="sxs-lookup"><span data-stu-id="eaa5e-141">people</span></span>    | <span data-ttu-id="eaa5e-142">Uma matriz de pessoas encontrada e renderizada no resultado da pesquisa</span><span class="sxs-lookup"><span data-stu-id="eaa5e-142">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="eaa5e-143">default-Selected-User-IDs</span><span class="sxs-lookup"><span data-stu-id="eaa5e-143">default-selected-user-ids</span></span> | <span data-ttu-id="eaa5e-144">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="eaa5e-144">defaultSelectedUserIds</span></span> | <span data-ttu-id="eaa5e-145">Quando é fornecida uma cadeia de caracteres de IDs de usuário separadas por vírgulas do Microsoft Graph, o componente renderiza os respectivos usuários como selecionados na inicialização.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-145">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="eaa5e-146">modo de seleção</span><span class="sxs-lookup"><span data-stu-id="eaa5e-146">selection-mode</span></span> | <span data-ttu-id="eaa5e-147">selectionMode</span><span class="sxs-lookup"><span data-stu-id="eaa5e-147">selectionMode</span></span> | <span data-ttu-id="eaa5e-148">Usado para indicar se é permitido selecionar vários usuários ou apenas um único usuário.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-148">Used to indicate whether to allow selecting multiple users or just a single user.</span></span> <span data-ttu-id="eaa5e-149">As opções disponíveis são: `single` , `multiple` .</span><span class="sxs-lookup"><span data-stu-id="eaa5e-149">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="eaa5e-150">O valor padrão é `multiple`.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-150">Default value is `multiple`.</span></span>
| <span data-ttu-id="eaa5e-151">PlaceHolder</span><span class="sxs-lookup"><span data-stu-id="eaa5e-151">placeholder</span></span> | <span data-ttu-id="eaa5e-152">PlaceHolder</span><span class="sxs-lookup"><span data-stu-id="eaa5e-152">placeholder</span></span> | <span data-ttu-id="eaa5e-153">O texto padrão que aparece para explicar como usar o componente.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-153">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="eaa5e-154">O valor padrão é `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-154">Default value is `Start typing a name`.</span></span>

<span data-ttu-id="eaa5e-155">Este é um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-155">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="eaa5e-156">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="eaa5e-156">Selected people</span></span>

<span data-ttu-id="eaa5e-157">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-157">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

<span data-ttu-id="eaa5e-159">Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="eaa5e-159">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="eaa5e-160">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-160">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="eaa5e-161">Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](/graph/api/resources/users?view=graph-rest-1.0) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-161">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="eaa5e-162">**Observação:** Se nenhum usuário for localizado para um `id` , nenhum dado será renderizado para isso `id` .</span><span class="sxs-lookup"><span data-stu-id="eaa5e-162">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="eaa5e-163">Eventos</span><span class="sxs-lookup"><span data-stu-id="eaa5e-163">Events</span></span>

<span data-ttu-id="eaa5e-164">Os eventos a seguir são acionados do componente.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-164">The following events are fired from the component.</span></span>

| <span data-ttu-id="eaa5e-165">Evento</span><span class="sxs-lookup"><span data-stu-id="eaa5e-165">Event</span></span> | <span data-ttu-id="eaa5e-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa5e-166">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="eaa5e-167">O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/escolhidas.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-167">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="eaa5e-168">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="eaa5e-168">CSS custom properties</span></span>

<span data-ttu-id="eaa5e-169">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-169">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a><span data-ttu-id="eaa5e-170">Modelos</span><span class="sxs-lookup"><span data-stu-id="eaa5e-170">Templates</span></span>

 <span data-ttu-id="eaa5e-171">`mgt-people-picker` o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-171">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="eaa5e-172">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-172">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="eaa5e-173">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="eaa5e-173">Data type</span></span> | <span data-ttu-id="eaa5e-174">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="eaa5e-174">Data context</span></span> | <span data-ttu-id="eaa5e-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa5e-175">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="eaa5e-176">Padrão.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-176">default</span></span> | <span data-ttu-id="eaa5e-177">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="eaa5e-177">null: no data</span></span> | <span data-ttu-id="eaa5e-178">O modelo usado para substituir a renderização de todo o componente.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-178">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="eaa5e-179">carregando</span><span class="sxs-lookup"><span data-stu-id="eaa5e-179">loading</span></span> | <span data-ttu-id="eaa5e-180">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="eaa5e-180">null: no data</span></span> | <span data-ttu-id="eaa5e-181">O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-181">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="eaa5e-182">erro</span><span class="sxs-lookup"><span data-stu-id="eaa5e-182">error</span></span> | <span data-ttu-id="eaa5e-183">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="eaa5e-183">null: no data</span></span> | <span data-ttu-id="eaa5e-184">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-184">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="eaa5e-185">sem dados</span><span class="sxs-lookup"><span data-stu-id="eaa5e-185">no-data</span></span> | <span data-ttu-id="eaa5e-186">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="eaa5e-186">null: no data</span></span> | <span data-ttu-id="eaa5e-187">Um modelo alternativo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-187">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="eaa5e-188">selecionado-pessoa</span><span class="sxs-lookup"><span data-stu-id="eaa5e-188">selected-person</span></span> | <span data-ttu-id="eaa5e-189">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="eaa5e-189">person: The person details object</span></span> | <span data-ttu-id="eaa5e-190">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-190">The template to render selected people.</span></span> |
| <span data-ttu-id="eaa5e-191">person</span><span class="sxs-lookup"><span data-stu-id="eaa5e-191">person</span></span> | <span data-ttu-id="eaa5e-192">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="eaa5e-192">person: The person details object</span></span> | <span data-ttu-id="eaa5e-193">O modelo para renderizar pessoas na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-193">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="eaa5e-194">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-194">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="eaa5e-195">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="eaa5e-195">Microsoft Graph permissions</span></span>

<span data-ttu-id="eaa5e-196">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-196">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="eaa5e-197">API</span><span class="sxs-lookup"><span data-stu-id="eaa5e-197">API</span></span>                                                                                                              | <span data-ttu-id="eaa5e-198">Permissão</span><span class="sxs-lookup"><span data-stu-id="eaa5e-198">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="eaa5e-199">/me/people</span><span class="sxs-lookup"><span data-stu-id="eaa5e-199">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="eaa5e-200">People.Read</span><span class="sxs-lookup"><span data-stu-id="eaa5e-200">People.Read</span></span>        |
| [<span data-ttu-id="eaa5e-201">/Users</span><span class="sxs-lookup"><span data-stu-id="eaa5e-201">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0)  | <span data-ttu-id="eaa5e-202">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="eaa5e-202">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="eaa5e-203">/groups</span><span class="sxs-lookup"><span data-stu-id="eaa5e-203">/groups</span></span>](/group-list?view=graph-rest-beta)  | <span data-ttu-id="eaa5e-204">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaa5e-204">Group.Read.All</span></span> |
| [<span data-ttu-id="eaa5e-205">/groups/ \$ {GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="eaa5e-205">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="eaa5e-206">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="eaa5e-206">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="eaa5e-207">/Users/$ {userprincípioname} </span><span class="sxs-lookup"><span data-stu-id="eaa5e-207">/users/${userPrincipleName} </span></span>](/graph/api/user-get?view=graph-rest-1.0)  | <span data-ttu-id="eaa5e-208">User.Read</span><span class="sxs-lookup"><span data-stu-id="eaa5e-208">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="eaa5e-209">Autenticação</span><span class="sxs-lookup"><span data-stu-id="eaa5e-209">Authentication</span></span>

<span data-ttu-id="eaa5e-210">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="eaa5e-210">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="eaa5e-211">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="eaa5e-211">Extend for more control</span></span>

<span data-ttu-id="eaa5e-212">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-212">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="eaa5e-213">Método</span><span class="sxs-lookup"><span data-stu-id="eaa5e-213">Method</span></span> | <span data-ttu-id="eaa5e-214">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa5e-214">Description</span></span> |
| - | - |
| <span data-ttu-id="eaa5e-215">renderInput</span><span class="sxs-lookup"><span data-stu-id="eaa5e-215">renderInput</span></span> | <span data-ttu-id="eaa5e-216">Renderiza a caixa de texto de entrada.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-216">Renders the input text box.</span></span> |
| <span data-ttu-id="eaa5e-217">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="eaa5e-217">renderSelectedPeople</span></span> | <span data-ttu-id="eaa5e-218">Renderiza os tokens de pessoas selecionados.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-218">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="eaa5e-219">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="eaa5e-219">renderSelectedPerson</span></span> | <span data-ttu-id="eaa5e-220">Renderiza um token de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-220">Renders an individual person token.</span></span> |
| <span data-ttu-id="eaa5e-221">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="eaa5e-221">renderFlyout</span></span> | <span data-ttu-id="eaa5e-222">Renderiza o cromo domenu.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-222">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="eaa5e-223">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="eaa5e-223">renderFlyoutContent</span></span> | <span data-ttu-id="eaa5e-224">Processa o estado apropriado no submenu de resultados.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-224">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="eaa5e-225">renderLoading</span><span class="sxs-lookup"><span data-stu-id="eaa5e-225">renderLoading</span></span> | <span data-ttu-id="eaa5e-226">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-226">Renders the loading state.</span></span> |
| <span data-ttu-id="eaa5e-227">renderNoData</span><span class="sxs-lookup"><span data-stu-id="eaa5e-227">renderNoData</span></span> | <span data-ttu-id="eaa5e-228">Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-228">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="eaa5e-229">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="eaa5e-229">renderSearchResults</span></span> | <span data-ttu-id="eaa5e-230">Renderiza a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-230">Renders the list of search results.</span></span> |
| <span data-ttu-id="eaa5e-231">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="eaa5e-231">renderPersonResult</span></span> | <span data-ttu-id="eaa5e-232">Renderiza um resultado de pesquisa de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="eaa5e-232">Renders an individual person search result.</span></span> |
