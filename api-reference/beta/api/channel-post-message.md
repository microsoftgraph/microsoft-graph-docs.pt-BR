---
title: Criar chatMessage em um canal
description: Criar novo chat no canal especificado.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9c4668c1f9c19cade4d737ee23273ebdd82f65d
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782760"
---
# <a name="create-chatmessage-in-channel"></a><span data-ttu-id="ddc09-103">Criar chat no canal</span><span class="sxs-lookup"><span data-stu-id="ddc09-103">Create chatMessage in channel</span></span>

<span data-ttu-id="ddc09-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddc09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddc09-105">Criar um novo [chat](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="ddc09-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="ddc09-106">**Observação** : não é recomendável usar essa API para a migração de dados.</span><span class="sxs-lookup"><span data-stu-id="ddc09-106">**Note** : We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="ddc09-107">Ele não tem a taxa de transferência necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="ddc09-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="ddc09-108">**Observação** : trata-se de uma violação dos [termos de uso](/legal/microsoft-apis/terms-of-use) para usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="ddc09-108">**Note** : It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="ddc09-109">Só envie mensagens que as pessoas lerám.</span><span class="sxs-lookup"><span data-stu-id="ddc09-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddc09-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddc09-110">Permissions</span></span>

<span data-ttu-id="ddc09-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddc09-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddc09-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddc09-113">Permission type</span></span>                        | <span data-ttu-id="ddc09-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddc09-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ddc09-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddc09-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddc09-116">ChannelMessage. Send, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ddc09-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ddc09-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddc09-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddc09-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddc09-118">Not supported.</span></span> |
| <span data-ttu-id="ddc09-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddc09-119">Application</span></span>                            | <span data-ttu-id="ddc09-120">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="ddc09-120">Teamwork.Migrate.All</span></span> |

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a><span data-ttu-id="ddc09-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddc09-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="ddc09-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc09-122">Request headers</span></span>

| <span data-ttu-id="ddc09-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ddc09-123">Name</span></span>          | <span data-ttu-id="ddc09-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddc09-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ddc09-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddc09-125">Authorization</span></span> | <span data-ttu-id="ddc09-126">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="ddc09-126">Bearer {code}.</span></span> <span data-ttu-id="ddc09-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddc09-127">Required.</span></span> |
| <span data-ttu-id="ddc09-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="ddc09-128">Content-type</span></span> | <span data-ttu-id="ddc09-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddc09-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddc09-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc09-131">Request body</span></span>

<span data-ttu-id="ddc09-132">No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="ddc09-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="ddc09-133">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="ddc09-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="ddc09-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddc09-134">Response</span></span>

<span data-ttu-id="ddc09-135">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddc09-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddc09-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddc09-136">Examples</span></span>

### <a name="example-1-create-a-message-in-a-specified-channel"></a><span data-ttu-id="ddc09-137">Exemplo 1: criar uma mensagem em um canal especificado</span><span class="sxs-lookup"><span data-stu-id="ddc09-137">Example 1: Create a message in a specified channel</span></span>

<span data-ttu-id="ddc09-138">Para obter uma lista mais abrangente de exemplos, consulte [criar chat em um canal ou em um chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="ddc09-138">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="ddc09-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc09-139">Request</span></span>
<span data-ttu-id="ddc09-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddc09-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddc09-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddc09-141">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="ddc09-142">C#</span><span class="sxs-lookup"><span data-stu-id="ddc09-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddc09-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddc09-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddc09-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddc09-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ddc09-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddc09-145">Response</span></span>

<span data-ttu-id="ddc09-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddc09-146">The following is an example of the response.</span></span>

> <span data-ttu-id="ddc09-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddc09-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-import-messages-text-only"></a><span data-ttu-id="ddc09-149">Exemplo 2: importar mensagens (somente texto)</span><span class="sxs-lookup"><span data-stu-id="ddc09-149">Example 2: Import messages (text only)</span></span>

> <span data-ttu-id="ddc09-150">**Observação** : nenhum escopo de permissão especial é necessário para este cenário porque a solicitação faz parte do **chat** ; os escopos para **chat** também são aplicados aqui.</span><span class="sxs-lookup"><span data-stu-id="ddc09-150">**Note** : No special permission scopes are required for this scenario because the request is part of **chatMessage** ; scopes for **chatMessage** apply here as well.</span></span>

#### <a name="request"></a><span data-ttu-id="ddc09-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc09-151">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ddc09-152">O exemplo a seguir mostra como importar mensagens Back-in-time usando as `createDateTime` `from` teclas e no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddc09-152">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

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

### <a name="response"></a><span data-ttu-id="ddc09-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddc09-153">Response</span></span>

<span data-ttu-id="ddc09-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddc09-154">The following is an example of the response.</span></span>

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

### <a name="example-3-import-messages-with-inline-images"></a><span data-ttu-id="ddc09-155">Exemplo 3: importar mensagens com imagens embutidas</span><span class="sxs-lookup"><span data-stu-id="ddc09-155">Example 3: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="ddc09-156">Atualmente, as imagens embutidas são o único tipo de mídia suportado pelo esquema de API de mensagens de importação.</span><span class="sxs-lookup"><span data-stu-id="ddc09-156">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="ddc09-157">**Observação** : nenhum escopo de permissão especial é necessário para este cenário porque a solicitação faz parte do **chat** ; os escopos para **chat** também são aplicados aqui.</span><span class="sxs-lookup"><span data-stu-id="ddc09-157">**Note** : No special permission scopes are required for this scenario because the request is part of **chatMessage** ; scopes for **chatMessage** apply here as well.</span></span>

#### <a name="request"></a><span data-ttu-id="ddc09-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc09-158">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ddc09-159">O exemplo a seguir mostra como importar mensagens de Back-in-time contendo imagens embutidas usando as `createDateTime` `from` teclas e no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddc09-159">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages

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

#### <a name="response"></a><span data-ttu-id="ddc09-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddc09-160">Response</span></span>

<span data-ttu-id="ddc09-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddc09-161">The following is an example of the response.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ddc09-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="ddc09-162">See also</span></span>

* [<span data-ttu-id="ddc09-163">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ddc09-163">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="ddc09-164">Create channel</span><span class="sxs-lookup"><span data-stu-id="ddc09-164">Create channel</span></span>](channel-post.md)

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
