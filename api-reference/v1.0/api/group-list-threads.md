---
title: Listar threads
description: Obter todos os threads de um grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7fad6a3e8f804f84ffae33dcc6165095c7e1b8c3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052303"
---
# <a name="list-threads"></a><span data-ttu-id="94ce4-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="94ce4-103">List threads</span></span>

<span data-ttu-id="94ce4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94ce4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94ce4-105">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="94ce4-105">Get all the threads of a group.</span></span>

><span data-ttu-id="94ce4-106">**Observação:** Você também pode [obter todos os threads de uma conversa](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="94ce4-106">**Note:** You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94ce4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94ce4-107">Permissions</span></span>
<span data-ttu-id="94ce4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94ce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94ce4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94ce4-110">Permission type</span></span>      | <span data-ttu-id="94ce4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94ce4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94ce4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94ce4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94ce4-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94ce4-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="94ce4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94ce4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94ce4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94ce4-115">Not supported.</span></span>    |
|<span data-ttu-id="94ce4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94ce4-116">Application</span></span> | <span data-ttu-id="94ce4-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94ce4-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94ce4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94ce4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94ce4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94ce4-119">Optional query parameters</span></span>
<span data-ttu-id="94ce4-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94ce4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94ce4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94ce4-121">Request headers</span></span>
| <span data-ttu-id="94ce4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94ce4-122">Header</span></span>       | <span data-ttu-id="94ce4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="94ce4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94ce4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="94ce4-124">Authorization</span></span>  | <span data-ttu-id="94ce4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94ce4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94ce4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94ce4-127">Request body</span></span>
<span data-ttu-id="94ce4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94ce4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94ce4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94ce4-129">Response</span></span>
<span data-ttu-id="94ce4-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94ce4-130">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94ce4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94ce4-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="94ce4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94ce4-132">Request</span></span>
<span data-ttu-id="94ce4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94ce4-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94ce4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94ce4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="94ce4-135">C#</span><span class="sxs-lookup"><span data-stu-id="94ce4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94ce4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94ce4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94ce4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94ce4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94ce4-138">Java</span><span class="sxs-lookup"><span data-stu-id="94ce4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94ce4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="94ce4-139">Response</span></span>
<span data-ttu-id="94ce4-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94ce4-140">The following is an example of the response.</span></span>
><span data-ttu-id="94ce4-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94ce4-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

