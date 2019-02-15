---
title: Tipo de recurso de usuário
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994465"
---
# <a name="channel-resource-type"></a><span data-ttu-id="f0958-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="f0958-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0958-104">Um canal é uma coleção de [chatMessages](chatmessage.md) dentro de um [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f0958-104">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="f0958-105">Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f0958-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="f0958-106">Os exemplos podem ser o canal “Equipe de almoço da sexta-feira” e o canal “Discussão de arquitetura" .</span><span class="sxs-lookup"><span data-stu-id="f0958-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="f0958-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f0958-107">Methods</span></span>

| <span data-ttu-id="f0958-108">Método</span><span class="sxs-lookup"><span data-stu-id="f0958-108">Method</span></span>       | <span data-ttu-id="f0958-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f0958-109">Return Type</span></span>  |<span data-ttu-id="f0958-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0958-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0958-111">List channels</span><span class="sxs-lookup"><span data-stu-id="f0958-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="f0958-112">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="f0958-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="f0958-113">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="f0958-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="f0958-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="f0958-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="f0958-115">channel</span><span class="sxs-lookup"><span data-stu-id="f0958-115">channel</span></span>](channel.md) | <span data-ttu-id="f0958-116">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="f0958-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="f0958-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="f0958-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="f0958-118">channel</span><span class="sxs-lookup"><span data-stu-id="f0958-118">channel</span></span>](channel.md) | <span data-ttu-id="f0958-119">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="f0958-120">Update channel</span><span class="sxs-lookup"><span data-stu-id="f0958-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="f0958-121">channel</span><span class="sxs-lookup"><span data-stu-id="f0958-121">channel</span></span>](channel.md) | <span data-ttu-id="f0958-122">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="f0958-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="f0958-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="f0958-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0958-124">None</span></span> | <span data-ttu-id="f0958-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-125">Delete a channel.</span></span>|
|[<span data-ttu-id="f0958-126">List channel messages</span><span class="sxs-lookup"><span data-stu-id="f0958-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="f0958-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f0958-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f0958-128">Obtenha mensagens em um canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="f0958-129">Enviar a mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="f0958-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="f0958-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f0958-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="f0958-131">Enviar uma mensagem para um canal</span><span class="sxs-lookup"><span data-stu-id="f0958-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |


## <a name="properties"></a><span data-ttu-id="f0958-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0958-132">Properties</span></span>
| <span data-ttu-id="f0958-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0958-133">Property</span></span>     | <span data-ttu-id="f0958-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0958-134">Type</span></span>   |<span data-ttu-id="f0958-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0958-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0958-136">description</span><span class="sxs-lookup"><span data-stu-id="f0958-136">description</span></span>|<span data-ttu-id="f0958-137">String</span><span class="sxs-lookup"><span data-stu-id="f0958-137">String</span></span>|<span data-ttu-id="f0958-138">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-138">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="f0958-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f0958-139">displayName</span></span>|<span data-ttu-id="f0958-140">String</span><span class="sxs-lookup"><span data-stu-id="f0958-140">String</span></span>|<span data-ttu-id="f0958-141">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f0958-141">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="f0958-142">id</span><span class="sxs-lookup"><span data-stu-id="f0958-142">id</span></span>|<span data-ttu-id="f0958-143">String</span><span class="sxs-lookup"><span data-stu-id="f0958-143">String</span></span>|<span data-ttu-id="f0958-144">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-144">The channels's unique identifier.</span></span> <span data-ttu-id="f0958-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0958-145">Read-only.</span></span>|
|<span data-ttu-id="f0958-146">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="f0958-146">isFavoriteByDefault</span></span>|<span data-ttu-id="f0958-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0958-147">Boolean</span></span>|<span data-ttu-id="f0958-148">Se o canal deve automaticamente ser marcado como “favorito” para todos os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="f0958-148">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="f0958-149">Padrão: `false`.</span><span class="sxs-lookup"><span data-stu-id="f0958-149">Default: `false`.</span></span>|
|<span data-ttu-id="f0958-150">email</span><span class="sxs-lookup"><span data-stu-id="f0958-150">email</span></span>|<span data-ttu-id="f0958-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0958-151">Boolean</span></span>| <span data-ttu-id="f0958-152">O endereço de email para enviar mensagens ao canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-152">The email address for sending messages to the channel.</span></span> <span data-ttu-id="f0958-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0958-153">Read-only.</span></span>|
|<span data-ttu-id="f0958-154">webUrl</span><span class="sxs-lookup"><span data-stu-id="f0958-154">webUrl</span></span>|<span data-ttu-id="f0958-155">String</span><span class="sxs-lookup"><span data-stu-id="f0958-155">String</span></span>|<span data-ttu-id="f0958-156">Um hiperlink que navegará até o canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f0958-156">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="f0958-157">Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-157">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="f0958-158">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="f0958-158">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="f0958-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0958-159">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f0958-160">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="f0958-160">Relationships</span></span>
| <span data-ttu-id="f0958-161">Relação</span><span class="sxs-lookup"><span data-stu-id="f0958-161">Relationship</span></span> | <span data-ttu-id="f0958-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0958-162">Type</span></span>   |<span data-ttu-id="f0958-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0958-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0958-164">messages</span><span class="sxs-lookup"><span data-stu-id="f0958-164">messages</span></span>|<span data-ttu-id="f0958-165">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="f0958-165">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="f0958-166">Uma coleção de todas as mensagens do canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-166">A collection of all the messages in the channel.</span></span> <span data-ttu-id="f0958-167">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="f0958-167">A navigation property.</span></span> <span data-ttu-id="f0958-168">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f0958-168">Nullable.</span></span> <span data-ttu-id="f0958-169">No momento, esse API tem suporte apenas à leitura, mas eventualmente terá suporte a mensagens escritas também.</span><span class="sxs-lookup"><span data-stu-id="f0958-169">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="f0958-170">guias</span><span class="sxs-lookup"><span data-stu-id="f0958-170">tabs</span></span>|<span data-ttu-id="f0958-171">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="f0958-171">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="f0958-172">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="f0958-172">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="f0958-173">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="f0958-173">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f0958-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0958-174">JSON representation</span></span>

<span data-ttu-id="f0958-175">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f0958-175">Here is a JSON representation of the resource</span></span>

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
