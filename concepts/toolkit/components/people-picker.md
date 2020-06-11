---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: e3e656c6aef0ab2af9878fb3e4738ade912c4685
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681883"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="82056-103">Componente de seletor de pessoas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="82056-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="82056-104">Você pode usar o `mgt-people-picker` componente da Web para procurar pessoas e/ou grupos.</span><span class="sxs-lookup"><span data-stu-id="82056-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="82056-105">Por padrão, o componente pesquisará todas as pessoas e usuários da organização, mas você pode alterar o comportamento para também pesquisar grupos ou apenas grupos.</span><span class="sxs-lookup"><span data-stu-id="82056-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="82056-106">Você também pode filtrar a pesquisa para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="82056-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="82056-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82056-107">Example</span></span>

<span data-ttu-id="82056-108">O exemplo a seguir mostra o `mgt-people-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="82056-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="82056-109">Comece a pesquisar um nome para ver os resultados renderizar e usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="82056-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="82056-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="82056-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="82056-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82056-111">Properties</span></span>

<span data-ttu-id="82056-112">Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos de `/me/people` `/users` extremidade e.</span><span class="sxs-lookup"><span data-stu-id="82056-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="82056-113">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="82056-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="82056-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="82056-114">Attribute</span></span> | <span data-ttu-id="82056-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82056-115">Property</span></span> | <span data-ttu-id="82056-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="82056-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="82056-117">show-Max</span><span class="sxs-lookup"><span data-stu-id="82056-117">show-max</span></span> | <span data-ttu-id="82056-118">showMax</span><span class="sxs-lookup"><span data-stu-id="82056-118">showMax</span></span>   | <span data-ttu-id="82056-119">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="82056-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="82056-120">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="82056-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="82056-121">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="82056-121">group-id</span></span>    | <span data-ttu-id="82056-122">groupId</span><span class="sxs-lookup"><span data-stu-id="82056-122">groupId</span></span>     | <span data-ttu-id="82056-123">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="82056-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="82056-124">tipo</span><span class="sxs-lookup"><span data-stu-id="82056-124">type</span></span>     | <span data-ttu-id="82056-125">tipo</span><span class="sxs-lookup"><span data-stu-id="82056-125">type</span></span>      | <span data-ttu-id="82056-126">O tipo de entidades a serem pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="82056-126">The type of entities to search for.</span></span> <span data-ttu-id="82056-127">As opções disponíveis são: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="82056-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="82056-128">O valor padrão é `person`.</span><span class="sxs-lookup"><span data-stu-id="82056-128">Default value is `person`.</span></span> <span data-ttu-id="82056-129">Este atributo não terá efeito se a `group-id` propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="82056-129">This attribute has no effect if `group-id` property is set.</span></span>                                                                            |
| <span data-ttu-id="82056-130">tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="82056-130">group-type</span></span>     | <span data-ttu-id="82056-131">groupType</span><span class="sxs-lookup"><span data-stu-id="82056-131">groupType</span></span>      | <span data-ttu-id="82056-132">O tipo de grupo a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="82056-132">The group type to search for.</span></span> <span data-ttu-id="82056-133">As opções disponíveis são: `unified` , `security` , `mailenabledsecurity` , `distribution` , `any` .</span><span class="sxs-lookup"><span data-stu-id="82056-133">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="82056-134">O valor padrão é `any`.</span><span class="sxs-lookup"><span data-stu-id="82056-134">Default value is `any`.</span></span> <span data-ttu-id="82056-135">Este atributo não terá efeito se a `type` propriedade for definida como `person` .</span><span class="sxs-lookup"><span data-stu-id="82056-135">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="82056-136">selecionado-pessoas</span><span class="sxs-lookup"><span data-stu-id="82056-136">selected-people</span></span>  | <span data-ttu-id="82056-137">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="82056-137">selectedPeople</span></span>     | <span data-ttu-id="82056-138">Uma matriz de pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="82056-138">An array of selected people.</span></span> <span data-ttu-id="82056-139">Defina esse valor para selecionar pessoas de forma programática.</span><span class="sxs-lookup"><span data-stu-id="82056-139">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="82056-140">people</span><span class="sxs-lookup"><span data-stu-id="82056-140">people</span></span>   | <span data-ttu-id="82056-141">people</span><span class="sxs-lookup"><span data-stu-id="82056-141">people</span></span>    | <span data-ttu-id="82056-142">Uma matriz de pessoas encontrada e renderizada no resultado da pesquisa</span><span class="sxs-lookup"><span data-stu-id="82056-142">An array of people found and rendered in the search result</span></span> |

<span data-ttu-id="82056-143">Este é um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="82056-143">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="82056-144">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="82056-144">Selected people</span></span>

<span data-ttu-id="82056-145">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="82056-145">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

<span data-ttu-id="82056-147">Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="82056-147">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="82056-148">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="82056-148">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="82056-149">Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.</span><span class="sxs-lookup"><span data-stu-id="82056-149">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="82056-150">**Observação:** Se nenhum usuário for localizado para um `id` , nenhum dado será renderizado para isso `id` .</span><span class="sxs-lookup"><span data-stu-id="82056-150">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="82056-151">Eventos</span><span class="sxs-lookup"><span data-stu-id="82056-151">Events</span></span>

<span data-ttu-id="82056-152">Os eventos a seguir são acionados do componente.</span><span class="sxs-lookup"><span data-stu-id="82056-152">The following events are fired from the component.</span></span>

| <span data-ttu-id="82056-153">Evento</span><span class="sxs-lookup"><span data-stu-id="82056-153">Event</span></span> | <span data-ttu-id="82056-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="82056-154">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="82056-155">O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/escolhidas.</span><span class="sxs-lookup"><span data-stu-id="82056-155">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="82056-156">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="82056-156">CSS custom properties</span></span>

<span data-ttu-id="82056-157">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="82056-157">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a><span data-ttu-id="82056-158">Modelos</span><span class="sxs-lookup"><span data-stu-id="82056-158">Templates</span></span>

 <span data-ttu-id="82056-159">`mgt-people-picker`o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="82056-159">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="82056-160">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="82056-160">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="82056-161">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="82056-161">Data type</span></span> | <span data-ttu-id="82056-162">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="82056-162">Data context</span></span> | <span data-ttu-id="82056-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="82056-163">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="82056-164">Padrão.</span><span class="sxs-lookup"><span data-stu-id="82056-164">default</span></span> | <span data-ttu-id="82056-165">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="82056-165">null: no data</span></span> | <span data-ttu-id="82056-166">O modelo usado para substituir a renderização de todo o componente.</span><span class="sxs-lookup"><span data-stu-id="82056-166">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="82056-167">carregando</span><span class="sxs-lookup"><span data-stu-id="82056-167">loading</span></span> | <span data-ttu-id="82056-168">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="82056-168">null: no data</span></span> | <span data-ttu-id="82056-169">O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="82056-169">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="82056-170">erro</span><span class="sxs-lookup"><span data-stu-id="82056-170">error</span></span> | <span data-ttu-id="82056-171">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="82056-171">null: no data</span></span> | <span data-ttu-id="82056-172">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="82056-172">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="82056-173">sem dados</span><span class="sxs-lookup"><span data-stu-id="82056-173">no-data</span></span> | <span data-ttu-id="82056-174">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="82056-174">null: no data</span></span> | <span data-ttu-id="82056-175">Um modelo alternativo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="82056-175">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="82056-176">selecionado-pessoa</span><span class="sxs-lookup"><span data-stu-id="82056-176">selected-person</span></span> | <span data-ttu-id="82056-177">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="82056-177">person: The person details object</span></span> | <span data-ttu-id="82056-178">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="82056-178">The template to render selected people.</span></span> |
| <span data-ttu-id="82056-179">vendedor</span><span class="sxs-lookup"><span data-stu-id="82056-179">person</span></span> | <span data-ttu-id="82056-180">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="82056-180">person: The person details object</span></span> | <span data-ttu-id="82056-181">O modelo para renderizar pessoas na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="82056-181">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="82056-182">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="82056-182">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="82056-183">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="82056-183">Microsoft Graph permissions</span></span>

<span data-ttu-id="82056-184">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="82056-184">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="82056-185">API</span><span class="sxs-lookup"><span data-stu-id="82056-185">API</span></span>                                                                                                              | <span data-ttu-id="82056-186">Permission</span><span class="sxs-lookup"><span data-stu-id="82056-186">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="82056-187">/me/people</span><span class="sxs-lookup"><span data-stu-id="82056-187">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="82056-188">People.Read</span><span class="sxs-lookup"><span data-stu-id="82056-188">People.Read</span></span>        |
| [<span data-ttu-id="82056-189">/Users</span><span class="sxs-lookup"><span data-stu-id="82056-189">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0)  | <span data-ttu-id="82056-190">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="82056-190">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="82056-191">/groups</span><span class="sxs-lookup"><span data-stu-id="82056-191">/groups</span></span>](/group-list?view=graph-rest-beta)  | <span data-ttu-id="82056-192">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="82056-192">Group.Read.All</span></span> |
| [<span data-ttu-id="82056-193">/groups/ \$ {GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="82056-193">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="82056-194">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="82056-194">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="82056-195">/Users/$ {userprincípioname}</span><span class="sxs-lookup"><span data-stu-id="82056-195">/users/${userPrincipleName} </span></span>](/graph/api/user-get?view=graph-rest-1.0)  | <span data-ttu-id="82056-196">User.Read</span><span class="sxs-lookup"><span data-stu-id="82056-196">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="82056-197">Autenticação</span><span class="sxs-lookup"><span data-stu-id="82056-197">Authentication</span></span>

<span data-ttu-id="82056-198">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="82056-198">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="82056-199">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="82056-199">Extend for more control</span></span>

<span data-ttu-id="82056-200">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="82056-200">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="82056-201">Método</span><span class="sxs-lookup"><span data-stu-id="82056-201">Method</span></span> | <span data-ttu-id="82056-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="82056-202">Description</span></span> |
| - | - |
| <span data-ttu-id="82056-203">renderInput</span><span class="sxs-lookup"><span data-stu-id="82056-203">renderInput</span></span> | <span data-ttu-id="82056-204">Renderiza a caixa de texto de entrada.</span><span class="sxs-lookup"><span data-stu-id="82056-204">Renders the input text box.</span></span> |
| <span data-ttu-id="82056-205">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="82056-205">renderSelectedPeople</span></span> | <span data-ttu-id="82056-206">Renderiza os tokens de pessoas selecionados.</span><span class="sxs-lookup"><span data-stu-id="82056-206">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="82056-207">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="82056-207">renderSelectedPerson</span></span> | <span data-ttu-id="82056-208">Renderiza um token de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="82056-208">Renders an individual person token.</span></span> |
| <span data-ttu-id="82056-209">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="82056-209">renderFlyout</span></span> | <span data-ttu-id="82056-210">Renderiza o cromo domenu.</span><span class="sxs-lookup"><span data-stu-id="82056-210">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="82056-211">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="82056-211">renderFlyoutContent</span></span> | <span data-ttu-id="82056-212">Processa o estado apropriado no submenu de resultados.</span><span class="sxs-lookup"><span data-stu-id="82056-212">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="82056-213">renderLoading</span><span class="sxs-lookup"><span data-stu-id="82056-213">renderLoading</span></span> | <span data-ttu-id="82056-214">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="82056-214">Renders the loading state.</span></span> |
| <span data-ttu-id="82056-215">renderNoData</span><span class="sxs-lookup"><span data-stu-id="82056-215">renderNoData</span></span> | <span data-ttu-id="82056-216">Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="82056-216">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="82056-217">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="82056-217">renderSearchResults</span></span> | <span data-ttu-id="82056-218">Renderiza a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="82056-218">Renders the list of search results.</span></span> |
| <span data-ttu-id="82056-219">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="82056-219">renderPersonResult</span></span> | <span data-ttu-id="82056-220">Renderiza um resultado de pesquisa de pessoa individual.</span><span class="sxs-lookup"><span data-stu-id="82056-220">Renders an individual person search result.</span></span> |
