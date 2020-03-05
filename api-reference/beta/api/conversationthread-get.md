---
title: Obter conversationThread
description: 'Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 78479d00fecc2eea7c7938bb5d5fc897c1535e67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436360"
---
# <a name="get-conversationthread"></a><span data-ttu-id="4adc0-104">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="4adc0-104">Get conversationThread</span></span>

<span data-ttu-id="4adc0-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4adc0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4adc0-p102">Obtenha um thread específico pertencente a um grupo. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="4adc0-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="4adc0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4adc0-108">Permissions</span></span>
<span data-ttu-id="4adc0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4adc0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4adc0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4adc0-111">Permission type</span></span>      | <span data-ttu-id="4adc0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4adc0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4adc0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4adc0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4adc0-114">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="4adc0-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="4adc0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4adc0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4adc0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4adc0-116">Not supported.</span></span>    |
|<span data-ttu-id="4adc0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4adc0-117">Application</span></span> | <span data-ttu-id="4adc0-118">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="4adc0-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4adc0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4adc0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="4adc0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4adc0-120">Optional query parameters</span></span>
<span data-ttu-id="4adc0-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4adc0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4adc0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4adc0-122">Request headers</span></span>
| <span data-ttu-id="4adc0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4adc0-123">Header</span></span>       | <span data-ttu-id="4adc0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="4adc0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4adc0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4adc0-125">Authorization</span></span>  | <span data-ttu-id="4adc0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4adc0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4adc0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4adc0-128">Request body</span></span>
<span data-ttu-id="4adc0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4adc0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4adc0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4adc0-130">Response</span></span>

<span data-ttu-id="4adc0-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4adc0-131">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4adc0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4adc0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4adc0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4adc0-133">Request</span></span>
<span data-ttu-id="4adc0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4adc0-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4adc0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4adc0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="4adc0-136">C#</span><span class="sxs-lookup"><span data-stu-id="4adc0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4adc0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4adc0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4adc0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4adc0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4adc0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4adc0-139">Response</span></span>
<span data-ttu-id="4adc0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4adc0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
