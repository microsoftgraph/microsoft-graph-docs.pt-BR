---
title: Obter uma resposta a uma mensagem de canal
description: Obter uma única resposta a uma mensagem em um canal de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c6dff7204068f6c9ebb3397cc8e745229e399efa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440343"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="fd11e-103">Obter uma resposta a uma mensagem de canal</span><span class="sxs-lookup"><span data-stu-id="fd11e-103">Get a reply to a channel message</span></span>

<span data-ttu-id="fd11e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fd11e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd11e-105">Obter uma única resposta a uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="fd11e-105">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd11e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd11e-106">Permissions</span></span>

<span data-ttu-id="fd11e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd11e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd11e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd11e-109">Permission Type</span></span>|<span data-ttu-id="fd11e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd11e-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="fd11e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd11e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="fd11e-112">ChannelMessage. Read. All, Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fd11e-112">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="fd11e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd11e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd11e-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fd11e-114">Not supported</span></span>|
|<span data-ttu-id="fd11e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd11e-115">Application</span></span>| <span data-ttu-id="fd11e-116">ChannelMessage. Read. All, Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fd11e-116">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="fd11e-117">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd11e-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="fd11e-118">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="fd11e-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="fd11e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd11e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd11e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fd11e-120">Optional query parameters</span></span>

<span data-ttu-id="fd11e-121">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="fd11e-121">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd11e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd11e-122">Request headers</span></span>

| <span data-ttu-id="fd11e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd11e-123">Header</span></span>       | <span data-ttu-id="fd11e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fd11e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd11e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd11e-125">Authorization</span></span>  | <span data-ttu-id="fd11e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd11e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd11e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd11e-128">Request body</span></span>

<span data-ttu-id="fd11e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd11e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd11e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd11e-130">Response</span></span>

<span data-ttu-id="fd11e-131">Se bem-sucedido, esse método retornará um `200 OK` código de resposta e um objeto [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd11e-131">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd11e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd11e-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fd11e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd11e-133">Request</span></span>

<span data-ttu-id="fd11e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd11e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd11e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd11e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
# <a name="c"></a>[<span data-ttu-id="fd11e-136">C#</span><span class="sxs-lookup"><span data-stu-id="fd11e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd11e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd11e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd11e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd11e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fd11e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd11e-139">Response</span></span>
<span data-ttu-id="fd11e-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd11e-140">Here is an example of the response.</span></span> 

><span data-ttu-id="fd11e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd11e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies/$entity",
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a reply to a channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
