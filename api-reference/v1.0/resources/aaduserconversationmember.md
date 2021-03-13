---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: aeb5dd5e21019b06f8757b37505d6e5e9f1a4354
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777388"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="b0eb5-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="b0eb5-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="b0eb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0eb5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0eb5-105">Representa um usuário do Azure Active Directory em uma [equipe](team.md), um [canal](channel.md), ou um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="b0eb5-105">Represents an Azure Active Directory user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="b0eb5-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="b0eb5-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b0eb5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0eb5-107">Methods</span></span>

| <span data-ttu-id="b0eb5-108">Método</span><span class="sxs-lookup"><span data-stu-id="b0eb5-108">Method</span></span>       | <span data-ttu-id="b0eb5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0eb5-109">Return Type</span></span>  |<span data-ttu-id="b0eb5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0eb5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0eb5-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="b0eb5-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="b0eb5-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b0eb5-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="b0eb5-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="b0eb5-114">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="b0eb5-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="b0eb5-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="b0eb5-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="b0eb5-116">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="b0eb5-117">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="b0eb5-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="b0eb5-118">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="b0eb5-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b0eb5-119">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="b0eb5-120">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="b0eb5-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="b0eb5-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="b0eb5-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="b0eb5-122">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="b0eb5-123">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="b0eb5-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="b0eb5-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0eb5-124">None</span></span>|<span data-ttu-id="b0eb5-125">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="b0eb5-126">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="b0eb5-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="b0eb5-127">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b0eb5-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b0eb5-128">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="b0eb5-129">Adicionar membro do canal</span><span class="sxs-lookup"><span data-stu-id="b0eb5-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="b0eb5-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="b0eb5-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="b0eb5-131">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-131">Add a member to a channel.</span></span> <span data-ttu-id="b0eb5-132">Somente suportado para `channel` com o membershipType de `private`.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="b0eb5-133">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="b0eb5-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="b0eb5-134">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b0eb5-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b0eb5-135">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="b0eb5-136">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="b0eb5-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="b0eb5-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="b0eb5-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="b0eb5-138">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="b0eb5-139">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="b0eb5-140">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="b0eb5-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="b0eb5-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0eb5-141">None</span></span> | <span data-ttu-id="b0eb5-142">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-142">Delete a member from a channel.</span></span> <span data-ttu-id="b0eb5-143">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-143">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="b0eb5-144">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="b0eb5-144">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="b0eb5-145">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="b0eb5-145">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="b0eb5-146">Obter a lista de todos os membros em um chat.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-146">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="b0eb5-147">Adicionar membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="b0eb5-147">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="b0eb5-148">Cabeçalho de local</span><span class="sxs-lookup"><span data-stu-id="b0eb5-148">Location header</span></span> | <span data-ttu-id="b0eb5-149">Adicionar um membro a um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-149">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="b0eb5-150">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="b0eb5-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="b0eb5-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="b0eb5-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="b0eb5-152">Obtenha um membro em um chat.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="b0eb5-153">Remover membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="b0eb5-153">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="b0eb5-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0eb5-154">None</span></span> | <span data-ttu-id="b0eb5-155">Remover um membro de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-155">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="b0eb5-156">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0eb5-156">Properties</span></span>

| <span data-ttu-id="b0eb5-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0eb5-157">Property</span></span>   | <span data-ttu-id="b0eb5-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0eb5-158">Type</span></span> |<span data-ttu-id="b0eb5-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0eb5-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0eb5-160">id</span><span class="sxs-lookup"><span data-stu-id="b0eb5-160">id</span></span>|<span data-ttu-id="b0eb5-161">String</span><span class="sxs-lookup"><span data-stu-id="b0eb5-161">String</span></span>| <span data-ttu-id="b0eb5-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-162">Read-only.</span></span> <span data-ttu-id="b0eb5-163">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="b0eb5-164">displayName</span><span class="sxs-lookup"><span data-stu-id="b0eb5-164">displayName</span></span>| <span data-ttu-id="b0eb5-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0eb5-165">string</span></span> | <span data-ttu-id="b0eb5-166">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-166">The display name of the user.</span></span> |
|<span data-ttu-id="b0eb5-167">funções</span><span class="sxs-lookup"><span data-stu-id="b0eb5-167">roles</span></span>| <span data-ttu-id="b0eb5-168">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0eb5-168">string collection</span></span> | <span data-ttu-id="b0eb5-169">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-169">The roles for that user.</span></span> |
|<span data-ttu-id="b0eb5-170">userId</span><span class="sxs-lookup"><span data-stu-id="b0eb5-170">userId</span></span>| <span data-ttu-id="b0eb5-171">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0eb5-171">string</span></span> | <span data-ttu-id="b0eb5-172">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-172">The guid of the user.</span></span> |
|<span data-ttu-id="b0eb5-173">email</span><span class="sxs-lookup"><span data-stu-id="b0eb5-173">email</span></span>| <span data-ttu-id="b0eb5-174">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0eb5-174">string</span></span>  | <span data-ttu-id="b0eb5-175">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-175">The email address of the user.</span></span> |
|<span data-ttu-id="b0eb5-176">tenantId</span><span class="sxs-lookup"><span data-stu-id="b0eb5-176">tenantId</span></span>| <span data-ttu-id="b0eb5-177">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0eb5-177">string</span></span>  | <span data-ttu-id="b0eb5-178">TenantId para o qual o usuário do Azure AD pertence.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-178">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="b0eb5-179">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="b0eb5-179">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="b0eb5-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0eb5-180">DateTimeOffset</span></span>  | <span data-ttu-id="b0eb5-181">O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-181">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="b0eb5-182">Essa propriedade é configurável somente para os membros de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-182">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0eb5-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0eb5-183">JSON representation</span></span>

<span data-ttu-id="b0eb5-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0eb5-184">The following is a JSON representation of the resource.</span></span>

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
  "id": "string (identifier)",
  "displayName" : "string",
  "visibleHistoryStartDateTime": "string (timestamp)",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string",
  "tenantId": "string"
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

