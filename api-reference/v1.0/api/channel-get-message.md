---
title: Obter mensagens do canal
description: Recupere uma única mensagem (sem suas respostas) no canal de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7f8d0266688c0347e0b21e2bc793e13fbeaac82d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515909"
---
# <a name="get-channel-message"></a><span data-ttu-id="900d3-103">Obter mensagens do canal</span><span class="sxs-lookup"><span data-stu-id="900d3-103">Get channel message</span></span>

<span data-ttu-id="900d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="900d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="900d3-105">Recupere uma única [mensagem](../resources/chatmessage.md) (sem suas respostas) no [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="900d3-105">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="900d3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="900d3-106">Permissions</span></span>
<span data-ttu-id="900d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="900d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="900d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="900d3-109">Permission Type</span></span>|<span data-ttu-id="900d3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="900d3-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="900d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="900d3-111">Delegated (work or school account)</span></span>| <span data-ttu-id="900d3-112">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="900d3-112">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="900d3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="900d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="900d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="900d3-114">Not supported.</span></span>|
|<span data-ttu-id="900d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="900d3-115">Application</span></span>| <span data-ttu-id="900d3-116">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="900d3-116">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="900d3-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="900d3-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="900d3-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="900d3-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="900d3-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="900d3-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="900d3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="900d3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="900d3-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="900d3-121">Optional query parameters</span></span>
<span data-ttu-id="900d3-122">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="900d3-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="900d3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="900d3-123">Request headers</span></span>
| <span data-ttu-id="900d3-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="900d3-124">Header</span></span>       | <span data-ttu-id="900d3-125">Valor</span><span class="sxs-lookup"><span data-stu-id="900d3-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="900d3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="900d3-126">Authorization</span></span>  | <span data-ttu-id="900d3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="900d3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="900d3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="900d3-129">Request body</span></span>
<span data-ttu-id="900d3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="900d3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="900d3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="900d3-131">Response</span></span>

<span data-ttu-id="900d3-132">Se bem-sucedido, esse método retornará um `200 OK` código de resposta e um objeto [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="900d3-132">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="900d3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="900d3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="900d3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="900d3-134">Request</span></span>
<span data-ttu-id="900d3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="900d3-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="900d3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="900d3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184
```
# <a name="c"></a>[<span data-ttu-id="900d3-137">C#</span><span class="sxs-lookup"><span data-stu-id="900d3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="900d3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="900d3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="900d3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="900d3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="900d3-140">Java</span><span class="sxs-lookup"><span data-stu-id="900d3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="900d3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="900d3-141">Response</span></span>
<span data-ttu-id="900d3-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="900d3-142">Here is an example of the response.</span></span> 

><span data-ttu-id="900d3-143">**Observação:** o objeto de resposta mostrado aqui foi encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="900d3-143">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="900d3-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="900d3-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages/$entity",
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
  ]
}
-->


