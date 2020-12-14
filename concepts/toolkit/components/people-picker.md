---
title: People-Picker componente
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: be72a31bd9e831f6584e2a7dfac9dea50892762a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659261"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="12d71-103">People-Picker componente no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="12d71-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="12d71-104">Você pode usar o `mgt-people-picker` componente da Web para procurar pessoas e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="12d71-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="12d71-105">Por padrão, o componente pesquisará todas as pessoas e usuários da organização, mas você pode alterar o comportamento para também pesquisar grupos ou apenas grupos.</span><span class="sxs-lookup"><span data-stu-id="12d71-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="12d71-106">Você também pode filtrar a pesquisa para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="12d71-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="12d71-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12d71-107">Example</span></span>

<span data-ttu-id="12d71-108">O exemplo a seguir mostra o `mgt-people-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="12d71-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="12d71-109">Comece a pesquisar um nome para ver os resultados renderizar e usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="12d71-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="12d71-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="12d71-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="12d71-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12d71-111">Properties</span></span>

<span data-ttu-id="12d71-112">Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos de `/me/people` `/users` extremidade e.</span><span class="sxs-lookup"><span data-stu-id="12d71-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="12d71-113">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="12d71-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="12d71-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="12d71-114">Attribute</span></span> | <span data-ttu-id="12d71-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12d71-115">Property</span></span> | <span data-ttu-id="12d71-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="12d71-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="12d71-117">show-Max</span><span class="sxs-lookup"><span data-stu-id="12d71-117">show-max</span></span> | <span data-ttu-id="12d71-118">showMax</span><span class="sxs-lookup"><span data-stu-id="12d71-118">showMax</span></span>   | <span data-ttu-id="12d71-119">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="12d71-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="12d71-120">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="12d71-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="12d71-121">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="12d71-121">group-id</span></span>    | <span data-ttu-id="12d71-122">groupId</span><span class="sxs-lookup"><span data-stu-id="12d71-122">groupId</span></span>     | <span data-ttu-id="12d71-123">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="12d71-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="12d71-124">type</span><span class="sxs-lookup"><span data-stu-id="12d71-124">type</span></span>     | <span data-ttu-id="12d71-125">type</span><span class="sxs-lookup"><span data-stu-id="12d71-125">type</span></span>      | <span data-ttu-id="12d71-126">O tipo de entidades a serem pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="12d71-126">The type of entities to search for.</span></span> <span data-ttu-id="12d71-127">As opções disponíveis são: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="12d71-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="12d71-128">O valor padrão é `person`.</span><span class="sxs-lookup"><span data-stu-id="12d71-128">Default value is `person`.</span></span> <span data-ttu-id="12d71-129">Este atributo não terá efeito se a `group-id` propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="12d71-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="12d71-130">pesquisa transitiva</span><span class="sxs-lookup"><span data-stu-id="12d71-130">transitive-search</span></span>     | <span data-ttu-id="12d71-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="12d71-131">transitiveSearch</span></span>      | <span data-ttu-id="12d71-132">Um valor booliano para executar uma pesquisa transitiva, retornando uma lista simples de todos os membros aninhados-por padrão, a pesquisa transitiva não é usada.</span><span class="sxs-lookup"><span data-stu-id="12d71-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="12d71-133">tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="12d71-133">group-type</span></span>     | <span data-ttu-id="12d71-134">groupType</span><span class="sxs-lookup"><span data-stu-id="12d71-134">groupType</span></span>      | <span data-ttu-id="12d71-135">O tipo de grupo a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="12d71-135">The group type to search for.</span></span> <span data-ttu-id="12d71-136">As opções disponíveis são: `unified` , `security` , `mailenabledsecurity` , `distribution` , `any` .</span><span class="sxs-lookup"><span data-stu-id="12d71-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="12d71-137">O valor padrão é `any`.</span><span class="sxs-lookup"><span data-stu-id="12d71-137">Default value is `any`.</span></span> <span data-ttu-id="12d71-138">Este atributo não terá efeito se a `type` propriedade for definida como `person` .</span><span class="sxs-lookup"><span data-stu-id="12d71-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="12d71-139">selecionado-pessoas</span><span class="sxs-lookup"><span data-stu-id="12d71-139">selected-people</span></span>  | <span data-ttu-id="12d71-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="12d71-140">selectedPeople</span></span>     | <span data-ttu-id="12d71-141">Uma matriz de pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="12d71-141">An array of selected people.</span></span> <span data-ttu-id="12d71-142">Defina esse valor para selecionar pessoas de forma programática.</span><span class="sxs-lookup"><span data-stu-id="12d71-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="12d71-143">people</span><span class="sxs-lookup"><span data-stu-id="12d71-143">people</span></span>   | <span data-ttu-id="12d71-144">people</span><span class="sxs-lookup"><span data-stu-id="12d71-144">people</span></span>    | <span data-ttu-id="12d71-145">Uma matriz de pessoas encontrada e renderizada no resultado da pesquisa</span><span class="sxs-lookup"><span data-stu-id="12d71-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="12d71-146">PlaceHolder</span><span class="sxs-lookup"><span data-stu-id="12d71-146">placeholder</span></span>   | <span data-ttu-id="12d71-147">PlaceHolder</span><span class="sxs-lookup"><span data-stu-id="12d71-147">placeholder</span></span>    | <span data-ttu-id="12d71-148">Uma cadeia de caracteres que representa o texto do espaço reservado de entrada.</span><span class="sxs-lookup"><span data-stu-id="12d71-148">A string representing input placeholder text.</span></span> <span data-ttu-id="12d71-149">O padrão é "começar a digitar um nome".</span><span class="sxs-lookup"><span data-stu-id="12d71-149">Default is "Start typing a name".</span></span>
| <span data-ttu-id="12d71-150">modo de seleção</span><span class="sxs-lookup"><span data-stu-id="12d71-150">selection-mode</span></span>   | <span data-ttu-id="12d71-151">selectionMode</span><span class="sxs-lookup"><span data-stu-id="12d71-151">selectionMode</span></span>   | <span data-ttu-id="12d71-152">Um valor String que permite que você especifique se o componente oferece suporte a várias pessoas selecionadas ou apenas uma.</span><span class="sxs-lookup"><span data-stu-id="12d71-152">A string value that allows you to specify whether the component supports multiple selected people or just one.</span></span> <span data-ttu-id="12d71-153">O padrão `multiple` é `single` a outra opção.</span><span class="sxs-lookup"><span data-stu-id="12d71-153">Default is `multiple`; `single` is the other option.</span></span>
| <span data-ttu-id="12d71-154">default-Selected-User-IDs</span><span class="sxs-lookup"><span data-stu-id="12d71-154">default-selected-user-ids</span></span> | <span data-ttu-id="12d71-155">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="12d71-155">defaultSelectedUserIds</span></span> | <span data-ttu-id="12d71-156">Quando é fornecida uma cadeia de caracteres de IDs de usuário separadas por vírgulas do Microsoft Graph, o componente renderiza os respectivos usuários como selecionados na inicialização.</span><span class="sxs-lookup"><span data-stu-id="12d71-156">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="12d71-157">modo de seleção</span><span class="sxs-lookup"><span data-stu-id="12d71-157">selection-mode</span></span> | <span data-ttu-id="12d71-158">selectionMode</span><span class="sxs-lookup"><span data-stu-id="12d71-158">selectionMode</span></span> | <span data-ttu-id="12d71-159">Usado para indicar se é permitido selecionar vários usuários ou apenas um único usuário.</span><span class="sxs-lookup"><span data-stu-id="12d71-159">Used to indicate whether to allow selecting multiple users or just a single user.</span></span> <span data-ttu-id="12d71-160">As opções disponíveis são: `single` , `multiple` .</span><span class="sxs-lookup"><span data-stu-id="12d71-160">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="12d71-161">O valor padrão é `multiple`.</span><span class="sxs-lookup"><span data-stu-id="12d71-161">Default value is `multiple`.</span></span>
| <span data-ttu-id="12d71-162">PlaceHolder</span><span class="sxs-lookup"><span data-stu-id="12d71-162">placeholder</span></span> | <span data-ttu-id="12d71-163">PlaceHolder</span><span class="sxs-lookup"><span data-stu-id="12d71-163">placeholder</span></span> | <span data-ttu-id="12d71-164">O texto padrão que aparece para explicar como usar o componente.</span><span class="sxs-lookup"><span data-stu-id="12d71-164">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="12d71-165">O valor padrão é `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="12d71-165">Default value is `Start typing a name`.</span></span>

