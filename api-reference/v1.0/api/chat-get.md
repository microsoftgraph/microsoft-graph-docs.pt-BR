---
title: Obter bate-papo
description: Recupere um único bate-papo.
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 866bfb702ff80474ee9791a230d14179a82c2faf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950133"
---
# <a name="get-chat"></a><span data-ttu-id="6e1c0-103">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="6e1c0-103">Get chat</span></span>

<span data-ttu-id="6e1c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e1c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e1c0-105">Recupere um único [bate-papo](../resources/chat.md) (sem suas mensagens).</span><span class="sxs-lookup"><span data-stu-id="6e1c0-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e1c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e1c0-106">Permissions</span></span>

<span data-ttu-id="6e1c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e1c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6e1c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e1c0-109">Permission type</span></span>      | <span data-ttu-id="6e1c0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e1c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e1c0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e1c0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6e1c0-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e1c0-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="6e1c0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e1c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e1c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-114">Not supported.</span></span>    |
|<span data-ttu-id="6e1c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e1c0-115">Application</span></span> | <span data-ttu-id="6e1c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e1c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e1c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{chat-id}
GET /users/{user-id}/chats/{chat-id}
GET /chats/{chat-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e1c0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e1c0-118">Optional query parameters</span></span>

<span data-ttu-id="6e1c0-119">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-119">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e1c0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e1c0-120">Request headers</span></span>

| <span data-ttu-id="6e1c0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e1c0-121">Header</span></span>       | <span data-ttu-id="6e1c0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e1c0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e1c0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e1c0-123">Authorization</span></span>  | <span data-ttu-id="6e1c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e1c0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e1c0-126">Request body</span></span>

<span data-ttu-id="6e1c0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e1c0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e1c0-128">Response</span></span>

<span data-ttu-id="6e1c0-129">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e1c0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e1c0-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6e1c0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e1c0-131">Request</span></span>
<span data-ttu-id="6e1c0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e1c0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e1c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces
```
# <a name="c"></a>[<span data-ttu-id="6e1c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="6e1c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e1c0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e1c0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e1c0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e1c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e1c0-137">Java</span><span class="sxs-lookup"><span data-stu-id="6e1c0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="6e1c0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e1c0-138">Response</span></span>
<span data-ttu-id="6e1c0-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-139">Here is an example of the response.</span></span> 

><span data-ttu-id="6e1c0-140">**Observação:** O objeto de resposta mostrado aqui é encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-140">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="6e1c0-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e1c0-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats/$entity",
    "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2019-04-18T23:51:42.099Z",
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z",
    "chatType": "oneOnOne"
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


