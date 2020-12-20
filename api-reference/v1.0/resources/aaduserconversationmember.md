---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c7e989adcafd4752dea6d2fca82ecfa7638bf1ec
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714120"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="e97ef-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="e97ef-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="e97ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e97ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e97ef-105">Representa um usuário do Azure Active Directory em uma [equipe](team.md), um [canal](channel.md), ou um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="e97ef-105">Represents an Azure Active Directory user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="e97ef-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="e97ef-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e97ef-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e97ef-107">Methods</span></span>

| <span data-ttu-id="e97ef-108">Método</span><span class="sxs-lookup"><span data-stu-id="e97ef-108">Method</span></span>       | <span data-ttu-id="e97ef-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e97ef-109">Return Type</span></span>  |<span data-ttu-id="e97ef-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e97ef-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e97ef-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="e97ef-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="e97ef-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e97ef-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="e97ef-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="e97ef-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="e97ef-114">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="e97ef-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="e97ef-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="e97ef-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="e97ef-116">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="e97ef-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="e97ef-117">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="e97ef-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="e97ef-118">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="e97ef-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="e97ef-119">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="e97ef-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="e97ef-120">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="e97ef-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="e97ef-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="e97ef-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="e97ef-122">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="e97ef-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="e97ef-123">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="e97ef-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="e97ef-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e97ef-124">None</span></span>|<span data-ttu-id="e97ef-125">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="e97ef-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="e97ef-126">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="e97ef-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="e97ef-127">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e97ef-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="e97ef-128">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="e97ef-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="e97ef-129">Adicionar membro do canal</span><span class="sxs-lookup"><span data-stu-id="e97ef-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="e97ef-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="e97ef-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="e97ef-131">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="e97ef-131">Add a member to a channel.</span></span> <span data-ttu-id="e97ef-132">Suportado só para o`channel`com MembershipType de.`private`</span><span class="sxs-lookup"><span data-stu-id="e97ef-132">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="e97ef-133">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="e97ef-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="e97ef-134">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e97ef-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="e97ef-135">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="e97ef-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="e97ef-136">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="e97ef-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="e97ef-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="e97ef-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="e97ef-138">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="e97ef-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="e97ef-139">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="e97ef-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="e97ef-140">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="e97ef-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="e97ef-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e97ef-141">None</span></span> | <span data-ttu-id="e97ef-142">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="e97ef-142">Delete a member from a channel.</span></span> <span data-ttu-id="e97ef-143">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="e97ef-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="e97ef-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e97ef-144">Properties</span></span>

| <span data-ttu-id="e97ef-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e97ef-145">Property</span></span>   | <span data-ttu-id="e97ef-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="e97ef-146">Type</span></span> |<span data-ttu-id="e97ef-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="e97ef-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e97ef-148">id</span><span class="sxs-lookup"><span data-stu-id="e97ef-148">id</span></span>|<span data-ttu-id="e97ef-149">String</span><span class="sxs-lookup"><span data-stu-id="e97ef-149">String</span></span>| <span data-ttu-id="e97ef-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e97ef-150">Read-only.</span></span> <span data-ttu-id="e97ef-151">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="e97ef-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="e97ef-152">displayName</span><span class="sxs-lookup"><span data-stu-id="e97ef-152">displayName</span></span>| <span data-ttu-id="e97ef-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e97ef-153">string</span></span> | <span data-ttu-id="e97ef-154">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="e97ef-154">The display name of the user.</span></span> |
|<span data-ttu-id="e97ef-155">funções</span><span class="sxs-lookup"><span data-stu-id="e97ef-155">roles</span></span>| <span data-ttu-id="e97ef-156">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e97ef-156">string collection</span></span> | <span data-ttu-id="e97ef-157">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="e97ef-157">The roles for that user.</span></span> |
|<span data-ttu-id="e97ef-158">userId</span><span class="sxs-lookup"><span data-stu-id="e97ef-158">userId</span></span>| <span data-ttu-id="e97ef-159">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e97ef-159">string</span></span> | <span data-ttu-id="e97ef-160">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="e97ef-160">The guid of the user.</span></span> |
|<span data-ttu-id="e97ef-161">email</span><span class="sxs-lookup"><span data-stu-id="e97ef-161">email</span></span>| <span data-ttu-id="e97ef-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e97ef-162">string</span></span>  | <span data-ttu-id="e97ef-163">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="e97ef-163">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e97ef-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e97ef-164">JSON representation</span></span>

<span data-ttu-id="e97ef-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e97ef-165">The following is a JSON representation of the resource.</span></span>

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

