---
title: Excluir conversationMember
description: Excluir um conversationMember de um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dee9dfbe5e77dba544517bbfdd277c25f85f4846
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491270"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="c7817-103">Excluir conversationMember</span><span class="sxs-lookup"><span data-stu-id="c7817-103">Delete conversationMember</span></span>

<span data-ttu-id="c7817-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7817-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7817-105">Excluir um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="c7817-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="c7817-106">Essa operação só é suportada em canais com [channelMembershipType](../resources/enums.md#channelmembershiptype-values) de `private` .</span><span class="sxs-lookup"><span data-stu-id="c7817-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="c7817-107">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="c7817-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7817-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7817-108">Permissions</span></span>

<span data-ttu-id="c7817-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7817-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7817-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7817-111">Permission Type</span></span>|<span data-ttu-id="c7817-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7817-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c7817-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7817-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c7817-114">ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c7817-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="c7817-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7817-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7817-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7817-116">Not supported.</span></span>|
|<span data-ttu-id="c7817-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7817-117">Application</span></span>| <span data-ttu-id="c7817-118">ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c7817-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7817-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7817-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c7817-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7817-120">Request headers</span></span>

| <span data-ttu-id="c7817-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7817-121">Header</span></span>       | <span data-ttu-id="c7817-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7817-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7817-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7817-123">Authorization</span></span>  | <span data-ttu-id="c7817-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7817-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7817-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7817-126">Request body</span></span>

<span data-ttu-id="c7817-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7817-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7817-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7817-128">Response</span></span>

<span data-ttu-id="c7817-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c7817-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c7817-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7817-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7817-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7817-131">Request</span></span>

<span data-ttu-id="c7817-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7817-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7817-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7817-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="c7817-134">C#</span><span class="sxs-lookup"><span data-stu-id="c7817-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7817-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7817-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7817-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7817-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7817-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7817-137">Response</span></span>

<span data-ttu-id="c7817-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7817-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
