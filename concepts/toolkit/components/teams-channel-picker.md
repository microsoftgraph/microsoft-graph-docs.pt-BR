---
title: Componente do Seletor de Canal do Microsoft Teams no microsoft graph Toolkit
description: Você pode usar o mgt-teams-channel-picker para pesquisar canais e equipes associadas ao usuário no Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 086ce7085f1802e40195fca9f54f2af460291fda
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266791"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1f3c8-103">Componente do Seletor de Canal do Microsoft Teams no microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1f3c8-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1f3c8-104">Você pode usar o `mgt-teams-channel-picker` componente para habilitar pesquisas para canais do Microsoft Teams associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="1f3c8-105">O componente pode pesquisar todas as equipes que o usuário ingressou e cada canal nessas equipes.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="1f3c8-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f3c8-106">Example</span></span>

<span data-ttu-id="1f3c8-107">O exemplo a seguir mostra o `mgt-teams-channel-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="1f3c8-108">Comece a procurar um canal ou equipe para ver os resultados renderizar.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="1f3c8-109">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="1f3c8-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="1f3c8-110">Obter o canal selecionado</span><span class="sxs-lookup"><span data-stu-id="1f3c8-110">Getting the selected channel</span></span>

<span data-ttu-id="1f3c8-111">Use a propriedade para recuperar o canal selecionado no momento `selectedItem` e a equipe pai.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="1f3c8-112">Esse valor será nulo se nenhum canal tiver sido selecionado.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="1f3c8-113">`selectedItem` contém duas propriedades: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) e `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span><span class="sxs-lookup"><span data-stu-id="1f3c8-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="1f3c8-114">Selecionar um canal</span><span class="sxs-lookup"><span data-stu-id="1f3c8-114">Selecting a channel</span></span>

<span data-ttu-id="1f3c8-115">Use o `selectChannelById(channelId: string)` método para selecionar programaticamente um canal.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="1f3c8-116">**Observação: o** seletor de canal do Teams só dá suporte à seleção de canal único.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="1f3c8-117">**Observação:** O canal fornecido (e a ID subsequente) deve pertencer a uma equipe que o usuário autenticado ingressou.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="1f3c8-118">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="1f3c8-118">CSS custom properties</span></span>

<span data-ttu-id="1f3c8-119">O `mgt-teams-channel-picker` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-teams-channel-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* channel background color */
    --dropdown-item-hover-background: #333d47; /* channel or team hover background */
    --dropdown-item-selected-background: #0F78D4; /* selected channel background color */

    --color: white; /* input area border focus color */
    --arrow-fill: #ffffff;
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* place holder text focus color */
}
```

## <a name="events"></a><span data-ttu-id="1f3c8-120">Eventos</span><span class="sxs-lookup"><span data-stu-id="1f3c8-120">Events</span></span>
| <span data-ttu-id="1f3c8-121">Evento</span><span class="sxs-lookup"><span data-stu-id="1f3c8-121">Event</span></span> | <span data-ttu-id="1f3c8-122">Detalhe</span><span class="sxs-lookup"><span data-stu-id="1f3c8-122">Detail</span></span> | <span data-ttu-id="1f3c8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f3c8-123">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1f3c8-124">selectionChanged</span><span class="sxs-lookup"><span data-stu-id="1f3c8-124">selectionChanged</span></span> | <span data-ttu-id="1f3c8-125">O detalhe contém o item selecionado no momento do `{channel : ` [MicrosoftGraph.Channel](/graph/api/resources/channel) `, team: ` [MicrosoftGraph.Team](/graph/api/resources/team)`}`</span><span class="sxs-lookup"><span data-stu-id="1f3c8-125">The detail contains the currently selected item  of `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team)`}`</span></span> | <span data-ttu-id="1f3c8-126">Acionado quando o usuário faz uma alteração na seleção de um canal.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-126">Fired when user makes a change in selection of a channel.</span></span> |

