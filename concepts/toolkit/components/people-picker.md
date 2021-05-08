---
title: People-Picker componente
description: Você pode usar o componente web do se picker mgt-people para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 3531c32ae4f33898b11f7d92f91115aa1cbf43a3
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266812"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c2aca-103">People-Picker componente no microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="c2aca-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c2aca-104">Você pode usar o `mgt-people-picker` componente web para pesquisar pessoas e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="c2aca-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="c2aca-105">Por padrão, o componente procurará por todas as pessoas e usuários na organização, mas você pode alterar o comportamento para também pesquisar grupos ou somente grupos.</span><span class="sxs-lookup"><span data-stu-id="c2aca-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="c2aca-106">Você também pode filtrar a pesquisa para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="c2aca-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="c2aca-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2aca-107">Example</span></span>

<span data-ttu-id="c2aca-108">O exemplo a seguir mostra o `mgt-people-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="c2aca-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="c2aca-109">Comece a procurar um nome para ver os resultados [](#properties) renderizar e use o editor de código para ver como as propriedades alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="c2aca-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="c2aca-110">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="c2aca-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="c2aca-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2aca-111">Properties</span></span>

<span data-ttu-id="c2aca-112">Por padrão, `mgt-people-picker` o componente busca pessoas dos pontos de extremidade `/me/people` `/users` e.</span><span class="sxs-lookup"><span data-stu-id="c2aca-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="c2aca-113">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="c2aca-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="c2aca-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="c2aca-114">Attribute</span></span> | <span data-ttu-id="c2aca-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2aca-115">Property</span></span> | <span data-ttu-id="c2aca-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2aca-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c2aca-117">show-max</span><span class="sxs-lookup"><span data-stu-id="c2aca-117">show-max</span></span> | <span data-ttu-id="c2aca-118">showMax</span><span class="sxs-lookup"><span data-stu-id="c2aca-118">showMax</span></span>   | <span data-ttu-id="c2aca-119">Um valor de número para indicar o número máximo de pessoas a mostrar.</span><span class="sxs-lookup"><span data-stu-id="c2aca-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="c2aca-120">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="c2aca-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="c2aca-121">group-id</span><span class="sxs-lookup"><span data-stu-id="c2aca-121">group-id</span></span>    | <span data-ttu-id="c2aca-122">groupId</span><span class="sxs-lookup"><span data-stu-id="c2aca-122">groupId</span></span>     | <span data-ttu-id="c2aca-123">Um valor de cadeia de caracteres que pertence a um grupo definido pelo Microsoft Graph para filtrar ainda mais os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c2aca-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="c2aca-124">tipo</span><span class="sxs-lookup"><span data-stu-id="c2aca-124">type</span></span>     | <span data-ttu-id="c2aca-125">tipo</span><span class="sxs-lookup"><span data-stu-id="c2aca-125">type</span></span>      | <span data-ttu-id="c2aca-126">O tipo de entidades a ser pesquisada.</span><span class="sxs-lookup"><span data-stu-id="c2aca-126">The type of entities to search for.</span></span> <span data-ttu-id="c2aca-127">As opções disponíveis são: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="c2aca-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="c2aca-128">O valor padrão é `person`.</span><span class="sxs-lookup"><span data-stu-id="c2aca-128">Default value is `person`.</span></span> <span data-ttu-id="c2aca-129">Esse atributo não terá efeito se `group-id` a propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="c2aca-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="c2aca-130">transitive-search</span><span class="sxs-lookup"><span data-stu-id="c2aca-130">transitive-search</span></span>     | <span data-ttu-id="c2aca-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="c2aca-131">transitiveSearch</span></span>      | <span data-ttu-id="c2aca-132">Um valor Boolean para executar uma pesquisa transitiva retornando uma lista simples de todos os membros aninhados - por padrão, a pesquisa transitiva não é usada.</span><span class="sxs-lookup"><span data-stu-id="c2aca-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="c2aca-133">tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="c2aca-133">group-type</span></span>     | <span data-ttu-id="c2aca-134">groupType</span><span class="sxs-lookup"><span data-stu-id="c2aca-134">groupType</span></span>      | <span data-ttu-id="c2aca-135">O tipo de grupo a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="c2aca-135">The group type to search for.</span></span> <span data-ttu-id="c2aca-136">As opções disponíveis são: `unified` , , , , `security` `mailenabledsecurity` `distribution` `any` .</span><span class="sxs-lookup"><span data-stu-id="c2aca-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="c2aca-137">O valor padrão é `any`.</span><span class="sxs-lookup"><span data-stu-id="c2aca-137">Default value is `any`.</span></span> <span data-ttu-id="c2aca-138">Esse atributo não terá efeito se a `type` propriedade for definida como `person` .</span><span class="sxs-lookup"><span data-stu-id="c2aca-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="c2aca-139">selected-people</span><span class="sxs-lookup"><span data-stu-id="c2aca-139">selected-people</span></span>  | <span data-ttu-id="c2aca-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="c2aca-140">selectedPeople</span></span>     | <span data-ttu-id="c2aca-141">Uma matriz de pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="c2aca-141">An array of selected people.</span></span> <span data-ttu-id="c2aca-142">De definir esse valor para selecionar pessoas programaticamente.</span><span class="sxs-lookup"><span data-stu-id="c2aca-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="c2aca-143">people</span><span class="sxs-lookup"><span data-stu-id="c2aca-143">people</span></span>   | <span data-ttu-id="c2aca-144">people</span><span class="sxs-lookup"><span data-stu-id="c2aca-144">people</span></span>    | <span data-ttu-id="c2aca-145">Uma matriz de pessoas encontradas e renderizadas no resultado da pesquisa</span><span class="sxs-lookup"><span data-stu-id="c2aca-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="c2aca-146">placeholder</span><span class="sxs-lookup"><span data-stu-id="c2aca-146">placeholder</span></span>   | <span data-ttu-id="c2aca-147">placeholder</span><span class="sxs-lookup"><span data-stu-id="c2aca-147">placeholder</span></span>    | <span data-ttu-id="c2aca-148">O texto padrão que parece explicar como usar o componente.</span><span class="sxs-lookup"><span data-stu-id="c2aca-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="c2aca-149">O valor padrão é `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="c2aca-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="c2aca-150">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="c2aca-150">default-selected-user-ids</span></span> | <span data-ttu-id="c2aca-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="c2aca-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="c2aca-152">Quando fornecido uma cadeia de caracteres de IDs de usuário separadas por vírgulas do Microsoft Graph, o componente renderiza os respectivos usuários como selecionados após a inicialização.</span><span class="sxs-lookup"><span data-stu-id="c2aca-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="c2aca-153">modo de seleção</span><span class="sxs-lookup"><span data-stu-id="c2aca-153">selection-mode</span></span> | <span data-ttu-id="c2aca-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="c2aca-154">selectionMode</span></span> | <span data-ttu-id="c2aca-155">Usado para indicar se é possível selecionar vários itens (usuários ou grupos) ou apenas um único item.</span><span class="sxs-lookup"><span data-stu-id="c2aca-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="c2aca-156">As opções disponíveis são: `single` , `multiple` .</span><span class="sxs-lookup"><span data-stu-id="c2aca-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="c2aca-157">O valor padrão é `multiple`.</span><span class="sxs-lookup"><span data-stu-id="c2aca-157">Default value is `multiple`.</span></span>
| <span data-ttu-id="c2aca-158">desabilitadas</span><span class="sxs-lookup"><span data-stu-id="c2aca-158">disabled</span></span> | <span data-ttu-id="c2aca-159">desabilitadas</span><span class="sxs-lookup"><span data-stu-id="c2aca-159">disabled</span></span> | <span data-ttu-id="c2aca-160">Define se o se picker de pessoas está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="c2aca-160">Sets whether the people picker is disabled.</span></span> <span data-ttu-id="c2aca-161">Quando desabilitado, o usuário não é capaz de pesquisar ou selecionar pessoas.</span><span class="sxs-lookup"><span data-stu-id="c2aca-161">When disabled, the user is not able to search or select people.</span></span>

