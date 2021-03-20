---
title: Responder a uma mensagem em um canal
description: Responder à mensagem existente em um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 29be6117b229da1d5b3921db7d52ae0e1897741c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948227"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="e5a4a-103">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="e5a4a-103">Reply to a message in a channel</span></span>

<span data-ttu-id="e5a4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5a4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5a4a-105">Crie uma nova resposta a [um chatMessage](../resources/chatmessage.md) em um canal [especificado](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="e5a4a-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="e5a4a-106">**Observação**: é uma violação dos termos [de](/legal/microsoft-apis/terms-of-use) uso usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="e5a4a-107">Envie apenas mensagens que as pessoas lerão.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-107">Only send messages that people will read.</span></span>
<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD001 -->

## <a name="permissions"></a><span data-ttu-id="e5a4a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5a4a-108">Permissions</span></span>
<span data-ttu-id="e5a4a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5a4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5a4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5a4a-111">Permission type</span></span>                        | <span data-ttu-id="e5a4a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5a4a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e5a4a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5a4a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5a4a-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5a4a-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e5a4a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5a4a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5a4a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-116">Not supported.</span></span> |
| <span data-ttu-id="e5a4a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5a4a-117">Application</span></span>                            | <span data-ttu-id="e5a4a-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="e5a4a-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="e5a4a-119">**Observação**: as permissões de aplicativo só *são* suportadas para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="e5a4a-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="e5a4a-120">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="e5a4a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5a4a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="e5a4a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5a4a-122">Request headers</span></span>
| <span data-ttu-id="e5a4a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e5a4a-123">Name</span></span>       | <span data-ttu-id="e5a4a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5a4a-124">Type</span></span> | <span data-ttu-id="e5a4a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5a4a-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5a4a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5a4a-126">Authorization</span></span>  | <span data-ttu-id="e5a4a-127">string</span><span class="sxs-lookup"><span data-stu-id="e5a4a-127">string</span></span>  | <span data-ttu-id="e5a4a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5a4a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5a4a-130">Request body</span></span>
<span data-ttu-id="e5a4a-131">No corpo da solicitação, fornece uma representação JSON de um [objeto message.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="e5a4a-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="e5a4a-132">Somente a propriedade body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="e5a4a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5a4a-133">Response</span></span>

<span data-ttu-id="e5a4a-134">Se tiver êxito, este método retornará `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example-1-create-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="e5a4a-135">Exemplo 1: Criar uma nova resposta para um chatMessage</span><span class="sxs-lookup"><span data-stu-id="e5a4a-135">Example 1: Create a new reply to a chatMessage</span></span>

<span data-ttu-id="e5a4a-136">Para obter uma lista mais abrangente de exemplos, consulte [Create chatMessage in a channel or a chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="e5a4a-136">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="e5a4a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5a4a-137">Request</span></span>
<span data-ttu-id="e5a4a-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5a4a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5a4a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[<span data-ttu-id="e5a4a-140">C#</span><span class="sxs-lookup"><span data-stu-id="e5a4a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5a4a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5a4a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5a4a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5a4a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5a4a-143">Java</span><span class="sxs-lookup"><span data-stu-id="e5a4a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e5a4a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5a4a-144">Response</span></span>

<span data-ttu-id="e5a4a-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-145">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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

### <a name="example-2-import-messages"></a><span data-ttu-id="e5a4a-146">Exemplo 2: Importar mensagens</span><span class="sxs-lookup"><span data-stu-id="e5a4a-146">Example 2: Import messages</span></span>

> <span data-ttu-id="e5a4a-147">**Observação**: o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-147">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="e5a4a-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5a4a-148">Request</span></span>

<span data-ttu-id="e5a4a-149">O exemplo a seguir mostra como importar mensagens back-in-time usando `createDateTime` as chaves e no corpo da `from` solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-149">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages/{messageId}/replies

{
   "replyToId":null,
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}
```

---
#### <a name="response"></a><span data-ttu-id="e5a4a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5a4a-150">Response</span></span>

<span data-ttu-id="e5a4a-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5a4a-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams/{teamId}/channels/{channelId}/messages/$entity",
   "id":"id-value",
   "replyToId":null,
   "etag":"id-value",
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
