---
title: Criar chatMessage em um canal
description: Crie um novo chatMessage no canal especificado.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0c6a6f5c8ee8fe98d1e65163c2c9a30bb5ec7301
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948274"
---
# <a name="create-chatmessage-in-channel"></a><span data-ttu-id="87dc2-103">Criar chatMessage no canal</span><span class="sxs-lookup"><span data-stu-id="87dc2-103">Create chatMessage in channel</span></span>

<span data-ttu-id="87dc2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87dc2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87dc2-105">Crie um [novo chatMessage](../resources/chatmessage.md) no canal [especificado](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="87dc2-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="87dc2-106">**Observação**: é uma violação dos termos [de](/legal/microsoft-apis/terms-of-use) uso usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="87dc2-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="87dc2-107">Envie apenas mensagens que as pessoas lerão.</span><span class="sxs-lookup"><span data-stu-id="87dc2-107">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="87dc2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="87dc2-108">Permissions</span></span>

<span data-ttu-id="87dc2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87dc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87dc2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87dc2-111">Permission type</span></span>                        | <span data-ttu-id="87dc2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87dc2-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="87dc2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87dc2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="87dc2-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87dc2-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="87dc2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87dc2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87dc2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87dc2-116">Not supported.</span></span> |
| <span data-ttu-id="87dc2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87dc2-117">Application</span></span>                            | <span data-ttu-id="87dc2-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="87dc2-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="87dc2-119">**Observação**: as permissões de aplicativo só *são* suportadas para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="87dc2-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="87dc2-120">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="87dc2-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a><span data-ttu-id="87dc2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87dc2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="87dc2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87dc2-122">Request headers</span></span>

| <span data-ttu-id="87dc2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="87dc2-123">Name</span></span>          | <span data-ttu-id="87dc2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="87dc2-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="87dc2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="87dc2-125">Authorization</span></span> | <span data-ttu-id="87dc2-126">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="87dc2-126">Bearer {code}.</span></span> <span data-ttu-id="87dc2-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87dc2-127">Required.</span></span> |
| <span data-ttu-id="87dc2-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="87dc2-128">Content-type</span></span> | <span data-ttu-id="87dc2-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87dc2-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87dc2-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87dc2-131">Request body</span></span>

<span data-ttu-id="87dc2-132">No corpo da solicitação, fornece uma representação JSON de um [objeto chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="87dc2-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="87dc2-133">Somente a propriedade body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="87dc2-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="87dc2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="87dc2-134">Response</span></span>

<span data-ttu-id="87dc2-135">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87dc2-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87dc2-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87dc2-136">Examples</span></span>

### <a name="example-1-create-a-message-in-a-specified-channel"></a><span data-ttu-id="87dc2-137">Exemplo 1: Criar uma mensagem em um canal especificado</span><span class="sxs-lookup"><span data-stu-id="87dc2-137">Example 1: Create a message in a specified channel</span></span>

<span data-ttu-id="87dc2-138">Para obter uma lista mais abrangente de exemplos, consulte [Create chatMessage in a channel or a chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="87dc2-138">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="87dc2-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87dc2-139">Request</span></span>
<span data-ttu-id="87dc2-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87dc2-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87dc2-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="87dc2-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_1"
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

# <a name="c"></a>[<span data-ttu-id="87dc2-142">C#</span><span class="sxs-lookup"><span data-stu-id="87dc2-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87dc2-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87dc2-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87dc2-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87dc2-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87dc2-145">Java</span><span class="sxs-lookup"><span data-stu-id="87dc2-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="87dc2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="87dc2-146">Response</span></span>

<span data-ttu-id="87dc2-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87dc2-147">The following is an example of the response.</span></span>

> <span data-ttu-id="87dc2-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87dc2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-import-messages-text-only"></a><span data-ttu-id="87dc2-150">Exemplo 2: Importar mensagens (somente texto)</span><span class="sxs-lookup"><span data-stu-id="87dc2-150">Example 2: Import messages (text only)</span></span>

> <span data-ttu-id="87dc2-151">**Observação**: o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.</span><span class="sxs-lookup"><span data-stu-id="87dc2-151">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="87dc2-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87dc2-152">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="87dc2-153">O exemplo a seguir mostra como importar mensagens back-in-time usando `createDateTime` as chaves e no corpo da `from` solicitação.</span><span class="sxs-lookup"><span data-stu-id="87dc2-153">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages

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

### <a name="response"></a><span data-ttu-id="87dc2-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="87dc2-154">Response</span></span>

<span data-ttu-id="87dc2-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87dc2-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('teamId')/channels('channelId')/messages/$entity",
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

### <a name="example-3-import-messages-with-inline-images"></a><span data-ttu-id="87dc2-156">Exemplo 3: Importar mensagens com imagens em linha</span><span class="sxs-lookup"><span data-stu-id="87dc2-156">Example 3: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="87dc2-157">Atualmente, as imagens em linha são o único tipo de mídia suportado pelo esquema de API de mensagem de importação.</span><span class="sxs-lookup"><span data-stu-id="87dc2-157">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="87dc2-158">**Observação**: o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.</span><span class="sxs-lookup"><span data-stu-id="87dc2-158">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="87dc2-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87dc2-159">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="87dc2-160">O exemplo a seguir mostra como importar mensagens back-in-time que contêm imagens em linha usando as chaves e `createDateTime` `from` no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87dc2-160">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"John Doe",
         "userIdentityType":"aadUser"
      }
   },
{
   "body":{
      "contentType":"html",
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"../hostedContents/1/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "hostedContents":[
      {
         "@microsoft.graph.temporaryId":"1",
         "contentBytes":"iVBORw0KGgoAAAANSUhEUgAAANcAAAExCAYAAADvFzeeAAAXjklEQVR4Ae2d/XNU1RnH+9e0FFrA0RCIyaS8hRA0HV5KbS1gHRgVpjMClY4GHJ3yYm1HCmXaWttaaZUZtIIFKYi8lFAkvOQ9u5vN225IARVBbX9/Os9NbrLZbMjmhCfJPX5+2Lmb3T25y3O+n/M599x7w9f+++UXwoMakIF7n4GvUdR7X1RqSk01A8CFuZm5GGUAuIwKi72wF3ABF+YyygBwGRUWc2Eu4AIuzGWUAeAyKizmwlzABVyYyygDwGVUWMyFuYALuDCXUQaAy6iwmAtzARdwfWXMdeuzT+TGxz3Sfb1LunrapL07IW3pePDQ5/qavqef0c+OdYAELuAac4jGGkLL9rdvfyo9N9ODQAqBGmmrwGlb/R0u3xG4gMspOC5hG882CoRaaCSA8n1ff9doIQMu4PIOrus3u+8ZVNnw6e/Od5AALuDKOyz5hmqiPnfnzi1J9bSbgRWCpvvQfY307wQu4BoxJCOFaDK8rwsQmQsUIQhWW93XSIsewAVckYdLQ24F0Ui/926AARdwRRounZ6Np7GyYdN9DzdFBC7gijRc43GMlQ1U9s/6HXJNjYELuHI<<-----Removed----->>>>",
         "contentType":"image/png"
      }
   ]
}
```

#### <a name="response"></a><span data-ttu-id="87dc2-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="87dc2-161">Response</span></span>

<span data-ttu-id="87dc2-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87dc2-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('teamId')/channels('channelId')/messages/$entity",
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
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"https://graph.microsoft.com/teams/teamId/channels/channelId/messages/id-value/hostedContents/hostedContentId/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}

```

## <a name="see-also"></a><span data-ttu-id="87dc2-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="87dc2-163">See also</span></span>

* [<span data-ttu-id="87dc2-164">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="87dc2-164">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="87dc2-165">Create channel</span><span class="sxs-lookup"><span data-stu-id="87dc2-165">Create channel</span></span>](channel-post.md)

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
