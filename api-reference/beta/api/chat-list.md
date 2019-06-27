---
title: Listar chats
description: Recupere a lista de chats de um usuário.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 180cfad72a8a8df60a58be5cedfab07fad40a5b7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261415"
---
# <a name="list-chats"></a><span data-ttu-id="4234b-103">Listar chats</span><span class="sxs-lookup"><span data-stu-id="4234b-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4234b-104">Recupere a lista de [chats](../resources/chat.md) dos quais o usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="4234b-104">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="4234b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4234b-105">Permissions</span></span>

<span data-ttu-id="4234b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4234b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4234b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4234b-108">Permission type</span></span>      | <span data-ttu-id="4234b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4234b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4234b-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4234b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4234b-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="4234b-111">Chat.Read</span></span>   |
|<span data-ttu-id="4234b-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4234b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4234b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4234b-113">Not supported.</span></span>    |
|<span data-ttu-id="4234b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4234b-114">Application</span></span> | <span data-ttu-id="4234b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4234b-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="4234b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4234b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4234b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4234b-117">Optional query parameters</span></span>

<span data-ttu-id="4234b-118">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4234b-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4234b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4234b-119">Request headers</span></span>

| <span data-ttu-id="4234b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4234b-120">Header</span></span>       | <span data-ttu-id="4234b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4234b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4234b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4234b-122">Authorization</span></span>  | <span data-ttu-id="4234b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4234b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4234b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4234b-125">Request body</span></span>

<span data-ttu-id="4234b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4234b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4234b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4234b-127">Response</span></span>

<span data-ttu-id="4234b-128">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4234b-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4234b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4234b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4234b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4234b-130">Request</span></span>

<span data-ttu-id="4234b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4234b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```

##### <a name="response"></a><span data-ttu-id="4234b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4234b-132">Response</span></span>

<span data-ttu-id="4234b-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4234b-133">Here is an example of the response.</span></span> 

><span data-ttu-id="4234b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4234b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats",
    "value": [
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-04-18T23:51:42.099Z",
            "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_0c5cfdbb-596f-4d39-b557-5d9516c94107@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-04-18T23:19:23.76Z",
            "lastUpdatedDateTime": "2019-04-18T23:19:21.994Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_3ee373aa-62fa-4fc6-b11f-9627d5b4a73d@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-03-21T22:30:14.867Z",
            "lastUpdatedDateTime": "2019-03-21T22:30:15.507Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_90a27c51-5c74-453b-944a-134ba86da790@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-02-06T03:38:58.062Z",
            "lastUpdatedDateTime": "2019-02-06T03:38:58.063Z"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4234b-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4234b-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4234b-137">C#</span><span class="sxs-lookup"><span data-stu-id="4234b-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chats-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4234b-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="4234b-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chats-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4234b-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4234b-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chats-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chat-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chat-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chat-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
