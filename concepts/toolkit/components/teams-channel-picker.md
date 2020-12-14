---
title: Componente seletor de canal do Microsoft Teams no Microsoft Graph Toolkit
description: Você pode usar o Requery-Teams-Channel-Picker para pesquisar canais e equipes associados ao usuário do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: c0b6e818f0c9c30314b5342fcfb6ef44978ec830
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660005"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="131d1-103">Componente seletor de canal do Microsoft Teams no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="131d1-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="131d1-104">A você pode usar o `mgt-teams-channel-picker` componente para habilitar pesquisas para os canais do Microsoft Teams associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="131d1-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="131d1-105">O componente pode pesquisar todas as equipes que o usuário ingressou e cada canal dessas equipes.</span><span class="sxs-lookup"><span data-stu-id="131d1-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="131d1-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="131d1-106">Example</span></span>

<span data-ttu-id="131d1-107">O exemplo a seguir mostra o `mgt-teams-channel-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="131d1-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="131d1-108">Comece a pesquisar um canal ou uma equipe para ver os resultados renderizar.</span><span class="sxs-lookup"><span data-stu-id="131d1-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="131d1-109">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="131d1-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="131d1-110">Obtendo o canal selecionado</span><span class="sxs-lookup"><span data-stu-id="131d1-110">Getting the selected channel</span></span>

<span data-ttu-id="131d1-111">Use a `selectedItem` propriedade para recuperar o canal e a equipe pai atualmente selecionados.</span><span class="sxs-lookup"><span data-stu-id="131d1-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="131d1-112">Esse valor será NULL se nenhum canal tiver sido selecionado.</span><span class="sxs-lookup"><span data-stu-id="131d1-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="131d1-113">`selectedItem` contém duas propriedades: `channel` ([MicrosoftGraph. Channel](/graph/api/resources/channel)) e `team` ([MicrosoftGraph. Team](/graph/api/resources/team)).</span><span class="sxs-lookup"><span data-stu-id="131d1-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="131d1-114">Selecionar um canal</span><span class="sxs-lookup"><span data-stu-id="131d1-114">Selecting a channel</span></span>

<span data-ttu-id="131d1-115">Use o `selectChannelById(channelId: string)` método para selecionar um canal de forma programática.</span><span class="sxs-lookup"><span data-stu-id="131d1-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="131d1-116">**Observação:** o seletor de canal do teams suporta apenas a seleção de canal único.</span><span class="sxs-lookup"><span data-stu-id="131d1-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="131d1-117">**Observação:** O canal fornecido (e a ID subsequente) deve pertencer a uma equipe que o usuário autenticado ingressou.</span><span class="sxs-lookup"><span data-stu-id="131d1-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="131d1-118">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="131d1-118">CSS custom properties</span></span>

<span data-ttu-id="131d1-119">O `mgt-teams-channel-picker` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="131d1-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="events"></a><span data-ttu-id="131d1-120">Eventos</span><span class="sxs-lookup"><span data-stu-id="131d1-120">Events</span></span>
| <span data-ttu-id="131d1-121">Evento</span><span class="sxs-lookup"><span data-stu-id="131d1-121">Event</span></span> | <span data-ttu-id="131d1-122">Detalhe</span><span class="sxs-lookup"><span data-stu-id="131d1-122">Detail</span></span> | <span data-ttu-id="131d1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="131d1-123">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="131d1-124">selectionChanged</span><span class="sxs-lookup"><span data-stu-id="131d1-124">selectionChanged</span></span> | <span data-ttu-id="131d1-125">O detalhe contém o item atualmente selecionado de `{channel : ` [MicrosoftGraph. Channel](/graph/api/resources/channel) `, team: ` [MicrosoftGraph. Team](/graph/api/resources/team)`}`</span><span class="sxs-lookup"><span data-stu-id="131d1-125">The detail contains the currently selected item  of `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team)`}`</span></span> | <span data-ttu-id="131d1-126">Acionado quando o usuário faz uma alteração na seleção de um canal.</span><span class="sxs-lookup"><span data-stu-id="131d1-126">Fired when user makes a change in selection of a channel.</span></span> |

