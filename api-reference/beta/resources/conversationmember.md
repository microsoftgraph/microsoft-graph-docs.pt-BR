---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 679ab696c0f5752d8e59a2cb9de560c11bcc4ca9
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060040"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="5e1f2-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="5e1f2-103">conversationMember resource type</span></span>

<span data-ttu-id="5e1f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e1f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e1f2-105">Representa um usuário em uma [equipe ou](team.md) canal [ou](channel.md) [chat.](chat.md)</span><span class="sxs-lookup"><span data-stu-id="5e1f2-105">Represents a user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span>
<span data-ttu-id="5e1f2-106">Consulte também [aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="5e1f2-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5e1f2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e1f2-107">Methods</span></span>

| <span data-ttu-id="5e1f2-108">Método</span><span class="sxs-lookup"><span data-stu-id="5e1f2-108">Method</span></span>       | <span data-ttu-id="5e1f2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e1f2-109">Return Type</span></span>  |<span data-ttu-id="5e1f2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e1f2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e1f2-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="5e1f2-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="5e1f2-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="5e1f2-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="5e1f2-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="5e1f2-114">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="5e1f2-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="5e1f2-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="5e1f2-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="5e1f2-116">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="5e1f2-117">Adicionar membros em massa à equipe.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="5e1f2-118">coleção[actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="5e1f2-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="5e1f2-119">Adicione vários membros à equipe em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="5e1f2-120">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="5e1f2-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="5e1f2-121">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="5e1f2-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="5e1f2-122">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="5e1f2-123">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="5e1f2-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="5e1f2-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="5e1f2-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="5e1f2-125">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="5e1f2-126">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="5e1f2-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="5e1f2-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e1f2-127">None</span></span>|<span data-ttu-id="5e1f2-128">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="5e1f2-129">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="5e1f2-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="5e1f2-130">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="5e1f2-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="5e1f2-131">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="5e1f2-132">Adicionar membro do canal</span><span class="sxs-lookup"><span data-stu-id="5e1f2-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="5e1f2-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="5e1f2-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="5e1f2-134">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-134">Add a member to a channel.</span></span> <span data-ttu-id="5e1f2-135">Somente suportado para `channel` com o membershipType de `private`.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-135">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="5e1f2-136">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="5e1f2-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="5e1f2-137">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="5e1f2-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="5e1f2-138">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="5e1f2-139">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="5e1f2-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="5e1f2-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="5e1f2-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="5e1f2-141">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="5e1f2-142">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="5e1f2-143">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="5e1f2-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="5e1f2-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e1f2-144">None</span></span> | <span data-ttu-id="5e1f2-145">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-145">Delete a member from a channel.</span></span> <span data-ttu-id="5e1f2-146">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="5e1f2-147">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="5e1f2-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="5e1f2-148">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="5e1f2-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="5e1f2-149">Obter a lista de todos os membros em um chat.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="5e1f2-150">Adicionar membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="5e1f2-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="5e1f2-151">Cabeçalho de local</span><span class="sxs-lookup"><span data-stu-id="5e1f2-151">Location header</span></span> | <span data-ttu-id="5e1f2-152">Adicionar um membro a um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="5e1f2-153">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="5e1f2-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="5e1f2-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="5e1f2-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="5e1f2-155">Obtenha um membro em um chat.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="5e1f2-156">Remover membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="5e1f2-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="5e1f2-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e1f2-157">None</span></span> | <span data-ttu-id="5e1f2-158">Remover um membro de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="5e1f2-159">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e1f2-159">Properties</span></span>

| <span data-ttu-id="5e1f2-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e1f2-160">Property</span></span>   | <span data-ttu-id="5e1f2-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e1f2-161">Type</span></span> |<span data-ttu-id="5e1f2-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e1f2-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e1f2-163">id</span><span class="sxs-lookup"><span data-stu-id="5e1f2-163">id</span></span>|<span data-ttu-id="5e1f2-164">String</span><span class="sxs-lookup"><span data-stu-id="5e1f2-164">String</span></span>| <span data-ttu-id="5e1f2-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-165">Read-only.</span></span> <span data-ttu-id="5e1f2-166">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-166">Unique ID of the user.</span></span>|
|<span data-ttu-id="5e1f2-167">displayName</span><span class="sxs-lookup"><span data-stu-id="5e1f2-167">displayName</span></span>| <span data-ttu-id="5e1f2-168">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e1f2-168">string</span></span> | <span data-ttu-id="5e1f2-169">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-169">The display name of the user.</span></span> |
|<span data-ttu-id="5e1f2-170">funções</span><span class="sxs-lookup"><span data-stu-id="5e1f2-170">roles</span></span>| <span data-ttu-id="5e1f2-171">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e1f2-171">string collection</span></span> | <span data-ttu-id="5e1f2-172">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-172">The roles for that user.</span></span> |
|<span data-ttu-id="5e1f2-173">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="5e1f2-173">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="5e1f2-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e1f2-174">DateTimeOffset</span></span> | <span data-ttu-id="5e1f2-175">O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-175">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="5e1f2-176">Essa propriedade é configurável somente para os membros de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-176">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5e1f2-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e1f2-177">JSON representation</span></span>

<span data-ttu-id="5e1f2-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e1f2-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


