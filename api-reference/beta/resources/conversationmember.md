---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f6b24b65a6ae25f8a05bf067659c04d49c06d24
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706055"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="c9ecd-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="c9ecd-103">conversationMember resource type</span></span>

<span data-ttu-id="c9ecd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9ecd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9ecd-105">Representa um usuário em um [bate-papo](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="c9ecd-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="c9ecd-106">Confira também [aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="c9ecd-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c9ecd-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c9ecd-107">Methods</span></span>

| <span data-ttu-id="c9ecd-108">Método</span><span class="sxs-lookup"><span data-stu-id="c9ecd-108">Method</span></span>       | <span data-ttu-id="c9ecd-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9ecd-109">Return Type</span></span>  |<span data-ttu-id="c9ecd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9ecd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9ecd-111">Listar membros da equipe</span><span class="sxs-lookup"><span data-stu-id="c9ecd-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="c9ecd-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c9ecd-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="c9ecd-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="c9ecd-114">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="c9ecd-114">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="c9ecd-115">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="c9ecd-115">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c9ecd-116">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-116">Get a member in the team.</span></span>|
|[<span data-ttu-id="c9ecd-117">Adicionar membro da equipe</span><span class="sxs-lookup"><span data-stu-id="c9ecd-117">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="c9ecd-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c9ecd-118">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="c9ecd-119">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-119">Add a new member to the team.</span></span>|
|[<span data-ttu-id="c9ecd-120">Adicionar membros da equipe em massa</span><span class="sxs-lookup"><span data-stu-id="c9ecd-120">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="c9ecd-121">coleção[actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="c9ecd-121">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="c9ecd-122">Adicione vários membros à equipe em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-122">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="c9ecd-123">Atualizar a função do membro da equipe</span><span class="sxs-lookup"><span data-stu-id="c9ecd-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="c9ecd-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c9ecd-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="c9ecd-125">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="c9ecd-126">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="c9ecd-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="c9ecd-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9ecd-127">None</span></span>|<span data-ttu-id="c9ecd-128">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="c9ecd-129">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="c9ecd-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="c9ecd-130">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c9ecd-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c9ecd-131">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="c9ecd-132">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="c9ecd-132">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="c9ecd-133">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c9ecd-133">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c9ecd-134">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-134">Get a member in a channel.</span></span>|
|[<span data-ttu-id="c9ecd-135">Criar membro do canal</span><span class="sxs-lookup"><span data-stu-id="c9ecd-135">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="c9ecd-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c9ecd-136">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c9ecd-137">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-137">Add a member to a channel.</span></span> <span data-ttu-id="c9ecd-138">Suportado só para o`channel`com MembershipType de.`private`</span><span class="sxs-lookup"><span data-stu-id="c9ecd-138">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="c9ecd-139">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="c9ecd-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="c9ecd-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c9ecd-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c9ecd-141">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="c9ecd-142">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="c9ecd-143">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="c9ecd-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="c9ecd-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9ecd-144">None</span></span> | <span data-ttu-id="c9ecd-145">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-145">Delete a member from a channel.</span></span> <span data-ttu-id="c9ecd-146">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="c9ecd-147">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="c9ecd-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="c9ecd-148">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c9ecd-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c9ecd-149">Obter a lista de todos os membros em um chat.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="c9ecd-150">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="c9ecd-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="c9ecd-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c9ecd-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c9ecd-152">Obter um membro em um chat.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="c9ecd-153">Adicionar membro de chat</span><span class="sxs-lookup"><span data-stu-id="c9ecd-153">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="c9ecd-154">Cabeçalho location</span><span class="sxs-lookup"><span data-stu-id="c9ecd-154">Location header</span></span> | <span data-ttu-id="c9ecd-155">Adicionar um membro a um chat.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-155">Add a member to a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="c9ecd-156">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9ecd-156">Properties</span></span>

| <span data-ttu-id="c9ecd-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9ecd-157">Property</span></span>   | <span data-ttu-id="c9ecd-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9ecd-158">Type</span></span> |<span data-ttu-id="c9ecd-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9ecd-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9ecd-160">id</span><span class="sxs-lookup"><span data-stu-id="c9ecd-160">id</span></span>|<span data-ttu-id="c9ecd-161">String</span><span class="sxs-lookup"><span data-stu-id="c9ecd-161">String</span></span>| <span data-ttu-id="c9ecd-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-162">Read-only.</span></span> <span data-ttu-id="c9ecd-163">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="c9ecd-164">displayName</span><span class="sxs-lookup"><span data-stu-id="c9ecd-164">displayName</span></span>| <span data-ttu-id="c9ecd-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9ecd-165">string</span></span> | <span data-ttu-id="c9ecd-166">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-166">The display name of the user.</span></span> |
|<span data-ttu-id="c9ecd-167">funções</span><span class="sxs-lookup"><span data-stu-id="c9ecd-167">roles</span></span>| <span data-ttu-id="c9ecd-168">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9ecd-168">string collection</span></span> | <span data-ttu-id="c9ecd-169">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-169">The roles for that user.</span></span> |
|<span data-ttu-id="c9ecd-170">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="c9ecd-170">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="c9ecd-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9ecd-171">DateTimeOffset</span></span> | <span data-ttu-id="c9ecd-172">O carimbo de data/hora que indica o quanto o histórico de uma conversa é compartilhado com o membro da conversa.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-172">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="c9ecd-173">Essa propriedade é configurável somente para os membros de um chat.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-173">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9ecd-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9ecd-174">JSON representation</span></span>

<span data-ttu-id="c9ecd-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9ecd-175">The following is a JSON representation of the resource.</span></span>

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


