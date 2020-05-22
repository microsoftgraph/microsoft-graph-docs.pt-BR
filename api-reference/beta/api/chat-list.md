---
title: Listar chats
description: Recupere a lista de chats de um usuário.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5c4c061c7f78fcb907f81481ea86c6a31b0692c1
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345678"
---
# <a name="list-chats"></a><span data-ttu-id="6849b-103">Listar chats</span><span class="sxs-lookup"><span data-stu-id="6849b-103">List chats</span></span>

<span data-ttu-id="6849b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6849b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6849b-105">Recupere a lista de [chats](../resources/chat.md) dos quais o usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="6849b-105">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="6849b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6849b-106">Permissions</span></span>

<span data-ttu-id="6849b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6849b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6849b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6849b-109">Permission type</span></span>      | <span data-ttu-id="6849b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6849b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6849b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6849b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6849b-112">Chat. ReadBasic, chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6849b-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="6849b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6849b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6849b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6849b-114">Not supported.</span></span>    |
|<span data-ttu-id="6849b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6849b-115">Application</span></span> | <span data-ttu-id="6849b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6849b-116">Not supported.</span></span>    |

> [!NOTE]
> <span data-ttu-id="6849b-117">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6849b-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="6849b-118">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="6849b-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="6849b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6849b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6849b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6849b-120">Optional query parameters</span></span>

<span data-ttu-id="6849b-121">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6849b-121">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6849b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6849b-122">Request headers</span></span>

| <span data-ttu-id="6849b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6849b-123">Header</span></span>       | <span data-ttu-id="6849b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6849b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6849b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6849b-125">Authorization</span></span>  | <span data-ttu-id="6849b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6849b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6849b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6849b-128">Request body</span></span>

<span data-ttu-id="6849b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6849b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6849b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6849b-130">Response</span></span>

<span data-ttu-id="6849b-131">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6849b-131">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6849b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6849b-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6849b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6849b-133">Request</span></span>

<span data-ttu-id="6849b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6849b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6849b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6849b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="6849b-136">C#</span><span class="sxs-lookup"><span data-stu-id="6849b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6849b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6849b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6849b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6849b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6849b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6849b-139">Response</span></span>

<span data-ttu-id="6849b-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6849b-140">Here is an example of the response.</span></span> 

><span data-ttu-id="6849b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6849b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
