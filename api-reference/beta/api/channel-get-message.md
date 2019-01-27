---
title: Obter mensagens do canal
description: Recupere uma única mensagem (sem suas respostas) no canal de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 26b59ac395af3de314469fdb419095bcb6133d6b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523201"
---
# <a name="get-channel-message"></a><span data-ttu-id="24fea-103">Obter mensagens do canal</span><span class="sxs-lookup"><span data-stu-id="24fea-103">Get channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24fea-104">Recupere uma única [mensagem](../resources/chatmessage.md) (sem suas respostas) no [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="24fea-104">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="24fea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="24fea-105">Permissions</span></span>
<span data-ttu-id="24fea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24fea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24fea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24fea-108">Permission type</span></span>|<span data-ttu-id="24fea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24fea-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="24fea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24fea-110">Delegated (work or school account)</span></span>|<span data-ttu-id="24fea-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24fea-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="24fea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24fea-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24fea-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="24fea-113">Not supported</span></span>|
|<span data-ttu-id="24fea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24fea-114">Application</span></span>| <span data-ttu-id="24fea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24fea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24fea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24fea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24fea-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24fea-117">Optional query parameters</span></span>
<span data-ttu-id="24fea-118">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="24fea-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24fea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24fea-119">Request headers</span></span>
| <span data-ttu-id="24fea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24fea-120">Header</span></span>       | <span data-ttu-id="24fea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="24fea-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24fea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="24fea-122">Authorization</span></span>  | <span data-ttu-id="24fea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24fea-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24fea-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24fea-125">Request body</span></span>
<span data-ttu-id="24fea-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24fea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24fea-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="24fea-127">Response</span></span>

<span data-ttu-id="24fea-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24fea-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24fea-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24fea-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24fea-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24fea-130">Request</span></span>
<span data-ttu-id="24fea-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24fea-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="24fea-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="24fea-132">Response</span></span>
<span data-ttu-id="24fea-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24fea-133">Here is an example of the response.</span></span> 

><span data-ttu-id="24fea-134">**Observação:** o objeto de resposta mostrado aqui foi encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24fea-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="24fea-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24fea-135">All the properties will be returned from an actual call.</span></span>
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
  "from": {
      "user": { 
        "id": "id-value",
        "displayName": "John Doe"
      }  
  },
  "etag": "id-value",
  "messageType": "message",
  "createdDateTime": "2018-07-09T07:40:20.152Z",
  "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
  "body": {
      "content": "Hello World",
      "contentType": "text"
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
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
