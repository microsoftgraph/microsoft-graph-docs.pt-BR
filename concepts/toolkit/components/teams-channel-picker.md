---
title: Microsoft Teams Componente selador de canal no Microsoft Graph Toolkit
description: Você pode usar o mgt-teams-channel-picker para pesquisar canais e equipes associadas ao usuário no microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: cd27db315de6b46c10c18e300ddb899ea042e428
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334728"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="99904-103">Microsoft Teams Componente selador de canal no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="99904-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="99904-104">Você pode usar o `mgt-teams-channel-picker` componente para habilitar pesquisas Microsoft Teams canais associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="99904-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="99904-105">O componente pode pesquisar todas as equipes que o usuário ingressou e cada canal nessas equipes.</span><span class="sxs-lookup"><span data-stu-id="99904-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="99904-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99904-106">Example</span></span>

<span data-ttu-id="99904-107">O exemplo a seguir mostra o `mgt-teams-channel-picker` componente.</span><span class="sxs-lookup"><span data-stu-id="99904-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="99904-108">Comece a procurar um canal ou equipe para ver os resultados renderizar.</span><span class="sxs-lookup"><span data-stu-id="99904-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="99904-109">Abrir este exemplo no mgt.dev</span><span class="sxs-lookup"><span data-stu-id="99904-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="99904-110">Obter o canal selecionado</span><span class="sxs-lookup"><span data-stu-id="99904-110">Getting the selected channel</span></span>

<span data-ttu-id="99904-111">Use a propriedade para recuperar o canal selecionado no momento `selectedItem` e a equipe pai.</span><span class="sxs-lookup"><span data-stu-id="99904-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="99904-112">Esse valor será nulo se nenhum canal tiver sido selecionado.</span><span class="sxs-lookup"><span data-stu-id="99904-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="99904-113">`selectedItem` contém duas propriedades: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) e `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span><span class="sxs-lookup"><span data-stu-id="99904-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="99904-114">Selecionar um canal</span><span class="sxs-lookup"><span data-stu-id="99904-114">Selecting a channel</span></span>

<span data-ttu-id="99904-115">Use o `selectChannelById(channelId: string)` método para selecionar programaticamente um canal.</span><span class="sxs-lookup"><span data-stu-id="99904-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="99904-116">**Observação:** o Teams seletor de canal só dá suporte à seleção de canal único.</span><span class="sxs-lookup"><span data-stu-id="99904-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="99904-117">**Observação:** O canal fornecido (e a ID subsequente) deve pertencer a uma equipe que o usuário autenticado ingressou.</span><span class="sxs-lookup"><span data-stu-id="99904-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="99904-118">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="99904-118">CSS custom properties</span></span>

<span data-ttu-id="99904-119">O `mgt-teams-channel-picker` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="99904-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="events"></a><span data-ttu-id="99904-120">Eventos</span><span class="sxs-lookup"><span data-stu-id="99904-120">Events</span></span>

<span data-ttu-id="99904-121">Evento</span><span class="sxs-lookup"><span data-stu-id="99904-121">Event</span></span> | <span data-ttu-id="99904-122">Quando é emitido</span><span class="sxs-lookup"><span data-stu-id="99904-122">When is it emitted</span></span> | <span data-ttu-id="99904-123">Dados personalizados</span><span class="sxs-lookup"><span data-stu-id="99904-123">Custom data</span></span> | <span data-ttu-id="99904-124">Cancelável</span><span class="sxs-lookup"><span data-stu-id="99904-124">Cancelable</span></span> | <span data-ttu-id="99904-125">Bolhas</span><span class="sxs-lookup"><span data-stu-id="99904-125">Bubbles</span></span> | <span data-ttu-id="99904-126">Funciona com modelo personalizado</span><span class="sxs-lookup"><span data-stu-id="99904-126">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`selectionChanged` | <span data-ttu-id="99904-127">Disparado quando o usuário faz uma alteração na seleção de um canal</span><span class="sxs-lookup"><span data-stu-id="99904-127">Fired when user makes a change in selection of a channel</span></span> | <span data-ttu-id="99904-128">O item selecionado no momento como equipe `{ channel: ` [de](/graph/api/resources/channel) `, team: ` [canal](/graph/api/resources/team)`}`</span><span class="sxs-lookup"><span data-stu-id="99904-128">The currently selected item as `{ channel: `[channel](/graph/api/resources/channel)`, team: `[team](/graph/api/resources/team)`}`</span></span> | <span data-ttu-id="99904-129">Não</span><span class="sxs-lookup"><span data-stu-id="99904-129">No</span></span> | <span data-ttu-id="99904-130">Não</span><span class="sxs-lookup"><span data-stu-id="99904-130">No</span></span> | <span data-ttu-id="99904-131">Sim</span><span class="sxs-lookup"><span data-stu-id="99904-131">Yes</span></span>

<span data-ttu-id="99904-132">Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).</span><span class="sxs-lookup"><span data-stu-id="99904-132">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="99904-133">Modelos</span><span class="sxs-lookup"><span data-stu-id="99904-133">Templates</span></span>

<span data-ttu-id="99904-134">`mgt-teams-channel-picker` oferece suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="99904-134">`mgt-teams-channel-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="99904-135">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.</span><span class="sxs-lookup"><span data-stu-id="99904-135">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="99904-136">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="99904-136">Data type</span></span> | <span data-ttu-id="99904-137">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="99904-137">Data context</span></span> | <span data-ttu-id="99904-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="99904-138">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="99904-139">loading</span><span class="sxs-lookup"><span data-stu-id="99904-139">loading</span></span> | <span data-ttu-id="99904-140">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="99904-140">null: no data</span></span> | <span data-ttu-id="99904-141">O modelo usado para renderizar o estado do selador enquanto a solicitação à Microsoft Graph está sendo feita.</span><span class="sxs-lookup"><span data-stu-id="99904-141">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="99904-142">erro</span><span class="sxs-lookup"><span data-stu-id="99904-142">error</span></span> | <span data-ttu-id="99904-143">null: sem dados</span><span class="sxs-lookup"><span data-stu-id="99904-143">null: no data</span></span>| <span data-ttu-id="99904-144">O modelo usado se a pesquisa do usuário não retornar usuários.</span><span class="sxs-lookup"><span data-stu-id="99904-144">The template used if user search returns no users.</span></span> |

