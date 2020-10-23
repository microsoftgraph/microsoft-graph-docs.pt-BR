---
title: tipo de recurso conversationMember
description: Representa o usuário em uma conversa.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 970e64ff358654aafee5b47a229a8425fdc69c9e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725831"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="fa2aa-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="fa2aa-103">conversationMember resource type</span></span>

<span data-ttu-id="fa2aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa2aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa2aa-105">Representa um usuário em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="fa2aa-105">Represents a user in a [team](team.md).</span></span>
<span data-ttu-id="fa2aa-106">Confira também [aadUserConversationMember](aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="fa2aa-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fa2aa-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fa2aa-107">Methods</span></span>

| <span data-ttu-id="fa2aa-108">Método</span><span class="sxs-lookup"><span data-stu-id="fa2aa-108">Method</span></span>       | <span data-ttu-id="fa2aa-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fa2aa-109">Return Type</span></span>  |<span data-ttu-id="fa2aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa2aa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa2aa-111">Listar membros</span><span class="sxs-lookup"><span data-stu-id="fa2aa-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="fa2aa-112">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="fa2aa-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="fa2aa-113">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="fa2aa-114">Obter membro</span><span class="sxs-lookup"><span data-stu-id="fa2aa-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="fa2aa-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fa2aa-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="fa2aa-116">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="fa2aa-117">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="fa2aa-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="fa2aa-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fa2aa-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="fa2aa-119">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="fa2aa-120">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="fa2aa-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="fa2aa-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fa2aa-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="fa2aa-122">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="fa2aa-123">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="fa2aa-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="fa2aa-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="fa2aa-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="fa2aa-125">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa2aa-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa2aa-126">Properties</span></span>

| <span data-ttu-id="fa2aa-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa2aa-127">Property</span></span>   | <span data-ttu-id="fa2aa-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa2aa-128">Type</span></span> |<span data-ttu-id="fa2aa-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa2aa-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa2aa-130">id</span><span class="sxs-lookup"><span data-stu-id="fa2aa-130">id</span></span>|<span data-ttu-id="fa2aa-131">String</span><span class="sxs-lookup"><span data-stu-id="fa2aa-131">String</span></span>| <span data-ttu-id="fa2aa-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-132">Read-only.</span></span> <span data-ttu-id="fa2aa-133">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="fa2aa-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fa2aa-134">displayName</span></span>| <span data-ttu-id="fa2aa-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa2aa-135">string</span></span> | <span data-ttu-id="fa2aa-136">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-136">The display name of the user.</span></span> |
|<span data-ttu-id="fa2aa-137">funções</span><span class="sxs-lookup"><span data-stu-id="fa2aa-137">roles</span></span>| <span data-ttu-id="fa2aa-138">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa2aa-138">string collection</span></span> | <span data-ttu-id="fa2aa-139">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-139">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa2aa-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa2aa-140">JSON representation</span></span>

<span data-ttu-id="fa2aa-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa2aa-141">The following is a JSON representation of the resource.</span></span>

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

