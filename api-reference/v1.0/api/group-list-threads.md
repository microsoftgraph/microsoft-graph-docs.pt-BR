---
title: Listar threads
description: Obter todos os threads de um grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1c9cb896efc4124de87f0142eb624881c99be798
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517037"
---
# <a name="list-threads"></a><span data-ttu-id="df689-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="df689-103">List threads</span></span>

<span data-ttu-id="df689-104">Namespace: Microsoft. Graph obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="df689-104">Namespace: microsoft.graph Get all the threads of a group.</span></span>

><span data-ttu-id="df689-105">Observação: você também pode [obter todos os threads de uma conversa](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="df689-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df689-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df689-106">Permissions</span></span>
<span data-ttu-id="df689-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df689-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df689-109">Permission type</span></span>      | <span data-ttu-id="df689-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df689-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df689-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df689-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df689-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df689-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df689-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df689-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df689-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df689-114">Not supported.</span></span>    |
|<span data-ttu-id="df689-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df689-115">Application</span></span> | <span data-ttu-id="df689-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df689-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df689-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df689-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df689-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="df689-118">Optional query parameters</span></span>
<span data-ttu-id="df689-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="df689-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df689-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df689-120">Request headers</span></span>
| <span data-ttu-id="df689-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df689-121">Header</span></span>       | <span data-ttu-id="df689-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df689-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df689-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df689-123">Authorization</span></span>  | <span data-ttu-id="df689-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df689-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df689-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df689-126">Request body</span></span>
<span data-ttu-id="df689-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df689-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df689-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df689-128">Response</span></span>
<span data-ttu-id="df689-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df689-129">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df689-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df689-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="df689-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df689-131">Request</span></span>
<span data-ttu-id="df689-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df689-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df689-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="df689-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="df689-134">C#</span><span class="sxs-lookup"><span data-stu-id="df689-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df689-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df689-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df689-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df689-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df689-137">Java</span><span class="sxs-lookup"><span data-stu-id="df689-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df689-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="df689-138">Response</span></span>
<span data-ttu-id="df689-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df689-139">The following is an example of the response.</span></span>
><span data-ttu-id="df689-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df689-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
