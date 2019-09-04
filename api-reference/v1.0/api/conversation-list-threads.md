---
title: Listar threads
description: Obtenha todos os threads em uma conversa de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 72ce57bf47e7188dfe98a57dbb7a9daef2767dd9
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727114"
---
# <a name="list-threads"></a><span data-ttu-id="7a74c-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="7a74c-103">List threads</span></span>

<span data-ttu-id="7a74c-104">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="7a74c-104">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="7a74c-105">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="7a74c-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7a74c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a74c-106">Permissions</span></span>
<span data-ttu-id="7a74c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a74c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a74c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a74c-109">Permission type</span></span>      | <span data-ttu-id="7a74c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a74c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a74c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a74c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7a74c-112">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="7a74c-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="7a74c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a74c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a74c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a74c-114">Not supported.</span></span>    |
|<span data-ttu-id="7a74c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a74c-115">Application</span></span> | <span data-ttu-id="7a74c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a74c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a74c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a74c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7a74c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a74c-118">Optional query parameters</span></span>
<span data-ttu-id="7a74c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a74c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7a74c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a74c-120">Request headers</span></span>
| <span data-ttu-id="7a74c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a74c-121">Header</span></span>       | <span data-ttu-id="7a74c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7a74c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a74c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a74c-123">Authorization</span></span>  | <span data-ttu-id="7a74c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a74c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a74c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a74c-126">Request body</span></span>
<span data-ttu-id="7a74c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a74c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a74c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a74c-128">Response</span></span>

<span data-ttu-id="7a74c-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a74c-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a74c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a74c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a74c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a74c-131">Request</span></span>
<span data-ttu-id="7a74c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a74c-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a74c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a74c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a74c-134">C#</span><span class="sxs-lookup"><span data-stu-id="7a74c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a74c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a74c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a74c-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7a74c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a74c-137">Java</span><span class="sxs-lookup"><span data-stu-id="7a74c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a74c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a74c-138">Response</span></span>
<span data-ttu-id="7a74c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a74c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
