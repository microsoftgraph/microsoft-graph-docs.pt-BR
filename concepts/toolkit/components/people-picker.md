---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: d77c6578d79edb60fbba08200dc033f032b39282
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275841"
---
# <a name="people-picker-component"></a><span data-ttu-id="0df75-103">Componente de seletor de pessoas</span><span class="sxs-lookup"><span data-stu-id="0df75-103">People-Picker component</span></span>

<span data-ttu-id="0df75-104">Você pode usar a `mgt-people-picker` pesquisa de componente da Web para um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0df75-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="0df75-105">Por padrão, o componente pesquisará todas as pessoas; Você também pode definir uma propriedade de grupo para filtrar os resultados.</span><span class="sxs-lookup"><span data-stu-id="0df75-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="0df75-106">Se o número de pessoas a serem exibidas exceder o `show-max` valor, nem todas as pessoas retornadas serão exibidas na lista de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0df75-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="0df75-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0df75-107">Example</span></span>

[<span data-ttu-id="0df75-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="0df75-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![gerenciamento de pessoas-seletor](./images/mgt-people-picker-image.png)

## <a name="properties"></a><span data-ttu-id="0df75-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0df75-110">Properties</span></span>

<span data-ttu-id="0df75-111">Por padrão, o `mgt-people-picker` componente busca eventos do `/me/people` ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="0df75-111">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="0df75-112">Use os atributos a seguir para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="0df75-112">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="0df75-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0df75-113">Property</span></span> | <span data-ttu-id="0df75-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="0df75-114">Attribute</span></span> | <span data-ttu-id="0df75-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="0df75-115">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0df75-116">showMax</span><span class="sxs-lookup"><span data-stu-id="0df75-116">showMax</span></span>  | <span data-ttu-id="0df75-117">show-Max</span><span class="sxs-lookup"><span data-stu-id="0df75-117">show-max</span></span>  | <span data-ttu-id="0df75-118">Um valor numérico para indicar o número máximo de pessoas a serem mostradas.</span><span class="sxs-lookup"><span data-stu-id="0df75-118">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="0df75-119">o valor padrão é 6.</span><span class="sxs-lookup"><span data-stu-id="0df75-119">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="0df75-120">people</span><span class="sxs-lookup"><span data-stu-id="0df75-120">people</span></span>   | <span data-ttu-id="0df75-121">people</span><span class="sxs-lookup"><span data-stu-id="0df75-121">people</span></span>    | <span data-ttu-id="0df75-122">Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="0df75-122">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="0df75-123">Use essa propriedade para acessar as pessoas carregadas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="0df75-123">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="0df75-124">Defina esse valor para carregar suas próprias pessoas.</span><span class="sxs-lookup"><span data-stu-id="0df75-124">Set this value to load your own people.</span></span> |
| <span data-ttu-id="0df75-125">group</span><span class="sxs-lookup"><span data-stu-id="0df75-125">group</span></span>    | <span data-ttu-id="0df75-126">group</span><span class="sxs-lookup"><span data-stu-id="0df75-126">group</span></span>     | <span data-ttu-id="0df75-127">Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0df75-127">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |

<span data-ttu-id="0df75-128">Apresentamos um exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="0df75-128">The following is an example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="css-custom-properties"></a><span data-ttu-id="0df75-129">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="0df75-129">CSS custom properties</span></span>

<span data-ttu-id="0df75-130">O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="0df75-130">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="0df75-131">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0df75-131">Microsoft Graph permissions</span></span>

<span data-ttu-id="0df75-132">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0df75-132">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="0df75-133">API</span><span class="sxs-lookup"><span data-stu-id="0df75-133">API</span></span>                                                                                                              | <span data-ttu-id="0df75-134">Permissão</span><span class="sxs-lookup"><span data-stu-id="0df75-134">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="0df75-135">/me/people</span><span class="sxs-lookup"><span data-stu-id="0df75-135">/me/people</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="0df75-136">People.Read</span><span class="sxs-lookup"><span data-stu-id="0df75-136">People.Read</span></span> |
| [<span data-ttu-id="0df75-137">/groups/\${GroupId}/Members</span><span class="sxs-lookup"><span data-stu-id="0df75-137">/groups/\${groupId}/members</span></span>](https://docs.microsoft.com/en-us/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="0df75-138">People.Read</span><span class="sxs-lookup"><span data-stu-id="0df75-138">People.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="0df75-139">Autenticação</span><span class="sxs-lookup"><span data-stu-id="0df75-139">Authentication</span></span>

<span data-ttu-id="0df75-140">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="0df75-140">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
