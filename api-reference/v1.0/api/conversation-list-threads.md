---
title: Listar threads
description: Obtenha todos os threads em uma conversa de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 69d1179dc74b275f8f9cf74b515ff2ebf9dc5349
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44743785"
---
# <a name="list-threads"></a><span data-ttu-id="4c807-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="4c807-103">List threads</span></span>

<span data-ttu-id="4c807-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c807-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c807-105">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="4c807-105">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="4c807-106">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="4c807-106">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c807-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c807-107">Permissions</span></span>
<span data-ttu-id="4c807-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4c807-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4c807-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c807-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c807-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c807-110">Permission type</span></span>      | <span data-ttu-id="4c807-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c807-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c807-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c807-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c807-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c807-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c807-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c807-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c807-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c807-115">Not supported.</span></span>    |
|<span data-ttu-id="4c807-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c807-116">Application</span></span> | <span data-ttu-id="4c807-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c807-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c807-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c807-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c807-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c807-119">Optional query parameters</span></span>
<span data-ttu-id="4c807-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c807-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4c807-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c807-121">Request headers</span></span>
| <span data-ttu-id="4c807-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c807-122">Header</span></span>       | <span data-ttu-id="4c807-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4c807-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c807-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c807-124">Authorization</span></span>  | <span data-ttu-id="4c807-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4c807-125">Bearer {token}.</span></span> <span data-ttu-id="4c807-126">Required.</span><span class="sxs-lookup"><span data-stu-id="4c807-126">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c807-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c807-127">Request body</span></span>
<span data-ttu-id="4c807-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c807-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c807-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c807-129">Response</span></span>

<span data-ttu-id="4c807-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c807-130">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c807-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c807-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c807-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c807-132">Request</span></span>
<span data-ttu-id="4c807-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c807-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c807-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c807-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="4c807-135">C#</span><span class="sxs-lookup"><span data-stu-id="4c807-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c807-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c807-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c807-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c807-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c807-138">Java</span><span class="sxs-lookup"><span data-stu-id="4c807-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c807-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c807-139">Response</span></span>
<span data-ttu-id="4c807-140">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="4c807-140">Here is an example of the response.</span></span> <span data-ttu-id="4c807-141">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="4c807-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4c807-142">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4c807-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
