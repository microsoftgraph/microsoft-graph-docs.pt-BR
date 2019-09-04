---
title: Obter mensagens do canal
description: Recupere uma única mensagem (sem suas respostas) no canal de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ddc07529b196f2d9e23033137fc1eb18cd1af701
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720036"
---
# <a name="get-channel-message"></a><span data-ttu-id="c31b7-103">Obter mensagens do canal</span><span class="sxs-lookup"><span data-stu-id="c31b7-103">Get channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c31b7-104">Recupere uma única [mensagem](../resources/chatmessage.md) (sem suas respostas) no [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="c31b7-104">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="c31b7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c31b7-105">Permissions</span></span>
<span data-ttu-id="c31b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c31b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c31b7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c31b7-108">Permission Type</span></span>|<span data-ttu-id="c31b7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c31b7-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c31b7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c31b7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c31b7-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31b7-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="c31b7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c31b7-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c31b7-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c31b7-113">Not supported</span></span>|
|<span data-ttu-id="c31b7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c31b7-114">Application</span></span>| <span data-ttu-id="c31b7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31b7-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="c31b7-116">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c31b7-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="c31b7-117">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c31b7-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c31b7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c31b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c31b7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c31b7-119">Optional query parameters</span></span>
<span data-ttu-id="c31b7-120">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="c31b7-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c31b7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c31b7-121">Request headers</span></span>
| <span data-ttu-id="c31b7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c31b7-122">Header</span></span>       | <span data-ttu-id="c31b7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c31b7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c31b7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c31b7-124">Authorization</span></span>  | <span data-ttu-id="c31b7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c31b7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c31b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c31b7-127">Request body</span></span>
<span data-ttu-id="c31b7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c31b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c31b7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c31b7-129">Response</span></span>

<span data-ttu-id="c31b7-130">Se bem-sucedido, esse método retornará um `200 OK` código de resposta e um objeto [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c31b7-130">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c31b7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c31b7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c31b7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c31b7-132">Request</span></span>
<span data-ttu-id="c31b7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c31b7-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c31b7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c31b7-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c31b7-135">C#</span><span class="sxs-lookup"><span data-stu-id="c31b7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c31b7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c31b7-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c31b7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c31b7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c31b7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c31b7-138">Response</span></span>
<span data-ttu-id="c31b7-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c31b7-139">Here is an example of the response.</span></span> 

><span data-ttu-id="c31b7-140">**Observação:** o objeto de resposta mostrado aqui foi encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c31b7-140">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="c31b7-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c31b7-141">All the properties will be returned from an actual call.</span></span>
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
