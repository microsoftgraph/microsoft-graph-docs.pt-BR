---
title: Receber chatMessagem em um canal ou chat
description: Recupere uma única mensagem (sem suas respostas) em um canal ou chat.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5d8ab3e40de66e2187701f67d1460eef5af14c8c
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51583019"
---
# <a name="get-chatmessage-in-a-channel-or-chat"></a><span data-ttu-id="83567-103">Receber chatMessagem em um canal ou chat</span><span class="sxs-lookup"><span data-stu-id="83567-103">Get chatMessage in a channel or chat</span></span>

<span data-ttu-id="83567-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83567-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83567-105">Recupere uma única [mensagem](../resources/chatmessage.md) ou uma [resposta de mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md) ou um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="83567-105">Retrieve a single [message](../resources/chatmessage.md) or a [message reply](../resources/chatmessage.md) in a [channel](../resources/channel.md) or a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83567-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="83567-106">Permissions</span></span>

<span data-ttu-id="83567-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83567-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="83567-109">Permissões para o canal</span><span class="sxs-lookup"><span data-stu-id="83567-109">Permissions for channel</span></span>

| <span data-ttu-id="83567-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83567-110">Permission type</span></span>                        | <span data-ttu-id="83567-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83567-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="83567-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83567-112">Delegated (work or school account)</span></span>| <span data-ttu-id="83567-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="83567-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="83567-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83567-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83567-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83567-115">Not supported.</span></span>|
|<span data-ttu-id="83567-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83567-116">Application</span></span>| <span data-ttu-id="83567-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83567-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="83567-118">Permissões para o chat</span><span class="sxs-lookup"><span data-stu-id="83567-118">Permissions for chat</span></span>

| <span data-ttu-id="83567-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83567-119">Permission type</span></span>                        | <span data-ttu-id="83567-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83567-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="83567-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83567-121">Delegated (work or school account)</span></span>| <span data-ttu-id="83567-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83567-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="83567-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83567-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83567-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83567-124">Not supported.</span></span>|
|<span data-ttu-id="83567-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83567-125">Application</span></span>| <span data-ttu-id="83567-126">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83567-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="83567-127">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="83567-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="83567-128">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="83567-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="83567-129">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="83567-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="83567-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83567-130">HTTP request</span></span>

<span data-ttu-id="83567-131">**Obter mensagens em um canal**</span><span class="sxs-lookup"><span data-stu-id="83567-131">**Get message in a channel**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}
```

<span data-ttu-id="83567-132">**Obter mensagens em um chat**</span><span class="sxs-lookup"><span data-stu-id="83567-132">**Get message in a chat**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}
GET /users/{user-id}/chats/{chat-id}/messages/{message-id}
GET /me/chats/{chat-id}/messages/{message-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83567-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83567-133">Optional query parameters</span></span>
<span data-ttu-id="83567-134">Este método não é compatível com os [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83567-134">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83567-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83567-135">Request headers</span></span>
| <span data-ttu-id="83567-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83567-136">Header</span></span>       | <span data-ttu-id="83567-137">Valor</span><span class="sxs-lookup"><span data-stu-id="83567-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83567-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="83567-138">Authorization</span></span>  | <span data-ttu-id="83567-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83567-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83567-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83567-141">Request body</span></span>
<span data-ttu-id="83567-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83567-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83567-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="83567-143">Response</span></span>

<span data-ttu-id="83567-144">Se bem-sucedido, esse método retornará um `200 OK` código de resposta e um objeto [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83567-144">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83567-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="83567-145">Examples</span></span>

### <a name="example-1-get-a-message-in-a-chat"></a><span data-ttu-id="83567-146">Exemplo 1: obter uma mensagem em um chat.</span><span class="sxs-lookup"><span data-stu-id="83567-146">Example 1: Get a message in a chat</span></span>
#### <a name="request"></a><span data-ttu-id="83567-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83567-147">Request</span></span>
<span data-ttu-id="83567-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83567-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_1"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces/messages/1612289992105
```

