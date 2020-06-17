---
title: Listar conversas
description: Recupere a lista de conversas desse grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f9b4b582f0ff3b414137298c08f6582e6fe5439f
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744037"
---
# <a name="list-conversations"></a><span data-ttu-id="92bdc-103">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="92bdc-103">List conversations</span></span>

<span data-ttu-id="92bdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92bdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92bdc-105">Recupere a lista de [conversas](../resources/conversation.md) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="92bdc-105">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="92bdc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92bdc-106">Permissions</span></span>
<span data-ttu-id="92bdc-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="92bdc-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="92bdc-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92bdc-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92bdc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92bdc-109">Permission type</span></span>      | <span data-ttu-id="92bdc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92bdc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92bdc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92bdc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="92bdc-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92bdc-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="92bdc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92bdc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92bdc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92bdc-114">Not supported.</span></span>    |
|<span data-ttu-id="92bdc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92bdc-115">Application</span></span> | <span data-ttu-id="92bdc-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92bdc-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92bdc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92bdc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92bdc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92bdc-118">Optional query parameters</span></span>
<span data-ttu-id="92bdc-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92bdc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92bdc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92bdc-120">Request headers</span></span>
| <span data-ttu-id="92bdc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92bdc-121">Header</span></span>       | <span data-ttu-id="92bdc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92bdc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92bdc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92bdc-123">Authorization</span></span>  | <span data-ttu-id="92bdc-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="92bdc-124">Bearer {token}.</span></span> <span data-ttu-id="92bdc-125">Required.</span><span class="sxs-lookup"><span data-stu-id="92bdc-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92bdc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92bdc-126">Request body</span></span>
<span data-ttu-id="92bdc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92bdc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92bdc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="92bdc-128">Response</span></span>
<span data-ttu-id="92bdc-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92bdc-129">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92bdc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92bdc-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="92bdc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92bdc-131">Request</span></span>
<span data-ttu-id="92bdc-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92bdc-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92bdc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="92bdc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
# <a name="c"></a>[<span data-ttu-id="92bdc-134">C#</span><span class="sxs-lookup"><span data-stu-id="92bdc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92bdc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92bdc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92bdc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92bdc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92bdc-137">Java</span><span class="sxs-lookup"><span data-stu-id="92bdc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="92bdc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="92bdc-138">Response</span></span>
<span data-ttu-id="92bdc-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92bdc-139">The following is an example of the response.</span></span>
><span data-ttu-id="92bdc-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="92bdc-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="92bdc-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="92bdc-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
