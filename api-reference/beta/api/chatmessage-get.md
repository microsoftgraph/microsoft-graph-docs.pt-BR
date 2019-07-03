---
title: Obter chat
description: Recupere as propriedades e os relacionamentos de um objeto chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c01b7e77fc7ef121c4c050e541c9b4a5f7b0da1d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437828"
---
# <a name="get-chatmessage"></a><span data-ttu-id="c3ee4-103">Obter chat</span><span class="sxs-lookup"><span data-stu-id="c3ee4-103">Get chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3ee4-104">Recupere as propriedades e os relacionamentos de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="c3ee4-104">Retrieve the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3ee4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3ee4-105">Permissions</span></span>

<span data-ttu-id="c3ee4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3ee4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3ee4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3ee4-108">Permission type</span></span>                        | <span data-ttu-id="c3ee4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3ee4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c3ee4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3ee4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3ee4-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3ee4-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="c3ee4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3ee4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3ee4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3ee4-113">Not supported.</span></span> |
| <span data-ttu-id="c3ee4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3ee4-114">Application</span></span>                            | <span data-ttu-id="c3ee4-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3ee4-115">Chat.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3ee4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3ee4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3ee4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c3ee4-117">Optional query parameters</span></span>

<span data-ttu-id="c3ee4-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c3ee4-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3ee4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3ee4-119">Request headers</span></span>

| <span data-ttu-id="c3ee4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c3ee4-120">Name</span></span>      |<span data-ttu-id="c3ee4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3ee4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3ee4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3ee4-122">Authorization</span></span> | <span data-ttu-id="c3ee4-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c3ee4-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3ee4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3ee4-124">Request body</span></span>

<span data-ttu-id="c3ee4-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3ee4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3ee4-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3ee4-126">Response</span></span>

<span data-ttu-id="c3ee4-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [chat](../resources/chatmessage.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3ee4-127">If successful, this method returns a `200 OK` response code and the requested [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3ee4-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3ee4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3ee4-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3ee4-129">Request</span></span>

<span data-ttu-id="c3ee4-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3ee4-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3ee4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3ee4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessage"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3ee4-132">C#</span><span class="sxs-lookup"><span data-stu-id="c3ee4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3ee4-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3ee4-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3ee4-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c3ee4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3ee4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3ee4-135">Response</span></span>

<span data-ttu-id="c3ee4-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c3ee4-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c3ee4-137">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c3ee4-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c3ee4-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3ee4-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": {
      "id": "id-value",
      "displayName": "displayName-value"
    },
    "device": {
      "id": "id-value",
      "displayName": "displayName-value"
    },
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "etag": "etag-value",
  "messageType": "messageType-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
