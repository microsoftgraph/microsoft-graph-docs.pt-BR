---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fe5b7c324a478ef399147a3d12370842ae368632
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081780"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="64f81-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="64f81-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="64f81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f81-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64f81-105">Representa um usuário do Azure Active Directory em um [chat](chat.md) ou [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="64f81-105">Represents an Azure Active Directory user in a [chat](chat.md) or [channel](channel.md).</span></span> <span data-ttu-id="64f81-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="64f81-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="64f81-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="64f81-107">Methods</span></span>

| <span data-ttu-id="64f81-108">Método</span><span class="sxs-lookup"><span data-stu-id="64f81-108">Method</span></span>       | <span data-ttu-id="64f81-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="64f81-109">Return Type</span></span>  |<span data-ttu-id="64f81-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f81-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64f81-111">Listar membros</span><span class="sxs-lookup"><span data-stu-id="64f81-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="64f81-112">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="64f81-112">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="64f81-113">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="64f81-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="64f81-114">Obter membro</span><span class="sxs-lookup"><span data-stu-id="64f81-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="64f81-115">conversationmember</span><span class="sxs-lookup"><span data-stu-id="64f81-115">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="64f81-116">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="64f81-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="64f81-117">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="64f81-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="64f81-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="64f81-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="64f81-119">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="64f81-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="64f81-120">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="64f81-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="64f81-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="64f81-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="64f81-122">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="64f81-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="64f81-123">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="64f81-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="64f81-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="64f81-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="64f81-125">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="64f81-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="64f81-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64f81-126">Properties</span></span>

| <span data-ttu-id="64f81-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64f81-127">Property</span></span>   | <span data-ttu-id="64f81-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="64f81-128">Type</span></span> |<span data-ttu-id="64f81-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f81-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64f81-130">id</span><span class="sxs-lookup"><span data-stu-id="64f81-130">id</span></span>|<span data-ttu-id="64f81-131">String</span><span class="sxs-lookup"><span data-stu-id="64f81-131">String</span></span>| <span data-ttu-id="64f81-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64f81-132">Read-only.</span></span> <span data-ttu-id="64f81-133">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="64f81-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="64f81-134">displayName</span><span class="sxs-lookup"><span data-stu-id="64f81-134">displayName</span></span>| <span data-ttu-id="64f81-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64f81-135">string</span></span> | <span data-ttu-id="64f81-136">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="64f81-136">The display name of the user.</span></span> |
|<span data-ttu-id="64f81-137">funções</span><span class="sxs-lookup"><span data-stu-id="64f81-137">roles</span></span>| <span data-ttu-id="64f81-138">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64f81-138">string collection</span></span> | <span data-ttu-id="64f81-139">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="64f81-139">The roles for that user.</span></span> |
|<span data-ttu-id="64f81-140">userId</span><span class="sxs-lookup"><span data-stu-id="64f81-140">userId</span></span>| <span data-ttu-id="64f81-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64f81-141">string</span></span> | <span data-ttu-id="64f81-142">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="64f81-142">The guid of the user.</span></span> |
|<span data-ttu-id="64f81-143">email</span><span class="sxs-lookup"><span data-stu-id="64f81-143">email</span></span>| <span data-ttu-id="64f81-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64f81-144">string</span></span>  | <span data-ttu-id="64f81-145">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="64f81-145">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64f81-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64f81-146">JSON representation</span></span>

<span data-ttu-id="64f81-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64f81-147">The following is a JSON representation of the resource.</span></span>

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


