---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca5115922dfb40239b8ca290a39f3c5953d4e4ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973972"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="1140d-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="1140d-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1140d-104">Representa um usuário em um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="1140d-104">Represents a user in a [chat](chat.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1140d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1140d-105">Methods</span></span>

| <span data-ttu-id="1140d-106">Método</span><span class="sxs-lookup"><span data-stu-id="1140d-106">Method</span></span>       | <span data-ttu-id="1140d-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1140d-107">Return Type</span></span>  |<span data-ttu-id="1140d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1140d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1140d-109">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="1140d-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="1140d-110">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="1140d-110">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="1140d-111">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1140d-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="1140d-112">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="1140d-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="1140d-113">conversationmember</span><span class="sxs-lookup"><span data-stu-id="1140d-113">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="1140d-114">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1140d-114">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="1140d-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1140d-115">Properties</span></span>

| <span data-ttu-id="1140d-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1140d-116">Property</span></span>     | <span data-ttu-id="1140d-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="1140d-117">Type</span></span>   |<span data-ttu-id="1140d-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1140d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1140d-119">id</span><span class="sxs-lookup"><span data-stu-id="1140d-119">id</span></span>|<span data-ttu-id="1140d-120">String</span><span class="sxs-lookup"><span data-stu-id="1140d-120">String</span></span>| <span data-ttu-id="1140d-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1140d-121">Read-only.</span></span> <span data-ttu-id="1140d-122">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1140d-122">Unique ID of the message.</span></span>|
|<span data-ttu-id="1140d-123">displayName</span><span class="sxs-lookup"><span data-stu-id="1140d-123">displayName</span></span>| <span data-ttu-id="1140d-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1140d-124">string</span></span> | <span data-ttu-id="1140d-125">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="1140d-125">The display name of the user.</span></span> |
|<span data-ttu-id="1140d-126">funções</span><span class="sxs-lookup"><span data-stu-id="1140d-126">roles</span></span>| <span data-ttu-id="1140d-127">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1140d-127">string collection</span></span> | <span data-ttu-id="1140d-128">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="1140d-128">The roles for that user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1140d-129">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="1140d-129">Relationships</span></span>

<span data-ttu-id="1140d-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1140d-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1140d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1140d-131">JSON representation</span></span>

<span data-ttu-id="1140d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1140d-132">The following is a JSON representation of the resource.</span></span>

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