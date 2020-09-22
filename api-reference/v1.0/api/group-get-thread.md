---
title: Obter thread de conversas
description: Obter um objeto thread.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 30eb4309b471adb5edc998da247f1535f71e1a68
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094735"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="f2b76-103">Obter thread de conversas</span><span class="sxs-lookup"><span data-stu-id="f2b76-103">Get conversation thread</span></span>

<span data-ttu-id="f2b76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b76-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2b76-105">Obter um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="f2b76-105">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2b76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2b76-106">Permissions</span></span>
<span data-ttu-id="f2b76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2b76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2b76-109">Permission type</span></span>      | <span data-ttu-id="f2b76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2b76-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2b76-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2b76-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2b76-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b76-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2b76-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2b76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2b76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2b76-114">Not supported.</span></span>    |
|<span data-ttu-id="f2b76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2b76-115">Application</span></span> | <span data-ttu-id="f2b76-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b76-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2b76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b76-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2b76-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2b76-118">Optional query parameters</span></span>
<span data-ttu-id="f2b76-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2b76-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2b76-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b76-120">Request headers</span></span>
| <span data-ttu-id="f2b76-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2b76-121">Header</span></span>       | <span data-ttu-id="f2b76-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2b76-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2b76-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2b76-123">Authorization</span></span>  | <span data-ttu-id="f2b76-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2b76-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2b76-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b76-126">Request body</span></span>
<span data-ttu-id="f2b76-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2b76-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2b76-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2b76-128">Response</span></span>
<span data-ttu-id="f2b76-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [thread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2b76-129">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2b76-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2b76-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f2b76-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b76-131">Request</span></span>
<span data-ttu-id="f2b76-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2b76-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2b76-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b76-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="c"></a>[<span data-ttu-id="f2b76-134">C#</span><span class="sxs-lookup"><span data-stu-id="f2b76-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2b76-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2b76-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2b76-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2b76-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2b76-137">Java</span><span class="sxs-lookup"><span data-stu-id="f2b76-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f2b76-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2b76-138">Response</span></span>
<span data-ttu-id="f2b76-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2b76-139">The following is an example of the response.</span></span>
><span data-ttu-id="f2b76-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2b76-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