#### <a name="response"></a><span data-ttu-id="83567-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="83567-149">Response</span></span>
<span data-ttu-id="83567-150">O exemplo a seguir mostra a resposta.`chatId`</span><span class="sxs-lookup"><span data-stu-id="83567-150">The following example shows the response.`chatId`</span></span> <span data-ttu-id="83567-151">identifica o [chat](../resources/chat.md) que contém essa mensagem.</span><span class="sxs-lookup"><span data-stu-id="83567-151">identifies the [chat](../resources/chat.md) that contains this message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5%40unq.gbl.spaces')/messages/$entity",
    "id": "1612289992105",
    "replyToId": null,
    "etag": "1612289992105",
    "messageType": "message",
    "createdDateTime": "2021-02-02T18:19:52.105Z",
    "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
    "importance": "normal",
    "locale": "en-us",
    "webUrl": null,
    "channelIdentity": null,
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Robin Kline",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "text",
        "content": "test"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-get-a-message-in-a-channel"></a><span data-ttu-id="83567-152">Exemplo 2: obter uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="83567-152">Example 2: Get a message in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="83567-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83567-153">Request</span></span>
<span data-ttu-id="83567-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83567-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_2"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349
```

#### <a name="response"></a><span data-ttu-id="83567-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="83567-155">Response</span></span>
<span data-ttu-id="83567-156">O exemplo a seguir mostra a resposta.`channelIdentity`</span><span class="sxs-lookup"><span data-stu-id="83567-156">The following example shows the response.`channelIdentity`</span></span> <span data-ttu-id="83567-157">identifica a [equipe](../resources/team.md) e o [canal](../resources/channel.md) que contêm essa mensagem.</span><span class="sxs-lookup"><span data-stu-id="83567-157">identifies the [team](../resources/team.md) and [channel](../resources/channel.md) that contains this message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1614618259349",
    "replyToId": null,
    "etag": "1614618259349",
    "messageType": "message",
    "createdDateTime": "2021-03-01T17:04:19.349Z",
    "lastModifiedDateTime": "2021-03-01T17:04:19.349Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1614618259349?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1614618259349&parentMessageId=1614618259349",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Robin Kline",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<div><div><div><span><img height=\"250\" src=\"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents/aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv/$value\" width=\"424.6575342465753\" style=\"vertical-align:bottom; width:424px; height:250px\"></span></div></div></div>"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-3-get-reply-to-a-message-in-a-channel"></a><span data-ttu-id="83567-158">Exemplo 3: obter resposta a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="83567-158">Example 3: Get reply to a message in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="83567-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83567-159">Request</span></span>
<span data-ttu-id="83567-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83567-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_3"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1612509044972/replies/1613671348387
```

#### <a name="response"></a><span data-ttu-id="83567-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="83567-161">Response</span></span>
<span data-ttu-id="83567-162">O exemplo a seguir mostra a resposta.`replyToId`</span><span class="sxs-lookup"><span data-stu-id="83567-162">The following example shows the response.`replyToId`</span></span> <span data-ttu-id="83567-163">contém a `id` da mensagem raiz.</span><span class="sxs-lookup"><span data-stu-id="83567-163">contains the `id` of the root message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1612509044972')/replies/$entity",
    "id": "1613671348387",
    "replyToId": "1612509044972",
    "etag": "1613671348387",
    "messageType": "message",
    "createdDateTime": "2021-02-18T18:02:28.387Z",
    "lastModifiedDateTime": "2021-02-18T18:02:28.387Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1613671348387?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1613671348387&parentMessageId=1612509044972",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Robin Kline",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<div><div>Test</div></div>"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a><span data-ttu-id="83567-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="83567-164">See also</span></span>

- [<span data-ttu-id="83567-165">Listar mensagens em um canal</span><span class="sxs-lookup"><span data-stu-id="83567-165">List messages in a channel</span></span>](channel-list-messages.md)
- [<span data-ttu-id="83567-166">Listar mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="83567-166">List messages in a chat</span></span>](chat-list-messages.md)
- [<span data-ttu-id="83567-167">Enviar mensagem em um canal ou um chat</span><span class="sxs-lookup"><span data-stu-id="83567-167">Send message in a channel or a chat</span></span>](chatmessage-post.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a single message (without its replies) in a channel or a chat.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->