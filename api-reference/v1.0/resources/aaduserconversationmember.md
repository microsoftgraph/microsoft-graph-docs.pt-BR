---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cf678e090f4af26aca1222ba464771111b0b6a60
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754296"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="522c6-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="522c6-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="522c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="522c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="522c6-105">Representa um usuário do Azure Active Directory em uma [equipe](team.md), um [canal](channel.md), ou um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="522c6-105">Represents an Azure Active Directory user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="522c6-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="522c6-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="522c6-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="522c6-107">Methods</span></span>

| <span data-ttu-id="522c6-108">Método</span><span class="sxs-lookup"><span data-stu-id="522c6-108">Method</span></span>       | <span data-ttu-id="522c6-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="522c6-109">Return Type</span></span>  |<span data-ttu-id="522c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="522c6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="522c6-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="522c6-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="522c6-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="522c6-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="522c6-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="522c6-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="522c6-114">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="522c6-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="522c6-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="522c6-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="522c6-116">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="522c6-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="522c6-117">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="522c6-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="522c6-118">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="522c6-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="522c6-119">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="522c6-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="522c6-120">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="522c6-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="522c6-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="522c6-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="522c6-122">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="522c6-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="522c6-123">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="522c6-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="522c6-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="522c6-124">None</span></span>|<span data-ttu-id="522c6-125">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="522c6-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="522c6-126">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="522c6-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="522c6-127">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="522c6-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="522c6-128">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="522c6-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="522c6-129">Adicionar membro do canal</span><span class="sxs-lookup"><span data-stu-id="522c6-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="522c6-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="522c6-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="522c6-131">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="522c6-131">Add a member to a channel.</span></span> <span data-ttu-id="522c6-132">Somente suportado para `channel` com o membershipType de `private`.</span><span class="sxs-lookup"><span data-stu-id="522c6-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="522c6-133">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="522c6-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="522c6-134">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="522c6-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="522c6-135">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="522c6-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="522c6-136">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="522c6-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="522c6-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="522c6-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="522c6-138">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="522c6-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="522c6-139">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="522c6-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="522c6-140">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="522c6-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="522c6-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="522c6-141">None</span></span> | <span data-ttu-id="522c6-142">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="522c6-142">Delete a member from a channel.</span></span> <span data-ttu-id="522c6-143">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="522c6-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="522c6-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="522c6-144">Properties</span></span>

| <span data-ttu-id="522c6-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="522c6-145">Property</span></span>   | <span data-ttu-id="522c6-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="522c6-146">Type</span></span> |<span data-ttu-id="522c6-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="522c6-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="522c6-148">id</span><span class="sxs-lookup"><span data-stu-id="522c6-148">id</span></span>|<span data-ttu-id="522c6-149">String</span><span class="sxs-lookup"><span data-stu-id="522c6-149">String</span></span>| <span data-ttu-id="522c6-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="522c6-150">Read-only.</span></span> <span data-ttu-id="522c6-151">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="522c6-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="522c6-152">displayName</span><span class="sxs-lookup"><span data-stu-id="522c6-152">displayName</span></span>| <span data-ttu-id="522c6-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522c6-153">string</span></span> | <span data-ttu-id="522c6-154">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="522c6-154">The display name of the user.</span></span> |
|<span data-ttu-id="522c6-155">funções</span><span class="sxs-lookup"><span data-stu-id="522c6-155">roles</span></span>| <span data-ttu-id="522c6-156">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="522c6-156">string collection</span></span> | <span data-ttu-id="522c6-157">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="522c6-157">The roles for that user.</span></span> |
|<span data-ttu-id="522c6-158">userId</span><span class="sxs-lookup"><span data-stu-id="522c6-158">userId</span></span>| <span data-ttu-id="522c6-159">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522c6-159">string</span></span> | <span data-ttu-id="522c6-160">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="522c6-160">The guid of the user.</span></span> |
|<span data-ttu-id="522c6-161">email</span><span class="sxs-lookup"><span data-stu-id="522c6-161">email</span></span>| <span data-ttu-id="522c6-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522c6-162">string</span></span>  | <span data-ttu-id="522c6-163">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="522c6-163">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="522c6-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="522c6-164">JSON representation</span></span>

<span data-ttu-id="522c6-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="522c6-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
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

