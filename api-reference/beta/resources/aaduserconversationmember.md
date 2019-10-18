---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 058164d44ef6d9d6ba6667cf1cb7249bf57c2a83
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633507"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="ed6f0-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="ed6f0-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed6f0-104">Representa um usuário do Azure Active Directory em um [chat](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="ed6f0-104">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="ed6f0-105">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="ed6f0-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ed6f0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed6f0-106">Methods</span></span>

| <span data-ttu-id="ed6f0-107">Método</span><span class="sxs-lookup"><span data-stu-id="ed6f0-107">Method</span></span>       | <span data-ttu-id="ed6f0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed6f0-108">Return Type</span></span>  |<span data-ttu-id="ed6f0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed6f0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed6f0-110">Listar membros</span><span class="sxs-lookup"><span data-stu-id="ed6f0-110">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="ed6f0-111">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="ed6f0-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="ed6f0-112">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-112">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="ed6f0-113">Obter membro</span><span class="sxs-lookup"><span data-stu-id="ed6f0-113">Get member groups</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="ed6f0-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="ed6f0-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="ed6f0-115">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-115">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="ed6f0-116">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="ed6f0-116">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="ed6f0-117">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ed6f0-117">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ed6f0-118">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-118">Add a member to a class.</span></span>|
|[<span data-ttu-id="ed6f0-119">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="ed6f0-119">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="ed6f0-120">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ed6f0-120">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ed6f0-121">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-121">Update a member in the channel.</span></span>|
|[<span data-ttu-id="ed6f0-122">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="ed6f0-122">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="ed6f0-123">conversationMember</span><span class="sxs-lookup"><span data-stu-id="ed6f0-123">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="ed6f0-124">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-124">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed6f0-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed6f0-125">Properties</span></span>

| <span data-ttu-id="ed6f0-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed6f0-126">Property</span></span>   | <span data-ttu-id="ed6f0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed6f0-127">Type</span></span> |<span data-ttu-id="ed6f0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed6f0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed6f0-129">id</span><span class="sxs-lookup"><span data-stu-id="ed6f0-129">id</span></span>|<span data-ttu-id="ed6f0-130">String</span><span class="sxs-lookup"><span data-stu-id="ed6f0-130">String</span></span>| <span data-ttu-id="ed6f0-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-131">Read-only.</span></span> <span data-ttu-id="ed6f0-132">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="ed6f0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ed6f0-133">displayName</span></span>| <span data-ttu-id="ed6f0-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed6f0-134">string</span></span> | <span data-ttu-id="ed6f0-135">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-135">The display name of the user.</span></span> |
|<span data-ttu-id="ed6f0-136">funções</span><span class="sxs-lookup"><span data-stu-id="ed6f0-136">roles</span></span>| <span data-ttu-id="ed6f0-137">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed6f0-137">string collection</span></span> | <span data-ttu-id="ed6f0-138">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-138">The roles for that user.</span></span> |
|<span data-ttu-id="ed6f0-139">userId</span><span class="sxs-lookup"><span data-stu-id="ed6f0-139">userId</span></span>| <span data-ttu-id="ed6f0-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed6f0-140">string</span></span> | <span data-ttu-id="ed6f0-141">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-141">The guid of the user.</span></span> |
|<span data-ttu-id="ed6f0-142">email</span><span class="sxs-lookup"><span data-stu-id="ed6f0-142">email</span></span>| <span data-ttu-id="ed6f0-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed6f0-143">string</span></span>  | <span data-ttu-id="ed6f0-144">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-144">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ed6f0-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed6f0-145">JSON representation</span></span>

<span data-ttu-id="ed6f0-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed6f0-146">The following is a JSON representation of the resource.</span></span>

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
