---
title: Listar mensagens do canal
description: 'Recupere a lista de mensagens (sem as respostas) em um canal de equipe. Para obter as respostas de uma mensagem, chame as respostas da mensagem da lista ou a API de resposta da mensagem recebida. '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 827192f0a85ca4fc5a46de2093d2f4f79b67662e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262094"
---
# <a name="list-channel-messages"></a><span data-ttu-id="86a63-104">Listar mensagens do canal</span><span class="sxs-lookup"><span data-stu-id="86a63-104">List channel messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86a63-105">Recupere a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [canal](../resources/channel.md) de [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="86a63-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> 

<span data-ttu-id="86a63-106">Para obter as respostas de uma mensagem, chame as [respostas de listar mensagens](channel-get-messagereply.md) ou a API de [respostas de obter mensagens](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="86a63-106">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="86a63-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="86a63-107">Permissions</span></span>

<span data-ttu-id="86a63-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a63-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86a63-110">Permission Type</span></span>|<span data-ttu-id="86a63-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86a63-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="86a63-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86a63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86a63-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86a63-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="86a63-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86a63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86a63-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="86a63-115">Not supported</span></span>|
|<span data-ttu-id="86a63-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86a63-116">Application</span></span>| <span data-ttu-id="86a63-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a63-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86a63-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86a63-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86a63-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86a63-119">Optional query parameters</span></span>

<span data-ttu-id="86a63-120">Você pode usar o parâmetro de consulta [$top](/graph/query-parameters#top-parameter) para controlar o número de itens por resposta.</span><span class="sxs-lookup"><span data-stu-id="86a63-120">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="86a63-121">No momento, não há suporte para os outros [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="86a63-121">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86a63-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86a63-122">Request headers</span></span>

| <span data-ttu-id="86a63-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86a63-123">Header</span></span>       | <span data-ttu-id="86a63-124">Valor</span><span class="sxs-lookup"><span data-stu-id="86a63-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86a63-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="86a63-125">Authorization</span></span>  | <span data-ttu-id="86a63-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86a63-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86a63-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86a63-128">Request body</span></span>

<span data-ttu-id="86a63-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86a63-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86a63-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a63-130">Response</span></span>

<span data-ttu-id="86a63-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86a63-131">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86a63-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86a63-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="86a63-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86a63-133">Request</span></span>

<span data-ttu-id="86a63-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86a63-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"],
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages
```
##### <a name="response"></a><span data-ttu-id="86a63-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a63-135">Response</span></span>
<span data-ttu-id="86a63-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86a63-136">Here is an example of the response.</span></span> 

><span data-ttu-id="86a63-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86a63-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages",
    "@odata.count": 3,
    "value": [
        {
            "id": "1555375673184",
            "replyToId": null,
            "etag": "1555375673184",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:47:53.184Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
                    "displayName": "Adele Vance",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div>Nice to join this team. <at id=\"0\">Megan Bowen</at>, have we got the March report ready please?</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Megan Bowen",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                            "displayName": "Megan Bowen",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        },
        {
            "id": "1548100551644",
            "replyToId": null,
            "etag": "1548100551893",
            "messageType": "message",
            "createdDateTime": "2019-01-21T19:55:51.644Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "c651e5be-7631-42ad-99c6-12c59def11fb",
                    "displayName": "Miriam Graham",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div>I've added an Excel tab to the channel containing the P&amp;L Summary. \r\n<div style=\"display:inline\"><at id=\"0\">Isaiah Langer</at></div> and team, please review the Sale Summary tab in particular, and make any necessary updates.</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Isaiah Langer",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "b525e831-bd00-45e5-860c-a4329ef5f5d8",
                            "displayName": "Isaiah Langer",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": [
                {
                    "reactionType": "like",
                    "createdDateTime": "2019-01-21T19:55:51.893Z",
                    "user": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "e1ecb745-c10f-40af-a9d4-cab946c80ac7",
                            "displayName": null,
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ]
        },
        {
            "id": "1548100547534",
            "replyToId": null,
            "etag": "1548100547534",
            "messageType": "message",
            "createdDateTime": "2019-01-21T19:55:47.534Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "high",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
                    "displayName": "Adele Vance",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div>Just a reminder to everyone to please update your monthly reports by this Friday!</div>"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="86a63-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="86a63-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="86a63-140">C#</span><span class="sxs-lookup"><span data-stu-id="86a63-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_messages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86a63-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="86a63-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_messages-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="86a63-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86a63-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_channel_messages-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
