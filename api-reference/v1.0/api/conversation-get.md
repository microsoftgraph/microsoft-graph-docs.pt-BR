---
title: Obter conversation
description: Recupera as propriedades e os relacionamentos do objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8cc29f0acd317087113c8c5c1f1e6d30a11d248d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518207"
---
# <a name="get-conversation"></a><span data-ttu-id="1c3ab-103">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="1c3ab-103">Get conversation</span></span>

<span data-ttu-id="1c3ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c3ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c3ab-105">Recupera as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="1c3ab-105">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c3ab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c3ab-106">Permissions</span></span>
<span data-ttu-id="1c3ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c3ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c3ab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c3ab-109">Permission type</span></span>      | <span data-ttu-id="1c3ab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c3ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c3ab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c3ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c3ab-112">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="1c3ab-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="1c3ab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c3ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c3ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c3ab-114">Not supported.</span></span>    |
|<span data-ttu-id="1c3ab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c3ab-115">Application</span></span> | <span data-ttu-id="1c3ab-116">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="1c3ab-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c3ab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c3ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c3ab-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c3ab-118">Optional query parameters</span></span>
<span data-ttu-id="1c3ab-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c3ab-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c3ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3ab-120">Request headers</span></span>
| <span data-ttu-id="1c3ab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c3ab-121">Header</span></span>       | <span data-ttu-id="1c3ab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1c3ab-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c3ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c3ab-123">Authorization</span></span>  | <span data-ttu-id="1c3ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c3ab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c3ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3ab-126">Request body</span></span>
<span data-ttu-id="1c3ab-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c3ab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c3ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c3ab-128">Response</span></span>

<span data-ttu-id="1c3ab-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c3ab-129">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c3ab-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c3ab-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c3ab-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c3ab-131">Request</span></span>
<span data-ttu-id="1c3ab-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c3ab-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c3ab-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c3ab-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="1c3ab-134">C#</span><span class="sxs-lookup"><span data-stu-id="1c3ab-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c3ab-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c3ab-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c3ab-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c3ab-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c3ab-137">Java</span><span class="sxs-lookup"><span data-stu-id="1c3ab-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c3ab-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c3ab-138">Response</span></span>
<span data-ttu-id="1c3ab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c3ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
