---
title: Obter bate-papo
description: Recupere um único bate-papo.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 90ee56388849759d6371e29c49461a94936788be
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971318"
---
# <a name="get-chat"></a><span data-ttu-id="ca151-103">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="ca151-103">Get chat</span></span>

<span data-ttu-id="ca151-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca151-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca151-105">Recupere um único [bate-papo](../resources/chat.md) (sem suas mensagens).</span><span class="sxs-lookup"><span data-stu-id="ca151-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca151-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca151-106">Permissions</span></span>

<span data-ttu-id="ca151-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca151-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ca151-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca151-109">Permission type</span></span>      | <span data-ttu-id="ca151-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca151-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca151-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca151-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca151-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca151-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="ca151-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca151-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca151-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca151-114">Not supported.</span></span>    |
|<span data-ttu-id="ca151-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca151-115">Application</span></span> | <span data-ttu-id="ca151-116">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca151-116">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="ca151-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ca151-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="ca151-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca151-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{chat-id}
GET /users/{user-id | user-principal-name}/chats/{chat-id}
GET /chats/{chat-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca151-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ca151-119">Optional query parameters</span></span>

<span data-ttu-id="ca151-120">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ca151-120">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca151-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca151-121">Request headers</span></span>

| <span data-ttu-id="ca151-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca151-122">Header</span></span>       | <span data-ttu-id="ca151-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ca151-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca151-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca151-124">Authorization</span></span>  | <span data-ttu-id="ca151-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca151-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca151-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca151-127">Request body</span></span>

<span data-ttu-id="ca151-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca151-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca151-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca151-129">Response</span></span>

<span data-ttu-id="ca151-130">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca151-130">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca151-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ca151-131">Examples</span></span>

### <a name="example-1-get-a-group-chat"></a><span data-ttu-id="ca151-132">Exemplo 1: obtenha um chat em grupo</span><span class="sxs-lookup"><span data-stu-id="ca151-132">Example 1: Get a group chat</span></span>
#### <a name="request"></a><span data-ttu-id="ca151-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca151-133">Request</span></span>
<span data-ttu-id="ca151-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca151-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_chat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2
```

#### <a name="response"></a><span data-ttu-id="ca151-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca151-135">Response</span></span>
<span data-ttu-id="ca151-136">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ca151-136">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:b8577894a63548969c5c92bb9c80c5e1@thread.v2",
    "topic": "test group 1",
    "createdDateTime": "2021-04-06T19:49:52.431Z",
    "lastUpdatedDateTime": "2021-04-06T19:54:04.306Z",
    "chatType": "group"
}
```

### <a name="example-2-get-a-users-one-on-one-chat"></a><span data-ttu-id="ca151-137">Exemplo 2: obtenha um bate-papo individual de um usuário</span><span class="sxs-lookup"><span data-stu-id="ca151-137">Example 2: Get a user's one on one chat</span></span>
#### <a name="request"></a><span data-ttu-id="ca151-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca151-138">Request</span></span>
<span data-ttu-id="ca151-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca151-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ca151-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca151-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces
```
# <a name="c"></a>[<span data-ttu-id="ca151-141">C#</span><span class="sxs-lookup"><span data-stu-id="ca151-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca151-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca151-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca151-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca151-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca151-144">Java</span><span class="sxs-lookup"><span data-stu-id="ca151-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca151-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca151-145">Response</span></span>
<span data-ttu-id="ca151-146">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ca151-146">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2019-04-18T23:51:42.099Z",
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z",
    "chatType": "oneOnOne",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces/0?tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34"
}
```

### <a name="example-3-get-a-chat-and-all-its-members"></a><span data-ttu-id="ca151-147">Exemplo 3: obtenha um bate-papo e todos os seus membros</span><span class="sxs-lookup"><span data-stu-id="ca151-147">Example 3: Get a chat and all its members</span></span>
#### <a name="request"></a><span data-ttu-id="ca151-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca151-148">Request</span></span>
<span data-ttu-id="ca151-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca151-149">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ca151-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca151-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_withmembers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2?$expand=members
```
# <a name="c"></a>[<span data-ttu-id="ca151-151">C#</span><span class="sxs-lookup"><span data-stu-id="ca151-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-withmembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca151-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca151-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-withmembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca151-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca151-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-withmembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca151-154">Java</span><span class="sxs-lookup"><span data-stu-id="ca151-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-withmembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca151-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca151-155">Response</span></span>
<span data-ttu-id="ca151-156">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="ca151-156">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats(members())/$entity",
    "id": "19:b8577894a63548969c5c92bb9c80c5e1@thread.v2",
    "topic": "test group 1",
    "createdDateTime": "2021-04-06T19:49:52.431Z",
    "lastUpdatedDateTime": "2021-04-21T17:13:44.033Z",
    "chatType": "group",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3Ab8577894a63548969c5c92bb9c80c5e1@thread.v2/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f",
    "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ab8577894a63548969c5c92bb9c80c5e1%40thread.v2')/members",
    "members": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzhjMGExYTY3LTUwY2UtNDExNC1iYjZjLWRhOWM1ZGJjZjZjYQ==",
            "roles": [
                "owner"
            ],
            "displayName": "John Doe",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
            "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
            "email": "john@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzQ1OTVkMmYyLTdiMzEtNDQ2Yy04NGZkLTliNzk1ZTYzMTE0Yg==",
            "roles": [
                "owner"
            ],
            "displayName": "Test User 1",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
            "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
            "email": "testuser1@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzgyZmU3NzU4LTViYjMtNGYwZC1hNDNmLWU1NTVmZDM5OWM2Zg==",
            "roles": [
                "owner"
            ],
            "displayName": "Test User 2",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
            "userId": "82fe7758-5bb3-4f0d-a43f-e555fd399c6f",
            "email": "testuser2@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==",
            "roles": [
                "owner"
            ],
            "displayName": "Test User 3",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
            "userId": "2c8d2b5c-1849-4066-b57d-e7a0e9e44ec8",
            "email": "testuser3@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzhlYTBlMzhiLWVmYjMtNDc1Ny05MjRhLTVmOTQwNjFjZjhjMg==",
            "roles": [
                "owner"
            ],
            "displayName": "Test User 4",
            "visibleHistoryStartDateTime": "2021-04-20T17:13:43.715Z",
            "userId": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "email": "testuser4@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        }
    ]
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


