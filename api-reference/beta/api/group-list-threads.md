---
title: Listar threads
description: Obter todos os threads de um grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f92c0260885f831eef2832bbd2dbdb5adaf87e55
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326265"
---
# <a name="list-threads"></a><span data-ttu-id="37b1f-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="37b1f-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37b1f-104">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="37b1f-104">Get all the threads of a group.</span></span>

<span data-ttu-id="37b1f-105">Observação: você também pode [obter todos os threads de uma conversa](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="37b1f-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37b1f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37b1f-106">Permissions</span></span>
<span data-ttu-id="37b1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37b1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37b1f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37b1f-109">Permission type</span></span>      | <span data-ttu-id="37b1f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37b1f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37b1f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37b1f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37b1f-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b1f-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="37b1f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37b1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37b1f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37b1f-114">Not supported.</span></span>    |
|<span data-ttu-id="37b1f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37b1f-115">Application</span></span> | <span data-ttu-id="37b1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37b1f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37b1f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37b1f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37b1f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37b1f-118">Optional query parameters</span></span>
<span data-ttu-id="37b1f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37b1f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37b1f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37b1f-120">Request headers</span></span>
| <span data-ttu-id="37b1f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37b1f-121">Header</span></span>       | <span data-ttu-id="37b1f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="37b1f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37b1f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37b1f-123">Authorization</span></span>  | <span data-ttu-id="37b1f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37b1f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37b1f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37b1f-126">Request body</span></span>
<span data-ttu-id="37b1f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37b1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37b1f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="37b1f-128">Response</span></span>
<span data-ttu-id="37b1f-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37b1f-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37b1f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37b1f-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="37b1f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37b1f-131">Request</span></span>
<span data-ttu-id="37b1f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37b1f-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="37b1f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="37b1f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="37b1f-134">C#</span><span class="sxs-lookup"><span data-stu-id="37b1f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37b1f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37b1f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="37b1f-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="37b1f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="37b1f-137">Java</span><span class="sxs-lookup"><span data-stu-id="37b1f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37b1f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="37b1f-138">Response</span></span>
<span data-ttu-id="37b1f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37b1f-139">The following is an example of the response.</span></span>
><span data-ttu-id="37b1f-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37b1f-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="37b1f-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37b1f-141">All the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
