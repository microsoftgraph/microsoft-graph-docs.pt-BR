---
title: Obter thread de conversas
description: Obter um objeto thread.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 05a71474c407f9fa3a797947978791123fa514ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053080"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="45f1c-103">Obter thread de conversas</span><span class="sxs-lookup"><span data-stu-id="45f1c-103">Get conversation thread</span></span>

<span data-ttu-id="45f1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45f1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45f1c-105">Obter um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="45f1c-105">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45f1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45f1c-106">Permissions</span></span>
<span data-ttu-id="45f1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45f1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45f1c-109">Permission type</span></span>      | <span data-ttu-id="45f1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45f1c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45f1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45f1c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45f1c-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f1c-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="45f1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45f1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45f1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45f1c-114">Not supported.</span></span>    |
|<span data-ttu-id="45f1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45f1c-115">Application</span></span> | <span data-ttu-id="45f1c-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f1c-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45f1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45f1c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45f1c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45f1c-118">Optional query parameters</span></span>
<span data-ttu-id="45f1c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45f1c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45f1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45f1c-120">Request headers</span></span>
| <span data-ttu-id="45f1c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45f1c-121">Header</span></span>       | <span data-ttu-id="45f1c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45f1c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="45f1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45f1c-123">Authorization</span></span>  | <span data-ttu-id="45f1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45f1c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45f1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45f1c-126">Request body</span></span>
<span data-ttu-id="45f1c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45f1c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45f1c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="45f1c-128">Response</span></span>
<span data-ttu-id="45f1c-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [thread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45f1c-129">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45f1c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45f1c-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="45f1c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45f1c-131">Request</span></span>
<span data-ttu-id="45f1c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45f1c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45f1c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="45f1c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="c"></a>[<span data-ttu-id="45f1c-134">C#</span><span class="sxs-lookup"><span data-stu-id="45f1c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45f1c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45f1c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45f1c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45f1c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45f1c-137">Java</span><span class="sxs-lookup"><span data-stu-id="45f1c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45f1c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="45f1c-138">Response</span></span>
<span data-ttu-id="45f1c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45f1c-139">The following is an example of the response.</span></span>
><span data-ttu-id="45f1c-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="45f1c-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

