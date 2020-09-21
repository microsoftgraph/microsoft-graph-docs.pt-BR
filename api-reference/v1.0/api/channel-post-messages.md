---
title: Criar chatMessage em um canal
description: Criar um novo chat no canal especificado.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ae273c120aa505b972a31794406bb700c7c49364
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063868"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="19a2e-103">Criar chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="19a2e-103">Create chatMessage in a channel</span></span>

<span data-ttu-id="19a2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19a2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19a2e-105">Criar um novo [chat](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="19a2e-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="19a2e-106">**Observação**: não é recomendável usar essa API para a migração de dados.</span><span class="sxs-lookup"><span data-stu-id="19a2e-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="19a2e-107">Ele não tem a taxa de transferência necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="19a2e-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="19a2e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="19a2e-108">Permissions</span></span>

<span data-ttu-id="19a2e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19a2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19a2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19a2e-111">Permission type</span></span>                        | <span data-ttu-id="19a2e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19a2e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19a2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19a2e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="19a2e-114">ChannelMessage. Send, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="19a2e-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="19a2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19a2e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19a2e-116">Not supported.</span></span> |
| <span data-ttu-id="19a2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19a2e-117">Application</span></span>                            | <span data-ttu-id="19a2e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19a2e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19a2e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="19a2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19a2e-120">Request headers</span></span>

| <span data-ttu-id="19a2e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="19a2e-121">Name</span></span>          | <span data-ttu-id="19a2e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19a2e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="19a2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19a2e-123">Authorization</span></span> | <span data-ttu-id="19a2e-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="19a2e-124">Bearer {code}.</span></span> <span data-ttu-id="19a2e-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19a2e-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a2e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19a2e-126">Request body</span></span>

<span data-ttu-id="19a2e-127">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="19a2e-127">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="19a2e-128">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="19a2e-128">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="19a2e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a2e-129">Response</span></span>

<span data-ttu-id="19a2e-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19a2e-130">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19a2e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19a2e-131">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="19a2e-132">Exemplo 1: Olá mundo</span><span class="sxs-lookup"><span data-stu-id="19a2e-132">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="19a2e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19a2e-133">Request</span></span>

<span data-ttu-id="19a2e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a2e-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="19a2e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="19a2e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="19a2e-136">C#</span><span class="sxs-lookup"><span data-stu-id="19a2e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19a2e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19a2e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19a2e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19a2e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19a2e-139">Java</span><span class="sxs-lookup"><span data-stu-id="19a2e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19a2e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a2e-140">Response</span></span>

<span data-ttu-id="19a2e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19a2e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="19a2e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19a2e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
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

### <a name="example-2-mentions"></a><span data-ttu-id="19a2e-144">Exemplo 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="19a2e-144">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="19a2e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19a2e-145">Request</span></span>
<span data-ttu-id="19a2e-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a2e-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
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

#### <a name="response"></a><span data-ttu-id="19a2e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a2e-147">Response</span></span>

<span data-ttu-id="19a2e-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19a2e-148">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
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

### <a name="example-3-cards"></a><span data-ttu-id="19a2e-149">Exemplo 3: cartões</span><span class="sxs-lookup"><span data-stu-id="19a2e-149">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="19a2e-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19a2e-150">Request</span></span>
<span data-ttu-id="19a2e-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a2e-151">The following is an example of the request.</span></span>

><span data-ttu-id="19a2e-152">**Observação:** A ID do anexo deve ser exclusiva e pode ser um novo GUID gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="19a2e-152">**Note:** The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="19a2e-153">No entanto, a ID do anexo deve ser a mesma nos elementos _Body_ e _Attachments_ .</span><span class="sxs-lookup"><span data-stu-id="19a2e-153">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
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

#### <a name="response"></a><span data-ttu-id="19a2e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a2e-154">Response</span></span>

<span data-ttu-id="19a2e-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19a2e-155">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('bdb7bcda-9c3b-4341-b9a9-f52bf9a23407')/channels('19%3A786524f437c042b68bac5c0511ad6be2%40thread.skype')/messages/$entity",
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

### <a name="example-4-file-attachments"></a><span data-ttu-id="19a2e-156">Exemplo 4: anexos de arquivo</span><span class="sxs-lookup"><span data-stu-id="19a2e-156">Example 4: File attachments</span></span>

#### <a name="request"></a><span data-ttu-id="19a2e-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19a2e-157">Request</span></span>
<span data-ttu-id="19a2e-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a2e-158">The following is an example of the request.</span></span>

><span data-ttu-id="19a2e-159">**Observação:** O arquivo já deve estar no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="19a2e-159">**Note:** The file must already be in SharePoint.</span></span> <span data-ttu-id="19a2e-160">Para localizar as propriedades do arquivo, obtenha o **driveItem** para o arquivo.</span><span class="sxs-lookup"><span data-stu-id="19a2e-160">To find the file properties, GET the **driveItem** for the file.</span></span> <span data-ttu-id="19a2e-161">Por exemplo,/drives/{ID}/Items/{ID}.</span><span class="sxs-lookup"><span data-stu-id="19a2e-161">For example, /drives/{id}/items/{id}.</span></span> <span data-ttu-id="19a2e-162">Sua ID de anexo é o GUID na **ETag** do **DriveItem**, seu **ContentURL** de anexo é o **WebUrl** da pasta do **driveItem**mais o nome do **driveItem**e o nome do anexo é o nome do **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="19a2e-162">Your attachment ID is the GUID in the **eTag** of the **driveItem**, your attachment **contentURL** is the **webUrl** of the **driveItem**'s folder plus the **driveItem**'s name, and your attachment name is the **driveItem**'s name.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "body": {
        "contentType": "html",
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "name": "Budget.docx"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="19a2e-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a2e-163">Response</span></span>

<span data-ttu-id="19a2e-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19a2e-164">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('13a99602-a5d3-4fed-99d2-7dc3ffe3730d')/channels('19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2')/messages/$entity",
    "id": "1589481435511",
    "replyToId": null,
    "etag": "1589481435511",
    "messageType": "message",
    "createdDateTime": "2020-05-14T18:37:15.511Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2/1589481435511?groupId=13a99602-a5d3-4fed-99d2-7dc3ffe3730d&tenantId=e5648b2b-1dea-445a-ab65-4f9326c2bd10&createdTime=1589481435511&parentMessageId=1589481435511",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "598efcd4-e549-402a-9602-0b50201faebe",
            "displayName": "MOD Administrator",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "content": null,
            "name": "Budget.docx",
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a><span data-ttu-id="19a2e-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="19a2e-165">See also</span></span>

- [<span data-ttu-id="19a2e-166">Referência de cartões</span><span class="sxs-lookup"><span data-stu-id="19a2e-166">Cards reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)

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

