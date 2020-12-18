---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4cd7b6ac208c719663eb04adf91a98ae6fa7da39
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714337"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="9c799-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="9c799-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="9c799-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c799-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c799-105">Representa um usuário do Azure Active Directory em uma [equipe](team.md) ou em um [canal](channel.md) ou em um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="9c799-105">Represents an Azure Active Directory user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span> <span data-ttu-id="9c799-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="9c799-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9c799-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9c799-107">Methods</span></span>

| <span data-ttu-id="9c799-108">Método</span><span class="sxs-lookup"><span data-stu-id="9c799-108">Method</span></span>       | <span data-ttu-id="9c799-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9c799-109">Return Type</span></span>  |<span data-ttu-id="9c799-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c799-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c799-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="9c799-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="9c799-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9c799-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="9c799-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="9c799-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="9c799-114">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="9c799-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="9c799-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9c799-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="9c799-116">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="9c799-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="9c799-117">Adicionar membros em massa à equipe.</span><span class="sxs-lookup"><span data-stu-id="9c799-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="9c799-118">coleção[actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="9c799-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="9c799-119">Adicione vários membros à equipe em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c799-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="9c799-120">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="9c799-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="9c799-121">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="9c799-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9c799-122">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="9c799-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="9c799-123">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="9c799-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="9c799-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9c799-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="9c799-125">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="9c799-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="9c799-126">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="9c799-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="9c799-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c799-127">None</span></span>|<span data-ttu-id="9c799-128">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="9c799-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="9c799-129">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="9c799-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="9c799-130">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9c799-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9c799-131">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="9c799-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="9c799-132">Adicionar membro do canal</span><span class="sxs-lookup"><span data-stu-id="9c799-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="9c799-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9c799-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9c799-134">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="9c799-134">Add a member to a channel.</span></span> <span data-ttu-id="9c799-135">Suportado só para o`channel`com MembershipType de.`private`</span><span class="sxs-lookup"><span data-stu-id="9c799-135">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="9c799-136">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="9c799-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="9c799-137">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9c799-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9c799-138">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="9c799-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="9c799-139">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="9c799-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="9c799-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9c799-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9c799-141">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="9c799-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="9c799-142">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="9c799-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="9c799-143">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="9c799-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="9c799-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c799-144">None</span></span> | <span data-ttu-id="9c799-145">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="9c799-145">Delete a member from a channel.</span></span> <span data-ttu-id="9c799-146">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="9c799-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="9c799-147">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="9c799-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="9c799-148">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9c799-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9c799-149">Obter a lista de todos os membros em um chat.</span><span class="sxs-lookup"><span data-stu-id="9c799-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="9c799-150">Adicionar membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="9c799-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="9c799-151">Cabeçalho de local</span><span class="sxs-lookup"><span data-stu-id="9c799-151">Location header</span></span> | <span data-ttu-id="9c799-152">Adicionar um membro a um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="9c799-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="9c799-153">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="9c799-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="9c799-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9c799-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9c799-155">Obtenha um membro em um chat.</span><span class="sxs-lookup"><span data-stu-id="9c799-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="9c799-156">Remover membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="9c799-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="9c799-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c799-157">None</span></span> | <span data-ttu-id="9c799-158">Remover um membro de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="9c799-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="9c799-159">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c799-159">Properties</span></span>

| <span data-ttu-id="9c799-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c799-160">Property</span></span>   | <span data-ttu-id="9c799-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c799-161">Type</span></span> |<span data-ttu-id="9c799-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c799-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c799-163">id</span><span class="sxs-lookup"><span data-stu-id="9c799-163">id</span></span>| <span data-ttu-id="9c799-164">String</span><span class="sxs-lookup"><span data-stu-id="9c799-164">String</span></span> | <span data-ttu-id="9c799-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c799-165">Read-only.</span></span> <span data-ttu-id="9c799-166">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c799-166">Unique ID of the user.</span></span>|
|<span data-ttu-id="9c799-167">displayName</span><span class="sxs-lookup"><span data-stu-id="9c799-167">displayName</span></span>| <span data-ttu-id="9c799-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c799-168">String</span></span> | <span data-ttu-id="9c799-169">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c799-169">The display name of the user.</span></span> |
|<span data-ttu-id="9c799-170">funções</span><span class="sxs-lookup"><span data-stu-id="9c799-170">roles</span></span>| <span data-ttu-id="9c799-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c799-171">String collection</span></span> | <span data-ttu-id="9c799-172">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="9c799-172">The roles for that user.</span></span> |
|<span data-ttu-id="9c799-173">userId</span><span class="sxs-lookup"><span data-stu-id="9c799-173">userId</span></span>| <span data-ttu-id="9c799-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c799-174">String</span></span> | <span data-ttu-id="9c799-175">O GUID do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c799-175">The GUID of the user.</span></span> |
|<span data-ttu-id="9c799-176">email</span><span class="sxs-lookup"><span data-stu-id="9c799-176">email</span></span>| <span data-ttu-id="9c799-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c799-177">String</span></span>  | <span data-ttu-id="9c799-178">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c799-178">The email address of the user.</span></span> |
|<span data-ttu-id="9c799-179">tenantId</span><span class="sxs-lookup"><span data-stu-id="9c799-179">tenantId</span></span>| <span data-ttu-id="9c799-180">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c799-180">string</span></span>  | <span data-ttu-id="9c799-181">TenantId para o qual o usuário do Azure AD pertence.</span><span class="sxs-lookup"><span data-stu-id="9c799-181">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="9c799-182">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9c799-182">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="9c799-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c799-183">DateTimeOffset</span></span>  | <span data-ttu-id="9c799-184">O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa.</span><span class="sxs-lookup"><span data-stu-id="9c799-184">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="9c799-185">Essa propriedade é configurável somente para os membros de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="9c799-185">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c799-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c799-186">JSON representation</span></span>

<span data-ttu-id="9c799-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c799-187">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aadUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String",
  "email": "String",
  "tenantId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