<span data-ttu-id="c2aca-162">A seguir, um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="c2aca-162">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="c2aca-163">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="c2aca-163">Selected people</span></span>

<span data-ttu-id="c2aca-164">A seção pessoas selecionadas do componente renderiza cada pessoa escolhida pelo desenvolvedor ou usuário.</span><span class="sxs-lookup"><span data-stu-id="c2aca-164">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="c2aca-166">Você pode preencher dados de pessoas selecionadas fazendo um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="c2aca-166">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="c2aca-167">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="c2aca-167">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="c2aca-168">Usando o método, que aceita uma matriz de IDs de usuário do Microsoft Graph para `selectUsersById()` encontrar detalhes de usuário [associados](/graph/api/resources/users) para seleção.</span><span class="sxs-lookup"><span data-stu-id="c2aca-168">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="c2aca-169">**Observação:** Se nenhum usuário for encontrado para `id` um , nenhum dado será renderizado para isso `id` .</span><span class="sxs-lookup"><span data-stu-id="c2aca-169">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="c2aca-170">Eventos</span><span class="sxs-lookup"><span data-stu-id="c2aca-170">Events</span></span>

<span data-ttu-id="c2aca-171">Os eventos a seguir são disparados do componente.</span><span class="sxs-lookup"><span data-stu-id="c2aca-171">The following events are fired from the component.</span></span>

