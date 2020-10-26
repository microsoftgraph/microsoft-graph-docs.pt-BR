---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3828871d1e5edaae067b7c9635908f061282ca1f
ms.sourcegitcommit: ab578b062c534db57844490f35e802df8a8f4dfa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2020
ms.locfileid: "48753371"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="c3439-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="c3439-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="c3439-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3439-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3439-105">Representa um usuário do Azure Active Directory em um [chat](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="c3439-105">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="c3439-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="c3439-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c3439-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c3439-107">Methods</span></span>

| <span data-ttu-id="c3439-108">Método</span><span class="sxs-lookup"><span data-stu-id="c3439-108">Method</span></span>       | <span data-ttu-id="c3439-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c3439-109">Return Type</span></span>  |<span data-ttu-id="c3439-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3439-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3439-111">Listar membros</span><span class="sxs-lookup"><span data-stu-id="c3439-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="c3439-112">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c3439-112">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="c3439-113">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="c3439-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="c3439-114">Obter membro</span><span class="sxs-lookup"><span data-stu-id="c3439-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="c3439-115">conversationmember</span><span class="sxs-lookup"><span data-stu-id="c3439-115">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="c3439-116">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="c3439-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="c3439-117">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="c3439-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="c3439-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c3439-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c3439-119">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="c3439-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="c3439-120">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="c3439-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="c3439-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c3439-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c3439-122">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="c3439-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="c3439-123">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="c3439-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="c3439-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c3439-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c3439-125">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="c3439-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3439-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3439-126">Properties</span></span>

| <span data-ttu-id="c3439-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3439-127">Property</span></span>   | <span data-ttu-id="c3439-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3439-128">Type</span></span> |<span data-ttu-id="c3439-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3439-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3439-130">id</span><span class="sxs-lookup"><span data-stu-id="c3439-130">id</span></span>|<span data-ttu-id="c3439-131">String</span><span class="sxs-lookup"><span data-stu-id="c3439-131">String</span></span>| <span data-ttu-id="c3439-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3439-132">Read-only.</span></span> <span data-ttu-id="c3439-133">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3439-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="c3439-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c3439-134">displayName</span></span>| <span data-ttu-id="c3439-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3439-135">string</span></span> | <span data-ttu-id="c3439-136">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3439-136">The display name of the user.</span></span> |
|<span data-ttu-id="c3439-137">funções</span><span class="sxs-lookup"><span data-stu-id="c3439-137">roles</span></span>| <span data-ttu-id="c3439-138">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3439-138">string collection</span></span> | <span data-ttu-id="c3439-139">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="c3439-139">The roles for that user.</span></span> |
|<span data-ttu-id="c3439-140">userId</span><span class="sxs-lookup"><span data-stu-id="c3439-140">userId</span></span>| <span data-ttu-id="c3439-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3439-141">string</span></span> | <span data-ttu-id="c3439-142">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3439-142">The guid of the user.</span></span> |
|<span data-ttu-id="c3439-143">email</span><span class="sxs-lookup"><span data-stu-id="c3439-143">email</span></span>| <span data-ttu-id="c3439-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3439-144">string</span></span>  | <span data-ttu-id="c3439-145">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3439-145">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3439-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3439-146">JSON representation</span></span>

<span data-ttu-id="c3439-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3439-147">The following is a JSON representation of the resource.</span></span>

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


