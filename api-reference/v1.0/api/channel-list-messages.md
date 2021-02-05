---
title: Listar mensagens do canal
description: 'Recupere a lista de mensagens (sem as respostas) em um canal de equipe. Para obter as respostas de uma mensagem, chame as respostas da mensagem da lista ou a API de resposta da mensagem recebida. '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ca64fabc676d42c43960bc8fc1c4620a7cf52a83
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115154"
---
# <a name="list-channel-messages"></a><span data-ttu-id="011ec-104">Listar mensagens do canal</span><span class="sxs-lookup"><span data-stu-id="011ec-104">List channel messages</span></span>

<span data-ttu-id="011ec-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="011ec-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="011ec-106">Recupere a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [canal](../resources/channel.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="011ec-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> 

<span data-ttu-id="011ec-107">Para obter as respostas de uma mensagem, chame as [respostas de listar mensagens](channel-list-messagereplies.md) ou a API de [respostas de obter mensagens](channel-get-messagereply.md).</span><span class="sxs-lookup"><span data-stu-id="011ec-107">To get the replies for a message, call the [list message replies](channel-list-messagereplies.md) or the [get message reply](channel-get-messagereply.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="011ec-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="011ec-108">Permissions</span></span>

<span data-ttu-id="011ec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="011ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="011ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="011ec-111">Permission Type</span></span>|<span data-ttu-id="011ec-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="011ec-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="011ec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="011ec-113">Delegated (work or school account)</span></span>| <span data-ttu-id="011ec-114">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="011ec-114">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="011ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="011ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="011ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="011ec-116">Not supported.</span></span>|
|<span data-ttu-id="011ec-117">Application</span><span class="sxs-lookup"><span data-stu-id="011ec-117">Application</span></span>| <span data-ttu-id="011ec-118">ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="011ec-118">ChannelMessage.Read.Group\*</span></span> |

> <span data-ttu-id="011ec-119">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="011ec-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="011ec-120">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="011ec-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="011ec-121">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="011ec-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="011ec-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="011ec-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="011ec-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="011ec-123">Optional query parameters</span></span>

<span data-ttu-id="011ec-124">Você pode usar o parâmetro de consulta [$top](/graph/query-parameters#top-parameter) para controlar o número de itens por resposta.</span><span class="sxs-lookup"><span data-stu-id="011ec-124">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="011ec-125">No momento, não há suporte para os outros [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="011ec-125">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

> <span data-ttu-id="011ec-126">**Observação:** [OBTER /teams/{id}/channels/{id}/messages/delta](chatmessage-delta.md) oferece suporte para a filtragem por data, que fornece dados semelhantes para OBTER /teams/{id}/channels/{id}/messages.</span><span class="sxs-lookup"><span data-stu-id="011ec-126">**Note:** [GET /teams/{id}/channels/{id}/messages/delta](chatmessage-delta.md) supports filtering by date, which provides similar data to GET /teams/{id}/channels/{id}/messages.</span></span>

## <a name="request-headers"></a><span data-ttu-id="011ec-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="011ec-127">Request headers</span></span>

| <span data-ttu-id="011ec-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="011ec-128">Header</span></span>       | <span data-ttu-id="011ec-129">Valor</span><span class="sxs-lookup"><span data-stu-id="011ec-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="011ec-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="011ec-130">Authorization</span></span>  | <span data-ttu-id="011ec-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="011ec-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="011ec-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="011ec-133">Request body</span></span>

<span data-ttu-id="011ec-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="011ec-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="011ec-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="011ec-135">Response</span></span>

<span data-ttu-id="011ec-136">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="011ec-136">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="011ec-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="011ec-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="011ec-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="011ec-138">Request</span></span>

<span data-ttu-id="011ec-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="011ec-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="011ec-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="011ec-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"],
  "name": "get_channel_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages
```
# <a name="c"></a>[<span data-ttu-id="011ec-141">C#</span><span class="sxs-lookup"><span data-stu-id="011ec-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="011ec-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="011ec-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="011ec-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="011ec-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="011ec-144">Java</span><span class="sxs-lookup"><span data-stu-id="011ec-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="011ec-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="011ec-145">Response</span></span>
<span data-ttu-id="011ec-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="011ec-146">Here is an example of the response.</span></span> 

><span data-ttu-id="011ec-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="011ec-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages",
    "@odata.count": 3,
    "value": [
        {
            "id": "1555375673184",
            "replyToId": null,
            "etag": "1555375673184",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:47:53.184Z",
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
  ]
}
-->


