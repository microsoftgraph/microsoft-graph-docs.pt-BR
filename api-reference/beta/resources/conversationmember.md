---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9e50c0ca27843461b41b4d86f29ce3604788866
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016762"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="7188a-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="7188a-103">conversationMember resource type</span></span>

<span data-ttu-id="7188a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7188a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7188a-105">Representa um usuário em um [bate-papo](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="7188a-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="7188a-106">Confira também [aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="7188a-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7188a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7188a-107">Methods</span></span>

| <span data-ttu-id="7188a-108">Método</span><span class="sxs-lookup"><span data-stu-id="7188a-108">Method</span></span>       | <span data-ttu-id="7188a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7188a-109">Return Type</span></span>  |<span data-ttu-id="7188a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7188a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7188a-111">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="7188a-111">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="7188a-112">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="7188a-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="7188a-113">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="7188a-113">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="7188a-114">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="7188a-114">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="7188a-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="7188a-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="7188a-116">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="7188a-116">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="7188a-117">Listar membros</span><span class="sxs-lookup"><span data-stu-id="7188a-117">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="7188a-118">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="7188a-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="7188a-119">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="7188a-119">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="7188a-120">Obter membro</span><span class="sxs-lookup"><span data-stu-id="7188a-120">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="7188a-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="7188a-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="7188a-122">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="7188a-122">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="7188a-123">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="7188a-123">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="7188a-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="7188a-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="7188a-125">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="7188a-125">Add a member to a channel.</span></span>|
|[<span data-ttu-id="7188a-126">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="7188a-126">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="7188a-127">conversationMember</span><span class="sxs-lookup"><span data-stu-id="7188a-127">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="7188a-128">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="7188a-128">Update a member in the channel.</span></span>|
|[<span data-ttu-id="7188a-129">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="7188a-129">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="7188a-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="7188a-130">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="7188a-131">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="7188a-131">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="7188a-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7188a-132">Properties</span></span>

| <span data-ttu-id="7188a-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7188a-133">Property</span></span>   | <span data-ttu-id="7188a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7188a-134">Type</span></span> |<span data-ttu-id="7188a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7188a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7188a-136">id</span><span class="sxs-lookup"><span data-stu-id="7188a-136">id</span></span>|<span data-ttu-id="7188a-137">String</span><span class="sxs-lookup"><span data-stu-id="7188a-137">String</span></span>| <span data-ttu-id="7188a-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7188a-138">Read-only.</span></span> <span data-ttu-id="7188a-139">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="7188a-139">Unique ID of the user.</span></span>|
|<span data-ttu-id="7188a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7188a-140">displayName</span></span>| <span data-ttu-id="7188a-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7188a-141">string</span></span> | <span data-ttu-id="7188a-142">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="7188a-142">The display name of the user.</span></span> |
|<span data-ttu-id="7188a-143">funções</span><span class="sxs-lookup"><span data-stu-id="7188a-143">roles</span></span>| <span data-ttu-id="7188a-144">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7188a-144">string collection</span></span> | <span data-ttu-id="7188a-145">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="7188a-145">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7188a-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7188a-146">JSON representation</span></span>

<span data-ttu-id="7188a-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7188a-147">The following is a JSON representation of the resource.</span></span>

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


