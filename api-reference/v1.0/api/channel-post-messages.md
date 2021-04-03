---
title: Enviar chatMessage em um canal
description: Crie um novo chatMessage no canal especificado.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5fa0705ef44c1a6d6748d41f87680877afc59bbb
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582897"
---
# <a name="send-chatmessage-in-channel"></a><span data-ttu-id="d9259-103">Enviar chatMessage no canal</span><span class="sxs-lookup"><span data-stu-id="d9259-103">Send chatMessage in channel</span></span>

<span data-ttu-id="d9259-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9259-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9259-105">Envie um [novo chatMessage](../resources/chatmessage.md) no canal [especificado](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="d9259-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="d9259-106">**Observação**: é uma violação dos termos [de](/legal/microsoft-apis/terms-of-use) uso usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="d9259-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="d9259-107">Envie apenas mensagens que as pessoas lerão.</span><span class="sxs-lookup"><span data-stu-id="d9259-107">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9259-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9259-108">Permissions</span></span>

<span data-ttu-id="d9259-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9259-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9259-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9259-111">Permission type</span></span>                        | <span data-ttu-id="d9259-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9259-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9259-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9259-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9259-114">ChannelMessage.Send</span><span class="sxs-lookup"><span data-stu-id="d9259-114">ChannelMessage.Send</span></span> |
| <span data-ttu-id="d9259-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9259-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9259-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9259-116">Not supported.</span></span> |
| <span data-ttu-id="d9259-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9259-117">Application</span></span>                            | <span data-ttu-id="d9259-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="d9259-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="d9259-119">**Observação**: as permissões de aplicativo só *são* suportadas para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="d9259-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="d9259-120">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="d9259-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a><span data-ttu-id="d9259-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9259-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="d9259-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9259-122">Request headers</span></span>

| <span data-ttu-id="d9259-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d9259-123">Name</span></span>          | <span data-ttu-id="d9259-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9259-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d9259-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9259-125">Authorization</span></span> | <span data-ttu-id="d9259-126">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="d9259-126">Bearer {code}.</span></span> <span data-ttu-id="d9259-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9259-127">Required.</span></span> |
| <span data-ttu-id="d9259-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="d9259-128">Content-type</span></span> | <span data-ttu-id="d9259-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9259-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9259-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9259-131">Request body</span></span>

<span data-ttu-id="d9259-132">No corpo da solicitação, fornece uma representação JSON de um [objeto chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="d9259-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="d9259-133">Somente a propriedade body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="d9259-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="d9259-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9259-134">Response</span></span>

<span data-ttu-id="d9259-135">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9259-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9259-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9259-136">Examples</span></span>

### <a name="example-1-create-a-message-in-a-specified-channel"></a><span data-ttu-id="d9259-137">Exemplo 1: Criar uma mensagem em um canal especificado</span><span class="sxs-lookup"><span data-stu-id="d9259-137">Example 1: Create a message in a specified channel</span></span>

<span data-ttu-id="d9259-138">Para obter uma lista mais abrangente de exemplos, consulte [Create chatMessage in a channel or a chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="d9259-138">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="d9259-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9259-139">Request</span></span>
<span data-ttu-id="d9259-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9259-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_channelmessage_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

### <a name="response"></a><span data-ttu-id="d9259-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9259-141">Response</span></span>

<span data-ttu-id="d9259-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9259-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1616990032035",
    "replyToId": null,
    "etag": "1616990032035",
    "messageType": "message",
    "createdDateTime": "2021-03-29T03:53:52.035Z",
    "lastModifiedDateTime": "2021-03-29T03:53:52.035Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616990032035?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990032035&parentMessageId=1616990032035",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Robin Kline",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "text",
        "content": "Hello World"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-import-messages"></a><span data-ttu-id="d9259-143">Exemplo 2: Importar mensagens</span><span class="sxs-lookup"><span data-stu-id="d9259-143">Example 2: Import messages</span></span>

> <span data-ttu-id="d9259-144">**Observação**: o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.</span><span class="sxs-lookup"><span data-stu-id="d9259-144">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="d9259-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9259-145">Request</span></span>

<span data-ttu-id="d9259-146">O exemplo a seguir mostra como importar mensagens back-in-time usando `createDateTime` as chaves e no corpo da `from` solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9259-146">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_channelmessage_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   }
}
```

### <a name="response"></a><span data-ttu-id="d9259-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9259-147">Response</span></span>

<span data-ttu-id="d9259-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9259-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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
         "displayName":"John Doe",
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

### <a name="example-3-import-messages-with-inline-images"></a><span data-ttu-id="d9259-149">Exemplo 3: Importar mensagens com imagens em linha</span><span class="sxs-lookup"><span data-stu-id="d9259-149">Example 3: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="d9259-150">Atualmente, as imagens em linha são o único tipo de mídia suportado pelo esquema de API de mensagem de importação.</span><span class="sxs-lookup"><span data-stu-id="d9259-150">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="d9259-151">**Observação**: o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.</span><span class="sxs-lookup"><span data-stu-id="d9259-151">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="d9259-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9259-152">Request</span></span>

<span data-ttu-id="d9259-153">O exemplo a seguir mostra como importar mensagens back-in-time que contêm imagens em linha usando as chaves e `createDateTime` `from` no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9259-153">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_channelmessage_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"John Doe",
         "userIdentityType":"aadUser"
      }
   },
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

#### <a name="response"></a><span data-ttu-id="d9259-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9259-154">Response</span></span>

<span data-ttu-id="d9259-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9259-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

## <a name="see-also"></a><span data-ttu-id="d9259-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="d9259-156">See also</span></span>

* [<span data-ttu-id="d9259-157">Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d9259-157">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="d9259-158">Create channel</span><span class="sxs-lookup"><span data-stu-id="d9259-158">Create channel</span></span>](channel-post.md)

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
