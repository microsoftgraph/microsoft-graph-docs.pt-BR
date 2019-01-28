---
title: Tipo de recurso de usuário
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 73775cb446e9cd90eaf31ade28f25638465c884e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510999"
---
# <a name="channel-resource-type"></a><span data-ttu-id="453c8-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="453c8-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="453c8-104">Um canal é uma coleção de [chatMessages](chatmessage.md) dentro de um [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="453c8-104">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="453c8-105">Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="453c8-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="453c8-106">Os exemplos podem ser o canal “Equipe de almoço da sexta-feira” e o canal “Discussão de arquitetura" .</span><span class="sxs-lookup"><span data-stu-id="453c8-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="453c8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="453c8-107">Methods</span></span>

| <span data-ttu-id="453c8-108">Método</span><span class="sxs-lookup"><span data-stu-id="453c8-108">Method</span></span>       | <span data-ttu-id="453c8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="453c8-109">Return Type</span></span>  |<span data-ttu-id="453c8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="453c8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="453c8-111">List channels</span><span class="sxs-lookup"><span data-stu-id="453c8-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="453c8-112">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="453c8-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="453c8-113">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="453c8-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="453c8-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="453c8-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="453c8-115">channel</span><span class="sxs-lookup"><span data-stu-id="453c8-115">channel</span></span>](channel.md) | <span data-ttu-id="453c8-116">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="453c8-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="453c8-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="453c8-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="453c8-118">channel</span><span class="sxs-lookup"><span data-stu-id="453c8-118">channel</span></span>](channel.md) | <span data-ttu-id="453c8-119">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="453c8-120">Update channel</span><span class="sxs-lookup"><span data-stu-id="453c8-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="453c8-121">channel</span><span class="sxs-lookup"><span data-stu-id="453c8-121">channel</span></span>](channel.md) | <span data-ttu-id="453c8-122">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="453c8-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="453c8-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="453c8-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="453c8-124">None</span></span> | <span data-ttu-id="453c8-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-125">Delete a channel.</span></span>|
|[<span data-ttu-id="453c8-126">List channel messages</span><span class="sxs-lookup"><span data-stu-id="453c8-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="453c8-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="453c8-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="453c8-128">Obtenha mensagens em um canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="453c8-129">Create chat thread</span><span class="sxs-lookup"><span data-stu-id="453c8-129">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="453c8-130">[chatThread](chatthread.md) collection</span><span class="sxs-lookup"><span data-stu-id="453c8-130">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="453c8-131">Crie um thread de conversa no canal específico.</span><span class="sxs-lookup"><span data-stu-id="453c8-131">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="453c8-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="453c8-132">Properties</span></span>
| <span data-ttu-id="453c8-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="453c8-133">Property</span></span>     | <span data-ttu-id="453c8-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="453c8-134">Type</span></span>   |<span data-ttu-id="453c8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="453c8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="453c8-136">description</span><span class="sxs-lookup"><span data-stu-id="453c8-136">description</span></span>|<span data-ttu-id="453c8-137">String</span><span class="sxs-lookup"><span data-stu-id="453c8-137">String</span></span>|<span data-ttu-id="453c8-138">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-138">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="453c8-139">displayName</span><span class="sxs-lookup"><span data-stu-id="453c8-139">displayName</span></span>|<span data-ttu-id="453c8-140">String</span><span class="sxs-lookup"><span data-stu-id="453c8-140">String</span></span>|<span data-ttu-id="453c8-141">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="453c8-141">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="453c8-142">id</span><span class="sxs-lookup"><span data-stu-id="453c8-142">id</span></span>|<span data-ttu-id="453c8-143">String</span><span class="sxs-lookup"><span data-stu-id="453c8-143">String</span></span>|<span data-ttu-id="453c8-144">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-144">The channels's unique identifier.</span></span> <span data-ttu-id="453c8-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="453c8-145">Read-only.</span></span>|
|<span data-ttu-id="453c8-146">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="453c8-146">isFavoriteByDefault</span></span>|<span data-ttu-id="453c8-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="453c8-147">Boolean</span></span>|<span data-ttu-id="453c8-148">Se o canal deve automaticamente ser marcado como “favorito” para todos os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="453c8-148">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="453c8-149">Padrão: `false`.</span><span class="sxs-lookup"><span data-stu-id="453c8-149">Default: `false`.</span></span>|
|<span data-ttu-id="453c8-150">email</span><span class="sxs-lookup"><span data-stu-id="453c8-150">email</span></span>|<span data-ttu-id="453c8-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="453c8-151">Boolean</span></span>| <span data-ttu-id="453c8-152">O endereço de email para enviar mensagens ao canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-152">The email address for sending messages to the channel.</span></span> <span data-ttu-id="453c8-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="453c8-153">Read-only.</span></span>|
|<span data-ttu-id="453c8-154">webUrl</span><span class="sxs-lookup"><span data-stu-id="453c8-154">webUrl</span></span>|<span data-ttu-id="453c8-155">String</span><span class="sxs-lookup"><span data-stu-id="453c8-155">String</span></span>|<span data-ttu-id="453c8-156">Um hiperlink que navegará até o canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="453c8-156">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="453c8-157">Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-157">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="453c8-158">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="453c8-158">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="453c8-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="453c8-159">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="453c8-160">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="453c8-160">Relationships</span></span>
| <span data-ttu-id="453c8-161">Relação</span><span class="sxs-lookup"><span data-stu-id="453c8-161">Relationship</span></span> | <span data-ttu-id="453c8-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="453c8-162">Type</span></span>   |<span data-ttu-id="453c8-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="453c8-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="453c8-164">messages</span><span class="sxs-lookup"><span data-stu-id="453c8-164">messages</span></span>|<span data-ttu-id="453c8-165">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="453c8-165">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="453c8-166">Uma coleção de todas as mensagens do canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-166">A collection of all the messages in the channel.</span></span> <span data-ttu-id="453c8-167">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="453c8-167">A navigation property.</span></span> <span data-ttu-id="453c8-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="453c8-168">Nullable.</span></span> <span data-ttu-id="453c8-169">No momento, esse API tem suporte apenas à leitura, mas eventualmente terá suporte a mensagens escritas também.</span><span class="sxs-lookup"><span data-stu-id="453c8-169">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="453c8-170">chatThreads</span><span class="sxs-lookup"><span data-stu-id="453c8-170">chatThreads</span></span>|<span data-ttu-id="453c8-171">[chatThread](chatthread.md) collection</span><span class="sxs-lookup"><span data-stu-id="453c8-171">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="453c8-172">(Está sendo extinto para favorecer a propriedade messages) chatThreads dá suporte à criação de novas mensagens, mas não à leitura de mensagens.</span><span class="sxs-lookup"><span data-stu-id="453c8-172">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="453c8-173">O ChatThreads é uma propriedade de navegação e é Anulável.</span><span class="sxs-lookup"><span data-stu-id="453c8-173">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="453c8-174">tabs</span><span class="sxs-lookup"><span data-stu-id="453c8-174">tabs</span></span>|<span data-ttu-id="453c8-175">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="453c8-175">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="453c8-176">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="453c8-176">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="453c8-177">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="453c8-177">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="453c8-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="453c8-178">JSON representation</span></span>

<span data-ttu-id="453c8-179">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="453c8-179">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
