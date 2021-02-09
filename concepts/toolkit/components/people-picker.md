---
title: People-Picker componente
description: Você pode usar o componente web mgt-people-picker para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 691955aa64ff0afc42b5f8912658a6f36e1d77ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161373"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="4dfab-103">People-Picker componente no Kit de Ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4dfab-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4dfab-104">Você pode usar o `mgt-people-picker` componente web para pesquisar pessoas e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="4dfab-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="4dfab-105">Por padrão, o componente pesquisa todas as pessoas e usuários na organização, mas você pode alterar o comportamento para também pesquisar grupos ou apenas grupos.</span><span class="sxs-lookup"><span data-stu-id="4dfab-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="4dfab-106">Você também pode filtrar a pesquisa para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="4dfab-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="4dfab-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dfab-107">Example</span></span>

<span data-ttu-id="4dfab-108">O exemplo a seguir mostra o `mgt-people-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="4dfab-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="4dfab-109">Comece procurando um nome para ver os resultados renderizar [](#properties) e use o editor de código para ver como as propriedades alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="4dfab-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="4dfab-110">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="4dfab-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="4dfab-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4dfab-111">Properties</span></span>

<span data-ttu-id="4dfab-112">Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos de extremidade e dos pontos de `/me/people` `/users` extremidade.</span><span class="sxs-lookup"><span data-stu-id="4dfab-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="4dfab-113">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="4dfab-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="4dfab-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="4dfab-114">Attribute</span></span> | <span data-ttu-id="4dfab-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dfab-115">Property</span></span> | <span data-ttu-id="4dfab-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dfab-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4dfab-117">show-max</span><span class="sxs-lookup"><span data-stu-id="4dfab-117">show-max</span></span> | <span data-ttu-id="4dfab-118">showMax</span><span class="sxs-lookup"><span data-stu-id="4dfab-118">showMax</span></span>   | <span data-ttu-id="4dfab-119">Um valor de número para indicar o número máximo de pessoas a mostrar.</span><span class="sxs-lookup"><span data-stu-id="4dfab-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="4dfab-120">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="4dfab-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="4dfab-121">group-id</span><span class="sxs-lookup"><span data-stu-id="4dfab-121">group-id</span></span>    | <span data-ttu-id="4dfab-122">groupId</span><span class="sxs-lookup"><span data-stu-id="4dfab-122">groupId</span></span>     | <span data-ttu-id="4dfab-123">Um valor de cadeia de caracteres que pertence a um grupo definido pelo Microsoft Graph para filtrar ainda mais os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4dfab-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="4dfab-124">type</span><span class="sxs-lookup"><span data-stu-id="4dfab-124">type</span></span>     | <span data-ttu-id="4dfab-125">type</span><span class="sxs-lookup"><span data-stu-id="4dfab-125">type</span></span>      | <span data-ttu-id="4dfab-126">O tipo de entidades a ser pesquisada.</span><span class="sxs-lookup"><span data-stu-id="4dfab-126">The type of entities to search for.</span></span> <span data-ttu-id="4dfab-127">As opções disponíveis são: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="4dfab-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="4dfab-128">O valor padrão é `person`.</span><span class="sxs-lookup"><span data-stu-id="4dfab-128">Default value is `person`.</span></span> <span data-ttu-id="4dfab-129">Esse atributo não terá efeito se `group-id` a propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="4dfab-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="4dfab-130">transitive-search</span><span class="sxs-lookup"><span data-stu-id="4dfab-130">transitive-search</span></span>     | <span data-ttu-id="4dfab-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="4dfab-131">transitiveSearch</span></span>      | <span data-ttu-id="4dfab-132">Um valor Boolean para executar uma pesquisa transitiva retornando uma lista simples de todos os membros aninhados - por padrão, a pesquisa transitiva não é usada.</span><span class="sxs-lookup"><span data-stu-id="4dfab-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="4dfab-133">tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="4dfab-133">group-type</span></span>     | <span data-ttu-id="4dfab-134">groupType</span><span class="sxs-lookup"><span data-stu-id="4dfab-134">groupType</span></span>      | <span data-ttu-id="4dfab-135">O tipo de grupo a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="4dfab-135">The group type to search for.</span></span> <span data-ttu-id="4dfab-136">As opções disponíveis são: `unified` , , , , `security` `mailenabledsecurity` `distribution` `any` .</span><span class="sxs-lookup"><span data-stu-id="4dfab-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="4dfab-137">O valor padrão é `any`.</span><span class="sxs-lookup"><span data-stu-id="4dfab-137">Default value is `any`.</span></span> <span data-ttu-id="4dfab-138">Esse atributo não terá efeito se a `type` propriedade estiver definida como `person` .</span><span class="sxs-lookup"><span data-stu-id="4dfab-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="4dfab-139">selected-people</span><span class="sxs-lookup"><span data-stu-id="4dfab-139">selected-people</span></span>  | <span data-ttu-id="4dfab-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="4dfab-140">selectedPeople</span></span>     | <span data-ttu-id="4dfab-141">Uma matriz de pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="4dfab-141">An array of selected people.</span></span> <span data-ttu-id="4dfab-142">De definir esse valor para selecionar pessoas de forma programática.</span><span class="sxs-lookup"><span data-stu-id="4dfab-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="4dfab-143">people</span><span class="sxs-lookup"><span data-stu-id="4dfab-143">people</span></span>   | <span data-ttu-id="4dfab-144">people</span><span class="sxs-lookup"><span data-stu-id="4dfab-144">people</span></span>    | <span data-ttu-id="4dfab-145">Uma matriz de pessoas encontradas e renderizadas no resultado da pesquisa</span><span class="sxs-lookup"><span data-stu-id="4dfab-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="4dfab-146">espaço reservado</span><span class="sxs-lookup"><span data-stu-id="4dfab-146">placeholder</span></span>   | <span data-ttu-id="4dfab-147">espaço reservado</span><span class="sxs-lookup"><span data-stu-id="4dfab-147">placeholder</span></span>    | <span data-ttu-id="4dfab-148">O texto padrão que parece explicar como usar o componente.</span><span class="sxs-lookup"><span data-stu-id="4dfab-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="4dfab-149">O valor padrão é `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="4dfab-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="4dfab-150">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="4dfab-150">default-selected-user-ids</span></span> | <span data-ttu-id="4dfab-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="4dfab-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="4dfab-152">Quando fornecida uma cadeia de caracteres de IDs de usuário separadas por vírgulas do Microsoft Graph, o componente renderiza os respectivos usuários conforme selecionado na inicialização.</span><span class="sxs-lookup"><span data-stu-id="4dfab-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="4dfab-153">modo de seleção</span><span class="sxs-lookup"><span data-stu-id="4dfab-153">selection-mode</span></span> | <span data-ttu-id="4dfab-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="4dfab-154">selectionMode</span></span> | <span data-ttu-id="4dfab-155">Usado para indicar se é para permitir a seleção de vários itens (usuários ou grupos) ou apenas um único item.</span><span class="sxs-lookup"><span data-stu-id="4dfab-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="4dfab-156">As opções disponíveis são: `single` , `multiple` .</span><span class="sxs-lookup"><span data-stu-id="4dfab-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="4dfab-157">O valor padrão é `multiple`.</span><span class="sxs-lookup"><span data-stu-id="4dfab-157">Default value is `multiple`.</span></span>

