---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 65ff9382de97ddcd7a0b4bd8a315f8350a80ec35
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023121"
---
# <a name="people-picker-component"></a><span data-ttu-id="a9822-103">Componente de seletor de pessoas</span><span class="sxs-lookup"><span data-stu-id="a9822-103">People-Picker component</span></span>

<span data-ttu-id="a9822-104">Você pode usar a `mgt-people-picker` pesquisa de componente da Web para um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a9822-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="a9822-105">Por padrão, o componente pesquisará todas as pessoas; Você também pode definir uma propriedade de grupo para filtrar os resultados.</span><span class="sxs-lookup"><span data-stu-id="a9822-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="a9822-106">Se o número de pessoas a serem exibidas exceder o `show-max` valor, nem todas as pessoas retornadas serão exibidas na lista de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a9822-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="a9822-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9822-107">Example</span></span>

[<span data-ttu-id="a9822-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="a9822-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![gerenciamento de pessoas-seletor](./images/mgt-people-picker-image.png)

## <a name="properties"></a><span data-ttu-id="a9822-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9822-110">Properties</span></span>

<span data-ttu-id="a9822-111">Por padrão, o `mgt-people-picker` componente busca eventos do `/me/people` ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="a9822-111">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="a9822-112">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="a9822-112">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="a9822-113">Atributo</span><span class="sxs-lookup"><span data-stu-id="a9822-113">Attribute</span></span> | <span data-ttu-id="a9822-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9822-114">Property</span></span> | <span data-ttu-id="a9822-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9822-115">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a9822-116">show-Max</span><span class="sxs-lookup"><span data-stu-id="a9822-116">show-max</span></span> | <span data-ttu-id="a9822-117">showMax</span><span class="sxs-lookup"><span data-stu-id="a9822-117">showMax</span></span>   | <span data-ttu-id="a9822-118">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="a9822-118">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="a9822-119">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="a9822-119">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="a9822-120">people</span><span class="sxs-lookup"><span data-stu-id="a9822-120">people</span></span>   | <span data-ttu-id="a9822-121">people</span><span class="sxs-lookup"><span data-stu-id="a9822-121">people</span></span>    | <span data-ttu-id="a9822-122">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="a9822-122">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="a9822-123">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="a9822-123">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="a9822-124">Defina esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="a9822-124">Set this value to load your own people.</span></span> |
| <span data-ttu-id="a9822-125">group</span><span class="sxs-lookup"><span data-stu-id="a9822-125">group</span></span>    | <span data-ttu-id="a9822-126">group</span><span class="sxs-lookup"><span data-stu-id="a9822-126">group</span></span>     | <span data-ttu-id="a9822-127">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a9822-127">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="a9822-128">selecionado-pessoas</span><span class="sxs-lookup"><span data-stu-id="a9822-128">selected-people</span></span>  | <span data-ttu-id="a9822-129">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="a9822-129">selectedPeople</span></span>     | <span data-ttu-id="a9822-130">Uma matriz do tipo `person`, representando pessoas selecionadas no componente.</span><span class="sxs-lookup"><span data-stu-id="a9822-130">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="a9822-131">Defina esse valor para escolher as pessoas selecionadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="a9822-131">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="a9822-132">Este é um `show-max` exemplo.</span><span class="sxs-lookup"><span data-stu-id="a9822-132">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="a9822-133">Pessoas selecionadas</span><span class="sxs-lookup"><span data-stu-id="a9822-133">Selected people</span></span>

<span data-ttu-id="a9822-134">A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="a9822-134">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

<span data-ttu-id="a9822-136">Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="a9822-136">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="a9822-137">Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a9822-137">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="a9822-138">Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.</span><span class="sxs-lookup"><span data-stu-id="a9822-138">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="a9822-139">**Observação:** Se nenhum usuário for localizado para um `id`, nenhum dado será renderizado para isso `id`.</span><span class="sxs-lookup"><span data-stu-id="a9822-139">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="a9822-140">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="a9822-140">CSS custom properties</span></span>

<span data-ttu-id="a9822-141">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="a9822-141">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="a9822-142">Modelos</span><span class="sxs-lookup"><span data-stu-id="a9822-142">Templates</span></span>

 <span data-ttu-id="a9822-143">`mgt-people-picker`o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="a9822-143">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="a9822-144">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="a9822-144">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="a9822-145">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="a9822-145">Data type</span></span> | <span data-ttu-id="a9822-146">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="a9822-146">Data context</span></span> | <span data-ttu-id="a9822-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9822-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a9822-148">carregando</span><span class="sxs-lookup"><span data-stu-id="a9822-148">loading</span></span> | <span data-ttu-id="a9822-149">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="a9822-149">null: no data</span></span> | <span data-ttu-id="a9822-150">O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="a9822-150">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="a9822-151">erro</span><span class="sxs-lookup"><span data-stu-id="a9822-151">error</span></span> | <span data-ttu-id="a9822-152">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="a9822-152">null: no data</span></span>| <span data-ttu-id="a9822-153">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="a9822-153">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="a9822-154">selecionado-pessoa</span><span class="sxs-lookup"><span data-stu-id="a9822-154">selected-person</span></span> |<span data-ttu-id="a9822-155">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9822-155">person: The person details object</span></span>| <span data-ttu-id="a9822-156">O modelo para renderizar as pessoas selecionadas.</span><span class="sxs-lookup"><span data-stu-id="a9822-156">The template to render selected people.</span></span> |
| <span data-ttu-id="a9822-157">vendedor</span><span class="sxs-lookup"><span data-stu-id="a9822-157">person</span></span> | <span data-ttu-id="a9822-158">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9822-158">person: The person details object</span></span>| <span data-ttu-id="a9822-159">O modelo para renderizar pessoas na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="a9822-159">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="a9822-160">Os exemplos a seguir mostram como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="a9822-160">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="a9822-161">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a9822-161">Microsoft Graph permissions</span></span>

<span data-ttu-id="a9822-162">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a9822-162">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="a9822-163">API</span><span class="sxs-lookup"><span data-stu-id="a9822-163">API</span></span>                                                                                                              | <span data-ttu-id="a9822-164">Permissão</span><span class="sxs-lookup"><span data-stu-id="a9822-164">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="a9822-165">/me/people</span><span class="sxs-lookup"><span data-stu-id="a9822-165">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="a9822-166">People.Read</span><span class="sxs-lookup"><span data-stu-id="a9822-166">People.Read</span></span>        |
| [<span data-ttu-id="a9822-167">/groups/\${GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="a9822-167">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="a9822-168">People.Read</span><span class="sxs-lookup"><span data-stu-id="a9822-168">People.Read</span></span>        |
| [<span data-ttu-id="a9822-169">/Users/$ {userprincípioname}</span><span class="sxs-lookup"><span data-stu-id="a9822-169">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="a9822-170">User. Readbasic. All</span><span class="sxs-lookup"><span data-stu-id="a9822-170">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="a9822-171">Autenticação</span><span class="sxs-lookup"><span data-stu-id="a9822-171">Authentication</span></span>

<span data-ttu-id="a9822-172">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="a9822-172">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
