---
title: Tipo de recurso de usuário
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1b77afb1560ed451683838a617123db013b71cd6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338756"
---
# <a name="channel-resource-type"></a><span data-ttu-id="e35a1-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="e35a1-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e35a1-104">[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas.</span><span class="sxs-lookup"><span data-stu-id="e35a1-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="e35a1-105">Cada canal é dedicado a um tópico específico, departamento ou projeto.</span><span class="sxs-lookup"><span data-stu-id="e35a1-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="e35a1-106">Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocotecem, onde os arquivos são compartilhados e as guias são adicionadas.</span><span class="sxs-lookup"><span data-stu-id="e35a1-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="e35a1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e35a1-107">Methods</span></span>

| <span data-ttu-id="e35a1-108">Método</span><span class="sxs-lookup"><span data-stu-id="e35a1-108">Method</span></span>       | <span data-ttu-id="e35a1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e35a1-109">Return Type</span></span>  |<span data-ttu-id="e35a1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e35a1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e35a1-111">List channels</span><span class="sxs-lookup"><span data-stu-id="e35a1-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="e35a1-112">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="e35a1-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="e35a1-113">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="e35a1-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="e35a1-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="e35a1-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="e35a1-115">channel</span><span class="sxs-lookup"><span data-stu-id="e35a1-115">channel</span></span>](channel.md) | <span data-ttu-id="e35a1-116">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="e35a1-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="e35a1-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="e35a1-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="e35a1-118">channel</span><span class="sxs-lookup"><span data-stu-id="e35a1-118">channel</span></span>](channel.md) | <span data-ttu-id="e35a1-119">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="e35a1-120">Update channel</span><span class="sxs-lookup"><span data-stu-id="e35a1-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="e35a1-121">channel</span><span class="sxs-lookup"><span data-stu-id="e35a1-121">channel</span></span>](channel.md) | <span data-ttu-id="e35a1-122">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="e35a1-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="e35a1-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="e35a1-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e35a1-124">None</span></span> | <span data-ttu-id="e35a1-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-125">Delete a channel.</span></span>|
|[<span data-ttu-id="e35a1-126">List channel messages</span><span class="sxs-lookup"><span data-stu-id="e35a1-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="e35a1-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e35a1-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="e35a1-128">Obtenha mensagens em um canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="e35a1-129">Enviar a mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="e35a1-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="e35a1-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e35a1-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="e35a1-131">Enviar uma mensagem para um canal</span><span class="sxs-lookup"><span data-stu-id="e35a1-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |
|[<span data-ttu-id="e35a1-132">Listar guias</span><span class="sxs-lookup"><span data-stu-id="e35a1-132">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="e35a1-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e35a1-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e35a1-134">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-134">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="e35a1-135">Obter guia</span><span class="sxs-lookup"><span data-stu-id="e35a1-135">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="e35a1-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e35a1-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e35a1-137">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-137">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="e35a1-138">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="e35a1-138">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="e35a1-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e35a1-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e35a1-140">Adiciona (fixa) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-140">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="e35a1-141">Remover guia</span><span class="sxs-lookup"><span data-stu-id="e35a1-141">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="e35a1-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e35a1-142">None</span></span> | <span data-ttu-id="e35a1-143">Remove (desafixa) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-143">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="e35a1-144">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="e35a1-144">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="e35a1-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e35a1-145">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e35a1-146">Atualiza as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="e35a1-146">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="e35a1-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e35a1-147">Properties</span></span>
| <span data-ttu-id="e35a1-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e35a1-148">Property</span></span>     | <span data-ttu-id="e35a1-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="e35a1-149">Type</span></span>   |<span data-ttu-id="e35a1-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="e35a1-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e35a1-151">description</span><span class="sxs-lookup"><span data-stu-id="e35a1-151">description</span></span>|<span data-ttu-id="e35a1-152">String</span><span class="sxs-lookup"><span data-stu-id="e35a1-152">String</span></span>|<span data-ttu-id="e35a1-153">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-153">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="e35a1-154">displayName</span><span class="sxs-lookup"><span data-stu-id="e35a1-154">displayName</span></span>|<span data-ttu-id="e35a1-155">String</span><span class="sxs-lookup"><span data-stu-id="e35a1-155">String</span></span>|<span data-ttu-id="e35a1-156">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e35a1-156">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="e35a1-157">id</span><span class="sxs-lookup"><span data-stu-id="e35a1-157">id</span></span>|<span data-ttu-id="e35a1-158">String</span><span class="sxs-lookup"><span data-stu-id="e35a1-158">String</span></span>|<span data-ttu-id="e35a1-159">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-159">The channels's unique identifier.</span></span> <span data-ttu-id="e35a1-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e35a1-160">Read-only.</span></span>|
|<span data-ttu-id="e35a1-161">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="e35a1-161">isFavoriteByDefault</span></span>|<span data-ttu-id="e35a1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e35a1-162">Boolean</span></span>|<span data-ttu-id="e35a1-163">Se o canal deve automaticamente ser marcado como “favorito” para todos os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="e35a1-163">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="e35a1-164">Padrão: `false`.</span><span class="sxs-lookup"><span data-stu-id="e35a1-164">Default: `false`.</span></span>|
|<span data-ttu-id="e35a1-165">email</span><span class="sxs-lookup"><span data-stu-id="e35a1-165">email</span></span>|<span data-ttu-id="e35a1-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e35a1-166">String</span></span>| <span data-ttu-id="e35a1-167">O endereço de email para enviar mensagens ao canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-167">The email address for sending messages to the channel.</span></span> <span data-ttu-id="e35a1-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e35a1-168">Read-only.</span></span>|
|<span data-ttu-id="e35a1-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="e35a1-169">webUrl</span></span>|<span data-ttu-id="e35a1-170">String</span><span class="sxs-lookup"><span data-stu-id="e35a1-170">String</span></span>|<span data-ttu-id="e35a1-171">Um hiperlink que navegará até o canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e35a1-171">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="e35a1-172">Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-172">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="e35a1-173">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="e35a1-173">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="e35a1-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e35a1-174">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e35a1-175">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="e35a1-175">Relationships</span></span>
| <span data-ttu-id="e35a1-176">Relação</span><span class="sxs-lookup"><span data-stu-id="e35a1-176">Relationship</span></span> | <span data-ttu-id="e35a1-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="e35a1-177">Type</span></span>   |<span data-ttu-id="e35a1-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="e35a1-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e35a1-179">messages</span><span class="sxs-lookup"><span data-stu-id="e35a1-179">messages</span></span>|<span data-ttu-id="e35a1-180">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="e35a1-180">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="e35a1-181">Uma coleção de todas as mensagens do canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-181">A collection of all the messages in the channel.</span></span> <span data-ttu-id="e35a1-182">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="e35a1-182">A navigation property.</span></span> <span data-ttu-id="e35a1-183">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e35a1-183">Nullable.</span></span> <span data-ttu-id="e35a1-184">No momento, esse API tem suporte apenas à leitura, mas eventualmente terá suporte a mensagens escritas também.</span><span class="sxs-lookup"><span data-stu-id="e35a1-184">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="e35a1-185">guias</span><span class="sxs-lookup"><span data-stu-id="e35a1-185">tabs</span></span>|<span data-ttu-id="e35a1-186">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="e35a1-186">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="e35a1-187">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="e35a1-187">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="e35a1-188">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="e35a1-188">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e35a1-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e35a1-189">JSON representation</span></span>

<span data-ttu-id="e35a1-190">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e35a1-190">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
