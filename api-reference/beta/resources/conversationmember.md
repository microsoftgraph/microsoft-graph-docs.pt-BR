---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f6908106390e527ab4e33e777dd232b58ead727a
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379266"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="377a4-103">tipo de recurso conversationMember</span><span class="sxs-lookup"><span data-stu-id="377a4-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="377a4-104">Representa um usuário em um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="377a4-104">Represents a user in a [chat](chat.md).</span></span>

## <a name="methods"></a><span data-ttu-id="377a4-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="377a4-105">Methods</span></span>

| <span data-ttu-id="377a4-106">Método</span><span class="sxs-lookup"><span data-stu-id="377a4-106">Method</span></span>       | <span data-ttu-id="377a4-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="377a4-107">Return Type</span></span>  |<span data-ttu-id="377a4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="377a4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="377a4-109">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="377a4-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="377a4-110">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="377a4-110">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="377a4-111">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="377a4-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="377a4-112">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="377a4-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="377a4-113">conversationmember</span><span class="sxs-lookup"><span data-stu-id="377a4-113">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="377a4-114">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="377a4-114">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="377a4-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="377a4-115">Properties</span></span>
| <span data-ttu-id="377a4-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="377a4-116">Property</span></span>     | <span data-ttu-id="377a4-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="377a4-117">Type</span></span>   |<span data-ttu-id="377a4-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="377a4-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="377a4-119">id</span><span class="sxs-lookup"><span data-stu-id="377a4-119">id</span></span>|<span data-ttu-id="377a4-120">String</span><span class="sxs-lookup"><span data-stu-id="377a4-120">String</span></span>| <span data-ttu-id="377a4-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="377a4-121">Read-only.</span></span> <span data-ttu-id="377a4-122">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="377a4-122">Unique ID of the message.</span></span>|
|<span data-ttu-id="377a4-123">displayName</span><span class="sxs-lookup"><span data-stu-id="377a4-123">displayName</span></span>| <span data-ttu-id="377a4-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="377a4-124">string</span></span> | <span data-ttu-id="377a4-125">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="377a4-125">The display name of the user.</span></span> |
|<span data-ttu-id="377a4-126">funções</span><span class="sxs-lookup"><span data-stu-id="377a4-126">roles</span></span>| <span data-ttu-id="377a4-127">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="377a4-127">string collection</span></span> | <span data-ttu-id="377a4-128">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="377a4-128">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="377a4-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="377a4-129">JSON representation</span></span>

<span data-ttu-id="377a4-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="377a4-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"]
}

```

## <a name="see-also"></a><span data-ttu-id="377a4-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="377a4-131">See Also</span></span>

[<span data-ttu-id="377a4-132">aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="377a4-132">aadUserConversationMember</span></span>](aaduserconversationmember.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