## <a name="templates"></a><span data-ttu-id="131d1-127">Modelos</span><span class="sxs-lookup"><span data-stu-id="131d1-127">Templates</span></span>

 <span data-ttu-id="131d1-128">`mgt-teams-channel-picker` o dá suporte a vários [modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="131d1-128">`mgt-teams-channel-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="131d1-129">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="131d1-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="131d1-130">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="131d1-130">Data type</span></span> | <span data-ttu-id="131d1-131">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="131d1-131">Data context</span></span> | <span data-ttu-id="131d1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="131d1-132">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="131d1-133">carregando</span><span class="sxs-lookup"><span data-stu-id="131d1-133">loading</span></span> | <span data-ttu-id="131d1-134">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="131d1-134">null: no data</span></span> | <span data-ttu-id="131d1-135">O modelo usado para renderizar o estado do seletor enquanto a solicitação para o Microsoft Graph está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="131d1-135">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="131d1-136">erro</span><span class="sxs-lookup"><span data-stu-id="131d1-136">error</span></span> | <span data-ttu-id="131d1-137">nulo: não há dados</span><span class="sxs-lookup"><span data-stu-id="131d1-137">null: no data</span></span>| <span data-ttu-id="131d1-138">O modelo usado se a pesquisa de usuário não retornar nenhum usuário.</span><span class="sxs-lookup"><span data-stu-id="131d1-138">The template used if user search returns no users.</span></span> |


<span data-ttu-id="131d1-139">O exemplo a seguir mostra como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="131d1-139">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="131d1-140">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="131d1-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="131d1-141">Este componente usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="131d1-141">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="131d1-142">API</span><span class="sxs-lookup"><span data-stu-id="131d1-142">API</span></span>                                                                                                              | <span data-ttu-id="131d1-143">Permissão</span><span class="sxs-lookup"><span data-stu-id="131d1-143">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="131d1-144">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="131d1-144">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="131d1-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="131d1-145">User.Read.All</span></span>        |
| [<span data-ttu-id="131d1-146">/equipes/$ {ID}/Channels</span><span class="sxs-lookup"><span data-stu-id="131d1-146">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="131d1-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="131d1-147">Group.Read.All</span></span>        |

## <a name="authentication"></a><span data-ttu-id="131d1-148">Autenticação</span><span class="sxs-lookup"><span data-stu-id="131d1-148">Authentication</span></span>

<span data-ttu-id="131d1-149">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="131d1-149">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="131d1-150">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="131d1-150">Extend for more control</span></span>

<span data-ttu-id="131d1-151">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos de substituição nas extensões de componente:</span><span class="sxs-lookup"><span data-stu-id="131d1-151">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="131d1-152">Método</span><span class="sxs-lookup"><span data-stu-id="131d1-152">Method</span></span> | <span data-ttu-id="131d1-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="131d1-153">Description</span></span> |
| - | - |
| <span data-ttu-id="131d1-154">renderSelected</span><span class="sxs-lookup"><span data-stu-id="131d1-154">renderSelected</span></span> | <span data-ttu-id="131d1-155">Renderiza a equipe e canal selecionados na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="131d1-155">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="131d1-156">renderInput</span><span class="sxs-lookup"><span data-stu-id="131d1-156">renderInput</span></span> | <span data-ttu-id="131d1-157">Renderiza a caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="131d1-157">Renders the input box.</span></span> |
| <span data-ttu-id="131d1-158">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="131d1-158">renderDropdown</span></span> | <span data-ttu-id="131d1-159">Renderiza o menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="131d1-159">Renders the dropdown.</span></span> |
| <span data-ttu-id="131d1-160">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="131d1-160">renderDropdownList</span></span> | <span data-ttu-id="131d1-161">Renderiza os itens no menu suspenso recursivamente.</span><span class="sxs-lookup"><span data-stu-id="131d1-161">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="131d1-162">renderItem</span><span class="sxs-lookup"><span data-stu-id="131d1-162">renderItem</span></span> | <span data-ttu-id="131d1-163">Renderiza uma equipe ou um canal na lista suspensa.</span><span class="sxs-lookup"><span data-stu-id="131d1-163">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="131d1-164">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="131d1-164">renderHighlightedText</span></span> | <span data-ttu-id="131d1-165">Renderiza o texto do canal, realçando a consulta de entrada.</span><span class="sxs-lookup"><span data-stu-id="131d1-165">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="131d1-166">renderLoading</span><span class="sxs-lookup"><span data-stu-id="131d1-166">renderLoading</span></span> | <span data-ttu-id="131d1-167">Renderiza o estado do menu suspenso de carregamento.</span><span class="sxs-lookup"><span data-stu-id="131d1-167">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="131d1-168">renderError</span><span class="sxs-lookup"><span data-stu-id="131d1-168">renderError</span></span> | <span data-ttu-id="131d1-169">Renderiza o estado de erro DropDown.</span><span class="sxs-lookup"><span data-stu-id="131d1-169">Renders the dropdown error state.</span></span> |
