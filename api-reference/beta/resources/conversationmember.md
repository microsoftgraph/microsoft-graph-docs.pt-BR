---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 796bbe9f64342f97a9ae18363fdc01dc1712d015
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507398"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="dc973-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc973-103">conversationMember resource type</span></span>

<span data-ttu-id="dc973-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dc973-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc973-105">Representa um usuário em um [bate-papo](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="dc973-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dc973-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dc973-106">Methods</span></span>

| <span data-ttu-id="dc973-107">Método</span><span class="sxs-lookup"><span data-stu-id="dc973-107">Method</span></span>       | <span data-ttu-id="dc973-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dc973-108">Return Type</span></span>  |<span data-ttu-id="dc973-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc973-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc973-110">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="dc973-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="dc973-111">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="dc973-111">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="dc973-112">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="dc973-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="dc973-113">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="dc973-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="dc973-114">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc973-114">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="dc973-115">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="dc973-115">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="dc973-116">Listar membros</span><span class="sxs-lookup"><span data-stu-id="dc973-116">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="dc973-117">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="dc973-117">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="dc973-118">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="dc973-118">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="dc973-119">Obter membro</span><span class="sxs-lookup"><span data-stu-id="dc973-119">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="dc973-120">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc973-120">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="dc973-121">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="dc973-121">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="dc973-122">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="dc973-122">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="dc973-123">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc973-123">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="dc973-124">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="dc973-124">Add a member to a channel.</span></span>|
|[<span data-ttu-id="dc973-125">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="dc973-125">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="dc973-126">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc973-126">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="dc973-127">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="dc973-127">Update a member in the channel.</span></span>|
|[<span data-ttu-id="dc973-128">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="dc973-128">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="dc973-129">conversationMember</span><span class="sxs-lookup"><span data-stu-id="dc973-129">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="dc973-130">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="dc973-130">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc973-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc973-131">Properties</span></span>

| <span data-ttu-id="dc973-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc973-132">Property</span></span>   | <span data-ttu-id="dc973-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc973-133">Type</span></span> |<span data-ttu-id="dc973-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc973-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc973-135">id</span><span class="sxs-lookup"><span data-stu-id="dc973-135">id</span></span>|<span data-ttu-id="dc973-136">String</span><span class="sxs-lookup"><span data-stu-id="dc973-136">String</span></span>| <span data-ttu-id="dc973-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc973-137">Read-only.</span></span> <span data-ttu-id="dc973-138">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="dc973-138">Unique ID of the user.</span></span>|
|<span data-ttu-id="dc973-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dc973-139">displayName</span></span>| <span data-ttu-id="dc973-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc973-140">string</span></span> | <span data-ttu-id="dc973-141">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="dc973-141">The display name of the user.</span></span> |
|<span data-ttu-id="dc973-142">funções</span><span class="sxs-lookup"><span data-stu-id="dc973-142">roles</span></span>| <span data-ttu-id="dc973-143">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc973-143">string collection</span></span> | <span data-ttu-id="dc973-144">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="dc973-144">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dc973-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc973-145">JSON representation</span></span>

<span data-ttu-id="dc973-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc973-146">The following is a JSON representation of the resource.</span></span>

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