<span data-ttu-id="12d71-166">Este é um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="12d71-166">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="12d71-167">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="12d71-167">Selected people</span></span>

<span data-ttu-id="12d71-168">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="12d71-168">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

<span data-ttu-id="12d71-170">Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="12d71-170">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="12d71-171">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="12d71-171">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="12d71-172">Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](/graph/api/resources/users) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.</span><span class="sxs-lookup"><span data-stu-id="12d71-172">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="12d71-173">**Observação:** Se nenhum usuário for localizado para um `id` , nenhum dado será renderizado para isso `id` .</span><span class="sxs-lookup"><span data-stu-id="12d71-173">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="12d71-174">Eventos</span><span class="sxs-lookup"><span data-stu-id="12d71-174">Events</span></span>

<span data-ttu-id="12d71-175">Os eventos a seguir são acionados do componente.</span><span class="sxs-lookup"><span data-stu-id="12d71-175">The following events are fired from the component.</span></span>

| <span data-ttu-id="12d71-176">Evento</span><span class="sxs-lookup"><span data-stu-id="12d71-176">Event</span></span> | <span data-ttu-id="12d71-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="12d71-177">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="12d71-178">O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/escolhidas.</span><span class="sxs-lookup"><span data-stu-id="12d71-178">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="12d71-179">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="12d71-179">CSS custom properties</span></span>

