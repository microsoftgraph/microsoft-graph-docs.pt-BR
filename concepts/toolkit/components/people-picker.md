---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 22ad36715dd0405d44214901a0adf90bb717b167
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955880"
---
# <a name="people-picker-component"></a><span data-ttu-id="ce541-103">Componente de seletor de pessoas</span><span class="sxs-lookup"><span data-stu-id="ce541-103">People-Picker component</span></span>

<span data-ttu-id="ce541-104">Você pode usar a `mgt-people-picker` pesquisa de componente da Web para um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ce541-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="ce541-105">Por padrão, o componente pesquisará todas as pessoas; Você também pode definir uma propriedade de grupo para filtrar os resultados.</span><span class="sxs-lookup"><span data-stu-id="ce541-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="ce541-106">Se o número de pessoas a serem exibidas exceder o `show-max` valor, nem todas as pessoas retornadas serão exibidas na lista de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ce541-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="ce541-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce541-107">Example</span></span>

[<span data-ttu-id="ce541-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="ce541-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![gerenciamento de pessoas-seletor](./images/mgt-people-picker-image.png)

## <a name="properties"></a><span data-ttu-id="ce541-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce541-110">Properties</span></span>

<span data-ttu-id="ce541-111">Por padrão, o `mgt-people-picker` componente busca eventos do `/me/people` ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ce541-111">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="ce541-112">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="ce541-112">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="ce541-113">Atributo</span><span class="sxs-lookup"><span data-stu-id="ce541-113">Attribute</span></span> | <span data-ttu-id="ce541-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce541-114">Property</span></span> | <span data-ttu-id="ce541-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce541-115">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ce541-116">show-Max</span><span class="sxs-lookup"><span data-stu-id="ce541-116">show-max</span></span> | <span data-ttu-id="ce541-117">showMax</span><span class="sxs-lookup"><span data-stu-id="ce541-117">showMax</span></span>   | <span data-ttu-id="ce541-118">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="ce541-118">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="ce541-119">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="ce541-119">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="ce541-120">people</span><span class="sxs-lookup"><span data-stu-id="ce541-120">people</span></span>   | <span data-ttu-id="ce541-121">people</span><span class="sxs-lookup"><span data-stu-id="ce541-121">people</span></span>    | <span data-ttu-id="ce541-122">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="ce541-122">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="ce541-123">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="ce541-123">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="ce541-124">Defina esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="ce541-124">Set this value to load your own people.</span></span> |
| <span data-ttu-id="ce541-125">group</span><span class="sxs-lookup"><span data-stu-id="ce541-125">group</span></span>    | <span data-ttu-id="ce541-126">group</span><span class="sxs-lookup"><span data-stu-id="ce541-126">group</span></span>     | <span data-ttu-id="ce541-127">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ce541-127">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="ce541-128">selecionado-pessoas</span><span class="sxs-lookup"><span data-stu-id="ce541-128">selected-people</span></span>  | <span data-ttu-id="ce541-129">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="ce541-129">selectedPeople</span></span>     | <span data-ttu-id="ce541-130">Uma matriz do tipo `person`, representando pessoas selecionadas no componente.</span><span class="sxs-lookup"><span data-stu-id="ce541-130">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="ce541-131">Defina esse valor para escolher as pessoas selecionadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="ce541-131">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="ce541-132">Este é um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="ce541-132">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="ce541-133">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="ce541-133">Selected people</span></span>

<span data-ttu-id="ce541-134">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="ce541-134">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

<span data-ttu-id="ce541-136">Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="ce541-136">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="ce541-137">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="ce541-137">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="ce541-138">Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.</span><span class="sxs-lookup"><span data-stu-id="ce541-138">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="ce541-139">**Observação:** Se nenhum usuário for localizado para um `id`, nenhum dado será renderizado para isso `id`.</span><span class="sxs-lookup"><span data-stu-id="ce541-139">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="ce541-140">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="ce541-140">CSS custom properties</span></span>

<span data-ttu-id="ce541-141">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="ce541-141">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="ce541-142">Modelos</span><span class="sxs-lookup"><span data-stu-id="ce541-142">Templates</span></span>

 <span data-ttu-id="ce541-143">`mgt-people-picker`o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="ce541-143">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="ce541-144">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="ce541-144">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="ce541-145">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="ce541-145">Data type</span></span> | <span data-ttu-id="ce541-146">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="ce541-146">Data context</span></span> | <span data-ttu-id="ce541-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce541-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="ce541-148">carregando</span><span class="sxs-lookup"><span data-stu-id="ce541-148">loading</span></span> | <span data-ttu-id="ce541-149">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="ce541-149">null: no data</span></span> | <span data-ttu-id="ce541-150">O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="ce541-150">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="ce541-151">erro</span><span class="sxs-lookup"><span data-stu-id="ce541-151">error</span></span> | <span data-ttu-id="ce541-152">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="ce541-152">null: no data</span></span>| <span data-ttu-id="ce541-153">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="ce541-153">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="ce541-154">selecionado-pessoa</span><span class="sxs-lookup"><span data-stu-id="ce541-154">selected-person</span></span> |<span data-ttu-id="ce541-155">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="ce541-155">person: The person details object</span></span>| <span data-ttu-id="ce541-156">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="ce541-156">The template to render selected people.</span></span> |
| <span data-ttu-id="ce541-157">person</span><span class="sxs-lookup"><span data-stu-id="ce541-157">person</span></span> | <span data-ttu-id="ce541-158">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="ce541-158">person: The person details object</span></span>| <span data-ttu-id="ce541-159">O modelo para renderizar pessoas na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="ce541-159">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="ce541-160">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="ce541-160">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ce541-161">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ce541-161">Microsoft Graph permissions</span></span>

<span data-ttu-id="ce541-162">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ce541-162">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="ce541-163">API</span><span class="sxs-lookup"><span data-stu-id="ce541-163">API</span></span>                                                                                                              | <span data-ttu-id="ce541-164">Permissão</span><span class="sxs-lookup"><span data-stu-id="ce541-164">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="ce541-165">/me/people</span><span class="sxs-lookup"><span data-stu-id="ce541-165">/me/people</span></span>](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="ce541-166">People.Read</span><span class="sxs-lookup"><span data-stu-id="ce541-166">People.Read</span></span> |
| [<span data-ttu-id="ce541-167">/groups/\${GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="ce541-167">/groups/\${groupId}/members</span></span>](https://docs.microsoft.com/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="ce541-168">People.Read</span><span class="sxs-lookup"><span data-stu-id="ce541-168">People.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="ce541-169">Autenticação</span><span class="sxs-lookup"><span data-stu-id="ce541-169">Authentication</span></span>

<span data-ttu-id="ce541-170">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="ce541-170">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
