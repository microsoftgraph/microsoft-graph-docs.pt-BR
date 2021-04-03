---
title: Enviar respostas a uma mensagem em um canal
description: Responder à mensagem existente em um canal.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c81936cf52af8990e04c025fc533343d96f6bdc
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582894"
---
# <a name="send-replies-to-a-message-in-a-channel"></a><span data-ttu-id="b048b-103">Enviar respostas a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="b048b-103">Send replies to a message in a channel</span></span>

<span data-ttu-id="b048b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b048b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b048b-105">Envie uma nova resposta a [um chatMessage](../resources/chatmessage.md) em um canal [especificado](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="b048b-105">Send a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="b048b-106">**Observação**: é uma violação dos termos [de](/legal/microsoft-apis/terms-of-use) uso usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="b048b-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="b048b-107">Envie apenas mensagens que as pessoas lerão.</span><span class="sxs-lookup"><span data-stu-id="b048b-107">Only send messages that people will read.</span></span>
<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD001 -->

## <a name="permissions"></a><span data-ttu-id="b048b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b048b-108">Permissions</span></span>
<span data-ttu-id="b048b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b048b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b048b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b048b-111">Permission type</span></span>                        | <span data-ttu-id="b048b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b048b-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b048b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b048b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b048b-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b048b-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b048b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b048b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b048b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b048b-116">Not supported.</span></span> |
| <span data-ttu-id="b048b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b048b-117">Application</span></span>                            | <span data-ttu-id="b048b-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="b048b-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="b048b-119">**Observação**: as permissões de aplicativo só *são* suportadas para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span><span class="sxs-lookup"><span data-stu-id="b048b-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="b048b-120">No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.</span><span class="sxs-lookup"><span data-stu-id="b048b-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="b048b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b048b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="b048b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b048b-122">Request headers</span></span>
| <span data-ttu-id="b048b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b048b-123">Name</span></span>       | <span data-ttu-id="b048b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b048b-124">Type</span></span> | <span data-ttu-id="b048b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b048b-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b048b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b048b-126">Authorization</span></span>  | <span data-ttu-id="b048b-127">string</span><span class="sxs-lookup"><span data-stu-id="b048b-127">string</span></span>  | <span data-ttu-id="b048b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b048b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b048b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b048b-130">Request body</span></span>
<span data-ttu-id="b048b-131">No corpo da solicitação, fornece uma representação JSON de um [objeto message.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="b048b-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="b048b-132">Somente a propriedade body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="b048b-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="b048b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b048b-133">Response</span></span>

<span data-ttu-id="b048b-134">Se tiver êxito, este método retornará `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="b048b-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="b048b-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b048b-135">Examples</span></span>

### <a name="example-1-send-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="b048b-136">Exemplo 1: Enviar uma nova resposta a um chatMessage</span><span class="sxs-lookup"><span data-stu-id="b048b-136">Example 1: Send a new reply to a chatMessage</span></span>

<span data-ttu-id="b048b-137">Para obter uma lista mais abrangente de exemplos, consulte [Create chatMessage in a channel or a chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="b048b-137">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

#### <a name="request"></a><span data-ttu-id="b048b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b048b-138">Request</span></span>
<span data-ttu-id="b048b-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b048b-139">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessagereply_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616990032035/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

#### <a name="response"></a><span data-ttu-id="b048b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b048b-140">Response</span></span>

<span data-ttu-id="b048b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b048b-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616990032035')/replies/$entity",
    "id": "1616990171266",
    "replyToId": "1616990032035",
    "etag": "1616990171266",
    "messageType": "message",
    "createdDateTime": "2021-03-29T03:56:11.266Z",
    "lastModifiedDateTime": "2021-03-29T03:56:11.266Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616990171266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990171266&parentMessageId=1616990032035",
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

### <a name="example-2-import-messages"></a><span data-ttu-id="b048b-142">Exemplo 2: Importar mensagens</span><span class="sxs-lookup"><span data-stu-id="b048b-142">Example 2: Import messages</span></span>

> <span data-ttu-id="b048b-143">**Observação**: o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.</span><span class="sxs-lookup"><span data-stu-id="b048b-143">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="b048b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b048b-144">Request</span></span>

<span data-ttu-id="b048b-145">O exemplo a seguir mostra como importar mensagens back-in-time usando `createDateTime` as chaves e no corpo da `from` solicitação.</span><span class="sxs-lookup"><span data-stu-id="b048b-145">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessagereply_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
         "displayName":"John Doe"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   }
}
```

#### <a name="response"></a><span data-ttu-id="b048b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b048b-146">Response</span></span>

<span data-ttu-id="b048b-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b048b-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
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
