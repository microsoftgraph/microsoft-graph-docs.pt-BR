---
title: Adicionar membro a um chat
description: Adicione um conversationMember a um chat.
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 04ec5dadc97cb2f7a3d8b054a99852a749e3474f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777311"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="6fe3e-103">Adicionar membro a um chat</span><span class="sxs-lookup"><span data-stu-id="6fe3e-103">Add member to a chat</span></span>

<span data-ttu-id="6fe3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fe3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fe3e-105">Adicione um [conversationMember](../resources/conversationmember.md) a um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="6fe3e-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fe3e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fe3e-106">Permissions</span></span>

<span data-ttu-id="6fe3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fe3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe3e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fe3e-109">Permission Type</span></span>|<span data-ttu-id="6fe3e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fe3e-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="6fe3e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fe3e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="6fe3e-112">ChatMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fe3e-112">ChatMember.ReadWrite</span></span> |
|<span data-ttu-id="6fe3e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fe3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fe3e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-114">Not supported.</span></span>|
|<span data-ttu-id="6fe3e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fe3e-115">Application</span></span>| <span data-ttu-id="6fe3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-116">Not supported.</span></span> |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="6fe3e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe3e-117">Request headers</span></span>

| <span data-ttu-id="6fe3e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fe3e-118">Header</span></span>       | <span data-ttu-id="6fe3e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="6fe3e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fe3e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fe3e-120">Authorization</span></span>  | <span data-ttu-id="6fe3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="6fe3e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6fe3e-123">Content-Type</span></span>|<span data-ttu-id="6fe3e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fe3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe3e-126">Request body</span></span>

<span data-ttu-id="6fe3e-127">No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="6fe3e-127">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6fe3e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fe3e-128">Response</span></span>

<span data-ttu-id="6fe3e-129">Se tiver êxito, este método retornará um código de resposta e um header location que fornece um caminho `201 Created` de URL para o objeto membro recém-criado.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-129">If successful, this method returns a `201 Created` response code and a Location header that provides a URL path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="6fe3e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6fe3e-130">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="6fe3e-131">Exemplo 1: adicionar um único membro a um chat e especificar o tempo de tempo para o histórico da conversa</span><span class="sxs-lookup"><span data-stu-id="6fe3e-131">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="6fe3e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe3e-132">Request</span></span>

<span data-ttu-id="6fe3e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-133">Here is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
}
```


#### <a name="response"></a><span data-ttu-id="6fe3e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fe3e-134">Response</span></span>

<span data-ttu-id="6fe3e-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-135">Here is an example of the response.</span></span>

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

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="6fe3e-136">Exemplo 2: adicionar um único membro a um chat do Microsoft Teams, sem compartilhar nenhum histórico de chat</span><span class="sxs-lookup"><span data-stu-id="6fe3e-136">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="6fe3e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe3e-137">Request</span></span>

<span data-ttu-id="6fe3e-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-138">Here is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```


#### <a name="response"></a><span data-ttu-id="6fe3e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fe3e-139">Response</span></span>

<span data-ttu-id="6fe3e-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-140">Here is an example of the response.</span></span>

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

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="6fe3e-141">Exemplo 3: adicionar um único membro a um chat do Microsoft Teams, compartilhando todo o histórico do chat</span><span class="sxs-lookup"><span data-stu-id="6fe3e-141">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="6fe3e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe3e-142">Request</span></span>

<span data-ttu-id="6fe3e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-143">Here is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z"
}
```


#### <a name="response"></a><span data-ttu-id="6fe3e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fe3e-144">Response</span></span>

<span data-ttu-id="6fe3e-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fe3e-145">Here is an example of the response.</span></span>

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


