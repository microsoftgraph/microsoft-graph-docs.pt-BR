---
title: Obter thread de conversas
description: Obter um objeto thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 63131aa1edc9a6a76c148017cf2a555f8c8fefc5
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219127"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="79bdc-103">Obter thread de conversas</span><span class="sxs-lookup"><span data-stu-id="79bdc-103">Get conversation thread</span></span>

<span data-ttu-id="79bdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79bdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79bdc-105">Obter um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="79bdc-105">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79bdc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79bdc-106">Permissions</span></span>
<span data-ttu-id="79bdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79bdc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79bdc-109">Permission type</span></span>      | <span data-ttu-id="79bdc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79bdc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79bdc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79bdc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="79bdc-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79bdc-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="79bdc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79bdc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79bdc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79bdc-114">Not supported.</span></span>    |
|<span data-ttu-id="79bdc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79bdc-115">Application</span></span> | <span data-ttu-id="79bdc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79bdc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79bdc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79bdc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79bdc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79bdc-118">Optional query parameters</span></span>
<span data-ttu-id="79bdc-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79bdc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79bdc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79bdc-120">Request headers</span></span>
| <span data-ttu-id="79bdc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79bdc-121">Header</span></span>       | <span data-ttu-id="79bdc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79bdc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79bdc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79bdc-123">Authorization</span></span>  | <span data-ttu-id="79bdc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79bdc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79bdc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79bdc-126">Request body</span></span>
<span data-ttu-id="79bdc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79bdc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79bdc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="79bdc-128">Response</span></span>
<span data-ttu-id="79bdc-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [thread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79bdc-129">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79bdc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79bdc-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="79bdc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79bdc-131">Request</span></span>
<span data-ttu-id="79bdc-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79bdc-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79bdc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="79bdc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="c"></a>[<span data-ttu-id="79bdc-134">C#</span><span class="sxs-lookup"><span data-stu-id="79bdc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79bdc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79bdc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79bdc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79bdc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79bdc-137">Java</span><span class="sxs-lookup"><span data-stu-id="79bdc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79bdc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="79bdc-138">Response</span></span>
<span data-ttu-id="79bdc-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79bdc-139">The following is an example of the response.</span></span>
><span data-ttu-id="79bdc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79bdc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
