---
title: Obter bate-papo
description: Recupere um único bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eb447e7f97f443119cf8ff29b467787a64323149
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863099"
---
# <a name="get-chat"></a><span data-ttu-id="4f2e2-103">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="4f2e2-103">Get chat</span></span>

<span data-ttu-id="4f2e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f2e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f2e2-105">Recupere um único [bate-papo](../resources/chat.md) (sem suas mensagens).</span><span class="sxs-lookup"><span data-stu-id="4f2e2-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f2e2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f2e2-106">Permissions</span></span>

<span data-ttu-id="4f2e2-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4f2e2-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f2e2-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4f2e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f2e2-109">Permission type</span></span>      | <span data-ttu-id="4f2e2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f2e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f2e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f2e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f2e2-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f2e2-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="4f2e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f2e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f2e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-114">Not supported.</span></span>    |
|<span data-ttu-id="4f2e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f2e2-115">Application</span></span> | <span data-ttu-id="4f2e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f2e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2e2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f2e2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f2e2-118">Optional query parameters</span></span>

<span data-ttu-id="4f2e2-119">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-119">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f2e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2e2-120">Request headers</span></span>

| <span data-ttu-id="4f2e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f2e2-121">Header</span></span>       | <span data-ttu-id="4f2e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f2e2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f2e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f2e2-123">Authorization</span></span>  | <span data-ttu-id="4f2e2-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-124">Bearer {token}.</span></span> <span data-ttu-id="4f2e2-125">Required.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f2e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2e2-126">Request body</span></span>

<span data-ttu-id="4f2e2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f2e2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f2e2-128">Response</span></span>

<span data-ttu-id="4f2e2-129">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f2e2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f2e2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f2e2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2e2-131">Request</span></span>
<span data-ttu-id="4f2e2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4f2e2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2e2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```
# <a name="c"></a>[<span data-ttu-id="4f2e2-134">C#</span><span class="sxs-lookup"><span data-stu-id="4f2e2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f2e2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f2e2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f2e2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f2e2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f2e2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f2e2-137">Response</span></span>
<span data-ttu-id="4f2e2-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-138">Here is an example of the response.</span></span> 

><span data-ttu-id="4f2e2-139">**Observação:** O objeto de resposta mostrado aqui é encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-139">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="4f2e2-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f2e2-140">All the properties will be returned from an actual call.</span></span>
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
