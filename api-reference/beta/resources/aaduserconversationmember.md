---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário em uma conversa.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: fd326482869d9f72778edc9d4c55996f7aa59045
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236458"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="db317-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="db317-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db317-104">Representa um usuário do Azure Active Directory em um [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="db317-104">Represents an Azure Active Directory user in a [chat](chat.md).</span></span> <span data-ttu-id="db317-105">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="db317-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="db317-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="db317-106">Methods</span></span>

| <span data-ttu-id="db317-107">Método</span><span class="sxs-lookup"><span data-stu-id="db317-107">Method</span></span>       | <span data-ttu-id="db317-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="db317-108">Return Type</span></span>  |<span data-ttu-id="db317-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="db317-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db317-110">Listar membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="db317-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="db317-111">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="db317-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="db317-112">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="db317-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="db317-113">Obter membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="db317-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="db317-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="db317-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="db317-115">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="db317-115">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="db317-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db317-116">Properties</span></span>
| <span data-ttu-id="db317-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db317-117">Property</span></span>     | <span data-ttu-id="db317-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="db317-118">Type</span></span>   |<span data-ttu-id="db317-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="db317-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db317-120">id</span><span class="sxs-lookup"><span data-stu-id="db317-120">id</span></span>|<span data-ttu-id="db317-121">String</span><span class="sxs-lookup"><span data-stu-id="db317-121">String</span></span>| <span data-ttu-id="db317-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db317-122">Read-only.</span></span> <span data-ttu-id="db317-123">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="db317-123">Unique ID of the message.</span></span>|
|<span data-ttu-id="db317-124">displayName</span><span class="sxs-lookup"><span data-stu-id="db317-124">displayName</span></span>| <span data-ttu-id="db317-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db317-125">string</span></span> | <span data-ttu-id="db317-126">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="db317-126">The display name of the user.</span></span> |
|<span data-ttu-id="db317-127">funções</span><span class="sxs-lookup"><span data-stu-id="db317-127">roles</span></span>| <span data-ttu-id="db317-128">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db317-128">string collection</span></span> | <span data-ttu-id="db317-129">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="db317-129">The roles for that user.</span></span> |
|<span data-ttu-id="db317-130">userId</span><span class="sxs-lookup"><span data-stu-id="db317-130">userId</span></span>| <span data-ttu-id="db317-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db317-131">string</span></span> | <span data-ttu-id="db317-132">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="db317-132">The guid of the user.</span></span> |
|<span data-ttu-id="db317-133">email</span><span class="sxs-lookup"><span data-stu-id="db317-133">email</span></span>| <span data-ttu-id="db317-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db317-134">string</span></span>  | <span data-ttu-id="db317-135">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="db317-135">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db317-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db317-136">JSON representation</span></span>

<span data-ttu-id="db317-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db317-137">The following is a JSON representation of the resource.</span></span>

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
