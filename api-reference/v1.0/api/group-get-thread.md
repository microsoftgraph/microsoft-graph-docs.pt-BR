---
title: Obter thread de conversas
description: Obter um objeto thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 90b8a8ffa032190e3540b97253ab14b05110d0b9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275709"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="6e14c-103">Obter thread de conversas</span><span class="sxs-lookup"><span data-stu-id="6e14c-103">Get conversation thread</span></span>
<span data-ttu-id="6e14c-104">Obter um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="6e14c-104">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e14c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e14c-105">Permissions</span></span>
<span data-ttu-id="6e14c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e14c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e14c-108">Permission type</span></span>      | <span data-ttu-id="6e14c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e14c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e14c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e14c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e14c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e14c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e14c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e14c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e14c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e14c-113">Not supported.</span></span>    |
|<span data-ttu-id="6e14c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e14c-114">Application</span></span> | <span data-ttu-id="6e14c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e14c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e14c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e14c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e14c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e14c-117">Optional query parameters</span></span>
<span data-ttu-id="6e14c-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e14c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e14c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e14c-119">Request headers</span></span>
| <span data-ttu-id="6e14c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e14c-120">Header</span></span>       | <span data-ttu-id="6e14c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6e14c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e14c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e14c-122">Authorization</span></span>  | <span data-ttu-id="6e14c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e14c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e14c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e14c-125">Request body</span></span>
<span data-ttu-id="6e14c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e14c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e14c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e14c-127">Response</span></span>
<span data-ttu-id="6e14c-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [thread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e14c-128">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e14c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e14c-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6e14c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e14c-130">Request</span></span>
<span data-ttu-id="6e14c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e14c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="6e14c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e14c-132">Response</span></span>
<span data-ttu-id="6e14c-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6e14c-133">The following is an example of the response.</span></span>
><span data-ttu-id="6e14c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e14c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6e14c-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6e14c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6e14c-137">C#</span><span class="sxs-lookup"><span data-stu-id="6e14c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_thread-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e14c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="6e14c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_thread-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6e14c-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6e14c-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_thread-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-get-thread.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-get-thread.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get-thread.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
