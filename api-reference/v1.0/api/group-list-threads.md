---
title: Listar threads
description: Obter todos os threads de um grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5a25ae865219dde471e1c8d467dac2d963056f66
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057608"
---
# <a name="list-threads"></a><span data-ttu-id="8eb70-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="8eb70-103">List threads</span></span>

<span data-ttu-id="8eb70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eb70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8eb70-105">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="8eb70-105">Get all the threads of a group.</span></span>

><span data-ttu-id="8eb70-106">**Observação:** Você também pode [obter todos os threads de uma conversa](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="8eb70-106">**Note:** You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8eb70-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8eb70-107">Permissions</span></span>
<span data-ttu-id="8eb70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eb70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eb70-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8eb70-110">Permission type</span></span>      | <span data-ttu-id="8eb70-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8eb70-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eb70-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8eb70-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8eb70-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb70-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8eb70-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8eb70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eb70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8eb70-115">Not supported.</span></span>    |
|<span data-ttu-id="8eb70-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8eb70-116">Application</span></span> | <span data-ttu-id="8eb70-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb70-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8eb70-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8eb70-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8eb70-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8eb70-119">Optional query parameters</span></span>
<span data-ttu-id="8eb70-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8eb70-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8eb70-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8eb70-121">Request headers</span></span>
| <span data-ttu-id="8eb70-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8eb70-122">Header</span></span>       | <span data-ttu-id="8eb70-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8eb70-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8eb70-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8eb70-124">Authorization</span></span>  | <span data-ttu-id="8eb70-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8eb70-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8eb70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8eb70-127">Request body</span></span>
<span data-ttu-id="8eb70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8eb70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8eb70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8eb70-129">Response</span></span>
<span data-ttu-id="8eb70-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8eb70-130">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eb70-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8eb70-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8eb70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8eb70-132">Request</span></span>
<span data-ttu-id="8eb70-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8eb70-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8eb70-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8eb70-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="8eb70-135">C#</span><span class="sxs-lookup"><span data-stu-id="8eb70-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8eb70-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8eb70-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8eb70-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8eb70-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8eb70-138">Java</span><span class="sxs-lookup"><span data-stu-id="8eb70-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8eb70-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8eb70-139">Response</span></span>
<span data-ttu-id="8eb70-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8eb70-140">The following is an example of the response.</span></span>
><span data-ttu-id="8eb70-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8eb70-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

