---
title: Respostas de mensagens de canal de lista
description: Liste todas as respostas de uma mensagem em um canal de uma equipe.
ms.openlocfilehash: 7133f48233f2b164aa6643ba896dd0612645e7e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033056"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="b614c-103">Respostas de mensagens de canal de lista</span><span class="sxs-lookup"><span data-stu-id="b614c-103">List channel message replies</span></span>

> <span data-ttu-id="b614c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b614c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b614c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b614c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b614c-106">Liste todas as respostas de uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b614c-106">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="b614c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b614c-107">Permissions</span></span>
<span data-ttu-id="b614c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b614c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b614c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b614c-110">Permission Type</span></span>|<span data-ttu-id="b614c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b614c-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b614c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b614c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b614c-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b614c-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="b614c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b614c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b614c-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b614c-115">Not supported</span></span>|
|<span data-ttu-id="b614c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b614c-116">Application</span></span>| <span data-ttu-id="b614c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b614c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b614c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b614c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b614c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b614c-119">Optional query parameters</span></span>
<span data-ttu-id="b614c-120">Os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não são suportados no momento.</span><span class="sxs-lookup"><span data-stu-id="b614c-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b614c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b614c-121">Request headers</span></span>
| <span data-ttu-id="b614c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b614c-122">Header</span></span>       | <span data-ttu-id="b614c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b614c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b614c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b614c-124">Authorization</span></span>  | <span data-ttu-id="b614c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b614c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b614c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b614c-127">Request body</span></span>
<span data-ttu-id="b614c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b614c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b614c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b614c-129">Response</span></span>
<span data-ttu-id="b614c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [chatmessage](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b614c-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b614c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b614c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b614c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b614c-132">Request</span></span>
<span data-ttu-id="b614c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b614c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
```
##### <a name="response"></a><span data-ttu-id="b614c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b614c-134">Response</span></span>
<span data-ttu-id="b614c-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b614c-135">Here is an example of the response.</span></span> 

><span data-ttu-id="b614c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b614c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "content": "This is a response to a message.",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
