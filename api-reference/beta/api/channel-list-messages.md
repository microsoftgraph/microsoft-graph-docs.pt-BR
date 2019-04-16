---
title: Listar mensagens do canal
description: 'Recupere a lista de mensagens (sem as respostas) em um canal de equipe. Para obter as respostas de uma mensagem, chame as respostas da mensagem da lista ou a API de resposta da mensagem recebida. '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 000e85db202ea08677876a288e6a68dc2e20ed52
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2019
ms.locfileid: "31890000"
---
# <a name="list-channel-messages"></a><span data-ttu-id="a8589-104">Listar mensagens do canal</span><span class="sxs-lookup"><span data-stu-id="a8589-104">List channel messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8589-105">Recupere a lista de [mensagens](../resources/chatmessage.md) (sem as respostas) em um [canal](../resources/channel.md) de [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a8589-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="a8589-106">Para obter as respostas de uma mensagem, chame as [respostas de listar mensagens](channel-get-messagereply.md) ou a API de [respostas de obter mensagens](channel-list-messagereplies.md).</span><span class="sxs-lookup"><span data-stu-id="a8589-106">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a8589-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8589-107">Permissions</span></span>
<span data-ttu-id="a8589-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8589-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8589-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8589-110">Permission Type</span></span>|<span data-ttu-id="a8589-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8589-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a8589-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8589-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8589-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8589-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="a8589-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8589-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8589-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8589-115">Not supported</span></span>|
|<span data-ttu-id="a8589-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8589-116">Application</span></span>| <span data-ttu-id="a8589-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8589-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8589-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8589-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8589-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8589-119">Optional query parameters</span></span>
<span data-ttu-id="a8589-120">Atualmente, os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não têm suporte.</span><span class="sxs-lookup"><span data-stu-id="a8589-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8589-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8589-121">Request headers</span></span>
| <span data-ttu-id="a8589-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8589-122">Header</span></span>       | <span data-ttu-id="a8589-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a8589-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8589-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8589-124">Authorization</span></span>  | <span data-ttu-id="a8589-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8589-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8589-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8589-127">Request body</span></span>
<span data-ttu-id="a8589-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8589-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8589-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8589-129">Response</span></span>

<span data-ttu-id="a8589-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8589-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8589-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8589-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8589-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8589-132">Request</span></span>
<span data-ttu-id="a8589-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8589-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="a8589-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8589-134">Response</span></span>
<span data-ttu-id="a8589-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8589-135">Here is an example of the response.</span></span> 

><span data-ttu-id="a8589-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8589-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "value": [
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
            "content": "Hello World",
            "contentType": "Text"
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
                "id": "id-value ",
                "mentionText": "Test User",
                "mentioned": {
                "user": {
                    "id": "id-value",
                    "displayName: "string"
                }
            }
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
