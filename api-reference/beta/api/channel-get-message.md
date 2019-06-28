---
title: Obter mensagens do canal
description: Recupere uma única mensagem (sem suas respostas) no canal de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6393ba9fdd5c012d24fd3e65ee707cda57c93cda
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35348639"
---
# <a name="get-channel-message"></a><span data-ttu-id="d4e16-103">Obter mensagens do canal</span><span class="sxs-lookup"><span data-stu-id="d4e16-103">Get channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e16-104">Recupere uma única [mensagem](../resources/chatmessage.md) (sem suas respostas) no [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d4e16-104">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4e16-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4e16-105">Permissions</span></span>
<span data-ttu-id="d4e16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e16-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4e16-108">Permission Type</span></span>|<span data-ttu-id="d4e16-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4e16-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="d4e16-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4e16-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e16-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e16-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e16-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4e16-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e16-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d4e16-113">Not supported</span></span>|
|<span data-ttu-id="d4e16-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4e16-114">Application</span></span>| <span data-ttu-id="d4e16-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e16-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4e16-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e16-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4e16-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4e16-117">Optional query parameters</span></span>
<span data-ttu-id="d4e16-118">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="d4e16-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4e16-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e16-119">Request headers</span></span>
| <span data-ttu-id="d4e16-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4e16-120">Header</span></span>       | <span data-ttu-id="d4e16-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d4e16-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4e16-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4e16-122">Authorization</span></span>  | <span data-ttu-id="d4e16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4e16-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4e16-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e16-125">Request body</span></span>
<span data-ttu-id="d4e16-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4e16-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4e16-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e16-127">Response</span></span>

<span data-ttu-id="d4e16-128">Se bem-sucedido, esse método retornará um `200 OK` código de resposta e um objeto [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e16-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e16-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4e16-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4e16-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e16-130">Request</span></span>
<span data-ttu-id="d4e16-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4e16-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184
```
##### <a name="response"></a><span data-ttu-id="d4e16-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e16-132">Response</span></span>
<span data-ttu-id="d4e16-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e16-133">Here is an example of the response.</span></span> 

><span data-ttu-id="d4e16-134">**Observação:** o objeto de resposta mostrado aqui foi encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d4e16-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="d4e16-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4e16-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages/$entity",
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
    "attachments": [
        {
            "id": "5e32f195-168a-474f-a273-123123123",
            "contentType": "reference",
            "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
            "content": null,
            "name": "Test.txt",
            "thumbnailUrl": null
        }
    ],
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
    "reactions": [
      {
        "reactionType": "like",
        "user": {
            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
            "displayName": "Megan Bowen",
            "userIdentityType": "aadUser"
        },
        "createdDateTime": "2019-04-16T00:58:53.184Z"
      }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d4e16-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d4e16-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d4e16-137">C#</span><span class="sxs-lookup"><span data-stu-id="d4e16-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4e16-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4e16-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d4e16-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4e16-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_channel_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
