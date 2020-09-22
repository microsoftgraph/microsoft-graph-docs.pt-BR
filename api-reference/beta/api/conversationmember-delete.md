---
title: Excluir conversationMember
description: Excluir um conversationMember de um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 85fd03831620e338af4dc9ab363fcb9e34fbf971
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002755"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="70860-103">Excluir conversationMember</span><span class="sxs-lookup"><span data-stu-id="70860-103">Delete conversationMember</span></span>

<span data-ttu-id="70860-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70860-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70860-105">Excluir um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="70860-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="70860-106">Essa operação só é suportada em canais com [channelMembershipType](../resources/enums.md#channelmembershiptype-values) de `private` .</span><span class="sxs-lookup"><span data-stu-id="70860-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="70860-107">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="70860-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="70860-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="70860-108">Permissions</span></span>

<span data-ttu-id="70860-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70860-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70860-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70860-111">Permission Type</span></span>|<span data-ttu-id="70860-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70860-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="70860-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70860-113">Delegated (work or school account)</span></span>| <span data-ttu-id="70860-114">ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="70860-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="70860-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70860-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70860-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70860-116">Not supported.</span></span>|
|<span data-ttu-id="70860-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70860-117">Application</span></span>| <span data-ttu-id="70860-118">ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="70860-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70860-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70860-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70860-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70860-120">Request headers</span></span>

| <span data-ttu-id="70860-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70860-121">Header</span></span>       | <span data-ttu-id="70860-122">Valor</span><span class="sxs-lookup"><span data-stu-id="70860-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70860-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70860-123">Authorization</span></span>  | <span data-ttu-id="70860-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70860-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70860-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70860-126">Request body</span></span>

<span data-ttu-id="70860-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70860-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70860-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="70860-128">Response</span></span>

<span data-ttu-id="70860-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="70860-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="70860-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70860-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="70860-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70860-131">Request</span></span>

<span data-ttu-id="70860-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70860-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70860-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="70860-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="70860-134">C#</span><span class="sxs-lookup"><span data-stu-id="70860-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70860-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70860-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70860-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70860-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70860-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="70860-137">Response</span></span>

<span data-ttu-id="70860-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70860-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


