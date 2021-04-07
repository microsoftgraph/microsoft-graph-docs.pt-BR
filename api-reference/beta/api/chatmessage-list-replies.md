---
title: Listar respostas de mensagem de canal
description: Listar todas as respostas de uma mensagem em um canal de uma equipe.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d47e5e1d063ef0aa43ca64f0a99aa422031677a5
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610152"
---
# <a name="list-replies"></a><span data-ttu-id="3c138-103">Listar respostas</span><span class="sxs-lookup"><span data-stu-id="3c138-103">List replies</span></span>

<span data-ttu-id="3c138-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c138-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c138-105">Listar todas as respostas a uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="3c138-105">List all the replies to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="3c138-106">Este método lista apenas as respostas da mensagem especificada, se alguma.</span><span class="sxs-lookup"><span data-stu-id="3c138-106">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="3c138-107">Para obter a mensagem em si, basta chamar [get channel message](chatmessage-get.md).</span><span class="sxs-lookup"><span data-stu-id="3c138-107">To get the message itself, simply call [get channel message](chatmessage-get.md).</span></span>

> <span data-ttu-id="3c138-108">**Observação**: Esta API oferece suporte à inscrição para alterações (criar, atualizar e excluir) usando [notificações de alteração](../resources/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="3c138-108">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="3c138-109">Isso permite aos chamadores assinar e obter alterações em tempo real.</span><span class="sxs-lookup"><span data-stu-id="3c138-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="3c138-110">Para obter detalhes, confira [obter notificações de](/graph/teams-changenotifications-chatmessage)de mensagens.</span><span class="sxs-lookup"><span data-stu-id="3c138-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c138-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="3c138-111">Permissions</span></span>
<span data-ttu-id="3c138-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c138-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c138-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c138-114">Permission Type</span></span>|<span data-ttu-id="3c138-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c138-115">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3c138-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c138-116">Delegated (work or school account)</span></span>| <span data-ttu-id="3c138-117">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c138-117">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="3c138-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c138-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c138-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c138-119">Not supported.</span></span>|
|<span data-ttu-id="3c138-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c138-120">Application</span></span>| <span data-ttu-id="3c138-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c138-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="3c138-122">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="3c138-122">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="3c138-123">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3c138-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="3c138-124">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="3c138-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="3c138-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c138-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c138-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c138-126">Optional query parameters</span></span>

<span data-ttu-id="3c138-127">Você pode usar o parâmetro de consulta [$top](/graph/query-parameters#top-parameter) para controlar o número de itens por resposta.</span><span class="sxs-lookup"><span data-stu-id="3c138-127">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="3c138-128">O valor máximo `$top` permitido é 50.</span><span class="sxs-lookup"><span data-stu-id="3c138-128">Maximum allowed `$top` value is 50.</span></span>
<span data-ttu-id="3c138-129">No momento, não há suporte para os outros [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c138-129">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c138-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c138-130">Request headers</span></span>
| <span data-ttu-id="3c138-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c138-131">Header</span></span>       | <span data-ttu-id="3c138-132">Valor</span><span class="sxs-lookup"><span data-stu-id="3c138-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c138-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c138-133">Authorization</span></span>  | <span data-ttu-id="3c138-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c138-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c138-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c138-136">Request body</span></span>
<span data-ttu-id="3c138-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c138-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c138-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c138-138">Response</span></span>
<span data-ttu-id="3c138-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c138-139">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c138-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c138-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c138-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c138-141">Request</span></span>
<span data-ttu-id="3c138-142">Neste exemplo, a mensagem especificada tem três respostas.</span><span class="sxs-lookup"><span data-stu-id="3c138-142">In this example, the specified message has three replies.</span></span>


# <a name="http"></a>[<span data-ttu-id="3c138-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c138-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_listmessagereplies_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616989510408/replies
```
# <a name="c"></a>[<span data-ttu-id="3c138-144">C#</span><span class="sxs-lookup"><span data-stu-id="3c138-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-listmessagereplies-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c138-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c138-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-listmessagereplies-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c138-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c138-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-listmessagereplies-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c138-147">Java</span><span class="sxs-lookup"><span data-stu-id="3c138-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-listmessagereplies-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c138-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c138-148">Response</span></span>
<span data-ttu-id="3c138-149">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c138-149">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616989510408')/replies",
    "@odata.count": 3,
    "value": [
        {
            "id": "1616989753153",
            "replyToId": "1616989510408",
            "etag": "1616989753153",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:13.153Z",
            "lastModifiedDateTime": "2021-03-29T03:49:13.153Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989753153?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989753153&parentMessageId=1616989510408",
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
                "content": "Reply3"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1616989750004",
            "replyToId": "1616989510408",
            "etag": "1616989750004",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:10.004Z",
            "lastModifiedDateTime": "2021-03-29T03:49:10.004Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989750004?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989750004&parentMessageId=1616989510408",
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
                "content": "Reply2"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1616989747416",
            "replyToId": "1616989510408",
            "etag": "1616989747416",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:07.416Z",
            "lastModifiedDateTime": "2021-03-29T03:49:07.416Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989747416?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989747416&parentMessageId=1616989510408",
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
                "content": "Reply1"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
