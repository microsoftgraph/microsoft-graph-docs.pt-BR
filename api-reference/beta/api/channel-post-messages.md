---
title: Criar chat em um canal
description: Criar um novo chat no canal especificado.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0681ded7bb45eea328f9ce6a61f65683aa4d8cf9
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720862"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="264dc-103">Criar chat em um canal</span><span class="sxs-lookup"><span data-stu-id="264dc-103">Create chatMessage in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="264dc-104">Criar um novo [chat](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="264dc-104">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="264dc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="264dc-105">Permissions</span></span>

<span data-ttu-id="264dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="264dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="264dc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="264dc-108">Permission type</span></span>                        | <span data-ttu-id="264dc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="264dc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="264dc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="264dc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="264dc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="264dc-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="264dc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="264dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="264dc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="264dc-113">Not supported.</span></span> |
| <span data-ttu-id="264dc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="264dc-114">Application</span></span>                            | <span data-ttu-id="264dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="264dc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="264dc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="264dc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="264dc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="264dc-117">Request headers</span></span>

| <span data-ttu-id="264dc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="264dc-118">Name</span></span>          | <span data-ttu-id="264dc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="264dc-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="264dc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="264dc-120">Authorization</span></span> | <span data-ttu-id="264dc-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="264dc-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="264dc-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="264dc-122">Request body</span></span>

<span data-ttu-id="264dc-123">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="264dc-123">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="264dc-124">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="264dc-124">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="264dc-125">Observação: não há suporte para o envio de mensagens com anexos e imagens.</span><span class="sxs-lookup"><span data-stu-id="264dc-125">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="264dc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="264dc-126">Response</span></span>

<span data-ttu-id="264dc-127">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="264dc-127">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="264dc-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="264dc-128">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="264dc-129">Exemplo 1: Olá mundo</span><span class="sxs-lookup"><span data-stu-id="264dc-129">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="264dc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="264dc-130">Request</span></span>
<span data-ttu-id="264dc-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="264dc-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

#### <a name="response"></a><span data-ttu-id="264dc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="264dc-132">Response</span></span>

<span data-ttu-id="264dc-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="264dc-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="264dc-134">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="264dc-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="264dc-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="264dc-135">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="264dc-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="264dc-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="264dc-137">C#</span><span class="sxs-lookup"><span data-stu-id="264dc-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="264dc-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="264dc-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-mentions"></a><span data-ttu-id="264dc-139">Exemplo 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="264dc-139">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="264dc-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="264dc-140">Request</span></span>
<span data-ttu-id="264dc-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="264dc-141">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="264dc-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="264dc-142">Response</span></span>

<span data-ttu-id="264dc-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="264dc-143">The following is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="264dc-144">Exemplo 3: cartões</span><span class="sxs-lookup"><span data-stu-id="264dc-144">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="264dc-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="264dc-145">Request</span></span>
<span data-ttu-id="264dc-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="264dc-146">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="264dc-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="264dc-147">Response</span></span>

<span data-ttu-id="264dc-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="264dc-148">The following is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="264dc-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="264dc-149">See also</span></span>

- [<span data-ttu-id="264dc-150">Referência de cartões</span><span class="sxs-lookup"><span data-stu-id="264dc-150">Cards Reference</span></span>](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards-reference)

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
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
