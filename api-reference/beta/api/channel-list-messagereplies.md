---
title: Listar respostas de mensagens de canal
description: Listar todas as respostas de uma mensagem em um canal de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c3c681c820f4cc855105ec1605be920a98a1430
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456455"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="c82f7-103">Listar respostas de mensagens de canal</span><span class="sxs-lookup"><span data-stu-id="c82f7-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c82f7-104">Listar todas as respostas de uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="c82f7-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="c82f7-105">Este método lista somente as respostas da mensagem especificada, se houver.</span><span class="sxs-lookup"><span data-stu-id="c82f7-105">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="c82f7-106">Para obter a mensagem em si, basta chamar [Message Get Channel](channel-get-message.md).</span><span class="sxs-lookup"><span data-stu-id="c82f7-106">To get the message itself, simply call [get channel message](channel-get-message.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c82f7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c82f7-107">Permissions</span></span>
<span data-ttu-id="c82f7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c82f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c82f7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c82f7-110">Permission Type</span></span>|<span data-ttu-id="c82f7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c82f7-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c82f7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c82f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c82f7-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82f7-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="c82f7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c82f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c82f7-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c82f7-115">Not supported</span></span>|
|<span data-ttu-id="c82f7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c82f7-116">Application</span></span>| <span data-ttu-id="c82f7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c82f7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c82f7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c82f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c82f7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c82f7-119">Optional query parameters</span></span>

<span data-ttu-id="c82f7-120">Você pode usar o [$Top](/graph/query-parameters#top-parameter) parâmetro de consulta para controlar o número de itens por resposta.</span><span class="sxs-lookup"><span data-stu-id="c82f7-120">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="c82f7-121">Os outros [parâmetros de consulta OData](/graph/query-parameters) não têm suporte no momento.</span><span class="sxs-lookup"><span data-stu-id="c82f7-121">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c82f7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c82f7-122">Request headers</span></span>
| <span data-ttu-id="c82f7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c82f7-123">Header</span></span>       | <span data-ttu-id="c82f7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c82f7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c82f7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c82f7-125">Authorization</span></span>  | <span data-ttu-id="c82f7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c82f7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c82f7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c82f7-128">Request body</span></span>
<span data-ttu-id="c82f7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c82f7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c82f7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c82f7-130">Response</span></span>
<span data-ttu-id="c82f7-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatmessage](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c82f7-131">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c82f7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c82f7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c82f7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c82f7-133">Request</span></span>
<span data-ttu-id="c82f7-134">Neste exemplo, a mensagem especificada tem duas respostas.</span><span class="sxs-lookup"><span data-stu-id="c82f7-134">In this example, the specified message has two replies.</span></span> <span data-ttu-id="c82f7-135">Cada resposta tem um ou mais objetos [chatMessageMention](../resources/chatmessagemention.md) .</span><span class="sxs-lookup"><span data-stu-id="c82f7-135">Each reply has one or more [chatMessageMention](../resources/chatmessagemention.md) objects.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies
```
##### <a name="response"></a><span data-ttu-id="c82f7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c82f7-136">Response</span></span>
<span data-ttu-id="c82f7-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c82f7-137">Here is an example of the response.</span></span> 

><span data-ttu-id="c82f7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c82f7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies",
    "@odata.count": 2,
    "value": [
        {
            "id": "1555377090002",
            "replyToId": "1555375673184",
            "etag": "1555377090002",
            "messageType": "message",
            "createdDateTime": "2019-04-16T01:11:30.002Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
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
                "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Megan",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                            "displayName": "Megan",
                            "userIdentityType": "aadUser"
                        }
                    }
                },
                {
                    "id": 1,
                    "mentionText": "Alex",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                            "displayName": "Alex",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        },
        {
            "id": "1555375848360",
            "replyToId": "1555375673184",
            "etag": "1555375848360",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:50:48.36Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
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
                "content": "<div><div>And, <at id=\"0\">Alex Wilber</at>, can we see the February report as well?</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Alex Wilber",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                            "displayName": "Alex Wilber",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
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
    "Error: /api-reference/beta/api/channel-list-messagereplies.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
