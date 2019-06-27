---
title: Listar threads
description: Obter todos os threads de um grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 051728fb5f077c9d82b6bff431e47913e75572d3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263004"
---
# <a name="list-threads"></a><span data-ttu-id="d292f-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="d292f-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d292f-104">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="d292f-104">Get all the threads of a group.</span></span>

<span data-ttu-id="d292f-105">Observação: você também pode [obter todos os threads de uma conversa](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="d292f-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d292f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d292f-106">Permissions</span></span>
<span data-ttu-id="d292f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d292f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d292f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d292f-109">Permission type</span></span>      | <span data-ttu-id="d292f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d292f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d292f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d292f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d292f-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d292f-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d292f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d292f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d292f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d292f-114">Not supported.</span></span>    |
|<span data-ttu-id="d292f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d292f-115">Application</span></span> | <span data-ttu-id="d292f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d292f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d292f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d292f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d292f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d292f-118">Optional query parameters</span></span>
<span data-ttu-id="d292f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d292f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d292f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d292f-120">Request headers</span></span>
| <span data-ttu-id="d292f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d292f-121">Header</span></span>       | <span data-ttu-id="d292f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d292f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d292f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d292f-123">Authorization</span></span>  | <span data-ttu-id="d292f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d292f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d292f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d292f-126">Request body</span></span>
<span data-ttu-id="d292f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d292f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d292f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d292f-128">Response</span></span>
<span data-ttu-id="d292f-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d292f-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d292f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d292f-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d292f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d292f-131">Request</span></span>
<span data-ttu-id="d292f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d292f-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="d292f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d292f-133">Response</span></span>
<span data-ttu-id="d292f-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d292f-134">The following is an example of the response.</span></span>
><span data-ttu-id="d292f-135">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d292f-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d292f-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d292f-136">All the properties will be returned from an actual call.</span></span>
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
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d292f-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d292f-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d292f-138">C#</span><span class="sxs-lookup"><span data-stu-id="d292f-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_threads-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d292f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d292f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_threads-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d292f-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d292f-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_threads-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
