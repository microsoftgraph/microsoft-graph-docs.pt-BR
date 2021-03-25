---
title: Responder a uma mensagem em um canal
description: Responder à mensagem existente em um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b7c9e4b706e848218d55ab1898a03096f2d5aba9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201096"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="fc7f4-103">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="fc7f4-103">Reply to a message in a channel</span></span>

<span data-ttu-id="fc7f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc7f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc7f4-105">Crie uma nova resposta a [um chatMessage](../resources/chatmessage.md) em um canal [especificado](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="fc7f4-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="fc7f4-106">**Observação**: é uma violação dos termos [de](/legal/microsoft-apis/terms-of-use) uso usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="fc7f4-107">Envie apenas mensagens que as pessoas lerão.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-107">Only send messages that people will read.</span></span>
<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD001 -->

## <a name="permissions"></a><span data-ttu-id="fc7f4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc7f4-108">Permissions</span></span>
<span data-ttu-id="fc7f4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc7f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc7f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc7f4-111">Permission type</span></span>                        | <span data-ttu-id="fc7f4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc7f4-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fc7f4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc7f4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc7f4-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc7f4-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="fc7f4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc7f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc7f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-116">Not supported.</span></span> |
| <span data-ttu-id="fc7f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc7f4-117">Application</span></span>                            | <span data-ttu-id="fc7f4-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="fc7f4-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="fc7f4-119">**Observação**: as permissões de aplicativo só *são* suportadas para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="fc7f4-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="fc7f4-120">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="fc7f4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc7f4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="fc7f4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7f4-122">Request headers</span></span>
| <span data-ttu-id="fc7f4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fc7f4-123">Name</span></span>       | <span data-ttu-id="fc7f4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc7f4-124">Type</span></span> | <span data-ttu-id="fc7f4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc7f4-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc7f4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc7f4-126">Authorization</span></span>  | <span data-ttu-id="fc7f4-127">string</span><span class="sxs-lookup"><span data-stu-id="fc7f4-127">string</span></span>  | <span data-ttu-id="fc7f4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc7f4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7f4-130">Request body</span></span>
<span data-ttu-id="fc7f4-131">No corpo da solicitação, fornece uma representação JSON de um [objeto message.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="fc7f4-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="fc7f4-132">Somente a propriedade body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="fc7f4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7f4-133">Response</span></span>

<span data-ttu-id="fc7f4-134">Se tiver êxito, este método retornará `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="fc7f4-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc7f4-135">Examples</span></span>

### <a name="example-1-create-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="fc7f4-136">Exemplo 1: Criar uma nova resposta para um chatMessage</span><span class="sxs-lookup"><span data-stu-id="fc7f4-136">Example 1: Create a new reply to a chatMessage</span></span>

<span data-ttu-id="fc7f4-137">Para obter uma lista mais abrangente de exemplos, consulte [Create chatMessage in a channel or a chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="fc7f4-137">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

#### <a name="request"></a><span data-ttu-id="fc7f4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7f4-138">Request</span></span>
<span data-ttu-id="fc7f4-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc7f4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc7f4-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[<span data-ttu-id="fc7f4-141">C#</span><span class="sxs-lookup"><span data-stu-id="fc7f4-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc7f4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc7f4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc7f4-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc7f4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc7f4-144">Java</span><span class="sxs-lookup"><span data-stu-id="fc7f4-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="fc7f4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7f4-145">Response</span></span>

<span data-ttu-id="fc7f4-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-146">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
    "id": "1591039710682",
    "replyToId": "1590776551682",
    "etag": "1591039710682",
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
            "id": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
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

### <a name="example-2-import-messages"></a><span data-ttu-id="fc7f4-147">Exemplo 2: Importar mensagens</span><span class="sxs-lookup"><span data-stu-id="fc7f4-147">Example 2: Import messages</span></span>

> <span data-ttu-id="fc7f4-148">**Observação**: o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-148">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="fc7f4-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7f4-149">Request</span></span>

<span data-ttu-id="fc7f4-150">O exemplo a seguir mostra como importar mensagens back-in-time usando `createDateTime` as chaves e no corpo da `from` solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-150">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
         "displayName":"Joh Doe"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   }
}
```

---
#### <a name="response"></a><span data-ttu-id="fc7f4-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7f4-151">Response</span></span>

<span data-ttu-id="fc7f4-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc7f4-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
   "id":"1591039710682",
   "replyToId":"1590776551682",
   "etag":"1591039710682",
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
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
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