<span data-ttu-id="4dfab-158">A seguir está um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="4dfab-158">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="4dfab-159">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="4dfab-159">Selected people</span></span>

<span data-ttu-id="4dfab-160">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou usuário.</span><span class="sxs-lookup"><span data-stu-id="4dfab-160">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="4dfab-162">Você pode preencher dados de pessoas selecionadas seguindo um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="4dfab-162">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="4dfab-163">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4dfab-163">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="4dfab-164">Usando o método, que aceita uma matriz de IDs de usuário do Microsoft Graph para `selectUsersById()` encontrar detalhes de usuário associados para seleção. [](/graph/api/resources/users)</span><span class="sxs-lookup"><span data-stu-id="4dfab-164">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="4dfab-165">**Observação:** Se nenhum usuário for encontrado para `id` um , nenhum dado será renderizado para `id` isso.</span><span class="sxs-lookup"><span data-stu-id="4dfab-165">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="4dfab-166">Eventos</span><span class="sxs-lookup"><span data-stu-id="4dfab-166">Events</span></span>

<span data-ttu-id="4dfab-167">Os eventos a seguir são disparados do componente.</span><span class="sxs-lookup"><span data-stu-id="4dfab-167">The following events are fired from the component.</span></span>

| <span data-ttu-id="4dfab-168">Evento</span><span class="sxs-lookup"><span data-stu-id="4dfab-168">Event</span></span> | <span data-ttu-id="4dfab-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dfab-169">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="4dfab-170">O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/selecionadas.</span><span class="sxs-lookup"><span data-stu-id="4dfab-170">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="4dfab-171">Propriedades personalizadas css</span><span class="sxs-lookup"><span data-stu-id="4dfab-171">CSS custom properties</span></span>

