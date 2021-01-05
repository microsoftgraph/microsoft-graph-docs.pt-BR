---
title: People-Picker componente
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 9c23abbb3d525a3110cca31b21f2ee24d3c9f26d
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753771"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="15915-103">People-Picker componente no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="15915-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="15915-104">Você pode usar o `mgt-people-picker` componente da Web para procurar pessoas e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="15915-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="15915-105">Por padrão, o componente pesquisará todas as pessoas e usuários da organização, mas você pode alterar o comportamento para também pesquisar grupos ou apenas grupos.</span><span class="sxs-lookup"><span data-stu-id="15915-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="15915-106">Você também pode filtrar a pesquisa para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="15915-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="15915-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15915-107">Example</span></span>

<span data-ttu-id="15915-108">O exemplo a seguir mostra o `mgt-people-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="15915-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="15915-109">Comece a pesquisar um nome para ver os resultados renderizar e usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="15915-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="15915-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="15915-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="15915-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15915-111">Properties</span></span>

<span data-ttu-id="15915-112">Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos de `/me/people` `/users` extremidade e.</span><span class="sxs-lookup"><span data-stu-id="15915-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="15915-113">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="15915-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="15915-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="15915-114">Attribute</span></span> | <span data-ttu-id="15915-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15915-115">Property</span></span> | <span data-ttu-id="15915-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="15915-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="15915-117">show-Max</span><span class="sxs-lookup"><span data-stu-id="15915-117">show-max</span></span> | <span data-ttu-id="15915-118">showMax</span><span class="sxs-lookup"><span data-stu-id="15915-118">showMax</span></span>   | <span data-ttu-id="15915-119">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="15915-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="15915-120">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="15915-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="15915-121">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="15915-121">group-id</span></span>    | <span data-ttu-id="15915-122">groupId</span><span class="sxs-lookup"><span data-stu-id="15915-122">groupId</span></span>     | <span data-ttu-id="15915-123">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="15915-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="15915-124">type</span><span class="sxs-lookup"><span data-stu-id="15915-124">type</span></span>     | <span data-ttu-id="15915-125">type</span><span class="sxs-lookup"><span data-stu-id="15915-125">type</span></span>      | <span data-ttu-id="15915-126">O tipo de entidades a serem pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="15915-126">The type of entities to search for.</span></span> <span data-ttu-id="15915-127">As opções disponíveis são: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="15915-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="15915-128">O valor padrão é `person`.</span><span class="sxs-lookup"><span data-stu-id="15915-128">Default value is `person`.</span></span> <span data-ttu-id="15915-129">Este atributo não terá efeito se a `group-id` propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="15915-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="15915-130">pesquisa transitiva</span><span class="sxs-lookup"><span data-stu-id="15915-130">transitive-search</span></span>     | <span data-ttu-id="15915-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="15915-131">transitiveSearch</span></span>      | <span data-ttu-id="15915-132">Um valor booliano para executar uma pesquisa transitiva, retornando uma lista simples de todos os membros aninhados-por padrão, a pesquisa transitiva não é usada.</span><span class="sxs-lookup"><span data-stu-id="15915-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="15915-133">tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="15915-133">group-type</span></span>     | <span data-ttu-id="15915-134">groupType</span><span class="sxs-lookup"><span data-stu-id="15915-134">groupType</span></span>      | <span data-ttu-id="15915-135">O tipo de grupo a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="15915-135">The group type to search for.</span></span> <span data-ttu-id="15915-136">As opções disponíveis são: `unified` , `security` , `mailenabledsecurity` , `distribution` , `any` .</span><span class="sxs-lookup"><span data-stu-id="15915-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="15915-137">O valor padrão é `any`.</span><span class="sxs-lookup"><span data-stu-id="15915-137">Default value is `any`.</span></span> <span data-ttu-id="15915-138">Este atributo não terá efeito se a `type` propriedade for definida como `person` .</span><span class="sxs-lookup"><span data-stu-id="15915-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="15915-139">selecionado-pessoas</span><span class="sxs-lookup"><span data-stu-id="15915-139">selected-people</span></span>  | <span data-ttu-id="15915-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="15915-140">selectedPeople</span></span>     | <span data-ttu-id="15915-141">Uma matriz de pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="15915-141">An array of selected people.</span></span> <span data-ttu-id="15915-142">Defina esse valor para selecionar pessoas de forma programática.</span><span class="sxs-lookup"><span data-stu-id="15915-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="15915-143">people</span><span class="sxs-lookup"><span data-stu-id="15915-143">people</span></span>   | <span data-ttu-id="15915-144">people</span><span class="sxs-lookup"><span data-stu-id="15915-144">people</span></span>    | <span data-ttu-id="15915-145">Uma matriz de pessoas encontrada e renderizada no resultado da pesquisa</span><span class="sxs-lookup"><span data-stu-id="15915-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="15915-146">PlaceHolder</span><span class="sxs-lookup"><span data-stu-id="15915-146">placeholder</span></span>   | <span data-ttu-id="15915-147">PlaceHolder</span><span class="sxs-lookup"><span data-stu-id="15915-147">placeholder</span></span>    | <span data-ttu-id="15915-148">O texto padrão que aparece para explicar como usar o componente.</span><span class="sxs-lookup"><span data-stu-id="15915-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="15915-149">O valor padrão é `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="15915-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="15915-150">default-Selected-User-IDs</span><span class="sxs-lookup"><span data-stu-id="15915-150">default-selected-user-ids</span></span> | <span data-ttu-id="15915-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="15915-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="15915-152">Quando é fornecida uma cadeia de caracteres de IDs de usuário separadas por vírgulas do Microsoft Graph, o componente renderiza os respectivos usuários como selecionados na inicialização.</span><span class="sxs-lookup"><span data-stu-id="15915-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="15915-153">modo de seleção</span><span class="sxs-lookup"><span data-stu-id="15915-153">selection-mode</span></span> | <span data-ttu-id="15915-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="15915-154">selectionMode</span></span> | <span data-ttu-id="15915-155">Usado para indicar se é permitido selecionar vários itens (usuários ou grupos) ou apenas um único item.</span><span class="sxs-lookup"><span data-stu-id="15915-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="15915-156">As opções disponíveis são: `single` , `multiple` .</span><span class="sxs-lookup"><span data-stu-id="15915-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="15915-157">O valor padrão é `multiple`.</span><span class="sxs-lookup"><span data-stu-id="15915-157">Default value is `multiple`.</span></span>

