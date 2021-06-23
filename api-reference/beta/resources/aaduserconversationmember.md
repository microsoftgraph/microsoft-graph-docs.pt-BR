---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c7d65249e6e284efeaf0b34a4ffaf027026932d4
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060277"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="4a7d6-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="4a7d6-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="4a7d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a7d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a7d6-105">Representa um usuário do Azure Active Directory em uma [equipe](team.md) ou em um [canal](channel.md) ou em um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="4a7d6-105">Represents an Azure Active Directory user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span> <span data-ttu-id="4a7d6-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="4a7d6-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4a7d6-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4a7d6-107">Methods</span></span>

| <span data-ttu-id="4a7d6-108">Método</span><span class="sxs-lookup"><span data-stu-id="4a7d6-108">Method</span></span>       | <span data-ttu-id="4a7d6-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4a7d6-109">Return Type</span></span>  |<span data-ttu-id="4a7d6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a7d6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a7d6-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="4a7d6-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="4a7d6-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4a7d6-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="4a7d6-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="4a7d6-114">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="4a7d6-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="4a7d6-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4a7d6-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="4a7d6-116">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="4a7d6-117">Adicionar membros em massa à equipe.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="4a7d6-118">coleção[actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="4a7d6-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="4a7d6-119">Adicione vários membros à equipe em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="4a7d6-120">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="4a7d6-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="4a7d6-121">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="4a7d6-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4a7d6-122">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="4a7d6-123">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="4a7d6-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="4a7d6-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4a7d6-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="4a7d6-125">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="4a7d6-126">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="4a7d6-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="4a7d6-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a7d6-127">None</span></span>|<span data-ttu-id="4a7d6-128">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="4a7d6-129">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="4a7d6-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="4a7d6-130">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4a7d6-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4a7d6-131">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="4a7d6-132">Adicionar membro do canal</span><span class="sxs-lookup"><span data-stu-id="4a7d6-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="4a7d6-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4a7d6-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="4a7d6-134">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-134">Add a member to a channel.</span></span> <span data-ttu-id="4a7d6-135">Somente suportado para `channel` com o membershipType de `private`.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-135">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="4a7d6-136">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="4a7d6-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="4a7d6-137">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4a7d6-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4a7d6-138">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="4a7d6-139">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="4a7d6-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="4a7d6-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4a7d6-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="4a7d6-141">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="4a7d6-142">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="4a7d6-143">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="4a7d6-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="4a7d6-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a7d6-144">None</span></span> | <span data-ttu-id="4a7d6-145">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-145">Delete a member from a channel.</span></span> <span data-ttu-id="4a7d6-146">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="4a7d6-147">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="4a7d6-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="4a7d6-148">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4a7d6-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4a7d6-149">Obter a lista de todos os membros em um chat.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="4a7d6-150">Adicionar membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="4a7d6-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="4a7d6-151">Cabeçalho de local</span><span class="sxs-lookup"><span data-stu-id="4a7d6-151">Location header</span></span> | <span data-ttu-id="4a7d6-152">Adicionar um membro a um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="4a7d6-153">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="4a7d6-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="4a7d6-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4a7d6-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="4a7d6-155">Obtenha um membro em um chat.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="4a7d6-156">Remover membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="4a7d6-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="4a7d6-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a7d6-157">None</span></span> | <span data-ttu-id="4a7d6-158">Remover um membro de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="4a7d6-159">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a7d6-159">Properties</span></span>

| <span data-ttu-id="4a7d6-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a7d6-160">Property</span></span>   | <span data-ttu-id="4a7d6-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a7d6-161">Type</span></span> |<span data-ttu-id="4a7d6-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a7d6-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a7d6-163">id</span><span class="sxs-lookup"><span data-stu-id="4a7d6-163">id</span></span>| <span data-ttu-id="4a7d6-164">String</span><span class="sxs-lookup"><span data-stu-id="4a7d6-164">String</span></span> | <span data-ttu-id="4a7d6-p105">Somente leitura. ID exclusiva do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-p105">Read-only. Unique ID of the user.</span></span>|
|<span data-ttu-id="4a7d6-167">displayName</span><span class="sxs-lookup"><span data-stu-id="4a7d6-167">displayName</span></span>| <span data-ttu-id="4a7d6-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a7d6-168">String</span></span> | <span data-ttu-id="4a7d6-169">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-169">The display name of the user.</span></span> |
|<span data-ttu-id="4a7d6-170">funções</span><span class="sxs-lookup"><span data-stu-id="4a7d6-170">roles</span></span>| <span data-ttu-id="4a7d6-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a7d6-171">String collection</span></span> | <span data-ttu-id="4a7d6-172">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-172">The roles for that user.</span></span> |
|<span data-ttu-id="4a7d6-173">userId</span><span class="sxs-lookup"><span data-stu-id="4a7d6-173">userId</span></span>| <span data-ttu-id="4a7d6-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a7d6-174">String</span></span> | <span data-ttu-id="4a7d6-175">O GUID do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-175">The GUID of the user.</span></span> |
|<span data-ttu-id="4a7d6-176">email</span><span class="sxs-lookup"><span data-stu-id="4a7d6-176">email</span></span>| <span data-ttu-id="4a7d6-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a7d6-177">String</span></span>  | <span data-ttu-id="4a7d6-178">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-178">The email address of the user.</span></span> |
|<span data-ttu-id="4a7d6-179">tenantId</span><span class="sxs-lookup"><span data-stu-id="4a7d6-179">tenantId</span></span>| <span data-ttu-id="4a7d6-180">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a7d6-180">string</span></span>  | <span data-ttu-id="4a7d6-181">TenantId para o qual o usuário do Azure AD pertence.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-181">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="4a7d6-182">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="4a7d6-182">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="4a7d6-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a7d6-183">DateTimeOffset</span></span>  | <span data-ttu-id="4a7d6-184">O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-184">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="4a7d6-185">Essa propriedade é configurável somente para os membros de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-185">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a7d6-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a7d6-186">JSON representation</span></span>

<span data-ttu-id="4a7d6-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a7d6-187">The following is a JSON representation of the resource.</span></span>

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
