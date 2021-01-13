---
title: Adicionar membro a um chat
description: Adicione um conversationMember a um chat.
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f3fe6c34d81e34f614f914780886902a8bf563c2
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843770"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="fa21f-103">Adicionar membro a um chat</span><span class="sxs-lookup"><span data-stu-id="fa21f-103">Add member to a chat</span></span>

<span data-ttu-id="fa21f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa21f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa21f-105">Adicione um [conversationMember](../resources/conversationmember.md) a um [chat.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="fa21f-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa21f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fa21f-106">Permissions</span></span>

<span data-ttu-id="fa21f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa21f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa21f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa21f-109">Permission Type</span></span>|<span data-ttu-id="fa21f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa21f-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="fa21f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa21f-111">Delegated (work or school account)</span></span>| <span data-ttu-id="fa21f-112">ChatMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa21f-112">ChatMember.ReadWrite</span></span> |
|<span data-ttu-id="fa21f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa21f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa21f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa21f-114">Not supported.</span></span>|
|<span data-ttu-id="fa21f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa21f-115">Application</span></span>| <span data-ttu-id="fa21f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa21f-116">Not supported.</span></span> |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="fa21f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa21f-117">Request headers</span></span>

| <span data-ttu-id="fa21f-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa21f-118">Header</span></span>       | <span data-ttu-id="fa21f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="fa21f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa21f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa21f-120">Authorization</span></span>  | <span data-ttu-id="fa21f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa21f-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="fa21f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa21f-123">Content-Type</span></span>|<span data-ttu-id="fa21f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa21f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa21f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa21f-126">Request body</span></span>

<span data-ttu-id="fa21f-127">No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="fa21f-127">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fa21f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa21f-128">Response</span></span>

<span data-ttu-id="fa21f-129">Se bem-sucedido, este método retorna um código de resposta e um título de local que fornece um caminho `201 Created` de URL para o objeto membro recém-criado.</span><span class="sxs-lookup"><span data-stu-id="fa21f-129">If successful, this method returns a `201 Created` response code and a Location header that provides a URL path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="fa21f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa21f-130">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="fa21f-131">Exemplo 1: Adicionar um único membro a um chat e especificar o período de tempo para o histórico da conversa</span><span class="sxs-lookup"><span data-stu-id="fa21f-131">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="fa21f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa21f-132">Request</span></span>

<span data-ttu-id="fa21f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa21f-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fa21f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa21f-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fa21f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa21f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa21f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa21f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa21f-137">Java</span><span class="sxs-lookup"><span data-stu-id="fa21f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fa21f-138">C#</span><span class="sxs-lookup"><span data-stu-id="fa21f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-specific-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="fa21f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa21f-139">Response</span></span>

<span data-ttu-id="fa21f-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa21f-140">Here is an example of the response.</span></span>

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

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="fa21f-141">Exemplo 2: Adicionando um único membro a um chat do Microsoft Teams, compartilhando sem histórico de chat</span><span class="sxs-lookup"><span data-stu-id="fa21f-141">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="fa21f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa21f-142">Request</span></span>

<span data-ttu-id="fa21f-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa21f-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fa21f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa21f-144">HTTP</span></span>](#tab/http)
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

# <a name="javascript"></a>[<span data-ttu-id="fa21f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa21f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa21f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa21f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa21f-147">Java</span><span class="sxs-lookup"><span data-stu-id="fa21f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fa21f-148">C#</span><span class="sxs-lookup"><span data-stu-id="fa21f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-no-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="fa21f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa21f-149">Response</span></span>

<span data-ttu-id="fa21f-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa21f-150">Here is an example of the response.</span></span>

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

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="fa21f-151">Exemplo 3: Adicionar um único membro a um chat do Microsoft Teams, compartilhando todo o histórico do chat</span><span class="sxs-lookup"><span data-stu-id="fa21f-151">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="fa21f-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa21f-152">Request</span></span>

<span data-ttu-id="fa21f-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa21f-153">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fa21f-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa21f-154">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fa21f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa21f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa21f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa21f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa21f-157">Java</span><span class="sxs-lookup"><span data-stu-id="fa21f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fa21f-158">C#</span><span class="sxs-lookup"><span data-stu-id="fa21f-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-all-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="fa21f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa21f-159">Response</span></span>

<span data-ttu-id="fa21f-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa21f-160">Here is an example of the response.</span></span>

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


