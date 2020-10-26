---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3dfee039c56d6a5b9d28807b5fe6227dd0ddbfc9
ms.sourcegitcommit: ab578b062c534db57844490f35e802df8a8f4dfa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2020
ms.locfileid: "48753364"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="c175e-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="c175e-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="c175e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c175e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c175e-105">Representa um usuário do Azure Active Directory em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="c175e-105">Represents an Azure Active Directory user in a [team](team.md).</span></span>
<span data-ttu-id="c175e-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="c175e-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c175e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c175e-107">Methods</span></span>

| <span data-ttu-id="c175e-108">Método</span><span class="sxs-lookup"><span data-stu-id="c175e-108">Method</span></span>       | <span data-ttu-id="c175e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c175e-109">Return Type</span></span>  |<span data-ttu-id="c175e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c175e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c175e-111">Listar membros</span><span class="sxs-lookup"><span data-stu-id="c175e-111">List members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="c175e-112">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c175e-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="c175e-113">Ver a lista de todos os usuários no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="c175e-113">Get the list of all users in the chat or channel.</span></span>|
|[<span data-ttu-id="c175e-114">Obter membro</span><span class="sxs-lookup"><span data-stu-id="c175e-114">Get member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="c175e-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c175e-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="c175e-116">Obter um único usuário no chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="c175e-116">Get a single user in the chat or channel.</span></span>|
|[<span data-ttu-id="c175e-117">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="c175e-117">Add member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="c175e-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c175e-118">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c175e-119">Adicionar um membro a um canal.</span><span class="sxs-lookup"><span data-stu-id="c175e-119">Add a member to a channel.</span></span>|
|[<span data-ttu-id="c175e-120">Atualizar membro</span><span class="sxs-lookup"><span data-stu-id="c175e-120">Update member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="c175e-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c175e-121">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c175e-122">Atualizar um membro no canal.</span><span class="sxs-lookup"><span data-stu-id="c175e-122">Update a member in the channel.</span></span>|
|[<span data-ttu-id="c175e-123">Excluir membro</span><span class="sxs-lookup"><span data-stu-id="c175e-123">Delete member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="c175e-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="c175e-124">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="c175e-125">Excluir um membro do canal.</span><span class="sxs-lookup"><span data-stu-id="c175e-125">Delete a member from the channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c175e-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c175e-126">Properties</span></span>

| <span data-ttu-id="c175e-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c175e-127">Property</span></span>   | <span data-ttu-id="c175e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c175e-128">Type</span></span> |<span data-ttu-id="c175e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c175e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c175e-130">id</span><span class="sxs-lookup"><span data-stu-id="c175e-130">id</span></span>|<span data-ttu-id="c175e-131">String</span><span class="sxs-lookup"><span data-stu-id="c175e-131">String</span></span>| <span data-ttu-id="c175e-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c175e-132">Read-only.</span></span> <span data-ttu-id="c175e-133">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c175e-133">Unique ID of the user.</span></span>|
|<span data-ttu-id="c175e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c175e-134">displayName</span></span>| <span data-ttu-id="c175e-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c175e-135">string</span></span> | <span data-ttu-id="c175e-136">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="c175e-136">The display name of the user.</span></span> |
|<span data-ttu-id="c175e-137">funções</span><span class="sxs-lookup"><span data-stu-id="c175e-137">roles</span></span>| <span data-ttu-id="c175e-138">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c175e-138">string collection</span></span> | <span data-ttu-id="c175e-139">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="c175e-139">The roles for that user.</span></span> |
|<span data-ttu-id="c175e-140">userId</span><span class="sxs-lookup"><span data-stu-id="c175e-140">userId</span></span>| <span data-ttu-id="c175e-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c175e-141">string</span></span> | <span data-ttu-id="c175e-142">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="c175e-142">The guid of the user.</span></span> |
|<span data-ttu-id="c175e-143">email</span><span class="sxs-lookup"><span data-stu-id="c175e-143">email</span></span>| <span data-ttu-id="c175e-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c175e-144">string</span></span>  | <span data-ttu-id="c175e-145">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="c175e-145">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c175e-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c175e-146">JSON representation</span></span>

<span data-ttu-id="c175e-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c175e-147">The following is a JSON representation of the resource.</span></span>

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

