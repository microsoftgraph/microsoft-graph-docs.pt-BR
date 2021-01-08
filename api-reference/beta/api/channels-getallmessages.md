---
title: 'canais: getAllMessages'
description: Recuperar todas as mensagens entre os canais de uma equipe.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4ad45990655059db63d90c79225c676e4cf06ec0
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784764"
---
# <a name="channels-getallmessages"></a><span data-ttu-id="7b750-103">canais: getAllMessages</span><span class="sxs-lookup"><span data-stu-id="7b750-103">channels: getAllMessages</span></span>

<span data-ttu-id="7b750-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b750-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b750-105">Recuperar todas as [mensagens](../resources/chatmessage.md) em todos os [canais](../resources/channel.md) de uma [equipe](../resources/team.md), incluindo conversas de texto, áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="7b750-105">Retrieve all [messages](../resources/chatmessage.md) across all [channels](../resources/channel.md) in a [team](../resources/team.md) including text, audio, and video conversations.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b750-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b750-106">Permissions</span></span>

<span data-ttu-id="7b750-107">As permissões a seguir são necessárias para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7b750-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="7b750-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b750-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b750-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b750-109">Permission type</span></span>      | <span data-ttu-id="7b750-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b750-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b750-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b750-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b750-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7b750-112">Not supported</span></span> |
|<span data-ttu-id="7b750-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b750-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b750-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7b750-114">Not supported</span></span> |
|<span data-ttu-id="7b750-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b750-115">Application</span></span> | <span data-ttu-id="7b750-116">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b750-116">ChannelMessage.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="7b750-117">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7b750-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="7b750-118">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="7b750-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="7b750-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b750-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b750-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7b750-120">Optional query parameters</span></span>

<span data-ttu-id="7b750-121">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b750-121">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="7b750-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b750-122">Request body</span></span>

<span data-ttu-id="7b750-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b750-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b750-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b750-124">Response</span></span>

<span data-ttu-id="7b750-125">Se bem-sucedido, este método retornará um código de resposta `200 OK` e também retornará todas as mensagens no canal.</span><span class="sxs-lookup"><span data-stu-id="7b750-125">If successful, this method returns a `200 OK` response code and also returns all the messages in the channel.</span></span>

## <a name="example"></a><span data-ttu-id="7b750-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b750-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b750-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b750-127">Request</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/0e05a7e4-a48d-4615-b0b7-c7494da9ce68/channels/getAllMessages
```

### <a name="response"></a><span data-ttu-id="7b750-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b750-128">Response</span></span>

><span data-ttu-id="7b750-129">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7b750-129">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metdata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/a5212c6a-a8b1-49cd-bd40-7f83f0a42861/channels/getAllMessages?$top=2&$skip=2",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/teams/ab5332ba-6dd9-46d3-ade5-5c61a2f148b2/channels/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/messages/1580173996201",
            "id": "1580173996201",
            "replyToId": null,
            "etag": "1580173996201",
            "messageType": "message",
            "createdDateTime": "2020-01-28T01:13:16.201Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/1580173996201?groupId=ab5332ba-6dd9-46d3-ade5-5c61a2f148b2&tenantId=e0d829d2-c239-4b28-9d08-c096da71be7a&createdTime=1580173996201&parentMessageId=1580173996201",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "a5212c6a-a8b1-49cd-bd40-7f83f0a42861",
                    "displayName": "spoons test",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Test"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.id": "https://graph.microsoft.com/beta/teams/ab5332ba-6dd9-46d3-ade5-5c61a2f148b2/channels/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/messages/1580768557513",
            "id": "1580768557513",
            "replyToId": null,
            "etag": "1580768557513",
            "messageType": "message",
            "createdDateTime": "2020-02-03T22:22:37.513Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "a5212c6a-a8b1-49cd-bd40-7f83f0a42861",
                    "displayName": "spoons test",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "hi user1,user3"
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