<span data-ttu-id="15915-158">Este é um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="15915-158">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="15915-159">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="15915-159">Selected people</span></span>

<span data-ttu-id="15915-160">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="15915-160">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

<span data-ttu-id="15915-162">Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="15915-162">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="15915-163">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="15915-163">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="15915-164">Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](/graph/api/resources/users) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.</span><span class="sxs-lookup"><span data-stu-id="15915-164">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="15915-165">**Observação:** Se nenhum usuário for localizado para um `id` , nenhum dado será renderizado para isso `id` .</span><span class="sxs-lookup"><span data-stu-id="15915-165">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="15915-166">Eventos</span><span class="sxs-lookup"><span data-stu-id="15915-166">Events</span></span>

<span data-ttu-id="15915-167">Os eventos a seguir são acionados do componente.</span><span class="sxs-lookup"><span data-stu-id="15915-167">The following events are fired from the component.</span></span>

| <span data-ttu-id="15915-168">Evento</span><span class="sxs-lookup"><span data-stu-id="15915-168">Event</span></span> | <span data-ttu-id="15915-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="15915-169">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="15915-170">O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/escolhidas.</span><span class="sxs-lookup"><span data-stu-id="15915-170">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="15915-171">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="15915-171">CSS custom properties</span></span>

<span data-ttu-id="15915-172">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="15915-172">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --color: white; /* input area border focus color */
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a><span data-ttu-id="15915-173">Modelos</span><span class="sxs-lookup"><span data-stu-id="15915-173">Templates</span></span>

 <span data-ttu-id="15915-174">`mgt-people-picker` o dá suporte a vários [modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="15915-174">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="15915-175">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="15915-175">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="15915-176">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="15915-176">Data type</span></span> | <span data-ttu-id="15915-177">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="15915-177">Data context</span></span> | <span data-ttu-id="15915-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="15915-178">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="15915-179">Padrão.</span><span class="sxs-lookup"><span data-stu-id="15915-179">default</span></span> | <span data-ttu-id="15915-180">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="15915-180">null: no data</span></span> | <span data-ttu-id="15915-181">O modelo usado para substituir a renderização de todo o componente.</span><span class="sxs-lookup"><span data-stu-id="15915-181">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="15915-182">carregando</span><span class="sxs-lookup"><span data-stu-id="15915-182">loading</span></span> | <span data-ttu-id="15915-183">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="15915-183">null: no data</span></span> | <span data-ttu-id="15915-184">O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="15915-184">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="15915-185">erro</span><span class="sxs-lookup"><span data-stu-id="15915-185">error</span></span> | <span data-ttu-id="15915-186">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="15915-186">null: no data</span></span> | <span data-ttu-id="15915-187">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="15915-187">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="15915-188">sem dados</span><span class="sxs-lookup"><span data-stu-id="15915-188">no-data</span></span> | <span data-ttu-id="15915-189">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="15915-189">null: no data</span></span> | <span data-ttu-id="15915-190">Um modelo alternativo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="15915-190">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="15915-191">selecionado-pessoa</span><span class="sxs-lookup"><span data-stu-id="15915-191">selected-person</span></span> | <span data-ttu-id="15915-192">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="15915-192">person: The person details object</span></span> | <span data-ttu-id="15915-193">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="15915-193">The template to render selected people.</span></span> |
| <span data-ttu-id="15915-194">vendedor</span><span class="sxs-lookup"><span data-stu-id="15915-194">person</span></span> | <span data-ttu-id="15915-195">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="15915-195">person: The person details object</span></span> | <span data-ttu-id="15915-196">O modelo para renderizar pessoas na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="15915-196">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="15915-197">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="15915-197">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="15915-198">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="15915-198">Microsoft Graph permissions</span></span>

<span data-ttu-id="15915-199">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="15915-199">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="15915-200">API</span><span class="sxs-lookup"><span data-stu-id="15915-200">API</span></span>                                                                                                              | <span data-ttu-id="15915-201">Permissão</span><span class="sxs-lookup"><span data-stu-id="15915-201">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="15915-202">/me/people</span><span class="sxs-lookup"><span data-stu-id="15915-202">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="15915-203">People.Read</span><span class="sxs-lookup"><span data-stu-id="15915-203">People.Read</span></span>        |
| [<span data-ttu-id="15915-204">/Users</span><span class="sxs-lookup"><span data-stu-id="15915-204">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="15915-205">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="15915-205">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="15915-206">/groups</span><span class="sxs-lookup"><span data-stu-id="15915-206">/groups</span></span>](/group-list)  | <span data-ttu-id="15915-207">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="15915-207">Group.Read.All</span></span> |
| [<span data-ttu-id="15915-208">/groups/ \$ {GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="15915-208">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="15915-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="15915-209">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="15915-210">/Users/$ {userprincípioname} </span><span class="sxs-lookup"><span data-stu-id="15915-210">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="15915-211">User.Read</span><span class="sxs-lookup"><span data-stu-id="15915-211">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="15915-212">Autenticação</span><span class="sxs-lookup"><span data-stu-id="15915-212">Authentication</span></span>

<span data-ttu-id="15915-213">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="15915-213">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="15915-214">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="15915-214">Extend for more control</span></span>

<span data-ttu-id="15915-215">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="15915-215">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="15915-216">Método</span><span class="sxs-lookup"><span data-stu-id="15915-216">Method</span></span> | <span data-ttu-id="15915-217">Descrição</span><span class="sxs-lookup"><span data-stu-id="15915-217">Description</span></span> |
| - | - |
| <span data-ttu-id="15915-218">renderInput</span><span class="sxs-lookup"><span data-stu-id="15915-218">renderInput</span></span> | <span data-ttu-id="15915-219">Renderiza a caixa de texto de entrada.</span><span class="sxs-lookup"><span data-stu-id="15915-219">Renders the input text box.</span></span> |
| <span data-ttu-id="15915-220">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="15915-220">renderSelectedPeople</span></span> | <span data-ttu-id="15915-221">Renderiza os tokens de pessoas selecionados.</span><span class="sxs-lookup"><span data-stu-id="15915-221">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="15915-222">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="15915-222">renderSelectedPerson</span></span> | <span data-ttu-id="15915-223">Renderiza um token de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="15915-223">Renders an individual person token.</span></span> |
| <span data-ttu-id="15915-224">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="15915-224">renderFlyout</span></span> | <span data-ttu-id="15915-225">Renderiza o cromo domenu.</span><span class="sxs-lookup"><span data-stu-id="15915-225">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="15915-226">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="15915-226">renderFlyoutContent</span></span> | <span data-ttu-id="15915-227">Processa o estado apropriado no submenu de resultados.</span><span class="sxs-lookup"><span data-stu-id="15915-227">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="15915-228">renderLoading</span><span class="sxs-lookup"><span data-stu-id="15915-228">renderLoading</span></span> | <span data-ttu-id="15915-229">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="15915-229">Renders the loading state.</span></span> |
| <span data-ttu-id="15915-230">renderNoData</span><span class="sxs-lookup"><span data-stu-id="15915-230">renderNoData</span></span> | <span data-ttu-id="15915-231">Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="15915-231">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="15915-232">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="15915-232">renderSearchResults</span></span> | <span data-ttu-id="15915-233">Renderiza a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="15915-233">Renders the list of search results.</span></span> |
| <span data-ttu-id="15915-234">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="15915-234">renderPersonResult</span></span> | <span data-ttu-id="15915-235">Renderiza um resultado de pesquisa de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="15915-235">Renders an individual person search result.</span></span> |
