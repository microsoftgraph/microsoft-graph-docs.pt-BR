---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f19c5a2b711ab6c39069364c641066f1d9c6dbf
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705965"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="0aaa4-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="0aaa4-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="0aaa4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aaa4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aaa4-105">Representa um usuário do Azure Active Directory em um [chat](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="0aaa4-105">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="0aaa4-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="0aaa4-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0aaa4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0aaa4-107">Methods</span></span>

| <span data-ttu-id="0aaa4-108">Método</span><span class="sxs-lookup"><span data-stu-id="0aaa4-108">Method</span></span>       | <span data-ttu-id="0aaa4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0aaa4-109">Return Type</span></span>  |<span data-ttu-id="0aaa4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0aaa4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0aaa4-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="0aaa4-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="0aaa4-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="0aaa4-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="0aaa4-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="0aaa4-114">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="0aaa4-114">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="0aaa4-115">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="0aaa4-115">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="0aaa4-116">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-116">Get a member in the team.</span></span>|
|[<span data-ttu-id="0aaa4-117">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="0aaa4-117">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="0aaa4-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0aaa4-118">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="0aaa4-119">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-119">Add a new member to the team.</span></span>|
|[<span data-ttu-id="0aaa4-120">Adicionar membros em massa à equipe.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-120">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="0aaa4-121">coleção[actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="0aaa4-121">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="0aaa4-122">Adicione vários membros à equipe em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-122">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="0aaa4-123">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="0aaa4-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="0aaa4-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0aaa4-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="0aaa4-125">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="0aaa4-126">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="0aaa4-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="0aaa4-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0aaa4-127">None</span></span>|<span data-ttu-id="0aaa4-128">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="0aaa4-129">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="0aaa4-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="0aaa4-130">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="0aaa4-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="0aaa4-131">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="0aaa4-132">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="0aaa4-132">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="0aaa4-133">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="0aaa4-133">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="0aaa4-134">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-134">Get a member in a channel.</span></span>|
|[<span data-ttu-id="0aaa4-135">Criar membro do canal</span><span class="sxs-lookup"><span data-stu-id="0aaa4-135">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="0aaa4-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0aaa4-136">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="0aaa4-137">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-137">Add a member to a channel.</span></span> <span data-ttu-id="0aaa4-138">Suportado só para o`channel`com MembershipType de.`private`</span><span class="sxs-lookup"><span data-stu-id="0aaa4-138">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="0aaa4-139">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="0aaa4-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="0aaa4-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0aaa4-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="0aaa4-141">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="0aaa4-142">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="0aaa4-143">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="0aaa4-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="0aaa4-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0aaa4-144">None</span></span> | <span data-ttu-id="0aaa4-145">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-145">Delete a member from a channel.</span></span> <span data-ttu-id="0aaa4-146">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="0aaa4-147">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="0aaa4-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="0aaa4-148">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="0aaa4-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="0aaa4-149">Obter a lista de todos os membros em um chat.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="0aaa4-150">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="0aaa4-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="0aaa4-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0aaa4-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="0aaa4-152">Obtenha um membro em um chat.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="0aaa4-153">Adicionar membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="0aaa4-153">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="0aaa4-154">Cabeçalho de local</span><span class="sxs-lookup"><span data-stu-id="0aaa4-154">Location header</span></span> | <span data-ttu-id="0aaa4-155">Adicionar um membro a um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-155">Add a member to a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="0aaa4-156">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0aaa4-156">Properties</span></span>

| <span data-ttu-id="0aaa4-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0aaa4-157">Property</span></span>   | <span data-ttu-id="0aaa4-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="0aaa4-158">Type</span></span> |<span data-ttu-id="0aaa4-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="0aaa4-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0aaa4-160">id</span><span class="sxs-lookup"><span data-stu-id="0aaa4-160">id</span></span>| <span data-ttu-id="0aaa4-161">String</span><span class="sxs-lookup"><span data-stu-id="0aaa4-161">String</span></span> | <span data-ttu-id="0aaa4-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-162">Read-only.</span></span> <span data-ttu-id="0aaa4-163">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="0aaa4-164">displayName</span><span class="sxs-lookup"><span data-stu-id="0aaa4-164">displayName</span></span>| <span data-ttu-id="0aaa4-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0aaa4-165">String</span></span> | <span data-ttu-id="0aaa4-166">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-166">The display name of the user.</span></span> |
|<span data-ttu-id="0aaa4-167">funções</span><span class="sxs-lookup"><span data-stu-id="0aaa4-167">roles</span></span>| <span data-ttu-id="0aaa4-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0aaa4-168">String collection</span></span> | <span data-ttu-id="0aaa4-169">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-169">The roles for that user.</span></span> |
|<span data-ttu-id="0aaa4-170">userId</span><span class="sxs-lookup"><span data-stu-id="0aaa4-170">userId</span></span>| <span data-ttu-id="0aaa4-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0aaa4-171">String</span></span> | <span data-ttu-id="0aaa4-172">O GUID do usuário.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-172">The GUID of the user.</span></span> |
|<span data-ttu-id="0aaa4-173">email</span><span class="sxs-lookup"><span data-stu-id="0aaa4-173">email</span></span>| <span data-ttu-id="0aaa4-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0aaa4-174">String</span></span>  | <span data-ttu-id="0aaa4-175">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-175">The email address of the user.</span></span> |
|<span data-ttu-id="0aaa4-176">tenantId</span><span class="sxs-lookup"><span data-stu-id="0aaa4-176">tenantId</span></span>| <span data-ttu-id="0aaa4-177">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0aaa4-177">string</span></span>  | <span data-ttu-id="0aaa4-178">TenantId para o qual o usuário do Azure AD pertence.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-178">TenantId which the Azure AD user belongs to.</span></span> |
|<span data-ttu-id="0aaa4-179">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="0aaa4-179">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="0aaa4-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aaa4-180">DateTimeOffset</span></span>  | <span data-ttu-id="0aaa4-181">O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-181">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="0aaa4-182">Essa propriedade é configurável somente para os membros de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-182">This property is settable only for members of a chat.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0aaa4-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0aaa4-183">JSON representation</span></span>

<span data-ttu-id="0aaa4-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0aaa4-184">The following is a JSON representation of the resource.</span></span>

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
