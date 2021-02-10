---
title: tipo de recurso conversationMember
description: Representa o usuário em uma conversa.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1629b46b12d91fd96dca72577027f0031ab0102a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161786"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="ab1aa-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="ab1aa-103">conversationMember resource type</span></span>

<span data-ttu-id="ab1aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab1aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab1aa-105">Representa um usuário em uma [equipe,](team.md)um [canal](channel.md)ou um [chat.](chat.md)</span><span class="sxs-lookup"><span data-stu-id="ab1aa-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="ab1aa-106">Consulte também [aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="ab1aa-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ab1aa-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ab1aa-107">Methods</span></span>

| <span data-ttu-id="ab1aa-108">Método</span><span class="sxs-lookup"><span data-stu-id="ab1aa-108">Method</span></span>       | <span data-ttu-id="ab1aa-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ab1aa-109">Return Type</span></span>  |<span data-ttu-id="ab1aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab1aa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab1aa-111">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="ab1aa-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="ab1aa-112">coleção [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ab1aa-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="ab1aa-113">Obtenha a lista de membros nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="ab1aa-114">Adicionar membro à equipe</span><span class="sxs-lookup"><span data-stu-id="ab1aa-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="ab1aa-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ab1aa-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="ab1aa-116">Adicione um novo membro à equipe.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="ab1aa-117">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="ab1aa-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="ab1aa-118">[conversationMember](conversationmember.md)coleção</span><span class="sxs-lookup"><span data-stu-id="ab1aa-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ab1aa-119">Obtenha um membro na equipe.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="ab1aa-120">Atualizar a função do membro</span><span class="sxs-lookup"><span data-stu-id="ab1aa-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="ab1aa-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ab1aa-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="ab1aa-122">Alterar um membro para um proprietário ou voltar para um membro regular.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="ab1aa-123">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="ab1aa-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="ab1aa-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab1aa-124">None</span></span>|<span data-ttu-id="ab1aa-125">Remova um membro existente da equipe.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="ab1aa-126">Listar membros do canal</span><span class="sxs-lookup"><span data-stu-id="ab1aa-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="ab1aa-127">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ab1aa-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ab1aa-128">Obter a lista de todos os membros em um canal.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="ab1aa-129">Adicionar membro do canal</span><span class="sxs-lookup"><span data-stu-id="ab1aa-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="ab1aa-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ab1aa-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="ab1aa-131">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-131">Add a member to a channel.</span></span> <span data-ttu-id="ab1aa-132">Suportado só para o`channel`com MembershipType de.`private`</span><span class="sxs-lookup"><span data-stu-id="ab1aa-132">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="ab1aa-133">Obter canal do membro</span><span class="sxs-lookup"><span data-stu-id="ab1aa-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="ab1aa-134">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ab1aa-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ab1aa-135">Obtenha um membro em um canal.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="ab1aa-136">Atualizar a função do membro do canal</span><span class="sxs-lookup"><span data-stu-id="ab1aa-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="ab1aa-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ab1aa-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="ab1aa-138">Atualize as propriedades de um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="ab1aa-139">Suportado só para o canal com MembershipType de`private`.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="ab1aa-140">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="ab1aa-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="ab1aa-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab1aa-141">None</span></span> | <span data-ttu-id="ab1aa-142">Exclua um membro de um canal.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-142">Delete a member from a channel.</span></span> <span data-ttu-id="ab1aa-143">Suportado só com o `channelType` de `private`.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab1aa-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab1aa-144">Properties</span></span>

| <span data-ttu-id="ab1aa-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab1aa-145">Property</span></span>   | <span data-ttu-id="ab1aa-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab1aa-146">Type</span></span> |<span data-ttu-id="ab1aa-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab1aa-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab1aa-148">id</span><span class="sxs-lookup"><span data-stu-id="ab1aa-148">id</span></span>|<span data-ttu-id="ab1aa-149">String</span><span class="sxs-lookup"><span data-stu-id="ab1aa-149">String</span></span>| <span data-ttu-id="ab1aa-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-150">Read-only.</span></span> <span data-ttu-id="ab1aa-151">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="ab1aa-152">displayName</span><span class="sxs-lookup"><span data-stu-id="ab1aa-152">displayName</span></span>| <span data-ttu-id="ab1aa-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab1aa-153">string</span></span> | <span data-ttu-id="ab1aa-154">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-154">The display name of the user.</span></span> |
|<span data-ttu-id="ab1aa-155">funções</span><span class="sxs-lookup"><span data-stu-id="ab1aa-155">roles</span></span>| <span data-ttu-id="ab1aa-156">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab1aa-156">string collection</span></span> | <span data-ttu-id="ab1aa-157">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-157">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab1aa-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab1aa-158">JSON representation</span></span>

<span data-ttu-id="ab1aa-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab1aa-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
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

