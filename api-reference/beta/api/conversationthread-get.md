---
title: Obter conversationThread
description: 'Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ef2dd2e2bedc87bff6eed4e2da260436342a5e73
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862921"
---
# <a name="get-conversationthread"></a><span data-ttu-id="5c4fc-104">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="5c4fc-104">Get conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c4fc-p102">Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="5c4fc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c4fc-107">Permissions</span></span>
<span data-ttu-id="5c4fc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c4fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c4fc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c4fc-110">Permission type</span></span>      | <span data-ttu-id="5c4fc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c4fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c4fc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c4fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5c4fc-113">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="5c4fc-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="5c4fc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c4fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c4fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-115">Not supported.</span></span>    |
|<span data-ttu-id="5c4fc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c4fc-116">Application</span></span> | <span data-ttu-id="5c4fc-117">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="5c4fc-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c4fc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c4fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c4fc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c4fc-119">Optional query parameters</span></span>
<span data-ttu-id="5c4fc-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5c4fc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c4fc-121">Request headers</span></span>
| <span data-ttu-id="5c4fc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c4fc-122">Header</span></span>       | <span data-ttu-id="5c4fc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5c4fc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c4fc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c4fc-124">Authorization</span></span>  | <span data-ttu-id="5c4fc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c4fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c4fc-127">Request body</span></span>
<span data-ttu-id="5c4fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c4fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c4fc-129">Response</span></span>

<span data-ttu-id="5c4fc-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c4fc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c4fc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c4fc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c4fc-132">Request</span></span>
<span data-ttu-id="5c4fc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5c4fc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c4fc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c4fc-135">C#</span><span class="sxs-lookup"><span data-stu-id="5c4fc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c4fc-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c4fc-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c4fc-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5c4fc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5c4fc-138">Java</span><span class="sxs-lookup"><span data-stu-id="5c4fc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c4fc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c4fc-139">Response</span></span>
<span data-ttu-id="5c4fc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c4fc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
