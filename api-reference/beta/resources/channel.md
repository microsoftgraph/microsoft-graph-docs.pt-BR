---
title: Tipo de recurso de usuário
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f78d6e8730e5f8168cbff94fa03dfbf5287dc5ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012986"
---
# <a name="channel-resource-type"></a><span data-ttu-id="4a2eb-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="4a2eb-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a2eb-104">[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="4a2eb-105">Cada canal é dedicado a um tópico específico, departamento ou projeto.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="4a2eb-106">Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocontecem, onde os arquivos são compartilhados e as guias são adicionadas.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="4a2eb-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4a2eb-107">Methods</span></span>

| <span data-ttu-id="4a2eb-108">Método</span><span class="sxs-lookup"><span data-stu-id="4a2eb-108">Method</span></span>       | <span data-ttu-id="4a2eb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4a2eb-109">Return Type</span></span>  |<span data-ttu-id="4a2eb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a2eb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a2eb-111">List channels</span><span class="sxs-lookup"><span data-stu-id="4a2eb-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="4a2eb-112">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="4a2eb-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="4a2eb-113">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="4a2eb-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="4a2eb-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="4a2eb-115">channel</span><span class="sxs-lookup"><span data-stu-id="4a2eb-115">channel</span></span>](channel.md) | <span data-ttu-id="4a2eb-116">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="4a2eb-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="4a2eb-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="4a2eb-118">channel</span><span class="sxs-lookup"><span data-stu-id="4a2eb-118">channel</span></span>](channel.md) | <span data-ttu-id="4a2eb-119">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="4a2eb-120">Update channel</span><span class="sxs-lookup"><span data-stu-id="4a2eb-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="4a2eb-121">channel</span><span class="sxs-lookup"><span data-stu-id="4a2eb-121">channel</span></span>](channel.md) | <span data-ttu-id="4a2eb-122">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="4a2eb-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="4a2eb-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="4a2eb-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a2eb-124">None</span></span> | <span data-ttu-id="4a2eb-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-125">Delete a channel.</span></span>|
|[<span data-ttu-id="4a2eb-126">List channel messages</span><span class="sxs-lookup"><span data-stu-id="4a2eb-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="4a2eb-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4a2eb-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4a2eb-128">Obtenha mensagens em um canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="4a2eb-129">Criar uma chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="4a2eb-129">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="4a2eb-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4a2eb-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4a2eb-131">Envie uma mensagem para um canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-131">Send a message to a channel</span></span> |
|[<span data-ttu-id="4a2eb-132">Criar uma resposta chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="4a2eb-132">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="4a2eb-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4a2eb-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4a2eb-134">Responda a uma mensagem em um canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-134">Reply to a message in a channel</span></span>|
|[<span data-ttu-id="4a2eb-135">Listar guias</span><span class="sxs-lookup"><span data-stu-id="4a2eb-135">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="4a2eb-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4a2eb-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4a2eb-137">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-137">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="4a2eb-138">Obter guia</span><span class="sxs-lookup"><span data-stu-id="4a2eb-138">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="4a2eb-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4a2eb-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4a2eb-140">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-140">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="4a2eb-141">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="4a2eb-141">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="4a2eb-142">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4a2eb-142">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4a2eb-143">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-143">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="4a2eb-144">Remover guia</span><span class="sxs-lookup"><span data-stu-id="4a2eb-144">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="4a2eb-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a2eb-145">None</span></span> | <span data-ttu-id="4a2eb-146">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-146">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="4a2eb-147">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="4a2eb-147">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="4a2eb-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4a2eb-148">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4a2eb-149">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-149">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="4a2eb-150">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a2eb-150">Properties</span></span>
| <span data-ttu-id="4a2eb-151">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a2eb-151">Property</span></span>     | <span data-ttu-id="4a2eb-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a2eb-152">Type</span></span>   |<span data-ttu-id="4a2eb-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a2eb-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a2eb-154">description</span><span class="sxs-lookup"><span data-stu-id="4a2eb-154">description</span></span>|<span data-ttu-id="4a2eb-155">String</span><span class="sxs-lookup"><span data-stu-id="4a2eb-155">String</span></span>|<span data-ttu-id="4a2eb-156">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-156">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="4a2eb-157">displayName</span><span class="sxs-lookup"><span data-stu-id="4a2eb-157">displayName</span></span>|<span data-ttu-id="4a2eb-158">String</span><span class="sxs-lookup"><span data-stu-id="4a2eb-158">String</span></span>|<span data-ttu-id="4a2eb-159">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-159">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="4a2eb-160">id</span><span class="sxs-lookup"><span data-stu-id="4a2eb-160">id</span></span>|<span data-ttu-id="4a2eb-161">String</span><span class="sxs-lookup"><span data-stu-id="4a2eb-161">String</span></span>|<span data-ttu-id="4a2eb-162">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-162">The channels's unique identifier.</span></span> <span data-ttu-id="4a2eb-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-163">Read-only.</span></span>|
|<span data-ttu-id="4a2eb-164">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="4a2eb-164">isFavoriteByDefault</span></span>|<span data-ttu-id="4a2eb-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a2eb-165">Boolean</span></span>|<span data-ttu-id="4a2eb-166">Se o canal deve automaticamente ser marcado como “favorito” para todos os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-166">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="4a2eb-167">Padrão: `false`.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-167">Default: `false`.</span></span>|
|<span data-ttu-id="4a2eb-168">email</span><span class="sxs-lookup"><span data-stu-id="4a2eb-168">email</span></span>|<span data-ttu-id="4a2eb-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a2eb-169">String</span></span>| <span data-ttu-id="4a2eb-170">O endereço de email para enviar mensagens ao canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-170">The email address for sending messages to the channel.</span></span> <span data-ttu-id="4a2eb-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-171">Read-only.</span></span>|
|<span data-ttu-id="4a2eb-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="4a2eb-172">webUrl</span></span>|<span data-ttu-id="4a2eb-173">String</span><span class="sxs-lookup"><span data-stu-id="4a2eb-173">String</span></span>|<span data-ttu-id="4a2eb-174">Um hiperlink que navegará até o canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-174">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="4a2eb-175">Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-175">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="4a2eb-176">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-176">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="4a2eb-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-177">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4a2eb-178">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="4a2eb-178">Relationships</span></span>
| <span data-ttu-id="4a2eb-179">Relação</span><span class="sxs-lookup"><span data-stu-id="4a2eb-179">Relationship</span></span> | <span data-ttu-id="4a2eb-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a2eb-180">Type</span></span>   |<span data-ttu-id="4a2eb-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a2eb-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a2eb-182">messages</span><span class="sxs-lookup"><span data-stu-id="4a2eb-182">messages</span></span>|<span data-ttu-id="4a2eb-183">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="4a2eb-183">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="4a2eb-184">Uma coleção de todas as mensagens do canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-184">A collection of all the messages in the channel.</span></span> <span data-ttu-id="4a2eb-185">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-185">A navigation property.</span></span> <span data-ttu-id="4a2eb-186">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-186">Nullable.</span></span> <span data-ttu-id="4a2eb-187">No momento, esse API tem suporte apenas à leitura, mas eventualmente terá suporte a mensagens escritas também.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-187">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="4a2eb-188">guias</span><span class="sxs-lookup"><span data-stu-id="4a2eb-188">tabs</span></span>|<span data-ttu-id="4a2eb-189">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="4a2eb-189">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="4a2eb-190">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-190">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="4a2eb-191">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="4a2eb-191">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4a2eb-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a2eb-192">JSON representation</span></span>

<span data-ttu-id="4a2eb-193">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4a2eb-193">Here is a JSON representation of the resource</span></span>

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
