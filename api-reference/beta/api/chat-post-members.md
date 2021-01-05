---
title: Adicionar membro a um chat
description: Adicionar um conversationMember a um chat.
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: eae4e307204fde0e897535ee414fba42cf1ce788
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753210"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="786f5-103">Adicionar membro a um chat</span><span class="sxs-lookup"><span data-stu-id="786f5-103">Add member to a chat</span></span>

<span data-ttu-id="786f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="786f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="786f5-105">Adicionar um [conversationMember](../resources/conversationmember.md) a um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="786f5-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="786f5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="786f5-106">Permissions</span></span>

<span data-ttu-id="786f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="786f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="786f5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="786f5-109">Permission Type</span></span>|<span data-ttu-id="786f5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="786f5-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="786f5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="786f5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="786f5-112">ChatMember. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="786f5-112">ChatMember.ReadWrite</span></span> |
|<span data-ttu-id="786f5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="786f5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="786f5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="786f5-114">Not supported.</span></span>|
|<span data-ttu-id="786f5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="786f5-115">Application</span></span>| <span data-ttu-id="786f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="786f5-116">Not supported.</span></span> |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="786f5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="786f5-117">Request headers</span></span>

| <span data-ttu-id="786f5-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="786f5-118">Header</span></span>       | <span data-ttu-id="786f5-119">Valor</span><span class="sxs-lookup"><span data-stu-id="786f5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="786f5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="786f5-120">Authorization</span></span>  | <span data-ttu-id="786f5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="786f5-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="786f5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="786f5-123">Content-Type</span></span>|<span data-ttu-id="786f5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="786f5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="786f5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="786f5-126">Request body</span></span>

<span data-ttu-id="786f5-127">No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="786f5-127">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="786f5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="786f5-128">Response</span></span>

<span data-ttu-id="786f5-129">Se tiver êxito, este método retornará um `201 Created` código de resposta e um cabeçalho de local que fornece um caminho de URL para o objeto membro recém-criado.</span><span class="sxs-lookup"><span data-stu-id="786f5-129">If successful, this method returns a `201 Created` response code and a Location header that provides a url path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="786f5-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="786f5-130">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="786f5-131">Exemplo 1: adicionar um único membro a um chat e especificar o TimeSpan para o histórico da conversa</span><span class="sxs-lookup"><span data-stu-id="786f5-131">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="786f5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="786f5-132">Request</span></span>

<span data-ttu-id="786f5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="786f5-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="786f5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="786f5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
}
```
# <a name="javascript"></a>[<span data-ttu-id="786f5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="786f5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="786f5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="786f5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="786f5-137">Java</span><span class="sxs-lookup"><span data-stu-id="786f5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="786f5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="786f5-138">Response</span></span>

<span data-ttu-id="786f5-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="786f5-139">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="786f5-140">Exemplo 2: adicionando um único membro a um chat do Microsoft Teams, não compartilhando histórico de chat</span><span class="sxs-lookup"><span data-stu-id="786f5-140">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="786f5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="786f5-141">Request</span></span>

<span data-ttu-id="786f5-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="786f5-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="786f5-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="786f5-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```

# <a name="javascript"></a>[<span data-ttu-id="786f5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="786f5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="786f5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="786f5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="786f5-146">Java</span><span class="sxs-lookup"><span data-stu-id="786f5-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="786f5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="786f5-147">Response</span></span>

<span data-ttu-id="786f5-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="786f5-148">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="786f5-149">Exemplo 3: adicionando um único membro a um chat do Microsoft Teams, compartilhando todo o histórico do chat</span><span class="sxs-lookup"><span data-stu-id="786f5-149">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="786f5-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="786f5-150">Request</span></span>

<span data-ttu-id="786f5-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="786f5-151">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="786f5-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="786f5-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z"
}
```
# <a name="javascript"></a>[<span data-ttu-id="786f5-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="786f5-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="786f5-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="786f5-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="786f5-155">Java</span><span class="sxs-lookup"><span data-stu-id="786f5-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="786f5-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="786f5-156">Response</span></span>

<span data-ttu-id="786f5-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="786f5-157">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```


