---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9e20a1aa0ef42f41a3fc300f804bb5477b5fe1cb
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633696"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="fccc0-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="fccc0-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fccc0-104">Representa um usuário em um [bate-papo](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="fccc0-104">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fccc0-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fccc0-105">Methods</span></span>

| <span data-ttu-id="fccc0-106">Método</span><span class="sxs-lookup"><span data-stu-id="fccc0-106">Method</span></span>       | <span data-ttu-id="fccc0-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fccc0-107">Return Type</span></span>  |<span data-ttu-id="fccc0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fccc0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fccc0-109">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="fccc0-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="fccc0-110">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="fccc0-110">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="fccc0-111">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="fccc0-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="fccc0-112">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="fccc0-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="fccc0-113">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fccc0-113">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="fccc0-114">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="fccc0-114">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="fccc0-115">Listar membros</span><span class="sxs-lookup"><span data-stu-id="fccc0-115">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="fccc0-116">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="fccc0-116">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="fccc0-117">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="fccc0-117">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="fccc0-118">Obter membro</span><span class="sxs-lookup"><span data-stu-id="fccc0-118">Get member groups</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="fccc0-119">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fccc0-119">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="fccc0-120">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="fccc0-120">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="fccc0-121">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="fccc0-121">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="fccc0-122">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fccc0-122">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="fccc0-123">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="fccc0-123">Add a member to a class.</span></span>|
|[<span data-ttu-id="fccc0-124">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="fccc0-124">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="fccc0-125">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fccc0-125">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="fccc0-126">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="fccc0-126">Update a member in the channel.</span></span>|
|[<span data-ttu-id="fccc0-127">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="fccc0-127">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="fccc0-128">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fccc0-128">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="fccc0-129">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="fccc0-129">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="fccc0-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fccc0-130">Properties</span></span>

| <span data-ttu-id="fccc0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fccc0-131">Property</span></span>   | <span data-ttu-id="fccc0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="fccc0-132">Type</span></span> |<span data-ttu-id="fccc0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fccc0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fccc0-134">id</span><span class="sxs-lookup"><span data-stu-id="fccc0-134">id</span></span>|<span data-ttu-id="fccc0-135">String</span><span class="sxs-lookup"><span data-stu-id="fccc0-135">String</span></span>| <span data-ttu-id="fccc0-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fccc0-136">Read-only.</span></span> <span data-ttu-id="fccc0-137">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="fccc0-137">Unique ID of the message.</span></span>|
|<span data-ttu-id="fccc0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="fccc0-138">displayName</span></span>| <span data-ttu-id="fccc0-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fccc0-139">string</span></span> | <span data-ttu-id="fccc0-140">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="fccc0-140">The display name of the user.</span></span> |
|<span data-ttu-id="fccc0-141">funções</span><span class="sxs-lookup"><span data-stu-id="fccc0-141">roles</span></span>| <span data-ttu-id="fccc0-142">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fccc0-142">string collection</span></span> | <span data-ttu-id="fccc0-143">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="fccc0-143">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fccc0-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fccc0-144">JSON representation</span></span>

<span data-ttu-id="fccc0-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fccc0-145">The following is a JSON representation of the resource.</span></span>

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
