---
title: Listar threads
description: Obtenha todos os threads em uma conversa de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 613d392a9e08c850f3fd6fb3517c7b2f1b7f977c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003060"
---
# <a name="list-threads"></a><span data-ttu-id="36028-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="36028-103">List threads</span></span>

<span data-ttu-id="36028-104">Obtém todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="36028-104">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="36028-105">Observação: Você também pode [obter todos os threads de um grupo](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="36028-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="36028-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36028-106">Permissions</span></span>
<span data-ttu-id="36028-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36028-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36028-109">Permission type</span></span>      | <span data-ttu-id="36028-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36028-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36028-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36028-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36028-112">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="36028-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="36028-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36028-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36028-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36028-114">Not supported.</span></span>    |
|<span data-ttu-id="36028-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36028-115">Application</span></span> | <span data-ttu-id="36028-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36028-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36028-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36028-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36028-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36028-118">Optional query parameters</span></span>
<span data-ttu-id="36028-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36028-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="36028-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36028-120">Request headers</span></span>
| <span data-ttu-id="36028-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36028-121">Header</span></span>       | <span data-ttu-id="36028-122">Valor</span><span class="sxs-lookup"><span data-stu-id="36028-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36028-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="36028-123">Authorization</span></span>  | <span data-ttu-id="36028-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36028-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36028-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36028-126">Request body</span></span>
<span data-ttu-id="36028-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36028-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36028-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="36028-128">Response</span></span>

<span data-ttu-id="36028-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36028-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36028-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36028-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36028-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36028-131">Request</span></span>
<span data-ttu-id="36028-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36028-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36028-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="36028-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36028-134">C#</span><span class="sxs-lookup"><span data-stu-id="36028-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36028-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="36028-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36028-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="36028-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36028-137">Java</span><span class="sxs-lookup"><span data-stu-id="36028-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36028-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="36028-138">Response</span></span>
<span data-ttu-id="36028-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36028-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
