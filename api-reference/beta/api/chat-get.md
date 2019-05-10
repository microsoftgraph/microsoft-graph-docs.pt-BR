---
title: Obter bate-papo
description: Recupere um único bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 19fce3e08788611cdbb03b7c70eb94753c5f7680
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591621"
---
# <a name="get-chat"></a><span data-ttu-id="078ff-103">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="078ff-103">Get chat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="078ff-104">Recupere um único [bate-papo](../resources/chat.md) (sem suas mensagens).</span><span class="sxs-lookup"><span data-stu-id="078ff-104">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="078ff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="078ff-105">Permissions</span></span>

<span data-ttu-id="078ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="078ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="078ff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="078ff-108">Permission type</span></span>      | <span data-ttu-id="078ff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="078ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="078ff-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="078ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="078ff-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="078ff-111">Chat.Read</span></span>   |
|<span data-ttu-id="078ff-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="078ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="078ff-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="078ff-113">Not supported.</span></span>    |
|<span data-ttu-id="078ff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="078ff-114">Application</span></span> | <span data-ttu-id="078ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="078ff-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="078ff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="078ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="078ff-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="078ff-117">Optional query parameters</span></span>

<span data-ttu-id="078ff-118">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="078ff-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="078ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="078ff-119">Request headers</span></span>

| <span data-ttu-id="078ff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="078ff-120">Header</span></span>       | <span data-ttu-id="078ff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="078ff-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="078ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="078ff-122">Authorization</span></span>  | <span data-ttu-id="078ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="078ff-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="078ff-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="078ff-125">Request body</span></span>

<span data-ttu-id="078ff-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="078ff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="078ff-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="078ff-127">Response</span></span>

<span data-ttu-id="078ff-128">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="078ff-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="078ff-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="078ff-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="078ff-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="078ff-130">Request</span></span>
<span data-ttu-id="078ff-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="078ff-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```

##### <a name="response"></a><span data-ttu-id="078ff-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="078ff-132">Response</span></span>
<span data-ttu-id="078ff-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="078ff-133">Here is an example of the response.</span></span> 

><span data-ttu-id="078ff-134">**Observação:** O objeto de resposta mostrado aqui é encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="078ff-134">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="078ff-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="078ff-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2019-04-18T23:51:42.099Z",
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="078ff-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="078ff-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="078ff-137">C#</span><span class="sxs-lookup"><span data-stu-id="078ff-137">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chat_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="078ff-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="078ff-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chat_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chat-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chat-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
