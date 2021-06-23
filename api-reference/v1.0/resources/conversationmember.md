---
title: tipo de recurso conversationMember
description: Representa o usuário em uma conversa.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c82f7e1ec927c73ad41771fc00e013dda1755a80
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060304"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="1cd9e-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="1cd9e-103">conversationMember resource type</span></span>

<span data-ttu-id="1cd9e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cd9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1cd9e-105">Representa um usuário em uma [equipe,](team.md)um [canal](channel.md)ou [um chat.](chat.md)</span><span class="sxs-lookup"><span data-stu-id="1cd9e-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="1cd9e-106">Consulte também [aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="1cd9e-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1cd9e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1cd9e-107">Methods</span></span>

| <span data-ttu-id="1cd9e-108">Método</span><span class="sxs-lookup"><span data-stu-id="1cd9e-108">Method</span></span>       | <span data-ttu-id="1cd9e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1cd9e-109">Return Type</span></span>  |<span data-ttu-id="1cd9e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd9e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cd9e-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="1cd9e-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="1cd9e-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="1cd9e-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="1cd9e-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="1cd9e-114">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="1cd9e-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="1cd9e-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="1cd9e-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="1cd9e-116">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="1cd9e-117">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="1cd9e-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="1cd9e-118">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="1cd9e-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="1cd9e-119">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="1cd9e-120">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="1cd9e-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="1cd9e-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="1cd9e-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="1cd9e-122">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="1cd9e-123">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="1cd9e-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="1cd9e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cd9e-124">None</span></span>|<span data-ttu-id="1cd9e-125">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="1cd9e-126">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="1cd9e-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="1cd9e-127">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="1cd9e-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="1cd9e-128">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="1cd9e-129">Adicionar membro do canal</span><span class="sxs-lookup"><span data-stu-id="1cd9e-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="1cd9e-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="1cd9e-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="1cd9e-131">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-131">Add a member to a channel.</span></span> <span data-ttu-id="1cd9e-132">Somente suportado para `channel` com o membershipType de `private`.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="1cd9e-133">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="1cd9e-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="1cd9e-134">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="1cd9e-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="1cd9e-135">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="1cd9e-136">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="1cd9e-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="1cd9e-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="1cd9e-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="1cd9e-138">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="1cd9e-139">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="1cd9e-140">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="1cd9e-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="1cd9e-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cd9e-141">None</span></span> | <span data-ttu-id="1cd9e-142">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-142">Delete a member from a channel.</span></span> <span data-ttu-id="1cd9e-143">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-143">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="1cd9e-144">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="1cd9e-144">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="1cd9e-145">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="1cd9e-145">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="1cd9e-146">Obter a lista de todos os membros em um chat.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-146">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="1cd9e-147">Adicionar membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="1cd9e-147">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="1cd9e-148">Cabeçalho de local</span><span class="sxs-lookup"><span data-stu-id="1cd9e-148">Location header</span></span> | <span data-ttu-id="1cd9e-149">Adicionar um membro a um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-149">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="1cd9e-150">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="1cd9e-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="1cd9e-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="1cd9e-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="1cd9e-152">Obtenha um membro em um chat.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="1cd9e-153">Remover membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="1cd9e-153">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="1cd9e-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cd9e-154">None</span></span> | <span data-ttu-id="1cd9e-155">Remover um membro de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-155">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="1cd9e-156">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cd9e-156">Properties</span></span>

| <span data-ttu-id="1cd9e-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cd9e-157">Property</span></span>   | <span data-ttu-id="1cd9e-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cd9e-158">Type</span></span> |<span data-ttu-id="1cd9e-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd9e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cd9e-160">id</span><span class="sxs-lookup"><span data-stu-id="1cd9e-160">id</span></span>|<span data-ttu-id="1cd9e-161">String</span><span class="sxs-lookup"><span data-stu-id="1cd9e-161">String</span></span>| <span data-ttu-id="1cd9e-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-162">Read-only.</span></span> <span data-ttu-id="1cd9e-163">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="1cd9e-164">displayName</span><span class="sxs-lookup"><span data-stu-id="1cd9e-164">displayName</span></span>| <span data-ttu-id="1cd9e-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cd9e-165">string</span></span> | <span data-ttu-id="1cd9e-166">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-166">The display name of the user.</span></span> |
|<span data-ttu-id="1cd9e-167">funções</span><span class="sxs-lookup"><span data-stu-id="1cd9e-167">roles</span></span>| <span data-ttu-id="1cd9e-168">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cd9e-168">string collection</span></span> | <span data-ttu-id="1cd9e-169">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-169">The roles for that user.</span></span> |
|<span data-ttu-id="1cd9e-170">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd9e-170">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="1cd9e-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd9e-171">DateTimeOffset</span></span> | <span data-ttu-id="1cd9e-172">O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-172">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="1cd9e-173">Essa propriedade é configurável somente para os membros de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-173">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1cd9e-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cd9e-174">JSON representation</span></span>

<span data-ttu-id="1cd9e-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cd9e-175">The following is a JSON representation of the resource.</span></span>

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