| <span data-ttu-id="c2aca-172">Evento</span><span class="sxs-lookup"><span data-stu-id="c2aca-172">Event</span></span> | <span data-ttu-id="c2aca-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2aca-173">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="c2aca-174">O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/selecionadas.</span><span class="sxs-lookup"><span data-stu-id="c2aca-174">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="c2aca-175">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="c2aca-175">CSS custom properties</span></span>

<span data-ttu-id="c2aca-176">O `mgt-people-picker` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="c2aca-176">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="c2aca-177">Modelos</span><span class="sxs-lookup"><span data-stu-id="c2aca-177">Templates</span></span>

 <span data-ttu-id="c2aca-178">`mgt-people-picker` oferece suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="c2aca-178">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="c2aca-179">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.</span><span class="sxs-lookup"><span data-stu-id="c2aca-179">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="c2aca-180">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="c2aca-180">Data type</span></span> | <span data-ttu-id="c2aca-181">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="c2aca-181">Data context</span></span> | <span data-ttu-id="c2aca-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2aca-182">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="c2aca-183">Padrão.</span><span class="sxs-lookup"><span data-stu-id="c2aca-183">default</span></span> | <span data-ttu-id="c2aca-184">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="c2aca-184">null: no data</span></span> | <span data-ttu-id="c2aca-185">O modelo usado para substituir a renderização de todo o componente.</span><span class="sxs-lookup"><span data-stu-id="c2aca-185">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="c2aca-186">loading</span><span class="sxs-lookup"><span data-stu-id="c2aca-186">loading</span></span> | <span data-ttu-id="c2aca-187">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="c2aca-187">null: no data</span></span> | <span data-ttu-id="c2aca-188">O modelo usado para renderizar o estado do selador enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="c2aca-188">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="c2aca-189">erro</span><span class="sxs-lookup"><span data-stu-id="c2aca-189">error</span></span> | <span data-ttu-id="c2aca-190">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="c2aca-190">null: no data</span></span> | <span data-ttu-id="c2aca-191">O modelo usado se a pesquisa do usuário não retornar usuários.</span><span class="sxs-lookup"><span data-stu-id="c2aca-191">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="c2aca-192">no-data</span><span class="sxs-lookup"><span data-stu-id="c2aca-192">no-data</span></span> | <span data-ttu-id="c2aca-193">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="c2aca-193">null: no data</span></span> | <span data-ttu-id="c2aca-194">Um modelo alternativo usado se a pesquisa do usuário não retornar usuários.</span><span class="sxs-lookup"><span data-stu-id="c2aca-194">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="c2aca-195">selected-person</span><span class="sxs-lookup"><span data-stu-id="c2aca-195">selected-person</span></span> | <span data-ttu-id="c2aca-196">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="c2aca-196">person: The person details object</span></span> | <span data-ttu-id="c2aca-197">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="c2aca-197">The template to render selected people.</span></span> |
| <span data-ttu-id="c2aca-198">person</span><span class="sxs-lookup"><span data-stu-id="c2aca-198">person</span></span> | <span data-ttu-id="c2aca-199">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="c2aca-199">person: The person details object</span></span> | <span data-ttu-id="c2aca-200">O modelo para renderizar pessoas no menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="c2aca-200">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="c2aca-201">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="c2aca-201">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="c2aca-202">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c2aca-202">Microsoft Graph permissions</span></span>

