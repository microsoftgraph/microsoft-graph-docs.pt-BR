---
title: Listar threads
description: Obter todos os threads de um grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 00317f4df1ac7fd43625266ce746ac15cbd9511a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440362"
---
# <a name="list-threads"></a><span data-ttu-id="f9a6f-103">Listar threads</span><span class="sxs-lookup"><span data-stu-id="f9a6f-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9a6f-104">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-104">Get all the threads of a group.</span></span>

<span data-ttu-id="f9a6f-105">Observação: você também pode [obter todos os threads de uma conversa](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="f9a6f-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9a6f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9a6f-106">Permissions</span></span>
<span data-ttu-id="f9a6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9a6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9a6f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9a6f-109">Permission type</span></span>      | <span data-ttu-id="f9a6f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9a6f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9a6f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9a6f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9a6f-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9a6f-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9a6f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9a6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9a6f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-114">Not supported.</span></span>    |
|<span data-ttu-id="f9a6f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9a6f-115">Application</span></span> | <span data-ttu-id="f9a6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9a6f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9a6f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9a6f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f9a6f-118">Optional query parameters</span></span>
<span data-ttu-id="f9a6f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9a6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9a6f-120">Request headers</span></span>
| <span data-ttu-id="f9a6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9a6f-121">Header</span></span>       | <span data-ttu-id="f9a6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9a6f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9a6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9a6f-123">Authorization</span></span>  | <span data-ttu-id="f9a6f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9a6f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9a6f-126">Request body</span></span>
<span data-ttu-id="f9a6f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9a6f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9a6f-128">Response</span></span>
<span data-ttu-id="f9a6f-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9a6f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9a6f-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f9a6f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9a6f-131">Request</span></span>
<span data-ttu-id="f9a6f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f9a6f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9a6f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9a6f-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9a6f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9a6f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9a6f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9a6f-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f9a6f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f9a6f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9a6f-137">Response</span></span>
<span data-ttu-id="f9a6f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-138">The following is an example of the response.</span></span>
><span data-ttu-id="f9a6f-139">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f9a6f-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9a6f-140">All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
