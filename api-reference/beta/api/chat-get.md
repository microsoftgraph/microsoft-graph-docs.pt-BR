---
title: Obter bate-papo
description: Recupere um único bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d444bb967aea89206c4c0a47d82cdcb6218c5e89
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287707"
---
# <a name="get-chat"></a><span data-ttu-id="6030e-103">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="6030e-103">Get chat</span></span>

<span data-ttu-id="6030e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6030e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6030e-105">Recupere um único [bate-papo](../resources/chat.md) (sem suas mensagens).</span><span class="sxs-lookup"><span data-stu-id="6030e-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="6030e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6030e-106">Permissions</span></span>

<span data-ttu-id="6030e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6030e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6030e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6030e-109">Permission type</span></span>      | <span data-ttu-id="6030e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6030e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6030e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6030e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6030e-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6030e-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="6030e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6030e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6030e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6030e-114">Not supported.</span></span>    |
|<span data-ttu-id="6030e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6030e-115">Application</span></span> | <span data-ttu-id="6030e-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6030e-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="6030e-117">Com as permissões do aplicativo, há suporte para um único chat, mas [obter uma lista de chats](chat-list.md) não é.</span><span class="sxs-lookup"><span data-stu-id="6030e-117">With application permissions, getting a single chat is supported, but [getting a list of chats](chat-list.md) is not.</span></span>

> [!NOTE]
> <span data-ttu-id="6030e-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6030e-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="6030e-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="6030e-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="6030e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6030e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6030e-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6030e-121">Optional query parameters</span></span>

<span data-ttu-id="6030e-122">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6030e-122">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6030e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6030e-123">Request headers</span></span>

| <span data-ttu-id="6030e-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6030e-124">Header</span></span>       | <span data-ttu-id="6030e-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6030e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6030e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6030e-126">Authorization</span></span>  | <span data-ttu-id="6030e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6030e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6030e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6030e-129">Request body</span></span>

<span data-ttu-id="6030e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6030e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6030e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6030e-131">Response</span></span>

<span data-ttu-id="6030e-132">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6030e-132">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6030e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6030e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6030e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6030e-134">Request</span></span>
<span data-ttu-id="6030e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6030e-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6030e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6030e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```
# <a name="c"></a>[<span data-ttu-id="6030e-137">C#</span><span class="sxs-lookup"><span data-stu-id="6030e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6030e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6030e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6030e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6030e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6030e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6030e-140">Response</span></span>
<span data-ttu-id="6030e-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6030e-141">Here is an example of the response.</span></span> 

><span data-ttu-id="6030e-142">**Observação:** O objeto de resposta mostrado aqui é encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6030e-142">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="6030e-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6030e-143">All the properties will be returned from an actual call.</span></span>
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
