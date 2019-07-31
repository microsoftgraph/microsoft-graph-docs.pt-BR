---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário em uma conversa.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c4e937d88a1e504c6774b2dcb657dee443d54843
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013630"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="1eeb1-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="1eeb1-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eeb1-104">Representa um usuário do Azure Active Directory em um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="1eeb1-104">Represents an Azure Active Directory user in a [chat](chat.md).</span></span> <span data-ttu-id="1eeb1-105">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="1eeb1-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1eeb1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1eeb1-106">Methods</span></span>

| <span data-ttu-id="1eeb1-107">Método</span><span class="sxs-lookup"><span data-stu-id="1eeb1-107">Method</span></span>       | <span data-ttu-id="1eeb1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1eeb1-108">Return Type</span></span>  |<span data-ttu-id="1eeb1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eeb1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1eeb1-110">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="1eeb1-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="1eeb1-111">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="1eeb1-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="1eeb1-112">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="1eeb1-113">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="1eeb1-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="1eeb1-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="1eeb1-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="1eeb1-115">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-115">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="1eeb1-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1eeb1-116">Properties</span></span>
| <span data-ttu-id="1eeb1-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1eeb1-117">Property</span></span>     | <span data-ttu-id="1eeb1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1eeb1-118">Type</span></span>   |<span data-ttu-id="1eeb1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eeb1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1eeb1-120">id</span><span class="sxs-lookup"><span data-stu-id="1eeb1-120">id</span></span>|<span data-ttu-id="1eeb1-121">String</span><span class="sxs-lookup"><span data-stu-id="1eeb1-121">String</span></span>| <span data-ttu-id="1eeb1-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-122">Read-only.</span></span> <span data-ttu-id="1eeb1-123">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-123">Unique ID of the message.</span></span>|
|<span data-ttu-id="1eeb1-124">displayName</span><span class="sxs-lookup"><span data-stu-id="1eeb1-124">displayName</span></span>| <span data-ttu-id="1eeb1-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeb1-125">string</span></span> | <span data-ttu-id="1eeb1-126">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-126">The display name of the user.</span></span> |
|<span data-ttu-id="1eeb1-127">funções</span><span class="sxs-lookup"><span data-stu-id="1eeb1-127">roles</span></span>| <span data-ttu-id="1eeb1-128">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeb1-128">string collection</span></span> | <span data-ttu-id="1eeb1-129">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-129">The roles for that user.</span></span> |
|<span data-ttu-id="1eeb1-130">userId</span><span class="sxs-lookup"><span data-stu-id="1eeb1-130">userId</span></span>| <span data-ttu-id="1eeb1-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeb1-131">string</span></span> | <span data-ttu-id="1eeb1-132">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-132">The guid of the user.</span></span> |
|<span data-ttu-id="1eeb1-133">email</span><span class="sxs-lookup"><span data-stu-id="1eeb1-133">email</span></span>| <span data-ttu-id="1eeb1-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeb1-134">string</span></span>  | <span data-ttu-id="1eeb1-135">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-135">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1eeb1-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1eeb1-136">JSON representation</span></span>

<span data-ttu-id="1eeb1-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1eeb1-137">The following is a JSON representation of the resource.</span></span>

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
