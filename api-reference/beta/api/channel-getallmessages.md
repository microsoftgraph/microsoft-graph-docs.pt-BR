---
title: 'channel: getAllMessages'
description: Recupere todas as mensagens entre os canais de uma equipe.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3174401b2d25bf2c7c00f0cffca2c048af7deca6
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546116"
---
# <a name="channel-getallmessages"></a><span data-ttu-id="a8428-103">channel: getAllMessages</span><span class="sxs-lookup"><span data-stu-id="a8428-103">channel: getAllMessages</span></span>

<span data-ttu-id="a8428-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8428-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8428-105">Recupere as [mensagens](../resources/chatmessage.md) em todos os [canais](../resources/channel.md) de uma [equipe](../resources/team.md), incluindo texto, áudio, e conversas de vídeo.</span><span class="sxs-lookup"><span data-stu-id="a8428-105">Retrieve [messages](../resources/chatmessage.md) across all [channels](../resources/channel.md) in a [team](../resources/team.md), including text, audio, and video conversations.</span></span> 

<span data-ttu-id="a8428-106">Para saber mais sobre o uso das APIs de exportação do Microsoft Teams para exportar conteúdo, consulte [Exportar conteúdo com as APIs de exportação do Microsoft Teams](/microsoftteams/export-teams-content).</span><span class="sxs-lookup"><span data-stu-id="a8428-106">To learn more about using the Microsoft Teams export APIs to export content, see [Export content with the Microsoft Teams export APIs](/microsoftteams/export-teams-content).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8428-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8428-107">Permissions</span></span>

<span data-ttu-id="a8428-p101">As seguintes permissões são obrigatórias para chamar esta API. Para saber mais, incluindo como escolher as permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8428-p101">The following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8428-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8428-110">Permission type</span></span>      | <span data-ttu-id="a8428-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8428-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8428-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8428-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a8428-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8428-113">Not supported</span></span> |
|<span data-ttu-id="a8428-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8428-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8428-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8428-115">Not supported</span></span> |
|<span data-ttu-id="a8428-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8428-116">Application</span></span> | <span data-ttu-id="a8428-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8428-117">ChannelMessage.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="a8428-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8428-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="a8428-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="a8428-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="a8428-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8428-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8428-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8428-121">Optional query parameters</span></span>

<span data-ttu-id="a8428-122">Você pode usar o parâmetro de consulta [$top](/graph/query-parameters#top-parameter) para controlar o número de itens por resposta.</span><span class="sxs-lookup"><span data-stu-id="a8428-122">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span>
<span data-ttu-id="a8428-123">Além disso, [$filter](/graph/query-parameters#filter-parameter) é suportado com **dateTime** intervalo de consulta em **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="a8428-123">Additionally, [$filter](/graph/query-parameters#filter-parameter) is supported with **dateTime** range query on **lastModifiedDateTime**.</span></span> <span data-ttu-id="a8428-124">No momento, não há suporte para os outros [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a8428-124">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-body"></a><span data-ttu-id="a8428-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8428-125">Request body</span></span>

<span data-ttu-id="a8428-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8428-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8428-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8428-127">Response</span></span>

<span data-ttu-id="a8428-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e também retornará todas as mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="a8428-128">If successful, this method returns a `200 OK` response code and also returns all the messages in the channel.</span></span>

## <a name="example"></a><span data-ttu-id="a8428-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8428-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8428-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8428-130">Request</span></span>

<span data-ttu-id="a8428-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8428-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8428-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8428-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allchannelmessages_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages
```
# <a name="c"></a>[<span data-ttu-id="a8428-133">C#</span><span class="sxs-lookup"><span data-stu-id="a8428-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allchannelmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8428-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8428-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allchannelmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8428-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8428-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allchannelmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8428-136">Java</span><span class="sxs-lookup"><span data-stu-id="a8428-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allchannelmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8428-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8428-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true,
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages?$skip=2",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1616990417393",
            "replyToId": null,
            "etag": "1616990417393",
            "messageType": "message",
            "createdDateTime": "2021-03-29T04:00:17.393Z",
            "lastModifiedDateTime": "2021-03-29T04:00:17.393Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3Ad5d2708d408c41d98424c1c354c19db3%40thread.tacv2/1616990417393?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990417393&parentMessageId=1616990417393",
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
                "content": "Test message"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:d5d2708d408c41d98424c1c354c19db3@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1616990171266",
            "replyToId": "1616990032035",
            "etag": "1616990171266",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:56:11.266Z",
            "lastModifiedDateTime": "2021-03-29T03:56:11.266Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616990171266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990171266&parentMessageId=1616990032035",
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
                "content": "Hello World"
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
  "description": "channels: getallmessages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