<span data-ttu-id="99904-145">O exemplo a seguir mostra como usar o `error` modelo.</span><span class="sxs-lookup"><span data-stu-id="99904-145">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="99904-146">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="99904-146">Microsoft Graph permissions</span></span>

<span data-ttu-id="99904-147">Este componente usa as seguintes APIs Graph Microsoft e permissões por padrão.</span><span class="sxs-lookup"><span data-stu-id="99904-147">This component uses the following Microsoft Graph APIs and permissions by default.</span></span>

| <span data-ttu-id="99904-148">API</span><span class="sxs-lookup"><span data-stu-id="99904-148">API</span></span>                                                                                                              | <span data-ttu-id="99904-149">Permissão</span><span class="sxs-lookup"><span data-stu-id="99904-149">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="99904-150">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="99904-150">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="99904-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="99904-151">User.Read.All</span></span>        |
| [<span data-ttu-id="99904-152">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="99904-152">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="99904-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="99904-153">Group.Read.All</span></span>        |

<span data-ttu-id="99904-154">Na versão 2.2, as permissões necessárias foram atualizadas para as permissões menos restritivas Teams baseadas em dados.</span><span class="sxs-lookup"><span data-stu-id="99904-154">In version 2.2, the required permissions have been updated to the less restrictive Teams-based permissions.</span></span> <span data-ttu-id="99904-155">Para evitar uma alteração de quebra, você precisa optar pelas novas permissões por meio de uma configuração global.</span><span class="sxs-lookup"><span data-stu-id="99904-155">To avoid a breaking change, you need to opt in to the new permissions via a global config.</span></span>

```ts
import {MgtTeamsChannelPicker} from "@microsoft/mgt-components";

MgtTeamsChannelPicker.config.useTeamsBasedScopes = true;
```

<span data-ttu-id="99904-156">Com `useTeamsBasedScopes` definido como , o Teams Selador de Canal usará os seguintes `true` escopos.</span><span class="sxs-lookup"><span data-stu-id="99904-156">With `useTeamsBasedScopes` set to `true`, the Teams Channel Picker will use the following scopes.</span></span> 

| <span data-ttu-id="99904-157">API</span><span class="sxs-lookup"><span data-stu-id="99904-157">API</span></span>                                                                                                              | <span data-ttu-id="99904-158">Permissão</span><span class="sxs-lookup"><span data-stu-id="99904-158">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="99904-159">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="99904-159">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="99904-160">Team.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="99904-160">Team.ReadBasic.All</span></span>        |
| [<span data-ttu-id="99904-161">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="99904-161">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="99904-162">Channel.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="99904-162">Channel.ReadBasic.All</span></span>        |

<span data-ttu-id="99904-163">Essas serão as permissões padrão na próxima grande atualização.</span><span class="sxs-lookup"><span data-stu-id="99904-163">These will be the default permissions in the next major update.</span></span>

## <a name="authentication"></a><span data-ttu-id="99904-164">Autenticação</span><span class="sxs-lookup"><span data-stu-id="99904-164">Authentication</span></span>

<span data-ttu-id="99904-165">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="99904-165">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="99904-166">Cache</span><span class="sxs-lookup"><span data-stu-id="99904-166">Cache</span></span>

<span data-ttu-id="99904-167">O `mgt-teams-channel-picker` componente não armazena dados em cache.</span><span class="sxs-lookup"><span data-stu-id="99904-167">The `mgt-teams-channel-picker` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="99904-168">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="99904-168">Extend for more control</span></span>

<span data-ttu-id="99904-169">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes:</span><span class="sxs-lookup"><span data-stu-id="99904-169">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="99904-170">Método</span><span class="sxs-lookup"><span data-stu-id="99904-170">Method</span></span> | <span data-ttu-id="99904-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="99904-171">Description</span></span> |
| - | - |
| <span data-ttu-id="99904-172">renderSelected</span><span class="sxs-lookup"><span data-stu-id="99904-172">renderSelected</span></span> | <span data-ttu-id="99904-173">Renderiza a equipe e o canal selecionados na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="99904-173">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="99904-174">renderInput</span><span class="sxs-lookup"><span data-stu-id="99904-174">renderInput</span></span> | <span data-ttu-id="99904-175">Renderiza a caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="99904-175">Renders the input box.</span></span> |
| <span data-ttu-id="99904-176">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="99904-176">renderDropdown</span></span> | <span data-ttu-id="99904-177">Renderiza o menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="99904-177">Renders the dropdown.</span></span> |
| <span data-ttu-id="99904-178">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="99904-178">renderDropdownList</span></span> | <span data-ttu-id="99904-179">Renderiza os itens no menu suspenso recursivamente.</span><span class="sxs-lookup"><span data-stu-id="99904-179">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="99904-180">renderItem</span><span class="sxs-lookup"><span data-stu-id="99904-180">renderItem</span></span> | <span data-ttu-id="99904-181">Renderiza uma equipe ou um canal na lista de menus suspensos.</span><span class="sxs-lookup"><span data-stu-id="99904-181">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="99904-182">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="99904-182">renderHighlightedText</span></span> | <span data-ttu-id="99904-183">Renderiza o texto do canal, realçando a consulta de entrada.</span><span class="sxs-lookup"><span data-stu-id="99904-183">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="99904-184">renderLoading</span><span class="sxs-lookup"><span data-stu-id="99904-184">renderLoading</span></span> | <span data-ttu-id="99904-185">Renderiza o estado suspenso de carregamento.</span><span class="sxs-lookup"><span data-stu-id="99904-185">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="99904-186">renderError</span><span class="sxs-lookup"><span data-stu-id="99904-186">renderError</span></span> | <span data-ttu-id="99904-187">Renderiza o estado de erro suspenso.</span><span class="sxs-lookup"><span data-stu-id="99904-187">Renders the dropdown error state.</span></span> |
