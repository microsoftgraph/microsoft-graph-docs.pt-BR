---
title: Enviar uma mensagem em um canal
description: Enviar uma nova mensagem no canal especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f1199be1949e34b5a9d4c5f461fe6ba03fdfe28b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328000"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="833a4-103">Enviar uma mensagem para um canal</span><span class="sxs-lookup"><span data-stu-id="833a4-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="833a4-104">Criar uma nova [mensagem](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="833a4-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="833a4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="833a4-105">Permissions</span></span>
<span data-ttu-id="833a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="833a4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="833a4-108">Permission type</span></span>      | <span data-ttu-id="833a4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="833a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="833a4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="833a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="833a4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="833a4-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="833a4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="833a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="833a4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="833a4-113">Not supported.</span></span>    |
|<span data-ttu-id="833a4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="833a4-114">Application</span></span> | <span data-ttu-id="833a4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="833a4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="833a4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="833a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="833a4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="833a4-117">Request headers</span></span>
| <span data-ttu-id="833a4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="833a4-118">Name</span></span>       | <span data-ttu-id="833a4-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="833a4-119">Type</span></span> | <span data-ttu-id="833a4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="833a4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="833a4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="833a4-121">Authorization</span></span>  | <span data-ttu-id="833a4-122">string</span><span class="sxs-lookup"><span data-stu-id="833a4-122">string</span></span>  | <span data-ttu-id="833a4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="833a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="833a4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="833a4-125">Request body</span></span>
<span data-ttu-id="833a4-126">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="833a4-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="833a4-127">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="833a4-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="833a4-128">Observação: não há suporte para o envio de mensagens com anexos e imagens.</span><span class="sxs-lookup"><span data-stu-id="833a4-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="833a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="833a4-129">Response</span></span>

<span data-ttu-id="833a4-130">Se bem-sucedido, este método retorna `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="833a4-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="833a4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="833a4-131">Examples</span></span> 

### <a name="example-1-hello-world"></a><span data-ttu-id="833a4-132">Exemplo 1: Olá mundo</span><span class="sxs-lookup"><span data-stu-id="833a4-132">Example 1: Hello World</span></span>

##### <a name="request"></a><span data-ttu-id="833a4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="833a4-133">Request</span></span>
<span data-ttu-id="833a4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="833a4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="833a4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="833a4-135">Response</span></span>

<span data-ttu-id="833a4-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="833a4-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
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
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-mentions"></a><span data-ttu-id="833a4-137">Exemplo 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="833a4-137">Example 2: @mentions</span></span>

##### <a name="request"></a><span data-ttu-id="833a4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="833a4-138">Request</span></span>
<span data-ttu-id="833a4-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="833a4-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="833a4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="833a4-140">Response</span></span>

<span data-ttu-id="833a4-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="833a4-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
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
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

### <a name="example-3-cards"></a><span data-ttu-id="833a4-142">Exemplo 3: cartões</span><span class="sxs-lookup"><span data-stu-id="833a4-142">Example 3: Cards</span></span>

##### <a name="request"></a><span data-ttu-id="833a4-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="833a4-143">Request</span></span>
<span data-ttu-id="833a4-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="833a4-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "subject": null,
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="833a4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="833a4-145">Response</span></span>

<span data-ttu-id="833a4-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="833a4-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('bdb7bcda-9c3b-4341-b9a9-f52bf9a23407')/channels('19%3A786524f437c042b68bac5c0511ad6be2%40thread.skype')/messages/$entity",
    "id": "1554837297516",
    "replyToId": null,
    "etag": "1554837297516",
    "messageType": "message",
    "createdDateTime": "2019-04-09T19:14:57.516Z",
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
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\n\\r\\n\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\n\\r\\n\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a><span data-ttu-id="833a4-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="833a4-147">See also</span></span>

- [<span data-ttu-id="833a4-148">Referência de cartões</span><span class="sxs-lookup"><span data-stu-id="833a4-148">Cards Reference</span></span>](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards-reference)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
