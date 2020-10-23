---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6057c8cf71ce0f8d71632267d3790c39b69b1eb1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735761"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="4471d-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="4471d-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="4471d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4471d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4471d-105">Representa um usuário do Azure Active Directory em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="4471d-105">Represents an Azure Active Directory user in a [team](team.md).</span></span>
<span data-ttu-id="4471d-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="4471d-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4471d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4471d-107">Methods</span></span>

| <span data-ttu-id="4471d-108">Método</span><span class="sxs-lookup"><span data-stu-id="4471d-108">Method</span></span>       | <span data-ttu-id="4471d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4471d-109">Return Type</span></span>  |<span data-ttu-id="4471d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4471d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4471d-111">Listar membros</span><span class="sxs-lookup"><span data-stu-id="4471d-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="4471d-112">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4471d-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4471d-113">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="4471d-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="4471d-114">Obter membro</span><span class="sxs-lookup"><span data-stu-id="4471d-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="4471d-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4471d-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="4471d-116">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="4471d-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="4471d-117">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="4471d-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="4471d-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4471d-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="4471d-119">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="4471d-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="4471d-120">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="4471d-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="4471d-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4471d-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="4471d-122">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="4471d-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="4471d-123">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="4471d-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="4471d-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4471d-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="4471d-125">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="4471d-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="4471d-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4471d-126">Properties</span></span>

| <span data-ttu-id="4471d-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4471d-127">Property</span></span>   | <span data-ttu-id="4471d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="4471d-128">Type</span></span> |<span data-ttu-id="4471d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="4471d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4471d-130">id</span><span class="sxs-lookup"><span data-stu-id="4471d-130">id</span></span>|<span data-ttu-id="4471d-131">String</span><span class="sxs-lookup"><span data-stu-id="4471d-131">String</span></span>| <span data-ttu-id="4471d-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4471d-132">Read-only.</span></span> <span data-ttu-id="4471d-133">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="4471d-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="4471d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4471d-134">displayName</span></span>| <span data-ttu-id="4471d-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4471d-135">string</span></span> | <span data-ttu-id="4471d-136">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="4471d-136">The display name of the user.</span></span> |
|<span data-ttu-id="4471d-137">funções</span><span class="sxs-lookup"><span data-stu-id="4471d-137">roles</span></span>| <span data-ttu-id="4471d-138">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4471d-138">string collection</span></span> | <span data-ttu-id="4471d-139">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="4471d-139">The roles for that user.</span></span> |
|<span data-ttu-id="4471d-140">userId</span><span class="sxs-lookup"><span data-stu-id="4471d-140">userId</span></span>| <span data-ttu-id="4471d-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4471d-141">string</span></span> | <span data-ttu-id="4471d-142">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="4471d-142">The guid of the user.</span></span> |
|<span data-ttu-id="4471d-143">email</span><span class="sxs-lookup"><span data-stu-id="4471d-143">email</span></span>| <span data-ttu-id="4471d-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4471d-144">string</span></span>  | <span data-ttu-id="4471d-145">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="4471d-145">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4471d-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4471d-146">JSON representation</span></span>

<span data-ttu-id="4471d-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4471d-147">The following is a JSON representation of the resource.</span></span>

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

