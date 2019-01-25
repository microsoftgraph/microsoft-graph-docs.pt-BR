---
title: Obtenha uma resposta a uma mensagem de canal
description: Obtenha uma única resposta a uma mensagem em um canal de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1bfd1ab079119a55cd9a031dc6a42e01074288be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515591"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="5fc42-103">Obtenha uma resposta a uma mensagem de canal</span><span class="sxs-lookup"><span data-stu-id="5fc42-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fc42-104">Obtenha uma única resposta a uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="5fc42-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fc42-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fc42-105">Permissions</span></span>
<span data-ttu-id="5fc42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fc42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fc42-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fc42-108">Permission Type</span></span>|<span data-ttu-id="5fc42-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fc42-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5fc42-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fc42-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5fc42-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fc42-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="5fc42-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fc42-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fc42-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5fc42-113">Not supported</span></span>|
|<span data-ttu-id="5fc42-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fc42-114">Application</span></span>| <span data-ttu-id="5fc42-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fc42-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fc42-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fc42-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fc42-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5fc42-117">Optional query parameters</span></span>
<span data-ttu-id="5fc42-118">Os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não são suportados no momento.</span><span class="sxs-lookup"><span data-stu-id="5fc42-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fc42-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fc42-119">Request headers</span></span>
| <span data-ttu-id="5fc42-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5fc42-120">Header</span></span>       | <span data-ttu-id="5fc42-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5fc42-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5fc42-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fc42-122">Authorization</span></span>  | <span data-ttu-id="5fc42-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fc42-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5fc42-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fc42-125">Request body</span></span>
<span data-ttu-id="5fc42-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5fc42-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fc42-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fc42-127">Response</span></span>
<span data-ttu-id="5fc42-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fc42-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5fc42-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fc42-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fc42-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fc42-130">Request</span></span>
<span data-ttu-id="5fc42-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fc42-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies/{id}
```
##### <a name="response"></a><span data-ttu-id="5fc42-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fc42-132">Response</span></span>
<span data-ttu-id="5fc42-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fc42-133">Here is an example of the response.</span></span> 

><span data-ttu-id="5fc42-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fc42-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "replyToId": "id-value",
  "from" : {
      "user": { 
        "id":  "id-value",
        "displayName": "John Doe"
      }  
  },
  "etag": "id-value",
  "messageType": "message",
  "createdDateTime": "2018-07-09T07:40:20.152Z",
  "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
  "body": {
      "content": "This is a response to a message.",
      "contentType": "Text"
  },
  "attachments": [
        {
            "id": "5e32f195-168a-474f-a273-12312312312",
            "contentType": "reference",
            "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
            "content": null,
            "name": "Test.txt",
            "thumbnailUrl": null
        }
  ],
  "mentions": [
      {
          "type": "user",
          "id": "id-value ",
          "mentionText": "Test User"
      }
  ],
  "importance": "normal",
  "reactions": [
      {
        "reactionType": "like",
        "user": {
            "id": "id-value",
            "displayName": "John Doe"
        },
        "createdDateTime": "2018-07-09T07:40:20.152Z"
      }
  ],
  "locale": "en-us"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
