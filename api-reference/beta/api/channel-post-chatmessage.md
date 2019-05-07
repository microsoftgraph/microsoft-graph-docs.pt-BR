---
title: Enviar uma mensagem em um canal
description: Enviar uma nova mensagem no canal especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7df36c50e58e1e52be3008a929d2a0b3b046f27
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635586"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="9b0ee-103">Enviar uma mensagem para um canal</span><span class="sxs-lookup"><span data-stu-id="9b0ee-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b0ee-104">Criar uma nova [mensagem](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b0ee-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b0ee-105">Permissions</span></span>
<span data-ttu-id="9b0ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b0ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b0ee-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b0ee-108">Permission type</span></span>      | <span data-ttu-id="9b0ee-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b0ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b0ee-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b0ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b0ee-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b0ee-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9b0ee-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b0ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b0ee-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-113">Not supported.</span></span>    |
|<span data-ttu-id="9b0ee-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b0ee-114">Application</span></span> | <span data-ttu-id="9b0ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b0ee-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b0ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="9b0ee-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b0ee-117">Request headers</span></span>
| <span data-ttu-id="9b0ee-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9b0ee-118">Name</span></span>       | <span data-ttu-id="9b0ee-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b0ee-119">Type</span></span> | <span data-ttu-id="9b0ee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b0ee-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9b0ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b0ee-121">Authorization</span></span>  | <span data-ttu-id="9b0ee-122">string</span><span class="sxs-lookup"><span data-stu-id="9b0ee-122">string</span></span>  | <span data-ttu-id="9b0ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b0ee-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b0ee-125">Request body</span></span>
<span data-ttu-id="9b0ee-126">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="9b0ee-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="9b0ee-127">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="9b0ee-128">Observação: não há suporte para o envio de mensagens com anexos e imagens.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="9b0ee-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b0ee-129">Response</span></span>

<span data-ttu-id="9b0ee-130">Se bem-sucedido, este método retorna `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="9b0ee-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9b0ee-131">Examples</span></span> 

### <a name="example-1-hello-world"></a><span data-ttu-id="9b0ee-132">Exemplo 1: Olá mundo</span><span class="sxs-lookup"><span data-stu-id="9b0ee-132">Example 1: Hello World</span></span>

##### <a name="request"></a><span data-ttu-id="9b0ee-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b0ee-133">Request</span></span>
<span data-ttu-id="9b0ee-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-134">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9b0ee-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b0ee-135">Response</span></span>

<span data-ttu-id="9b0ee-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-136">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9b0ee-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9b0ee-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9b0ee-138">Basic</span><span class="sxs-lookup"><span data-stu-id="9b0ee-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b0ee-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b0ee-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-mentions"></a><span data-ttu-id="9b0ee-140">Exemplo 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="9b0ee-140">Example 2: @mentions</span></span>

##### <a name="request"></a><span data-ttu-id="9b0ee-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b0ee-141">Request</span></span>
<span data-ttu-id="9b0ee-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9b0ee-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b0ee-143">Response</span></span>

<span data-ttu-id="9b0ee-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-144">Here is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="9b0ee-145">Exemplo 3: cartões</span><span class="sxs-lookup"><span data-stu-id="9b0ee-145">Example 3: Cards</span></span>

##### <a name="request"></a><span data-ttu-id="9b0ee-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b0ee-146">Request</span></span>
<span data-ttu-id="9b0ee-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9b0ee-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b0ee-148">Response</span></span>

<span data-ttu-id="9b0ee-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b0ee-149">Here is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9b0ee-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="9b0ee-150">See also</span></span>

- [<span data-ttu-id="9b0ee-151">Referência de cartões</span><span class="sxs-lookup"><span data-stu-id="9b0ee-151">Cards Reference</span></span>](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards-reference)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