<span data-ttu-id="12d71-180">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="12d71-180">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="12d71-181">Modelos</span><span class="sxs-lookup"><span data-stu-id="12d71-181">Templates</span></span>

 <span data-ttu-id="12d71-182">`mgt-people-picker` o dá suporte a vários [modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="12d71-182">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="12d71-183">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="12d71-183">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="12d71-184">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="12d71-184">Data type</span></span> | <span data-ttu-id="12d71-185">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="12d71-185">Data context</span></span> | <span data-ttu-id="12d71-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="12d71-186">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="12d71-187">Padrão.</span><span class="sxs-lookup"><span data-stu-id="12d71-187">default</span></span> | <span data-ttu-id="12d71-188">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="12d71-188">null: no data</span></span> | <span data-ttu-id="12d71-189">O modelo usado para substituir a renderização de todo o componente.</span><span class="sxs-lookup"><span data-stu-id="12d71-189">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="12d71-190">carregando</span><span class="sxs-lookup"><span data-stu-id="12d71-190">loading</span></span> | <span data-ttu-id="12d71-191">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="12d71-191">null: no data</span></span> | <span data-ttu-id="12d71-192">O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="12d71-192">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="12d71-193">erro</span><span class="sxs-lookup"><span data-stu-id="12d71-193">error</span></span> | <span data-ttu-id="12d71-194">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="12d71-194">null: no data</span></span> | <span data-ttu-id="12d71-195">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="12d71-195">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="12d71-196">sem dados</span><span class="sxs-lookup"><span data-stu-id="12d71-196">no-data</span></span> | <span data-ttu-id="12d71-197">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="12d71-197">null: no data</span></span> | <span data-ttu-id="12d71-198">Um modelo alternativo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="12d71-198">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="12d71-199">selecionado-pessoa</span><span class="sxs-lookup"><span data-stu-id="12d71-199">selected-person</span></span> | <span data-ttu-id="12d71-200">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="12d71-200">person: The person details object</span></span> | <span data-ttu-id="12d71-201">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="12d71-201">The template to render selected people.</span></span> |
| <span data-ttu-id="12d71-202">vendedor</span><span class="sxs-lookup"><span data-stu-id="12d71-202">person</span></span> | <span data-ttu-id="12d71-203">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="12d71-203">person: The person details object</span></span> | <span data-ttu-id="12d71-204">O modelo para renderizar pessoas na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="12d71-204">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="12d71-205">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="12d71-205">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="12d71-206">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="12d71-206">Microsoft Graph permissions</span></span>

<span data-ttu-id="12d71-207">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="12d71-207">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="12d71-208">API</span><span class="sxs-lookup"><span data-stu-id="12d71-208">API</span></span>                                                                                                              | <span data-ttu-id="12d71-209">Permissão</span><span class="sxs-lookup"><span data-stu-id="12d71-209">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="12d71-210">/me/people</span><span class="sxs-lookup"><span data-stu-id="12d71-210">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="12d71-211">People.Read</span><span class="sxs-lookup"><span data-stu-id="12d71-211">People.Read</span></span>        |
| [<span data-ttu-id="12d71-212">/Users</span><span class="sxs-lookup"><span data-stu-id="12d71-212">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="12d71-213">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="12d71-213">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="12d71-214">/groups</span><span class="sxs-lookup"><span data-stu-id="12d71-214">/groups</span></span>](/group-list)  | <span data-ttu-id="12d71-215">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="12d71-215">Group.Read.All</span></span> |
| [<span data-ttu-id="12d71-216">/groups/ \$ {GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="12d71-216">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="12d71-217">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="12d71-217">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="12d71-218">/Users/$ {userprincípioname} </span><span class="sxs-lookup"><span data-stu-id="12d71-218">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="12d71-219">User.Read</span><span class="sxs-lookup"><span data-stu-id="12d71-219">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="12d71-220">Autenticação</span><span class="sxs-lookup"><span data-stu-id="12d71-220">Authentication</span></span>

<span data-ttu-id="12d71-221">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="12d71-221">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="12d71-222">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="12d71-222">Extend for more control</span></span>

<span data-ttu-id="12d71-223">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="12d71-223">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="12d71-224">Método</span><span class="sxs-lookup"><span data-stu-id="12d71-224">Method</span></span> | <span data-ttu-id="12d71-225">Descrição</span><span class="sxs-lookup"><span data-stu-id="12d71-225">Description</span></span> |
| - | - |
| <span data-ttu-id="12d71-226">renderInput</span><span class="sxs-lookup"><span data-stu-id="12d71-226">renderInput</span></span> | <span data-ttu-id="12d71-227">Renderiza a caixa de texto de entrada.</span><span class="sxs-lookup"><span data-stu-id="12d71-227">Renders the input text box.</span></span> |
| <span data-ttu-id="12d71-228">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="12d71-228">renderSelectedPeople</span></span> | <span data-ttu-id="12d71-229">Renderiza os tokens de pessoas selecionados.</span><span class="sxs-lookup"><span data-stu-id="12d71-229">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="12d71-230">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="12d71-230">renderSelectedPerson</span></span> | <span data-ttu-id="12d71-231">Renderiza um token de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="12d71-231">Renders an individual person token.</span></span> |
| <span data-ttu-id="12d71-232">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="12d71-232">renderFlyout</span></span> | <span data-ttu-id="12d71-233">Renderiza o cromo domenu.</span><span class="sxs-lookup"><span data-stu-id="12d71-233">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="12d71-234">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="12d71-234">renderFlyoutContent</span></span> | <span data-ttu-id="12d71-235">Processa o estado apropriado no submenu de resultados.</span><span class="sxs-lookup"><span data-stu-id="12d71-235">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="12d71-236">renderLoading</span><span class="sxs-lookup"><span data-stu-id="12d71-236">renderLoading</span></span> | <span data-ttu-id="12d71-237">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="12d71-237">Renders the loading state.</span></span> |
| <span data-ttu-id="12d71-238">renderNoData</span><span class="sxs-lookup"><span data-stu-id="12d71-238">renderNoData</span></span> | <span data-ttu-id="12d71-239">Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="12d71-239">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="12d71-240">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="12d71-240">renderSearchResults</span></span> | <span data-ttu-id="12d71-241">Renderiza a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="12d71-241">Renders the list of search results.</span></span> |
| <span data-ttu-id="12d71-242">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="12d71-242">renderPersonResult</span></span> | <span data-ttu-id="12d71-243">Renderiza um resultado de pesquisa de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="12d71-243">Renders an individual person search result.</span></span> |
