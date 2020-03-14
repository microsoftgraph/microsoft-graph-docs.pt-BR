---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 91b11006df02d563902b99c79c4b1ec09bb7e50a
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639937"
---
# <a name="people-picker-component"></a><span data-ttu-id="8477f-103">Componente de seletor de pessoas</span><span class="sxs-lookup"><span data-stu-id="8477f-103">People-Picker component</span></span>

<span data-ttu-id="8477f-104">Você pode usar a `mgt-people-picker` pesquisa de componente da Web para um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8477f-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="8477f-105">Por padrão, o componente pesquisará todas as pessoas; Você também pode definir uma propriedade de grupo para filtrar os resultados.</span><span class="sxs-lookup"><span data-stu-id="8477f-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="8477f-106">Se o número de pessoas a serem exibidas exceder o `show-max` valor, nem todas as pessoas retornadas serão exibidas na lista de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8477f-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="8477f-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8477f-107">Example</span></span>

<span data-ttu-id="8477f-108">O exemplo a seguir mostra `mgt-people-picker` o componente.</span><span class="sxs-lookup"><span data-stu-id="8477f-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="8477f-109">Comece a pesquisar um nome para ver os resultados renderizar e usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="8477f-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="8477f-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="8477f-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="8477f-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8477f-111">Properties</span></span>

<span data-ttu-id="8477f-112">Por padrão, o `mgt-people-picker` componente busca eventos do `/me/people` ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="8477f-112">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="8477f-113">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="8477f-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="8477f-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="8477f-114">Attribute</span></span> | <span data-ttu-id="8477f-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8477f-115">Property</span></span> | <span data-ttu-id="8477f-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="8477f-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8477f-117">show-Max</span><span class="sxs-lookup"><span data-stu-id="8477f-117">show-max</span></span> | <span data-ttu-id="8477f-118">showMax</span><span class="sxs-lookup"><span data-stu-id="8477f-118">showMax</span></span>   | <span data-ttu-id="8477f-119">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="8477f-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="8477f-120">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="8477f-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="8477f-121">people</span><span class="sxs-lookup"><span data-stu-id="8477f-121">people</span></span>   | <span data-ttu-id="8477f-122">people</span><span class="sxs-lookup"><span data-stu-id="8477f-122">people</span></span>    | <span data-ttu-id="8477f-123">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="8477f-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="8477f-124">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="8477f-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="8477f-125">Defina esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="8477f-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="8477f-126">group</span><span class="sxs-lookup"><span data-stu-id="8477f-126">group</span></span>    | <span data-ttu-id="8477f-127">group</span><span class="sxs-lookup"><span data-stu-id="8477f-127">group</span></span>     | <span data-ttu-id="8477f-128">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8477f-128">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="8477f-129">selecionado-pessoas</span><span class="sxs-lookup"><span data-stu-id="8477f-129">selected-people</span></span>  | <span data-ttu-id="8477f-130">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="8477f-130">selectedPeople</span></span>     | <span data-ttu-id="8477f-131">Uma matriz do tipo `person`, representando pessoas selecionadas no componente.</span><span class="sxs-lookup"><span data-stu-id="8477f-131">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="8477f-132">Defina esse valor para escolher as pessoas selecionadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="8477f-132">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="8477f-133">Este é um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="8477f-133">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="8477f-134">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="8477f-134">Selected people</span></span>

<span data-ttu-id="8477f-135">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8477f-135">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

<span data-ttu-id="8477f-137">Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="8477f-137">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="8477f-138">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="8477f-138">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="8477f-139">Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.</span><span class="sxs-lookup"><span data-stu-id="8477f-139">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="8477f-140">**Observação:** Se nenhum usuário for localizado para um `id`, nenhum dado será renderizado para isso `id`.</span><span class="sxs-lookup"><span data-stu-id="8477f-140">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="8477f-141">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="8477f-141">CSS custom properties</span></span>

<span data-ttu-id="8477f-142">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="8477f-142">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="8477f-143">Modelos</span><span class="sxs-lookup"><span data-stu-id="8477f-143">Templates</span></span>

 <span data-ttu-id="8477f-144">`mgt-people-picker`o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="8477f-144">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="8477f-145">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="8477f-145">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="8477f-146">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="8477f-146">Data type</span></span> | <span data-ttu-id="8477f-147">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="8477f-147">Data context</span></span> | <span data-ttu-id="8477f-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="8477f-148">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8477f-149">carregando</span><span class="sxs-lookup"><span data-stu-id="8477f-149">loading</span></span> | <span data-ttu-id="8477f-150">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="8477f-150">null: no data</span></span> | <span data-ttu-id="8477f-151">O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="8477f-151">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="8477f-152">erro</span><span class="sxs-lookup"><span data-stu-id="8477f-152">error</span></span> | <span data-ttu-id="8477f-153">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="8477f-153">null: no data</span></span>| <span data-ttu-id="8477f-154">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="8477f-154">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="8477f-155">selecionado-pessoa</span><span class="sxs-lookup"><span data-stu-id="8477f-155">selected-person</span></span> |<span data-ttu-id="8477f-156">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="8477f-156">person: The person details object</span></span>| <span data-ttu-id="8477f-157">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="8477f-157">The template to render selected people.</span></span> |
| <span data-ttu-id="8477f-158">vendedor</span><span class="sxs-lookup"><span data-stu-id="8477f-158">person</span></span> | <span data-ttu-id="8477f-159">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="8477f-159">person: The person details object</span></span>| <span data-ttu-id="8477f-160">O modelo para renderizar pessoas na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="8477f-160">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="8477f-161">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="8477f-161">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8477f-162">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8477f-162">Microsoft Graph permissions</span></span>

<span data-ttu-id="8477f-163">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8477f-163">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="8477f-164">API</span><span class="sxs-lookup"><span data-stu-id="8477f-164">API</span></span>                                                                                                              | <span data-ttu-id="8477f-165">Permissão</span><span class="sxs-lookup"><span data-stu-id="8477f-165">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="8477f-166">/me/people</span><span class="sxs-lookup"><span data-stu-id="8477f-166">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="8477f-167">People.Read</span><span class="sxs-lookup"><span data-stu-id="8477f-167">People.Read</span></span>        |
| [<span data-ttu-id="8477f-168">/groups/\${GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="8477f-168">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="8477f-169">People.Read</span><span class="sxs-lookup"><span data-stu-id="8477f-169">People.Read</span></span>        |
| [<span data-ttu-id="8477f-170">/Users/$ {userprincípioname}</span><span class="sxs-lookup"><span data-stu-id="8477f-170">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="8477f-171">User. Readbasic. All</span><span class="sxs-lookup"><span data-stu-id="8477f-171">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="8477f-172">Autenticação</span><span class="sxs-lookup"><span data-stu-id="8477f-172">Authentication</span></span>

<span data-ttu-id="8477f-173">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="8477f-173">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
