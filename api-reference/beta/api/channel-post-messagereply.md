---
title: Responder a uma mensagem em um canal
description: Responder a uma mensagem existente em um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd656b24e107a8884acb96c5fe2d09861fa54ed2
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192333"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="e43e9-103">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="e43e9-103">Reply to a message in a channel</span></span>

<span data-ttu-id="e43e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e43e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e43e9-105">Criar uma nova resposta para um [chat](../resources/chatmessage.md) em um [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="e43e9-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="e43e9-106">**Observação**: não é recomendável usar essa API para a migração de dados.</span><span class="sxs-lookup"><span data-stu-id="e43e9-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="e43e9-107">Ele não tem a taxa de transferência necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="e43e9-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="e43e9-108">**Observação**: trata-se de uma violação dos [termos de uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) para usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="e43e9-108">**Note**: It is a violation of the [terms of use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="e43e9-109">Só envie mensagens que as pessoas lerám.</span><span class="sxs-lookup"><span data-stu-id="e43e9-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="e43e9-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e43e9-110">Permissions</span></span>
<span data-ttu-id="e43e9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e43e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e43e9-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e43e9-113">Permission type</span></span>      | <span data-ttu-id="e43e9-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e43e9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e43e9-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e43e9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e43e9-116">ChannelMessage. Send, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e43e9-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="e43e9-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e43e9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e43e9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e43e9-118">Not supported.</span></span>    |
|<span data-ttu-id="e43e9-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e43e9-119">Application</span></span> | <span data-ttu-id="e43e9-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e43e9-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e43e9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e43e9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="e43e9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e43e9-122">Request headers</span></span>
| <span data-ttu-id="e43e9-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e43e9-123">Name</span></span>       | <span data-ttu-id="e43e9-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e43e9-124">Type</span></span> | <span data-ttu-id="e43e9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e43e9-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e43e9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e43e9-126">Authorization</span></span>  | <span data-ttu-id="e43e9-127">string</span><span class="sxs-lookup"><span data-stu-id="e43e9-127">string</span></span>  | <span data-ttu-id="e43e9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e43e9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e43e9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e43e9-130">Request body</span></span>
<span data-ttu-id="e43e9-131">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="e43e9-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="e43e9-132">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="e43e9-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="e43e9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e43e9-133">Response</span></span>

<span data-ttu-id="e43e9-134">Se bem-sucedido, este método retorna `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="e43e9-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="e43e9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e43e9-135">Example</span></span>

<span data-ttu-id="e43e9-136">Para obter uma lista mais abrangente de exemplos, consulte [criar chat em um canal ou em um chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="e43e9-136">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="e43e9-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e43e9-137">Request</span></span>
<span data-ttu-id="e43e9-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e43e9-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e43e9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e43e9-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e43e9-140">C#</span><span class="sxs-lookup"><span data-stu-id="e43e9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e43e9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e43e9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e43e9-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e43e9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e43e9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e43e9-143">Response</span></span>

<span data-ttu-id="e43e9-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e43e9-144">The following is an example of the response.</span></span>
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


