---
title: Listar respostas
description: Recupere uma lista de objetos chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a79d94029a085e48677ed601795b834fc095db2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261438"
---
# <a name="list-replies"></a><span data-ttu-id="fc8e2-103">Listar respostas</span><span class="sxs-lookup"><span data-stu-id="fc8e2-103">List replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc8e2-104">Recupere uma lista de objetos chat.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-104">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc8e2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc8e2-105">Permissions</span></span>

<span data-ttu-id="fc8e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc8e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc8e2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc8e2-108">Permission type</span></span>                        | <span data-ttu-id="fc8e2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc8e2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fc8e2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc8e2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc8e2-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc8e2-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="fc8e2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc8e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc8e2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-113">Not supported.</span></span> |
| <span data-ttu-id="fc8e2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc8e2-114">Application</span></span>                            | <span data-ttu-id="fc8e2-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc8e2-115">Chat.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc8e2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc8e2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
GET /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc8e2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc8e2-117">Optional query parameters</span></span>

<span data-ttu-id="fc8e2-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc8e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8e2-119">Request headers</span></span>

| <span data-ttu-id="fc8e2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fc8e2-120">Name</span></span>      |<span data-ttu-id="fc8e2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc8e2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fc8e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc8e2-122">Authorization</span></span> | <span data-ttu-id="fc8e2-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="fc8e2-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc8e2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8e2-124">Request body</span></span>

<span data-ttu-id="fc8e2-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc8e2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc8e2-126">Response</span></span>

<span data-ttu-id="fc8e2-127">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-127">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc8e2-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc8e2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc8e2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8e2-129">Request</span></span>

<span data-ttu-id="fc8e2-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```

### <a name="response"></a><span data-ttu-id="fc8e2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc8e2-131">Response</span></span>

<span data-ttu-id="fc8e2-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="fc8e2-133">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fc8e2-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc8e2-134">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc8e2-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fc8e2-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="fc8e2-136">C#</span><span class="sxs-lookup"><span data-stu-id="fc8e2-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_replies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc8e2-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc8e2-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_replies-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fc8e2-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fc8e2-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_replies-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessage-list-replies.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chatmessage-list-replies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chatmessage-list-replies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
