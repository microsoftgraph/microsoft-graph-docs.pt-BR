---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a8e4c94681065d9686e9f17888d3abf35885a65
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658039"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="4cc6c-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="4cc6c-103">conversationMember resource type</span></span>

<span data-ttu-id="4cc6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cc6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cc6c-105">Representa um usuário em um [bate-papo](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="4cc6c-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="4cc6c-106">Confira também [aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="4cc6c-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4cc6c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4cc6c-107">Methods</span></span>

| <span data-ttu-id="4cc6c-108">Método</span><span class="sxs-lookup"><span data-stu-id="4cc6c-108">Method</span></span>       | <span data-ttu-id="4cc6c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4cc6c-109">Return Type</span></span>  |<span data-ttu-id="4cc6c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cc6c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4cc6c-111">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="4cc6c-111">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="4cc6c-112">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4cc6c-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4cc6c-113">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-113">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="4cc6c-114">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="4cc6c-114">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="4cc6c-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4cc6c-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="4cc6c-116">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-116">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="4cc6c-117">Listar membros da equipe</span><span class="sxs-lookup"><span data-stu-id="4cc6c-117">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="4cc6c-118">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4cc6c-118">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="4cc6c-119">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-119">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="4cc6c-120">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="4cc6c-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="4cc6c-121">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="4cc6c-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4cc6c-122">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="4cc6c-123">Adicionar membro da equipe</span><span class="sxs-lookup"><span data-stu-id="4cc6c-123">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="4cc6c-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4cc6c-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="4cc6c-125">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-125">Add a new member to the team.</span></span>|
|[<span data-ttu-id="4cc6c-126">Adicionar membros da equipe em massa</span><span class="sxs-lookup"><span data-stu-id="4cc6c-126">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="4cc6c-127">coleção [actionResultPart](../resources/actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="4cc6c-127">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="4cc6c-128">Adicionar vários membros à equipe em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-128">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="4cc6c-129">Atualizar a função do membro da equipe</span><span class="sxs-lookup"><span data-stu-id="4cc6c-129">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="4cc6c-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4cc6c-130">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="4cc6c-131">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-131">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="4cc6c-132">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="4cc6c-132">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="4cc6c-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4cc6c-133">None</span></span>|<span data-ttu-id="4cc6c-134">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-134">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="4cc6c-135">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="4cc6c-135">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="4cc6c-136">[conversationMember](conversationmember.md) coleção</span><span class="sxs-lookup"><span data-stu-id="4cc6c-136">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4cc6c-137">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-137">Get a member in a channel.</span></span>|
|[<span data-ttu-id="4cc6c-138">Criar membro do canal</span><span class="sxs-lookup"><span data-stu-id="4cc6c-138">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="4cc6c-139">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4cc6c-139">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="4cc6c-140">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-140">Add a member to a channel.</span></span> <span data-ttu-id="4cc6c-141">Suportado só para o`channel`com MembershipType de.`private`</span><span class="sxs-lookup"><span data-stu-id="4cc6c-141">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="4cc6c-142">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="4cc6c-142">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="4cc6c-143">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4cc6c-143">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="4cc6c-144">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-144">Update the properties of a member of the channel.</span></span> <span data-ttu-id="4cc6c-145">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-145">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="4cc6c-146">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="4cc6c-146">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="4cc6c-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4cc6c-147">None</span></span> | <span data-ttu-id="4cc6c-148">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-148">Delete a member from a channel.</span></span> <span data-ttu-id="4cc6c-149">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-149">Only supported for `channelType` of `private`.</span></span>|



## <a name="properties"></a><span data-ttu-id="4cc6c-150">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cc6c-150">Properties</span></span>

| <span data-ttu-id="4cc6c-151">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cc6c-151">Property</span></span>   | <span data-ttu-id="4cc6c-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cc6c-152">Type</span></span> |<span data-ttu-id="4cc6c-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cc6c-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cc6c-154">id</span><span class="sxs-lookup"><span data-stu-id="4cc6c-154">id</span></span>|<span data-ttu-id="4cc6c-155">String</span><span class="sxs-lookup"><span data-stu-id="4cc6c-155">String</span></span>| <span data-ttu-id="4cc6c-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-156">Read-only.</span></span> <span data-ttu-id="4cc6c-157">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-157">Unique ID of the user.</span></span>|
|<span data-ttu-id="4cc6c-158">displayName</span><span class="sxs-lookup"><span data-stu-id="4cc6c-158">displayName</span></span>| <span data-ttu-id="4cc6c-159">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cc6c-159">string</span></span> | <span data-ttu-id="4cc6c-160">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-160">The display name of the user.</span></span> |
|<span data-ttu-id="4cc6c-161">funções</span><span class="sxs-lookup"><span data-stu-id="4cc6c-161">roles</span></span>| <span data-ttu-id="4cc6c-162">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cc6c-162">string collection</span></span> | <span data-ttu-id="4cc6c-163">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-163">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4cc6c-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cc6c-164">JSON representation</span></span>

<span data-ttu-id="4cc6c-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4cc6c-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
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