<span data-ttu-id="4dfab-172">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="4dfab-172">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="4dfab-173">Modelos</span><span class="sxs-lookup"><span data-stu-id="4dfab-173">Templates</span></span>

 <span data-ttu-id="4dfab-174">`mgt-people-picker` oferece suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="4dfab-174">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="4dfab-175">Para especificar um modelo, inclua um elemento dentro de um componente e de definir `<template>` o valor como um dos `data-type` seguintes.</span><span class="sxs-lookup"><span data-stu-id="4dfab-175">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="4dfab-176">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="4dfab-176">Data type</span></span> | <span data-ttu-id="4dfab-177">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="4dfab-177">Data context</span></span> | <span data-ttu-id="4dfab-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dfab-178">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="4dfab-179">Padrão.</span><span class="sxs-lookup"><span data-stu-id="4dfab-179">default</span></span> | <span data-ttu-id="4dfab-180">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="4dfab-180">null: no data</span></span> | <span data-ttu-id="4dfab-181">O modelo usado para substituir a renderização do componente inteiro.</span><span class="sxs-lookup"><span data-stu-id="4dfab-181">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="4dfab-182">carregando</span><span class="sxs-lookup"><span data-stu-id="4dfab-182">loading</span></span> | <span data-ttu-id="4dfab-183">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="4dfab-183">null: no data</span></span> | <span data-ttu-id="4dfab-184">O modelo usado para renderizar o estado do selador enquanto a solicitação para o gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="4dfab-184">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="4dfab-185">erro</span><span class="sxs-lookup"><span data-stu-id="4dfab-185">error</span></span> | <span data-ttu-id="4dfab-186">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="4dfab-186">null: no data</span></span> | <span data-ttu-id="4dfab-187">O modelo usado se a pesquisa do usuário não retornar usuários.</span><span class="sxs-lookup"><span data-stu-id="4dfab-187">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="4dfab-188">no-data</span><span class="sxs-lookup"><span data-stu-id="4dfab-188">no-data</span></span> | <span data-ttu-id="4dfab-189">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="4dfab-189">null: no data</span></span> | <span data-ttu-id="4dfab-190">Um modelo alternativo usado se a pesquisa do usuário não retornar usuários.</span><span class="sxs-lookup"><span data-stu-id="4dfab-190">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="4dfab-191">selected-person</span><span class="sxs-lookup"><span data-stu-id="4dfab-191">selected-person</span></span> | <span data-ttu-id="4dfab-192">pessoa: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="4dfab-192">person: The person details object</span></span> | <span data-ttu-id="4dfab-193">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="4dfab-193">The template to render selected people.</span></span> |
| <span data-ttu-id="4dfab-194">person</span><span class="sxs-lookup"><span data-stu-id="4dfab-194">person</span></span> | <span data-ttu-id="4dfab-195">pessoa: O objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="4dfab-195">person: The person details object</span></span> | <span data-ttu-id="4dfab-196">O modelo para renderizar pessoas no menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="4dfab-196">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="4dfab-197">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="4dfab-197">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="4dfab-198">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4dfab-198">Microsoft Graph permissions</span></span>

