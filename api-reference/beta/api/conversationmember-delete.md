---
title: Excluir conversationMember
description: Excluir um conversationMember de um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0774b2c214191949857444ae7d6673bd2b49bade
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288554"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="39613-103">Excluir conversationMember</span><span class="sxs-lookup"><span data-stu-id="39613-103">Delete conversationMember</span></span>

<span data-ttu-id="39613-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39613-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39613-105">Excluir um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="39613-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="39613-106">Essa operação só é suportada em canais com [channelMembershipType](../resources/enums.md#channelmembershiptype-values) de `private` .</span><span class="sxs-lookup"><span data-stu-id="39613-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="39613-107">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="39613-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="39613-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="39613-108">Permissions</span></span>

<span data-ttu-id="39613-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39613-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39613-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39613-111">Permission Type</span></span>|<span data-ttu-id="39613-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39613-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="39613-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39613-113">Delegated (work or school account)</span></span>| <span data-ttu-id="39613-114">ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="39613-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="39613-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39613-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39613-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39613-116">Not supported.</span></span>|
|<span data-ttu-id="39613-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39613-117">Application</span></span>| <span data-ttu-id="39613-118">Member. ReadWrite. Group ([RSC](https://aka.ms/teams-rsc)), ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="39613-118">Member.ReadWrite.Group ([RSC](https://aka.ms/teams-rsc)), ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39613-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39613-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="39613-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39613-120">Request headers</span></span>

| <span data-ttu-id="39613-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39613-121">Header</span></span>       | <span data-ttu-id="39613-122">Valor</span><span class="sxs-lookup"><span data-stu-id="39613-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="39613-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="39613-123">Authorization</span></span>  | <span data-ttu-id="39613-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39613-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39613-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39613-126">Request body</span></span>

<span data-ttu-id="39613-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39613-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39613-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="39613-128">Response</span></span>

<span data-ttu-id="39613-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="39613-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="39613-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39613-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="39613-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39613-131">Request</span></span>

<span data-ttu-id="39613-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39613-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39613-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="39613-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="39613-134">C#</span><span class="sxs-lookup"><span data-stu-id="39613-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39613-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39613-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39613-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39613-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="39613-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="39613-137">Response</span></span>

<span data-ttu-id="39613-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39613-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
