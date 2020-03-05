---
title: Criar chatMessage em um canal
description: Criar um novo chat no canal especificado.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 02d91e5880e1eb19b7da18c36177f080c9154083
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440126"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="bc462-103">Criar chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="bc462-103">Create chatMessage in a channel</span></span>

<span data-ttu-id="bc462-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bc462-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc462-105">Criar um novo [chat](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="bc462-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="bc462-106">**Observação**: não é recomendável usar essa API para a migração de dados.</span><span class="sxs-lookup"><span data-stu-id="bc462-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="bc462-107">Ele não tem a taxa de transferência necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="bc462-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc462-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc462-108">Permissions</span></span>

<span data-ttu-id="bc462-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc462-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc462-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc462-111">Permission type</span></span>                        | <span data-ttu-id="bc462-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc462-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bc462-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc462-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc462-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc462-114">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bc462-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc462-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc462-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc462-116">Not supported.</span></span> |
| <span data-ttu-id="bc462-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc462-117">Application</span></span>                            | <span data-ttu-id="bc462-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc462-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc462-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc462-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="bc462-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc462-120">Request headers</span></span>

| <span data-ttu-id="bc462-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bc462-121">Name</span></span>          | <span data-ttu-id="bc462-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc462-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bc462-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc462-123">Authorization</span></span> | <span data-ttu-id="bc462-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="bc462-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc462-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc462-125">Request body</span></span>

<span data-ttu-id="bc462-126">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="bc462-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="bc462-127">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="bc462-127">Only the body property is mandatory, other properties are optional.</span></span>


## <a name="response"></a><span data-ttu-id="bc462-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc462-128">Response</span></span>

<span data-ttu-id="bc462-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc462-129">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc462-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bc462-130">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="bc462-131">Exemplo 1: Olá mundo</span><span class="sxs-lookup"><span data-stu-id="bc462-131">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="bc462-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc462-132">Request</span></span>
<span data-ttu-id="bc462-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc462-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc462-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc462-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bc462-135">C#</span><span class="sxs-lookup"><span data-stu-id="bc462-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc462-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc462-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc462-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc462-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bc462-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc462-138">Response</span></span>

<span data-ttu-id="bc462-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc462-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="bc462-140">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bc462-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc462-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc462-141">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-mentions"></a><span data-ttu-id="bc462-142">Exemplo 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="bc462-142">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="bc462-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc462-143">Request</span></span>
<span data-ttu-id="bc462-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc462-144">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="bc462-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc462-145">Response</span></span>

<span data-ttu-id="bc462-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc462-146">The following is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="bc462-147">Exemplo 3: cartões</span><span class="sxs-lookup"><span data-stu-id="bc462-147">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="bc462-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc462-148">Request</span></span>
<span data-ttu-id="bc462-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc462-149">The following is an example of the request.</span></span>

> <span data-ttu-id="bc462-150">Observação: a ID do anexo deve ser exclusiva e pode ser um novo GUID gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="bc462-150">Note: The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="bc462-151">No entanto, a ID do anexo deve ser a mesma nos elementos _Body_ e _Attachments_ .</span><span class="sxs-lookup"><span data-stu-id="bc462-151">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>

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

#### <a name="response"></a><span data-ttu-id="bc462-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc462-152">Response</span></span>

<span data-ttu-id="bc462-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc462-153">The following is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bc462-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="bc462-154">See also</span></span>

- [<span data-ttu-id="bc462-155">Referência de cartões</span><span class="sxs-lookup"><span data-stu-id="bc462-155">Cards Reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)

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
  ]
}
-->