<span data-ttu-id="4dfab-199">Esse componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4dfab-199">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="4dfab-200">API</span><span class="sxs-lookup"><span data-stu-id="4dfab-200">API</span></span>                                                                                                              | <span data-ttu-id="4dfab-201">Permissão</span><span class="sxs-lookup"><span data-stu-id="4dfab-201">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="4dfab-202">/me/people</span><span class="sxs-lookup"><span data-stu-id="4dfab-202">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="4dfab-203">People.Read</span><span class="sxs-lookup"><span data-stu-id="4dfab-203">People.Read</span></span>        |
| [<span data-ttu-id="4dfab-204">/users</span><span class="sxs-lookup"><span data-stu-id="4dfab-204">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="4dfab-205">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4dfab-205">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="4dfab-206">/groups</span><span class="sxs-lookup"><span data-stu-id="4dfab-206">/groups</span></span>](/group-list)  | <span data-ttu-id="4dfab-207">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4dfab-207">Group.Read.All</span></span> |
| [<span data-ttu-id="4dfab-208">/groups/ \$ {groupId}/members</span><span class="sxs-lookup"><span data-stu-id="4dfab-208">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="4dfab-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4dfab-209">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="4dfab-210">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="4dfab-210">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="4dfab-211">User.Read</span><span class="sxs-lookup"><span data-stu-id="4dfab-211">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="4dfab-212">Autenticação</span><span class="sxs-lookup"><span data-stu-id="4dfab-212">Authentication</span></span>

<span data-ttu-id="4dfab-213">O controle usa o provedor de autenticação global descrito na [documentação de autenticação.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="4dfab-213">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="4dfab-214">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="4dfab-214">Extend for more control</span></span>

<span data-ttu-id="4dfab-215">Para cenários mais complexos ou uma experiência de trabalho realmente personalizada, esse componente expõe vários métodos para substituição `protected render*` em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="4dfab-215">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="4dfab-216">Método</span><span class="sxs-lookup"><span data-stu-id="4dfab-216">Method</span></span> | <span data-ttu-id="4dfab-217">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dfab-217">Description</span></span> |
| - | - |
| <span data-ttu-id="4dfab-218">renderInput</span><span class="sxs-lookup"><span data-stu-id="4dfab-218">renderInput</span></span> | <span data-ttu-id="4dfab-219">Renderiza a caixa de texto de entrada.</span><span class="sxs-lookup"><span data-stu-id="4dfab-219">Renders the input text box.</span></span> |
| <span data-ttu-id="4dfab-220">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="4dfab-220">renderSelectedPeople</span></span> | <span data-ttu-id="4dfab-221">Renderiza os tokens de pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="4dfab-221">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="4dfab-222">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="4dfab-222">renderSelectedPerson</span></span> | <span data-ttu-id="4dfab-223">Renderiza um token de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="4dfab-223">Renders an individual person token.</span></span> |
| <span data-ttu-id="4dfab-224">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="4dfab-224">renderFlyout</span></span> | <span data-ttu-id="4dfab-225">Renderiza o cromado do flyout.</span><span class="sxs-lookup"><span data-stu-id="4dfab-225">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="4dfab-226">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="4dfab-226">renderFlyoutContent</span></span> | <span data-ttu-id="4dfab-227">Renderiza o estado apropriado no flyout de resultados.</span><span class="sxs-lookup"><span data-stu-id="4dfab-227">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="4dfab-228">renderLoading</span><span class="sxs-lookup"><span data-stu-id="4dfab-228">renderLoading</span></span> | <span data-ttu-id="4dfab-229">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="4dfab-229">Renders the loading state.</span></span> |
| <span data-ttu-id="4dfab-230">renderNoData</span><span class="sxs-lookup"><span data-stu-id="4dfab-230">renderNoData</span></span> | <span data-ttu-id="4dfab-231">Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4dfab-231">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="4dfab-232">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="4dfab-232">renderSearchResults</span></span> | <span data-ttu-id="4dfab-233">Renderiza a lista de resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4dfab-233">Renders the list of search results.</span></span> |
| <span data-ttu-id="4dfab-234">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="4dfab-234">renderPersonResult</span></span> | <span data-ttu-id="4dfab-235">Renderiza um resultado de pesquisa de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="4dfab-235">Renders an individual person search result.</span></span> |
