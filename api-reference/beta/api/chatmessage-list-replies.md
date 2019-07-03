---
title: Listar respostas
description: Recupere uma lista de objetos chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 44d90dd085a09639467c054dbc2af516d270eb3b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437744"
---
# <a name="list-replies"></a><span data-ttu-id="a5e81-103">Listar respostas</span><span class="sxs-lookup"><span data-stu-id="a5e81-103">List replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5e81-104">Recupere uma lista de objetos chat.</span><span class="sxs-lookup"><span data-stu-id="a5e81-104">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5e81-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5e81-105">Permissions</span></span>

<span data-ttu-id="a5e81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5e81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5e81-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5e81-108">Permission type</span></span>                        | <span data-ttu-id="a5e81-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5e81-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5e81-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5e81-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5e81-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5e81-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="a5e81-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5e81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5e81-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e81-113">Not supported.</span></span> |
| <span data-ttu-id="a5e81-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5e81-114">Application</span></span>                            | <span data-ttu-id="a5e81-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5e81-115">Chat.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5e81-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e81-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
GET /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5e81-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5e81-117">Optional query parameters</span></span>

<span data-ttu-id="a5e81-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e81-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5e81-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e81-119">Request headers</span></span>

| <span data-ttu-id="a5e81-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a5e81-120">Name</span></span>      |<span data-ttu-id="a5e81-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5e81-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5e81-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5e81-122">Authorization</span></span> | <span data-ttu-id="a5e81-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a5e81-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5e81-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e81-124">Request body</span></span>

<span data-ttu-id="a5e81-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5e81-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5e81-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e81-126">Response</span></span>

<span data-ttu-id="a5e81-127">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e81-127">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5e81-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5e81-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5e81-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e81-129">Request</span></span>

<span data-ttu-id="a5e81-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5e81-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a5e81-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e81-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5e81-132">C#</span><span class="sxs-lookup"><span data-stu-id="a5e81-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5e81-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5e81-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5e81-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a5e81-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5e81-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e81-135">Response</span></span>

<span data-ttu-id="a5e81-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e81-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a5e81-137">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5e81-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5e81-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5e81-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