## <a name="templates"></a><span data-ttu-id="1f3c8-127">Modelos</span><span class="sxs-lookup"><span data-stu-id="1f3c8-127">Templates</span></span>

 <span data-ttu-id="1f3c8-128">`mgt-teams-channel-picker` oferece suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-128">`mgt-teams-channel-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="1f3c8-129">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="1f3c8-130">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="1f3c8-130">Data type</span></span> | <span data-ttu-id="1f3c8-131">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="1f3c8-131">Data context</span></span> | <span data-ttu-id="1f3c8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f3c8-132">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1f3c8-133">loading</span><span class="sxs-lookup"><span data-stu-id="1f3c8-133">loading</span></span> | <span data-ttu-id="1f3c8-134">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="1f3c8-134">null: no data</span></span> | <span data-ttu-id="1f3c8-135">O modelo usado para renderizar o estado do selador enquanto a solicitação ao Microsoft Graph está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-135">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="1f3c8-136">erro</span><span class="sxs-lookup"><span data-stu-id="1f3c8-136">error</span></span> | <span data-ttu-id="1f3c8-137">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="1f3c8-137">null: no data</span></span>| <span data-ttu-id="1f3c8-138">O modelo usado se a pesquisa do usuário não retornar usuários.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-138">The template used if user search returns no users.</span></span> |


<span data-ttu-id="1f3c8-139">O exemplo a seguir mostra como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-139">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="1f3c8-140">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1f3c8-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="1f3c8-141">Esse componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-141">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="1f3c8-142">API</span><span class="sxs-lookup"><span data-stu-id="1f3c8-142">API</span></span>                                                                                                              | <span data-ttu-id="1f3c8-143">Permissão</span><span class="sxs-lookup"><span data-stu-id="1f3c8-143">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="1f3c8-144">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="1f3c8-144">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="1f3c8-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f3c8-145">User.Read.All</span></span>        |
| [<span data-ttu-id="1f3c8-146">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="1f3c8-146">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="1f3c8-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f3c8-147">Group.Read.All</span></span>        |

## <a name="authentication"></a><span data-ttu-id="1f3c8-148">Autenticação</span><span class="sxs-lookup"><span data-stu-id="1f3c8-148">Authentication</span></span>

<span data-ttu-id="1f3c8-149">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="1f3c8-149">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="1f3c8-150">Cache</span><span class="sxs-lookup"><span data-stu-id="1f3c8-150">Cache</span></span>

<span data-ttu-id="1f3c8-151">O `mgt-teams-channel-picker` componente não armazena dados em cache.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-151">The `mgt-teams-channel-picker` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="1f3c8-152">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="1f3c8-152">Extend for more control</span></span>

<span data-ttu-id="1f3c8-153">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes:</span><span class="sxs-lookup"><span data-stu-id="1f3c8-153">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="1f3c8-154">Método</span><span class="sxs-lookup"><span data-stu-id="1f3c8-154">Method</span></span> | <span data-ttu-id="1f3c8-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f3c8-155">Description</span></span> |
| - | - |
| <span data-ttu-id="1f3c8-156">renderSelected</span><span class="sxs-lookup"><span data-stu-id="1f3c8-156">renderSelected</span></span> | <span data-ttu-id="1f3c8-157">Renderiza a equipe e o canal selecionados na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-157">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="1f3c8-158">renderInput</span><span class="sxs-lookup"><span data-stu-id="1f3c8-158">renderInput</span></span> | <span data-ttu-id="1f3c8-159">Renderiza a caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-159">Renders the input box.</span></span> |
| <span data-ttu-id="1f3c8-160">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="1f3c8-160">renderDropdown</span></span> | <span data-ttu-id="1f3c8-161">Renderiza o menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-161">Renders the dropdown.</span></span> |
| <span data-ttu-id="1f3c8-162">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="1f3c8-162">renderDropdownList</span></span> | <span data-ttu-id="1f3c8-163">Renderiza os itens no menu suspenso recursivamente.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-163">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="1f3c8-164">renderItem</span><span class="sxs-lookup"><span data-stu-id="1f3c8-164">renderItem</span></span> | <span data-ttu-id="1f3c8-165">Renderiza uma equipe ou um canal na lista de menus suspensos.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-165">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="1f3c8-166">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="1f3c8-166">renderHighlightedText</span></span> | <span data-ttu-id="1f3c8-167">Renderiza o texto do canal, realçando a consulta de entrada.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-167">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="1f3c8-168">renderLoading</span><span class="sxs-lookup"><span data-stu-id="1f3c8-168">renderLoading</span></span> | <span data-ttu-id="1f3c8-169">Renderiza o estado suspenso de carregamento.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-169">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="1f3c8-170">renderError</span><span class="sxs-lookup"><span data-stu-id="1f3c8-170">renderError</span></span> | <span data-ttu-id="1f3c8-171">Renderiza o estado de erro suspenso.</span><span class="sxs-lookup"><span data-stu-id="1f3c8-171">Renders the dropdown error state.</span></span> |
