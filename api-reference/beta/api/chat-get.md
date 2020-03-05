---
title: Obter bate-papo
description: Recupere um único bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4e0e9126564074d34fd88d48751440dede270d8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438649"
---
# <a name="get-chat"></a><span data-ttu-id="0061c-103">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="0061c-103">Get chat</span></span>

<span data-ttu-id="0061c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0061c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0061c-105">Recupere um único [bate-papo](../resources/chat.md) (sem suas mensagens).</span><span class="sxs-lookup"><span data-stu-id="0061c-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="0061c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0061c-106">Permissions</span></span>

<span data-ttu-id="0061c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0061c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0061c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0061c-109">Permission type</span></span>      | <span data-ttu-id="0061c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0061c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0061c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0061c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0061c-112">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="0061c-112">Chat.Read</span></span>   |
|<span data-ttu-id="0061c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0061c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0061c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0061c-114">Not supported.</span></span>    |
|<span data-ttu-id="0061c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0061c-115">Application</span></span> | <span data-ttu-id="0061c-116">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0061c-116">Chat.Read.All, Chat.ReadWrite.All</span></span>   |

> [!NOTE]
> <span data-ttu-id="0061c-117">Com as permissões do aplicativo, há suporte para um único chat, mas [obter uma lista de chats](chat-list.md) não é.</span><span class="sxs-lookup"><span data-stu-id="0061c-117">With application permissions, getting a single chat is supported, but [getting a list of chats](chat-list.md) is not.</span></span>

> [!NOTE]
> <span data-ttu-id="0061c-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0061c-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="0061c-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="0061c-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="0061c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0061c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0061c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0061c-121">Optional query parameters</span></span>

<span data-ttu-id="0061c-122">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0061c-122">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0061c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0061c-123">Request headers</span></span>

| <span data-ttu-id="0061c-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0061c-124">Header</span></span>       | <span data-ttu-id="0061c-125">Valor</span><span class="sxs-lookup"><span data-stu-id="0061c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0061c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0061c-126">Authorization</span></span>  | <span data-ttu-id="0061c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0061c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0061c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0061c-129">Request body</span></span>

<span data-ttu-id="0061c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0061c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0061c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0061c-131">Response</span></span>

<span data-ttu-id="0061c-132">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0061c-132">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0061c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0061c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0061c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0061c-134">Request</span></span>
<span data-ttu-id="0061c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0061c-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0061c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0061c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```
# <a name="c"></a>[<span data-ttu-id="0061c-137">C#</span><span class="sxs-lookup"><span data-stu-id="0061c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0061c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0061c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0061c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0061c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0061c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0061c-140">Response</span></span>
<span data-ttu-id="0061c-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0061c-141">Here is an example of the response.</span></span> 

><span data-ttu-id="0061c-142">**Observação:** O objeto de resposta mostrado aqui é encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0061c-142">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="0061c-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0061c-143">All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