<span data-ttu-id="c2aca-203">Esse componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2aca-203">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="c2aca-204">API</span><span class="sxs-lookup"><span data-stu-id="c2aca-204">API</span></span>                                                                                                              | <span data-ttu-id="c2aca-205">Permissão</span><span class="sxs-lookup"><span data-stu-id="c2aca-205">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="c2aca-206">/me/people</span><span class="sxs-lookup"><span data-stu-id="c2aca-206">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="c2aca-207">People.Read</span><span class="sxs-lookup"><span data-stu-id="c2aca-207">People.Read</span></span>        |
| [<span data-ttu-id="c2aca-208">/users</span><span class="sxs-lookup"><span data-stu-id="c2aca-208">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="c2aca-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="c2aca-209">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="c2aca-210">/groups</span><span class="sxs-lookup"><span data-stu-id="c2aca-210">/groups</span></span>](/group-list)  | <span data-ttu-id="c2aca-211">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2aca-211">Group.Read.All</span></span> |
| [<span data-ttu-id="c2aca-212">/groups/ \$ {groupId}/members</span><span class="sxs-lookup"><span data-stu-id="c2aca-212">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="c2aca-213">GroupMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2aca-213">GroupMember.Read.All</span></span>        |
| [<span data-ttu-id="c2aca-214">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="c2aca-214">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="c2aca-215">User.Read</span><span class="sxs-lookup"><span data-stu-id="c2aca-215">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="c2aca-216">Autenticação</span><span class="sxs-lookup"><span data-stu-id="c2aca-216">Authentication</span></span>

<span data-ttu-id="c2aca-217">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="c2aca-217">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="c2aca-218">Cache</span><span class="sxs-lookup"><span data-stu-id="c2aca-218">Cache</span></span>

|<span data-ttu-id="c2aca-219">Armazenamento de objetos</span><span class="sxs-lookup"><span data-stu-id="c2aca-219">Object store</span></span>|<span data-ttu-id="c2aca-220">Dados armazenados em cache</span><span class="sxs-lookup"><span data-stu-id="c2aca-220">Cached data</span></span>|<span data-ttu-id="c2aca-221">Comentários</span><span class="sxs-lookup"><span data-stu-id="c2aca-221">Remarks</span></span>|
|---------|-----------|-------|
|`groups`|<span data-ttu-id="c2aca-222">Lista de grupos</span><span class="sxs-lookup"><span data-stu-id="c2aca-222">List of groups</span></span>|<span data-ttu-id="c2aca-223">Usado quando `type` está definido como `PersonType.group`</span><span class="sxs-lookup"><span data-stu-id="c2aca-223">Used when `type` is set to `PersonType.group`</span></span>|
|`people`|<span data-ttu-id="c2aca-224">Lista de pessoas</span><span class="sxs-lookup"><span data-stu-id="c2aca-224">List of people</span></span>|<span data-ttu-id="c2aca-225">Usado quando `type` está definido como `PersonType.person` ou `PersonType.any`</span><span class="sxs-lookup"><span data-stu-id="c2aca-225">Used when `type` is set to `PersonType.person` or `PersonType.any`</span></span>|
|`users`|<span data-ttu-id="c2aca-226">Lista de usuários</span><span class="sxs-lookup"><span data-stu-id="c2aca-226">List of users</span></span>|<span data-ttu-id="c2aca-227">Usado quando `groupId` especificado</span><span class="sxs-lookup"><span data-stu-id="c2aca-227">Used when `groupId` specified</span></span>|

<span data-ttu-id="c2aca-228">Consulte [Cache para](../customize-components/cache.md) obter mais detalhes sobre como configurar o cache.</span><span class="sxs-lookup"><span data-stu-id="c2aca-228">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="c2aca-229">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="c2aca-229">Extend for more control</span></span>

<span data-ttu-id="c2aca-230">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.</span><span class="sxs-lookup"><span data-stu-id="c2aca-230">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="c2aca-231">Método</span><span class="sxs-lookup"><span data-stu-id="c2aca-231">Method</span></span> | <span data-ttu-id="c2aca-232">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2aca-232">Description</span></span> |
| - | - |
| <span data-ttu-id="c2aca-233">renderInput</span><span class="sxs-lookup"><span data-stu-id="c2aca-233">renderInput</span></span> | <span data-ttu-id="c2aca-234">Renderiza a caixa de texto de entrada.</span><span class="sxs-lookup"><span data-stu-id="c2aca-234">Renders the input text box.</span></span> |
| <span data-ttu-id="c2aca-235">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="c2aca-235">renderSelectedPeople</span></span> | <span data-ttu-id="c2aca-236">Renderiza os tokens de pessoas selecionados.</span><span class="sxs-lookup"><span data-stu-id="c2aca-236">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="c2aca-237">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="c2aca-237">renderSelectedPerson</span></span> | <span data-ttu-id="c2aca-238">Renderiza um token de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="c2aca-238">Renders an individual person token.</span></span> |
| <span data-ttu-id="c2aca-239">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="c2aca-239">renderFlyout</span></span> | <span data-ttu-id="c2aca-240">Renderiza o cromado do flyout.</span><span class="sxs-lookup"><span data-stu-id="c2aca-240">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="c2aca-241">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="c2aca-241">renderFlyoutContent</span></span> | <span data-ttu-id="c2aca-242">Renderiza o estado apropriado no sobrevoo de resultados.</span><span class="sxs-lookup"><span data-stu-id="c2aca-242">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="c2aca-243">renderLoading</span><span class="sxs-lookup"><span data-stu-id="c2aca-243">renderLoading</span></span> | <span data-ttu-id="c2aca-244">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="c2aca-244">Renders the loading state.</span></span> |
| <span data-ttu-id="c2aca-245">renderNoData</span><span class="sxs-lookup"><span data-stu-id="c2aca-245">renderNoData</span></span> | <span data-ttu-id="c2aca-246">Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c2aca-246">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="c2aca-247">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="c2aca-247">renderSearchResults</span></span> | <span data-ttu-id="c2aca-248">Renderiza a lista de resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c2aca-248">Renders the list of search results.</span></span> |
| <span data-ttu-id="c2aca-249">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="c2aca-249">renderPersonResult</span></span> | <span data-ttu-id="c2aca-250">Renderiza um resultado de pesquisa de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="c2aca-250">Renders an individual person search result.</span></span> |
