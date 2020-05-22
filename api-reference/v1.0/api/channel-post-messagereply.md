---
title: Responder a uma mensagem em um canal
description: Responder a uma mensagem existente em um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 86d246098801954c811d56e2357356f9b5c4a4c2
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345797"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="0c9d4-103">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="0c9d4-103">Reply to a message in a channel</span></span>

<span data-ttu-id="0c9d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c9d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c9d4-105">Criar uma nova resposta a uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="0c9d4-105">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="0c9d4-106">**Observação**: não é recomendável usar essa API para a migração de dados.</span><span class="sxs-lookup"><span data-stu-id="0c9d4-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="0c9d4-107">Ele não tem a taxa de transferência necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="0c9d4-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c9d4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c9d4-108">Permissions</span></span>

<span data-ttu-id="0c9d4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c9d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c9d4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c9d4-111">Permission type</span></span>      | <span data-ttu-id="0c9d4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c9d4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c9d4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c9d4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0c9d4-114">ChannelMessage. Send, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0c9d4-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="0c9d4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c9d4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c9d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c9d4-116">Not supported.</span></span>    |
| <span data-ttu-id="0c9d4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c9d4-117">Application</span></span>                           | <span data-ttu-id="0c9d4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c9d4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c9d4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c9d4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="0c9d4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c9d4-120">Request headers</span></span>

| <span data-ttu-id="0c9d4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0c9d4-121">Name</span></span>       | <span data-ttu-id="0c9d4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c9d4-122">Type</span></span> | <span data-ttu-id="0c9d4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c9d4-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c9d4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c9d4-124">Authorization</span></span>  | <span data-ttu-id="0c9d4-125">string</span><span class="sxs-lookup"><span data-stu-id="0c9d4-125">string</span></span>  | <span data-ttu-id="0c9d4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c9d4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c9d4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c9d4-128">Request body</span></span>

<span data-ttu-id="0c9d4-129">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="0c9d4-129">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="0c9d4-130">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="0c9d4-130">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="0c9d4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c9d4-131">Response</span></span>

<span data-ttu-id="0c9d4-132">Se bem-sucedido, este método retorna `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="0c9d4-132">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="0c9d4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c9d4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c9d4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c9d4-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0c9d4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c9d4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="0c9d4-136">C#</span><span class="sxs-lookup"><span data-stu-id="0c9d4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c9d4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c9d4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c9d4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c9d4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c9d4-139">Java</span><span class="sxs-lookup"><span data-stu-id="0c9d4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0c9d4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c9d4-140">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
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
