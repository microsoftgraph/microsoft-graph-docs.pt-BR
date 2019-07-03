---
title: Responder a uma mensagem em um canal
description: Responder a uma mensagem existente em um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5ec85176c2a66dae9c9160447e85846585042865
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438388"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="60f6c-103">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="60f6c-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60f6c-104">Criar uma nova resposta a uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="60f6c-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="60f6c-105">**Observação**: não é recomendável usar essa API para a migração de dados.</span><span class="sxs-lookup"><span data-stu-id="60f6c-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="60f6c-106">Ele não tem a taxa de transferência necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="60f6c-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="60f6c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="60f6c-107">Permissions</span></span>
<span data-ttu-id="60f6c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60f6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60f6c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60f6c-110">Permission type</span></span>      | <span data-ttu-id="60f6c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60f6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60f6c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60f6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="60f6c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60f6c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60f6c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60f6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60f6c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60f6c-115">Not supported.</span></span>    |
|<span data-ttu-id="60f6c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60f6c-116">Application</span></span> | <span data-ttu-id="60f6c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60f6c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60f6c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60f6c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="60f6c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60f6c-119">Request headers</span></span>
| <span data-ttu-id="60f6c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="60f6c-120">Name</span></span>       | <span data-ttu-id="60f6c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="60f6c-121">Type</span></span> | <span data-ttu-id="60f6c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="60f6c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60f6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60f6c-123">Authorization</span></span>  | <span data-ttu-id="60f6c-124">string</span><span class="sxs-lookup"><span data-stu-id="60f6c-124">string</span></span>  | <span data-ttu-id="60f6c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60f6c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60f6c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60f6c-127">Request body</span></span>
<span data-ttu-id="60f6c-128">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="60f6c-128">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="60f6c-129">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="60f6c-129">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="60f6c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f6c-130">Response</span></span>

<span data-ttu-id="60f6c-131">Se bem-sucedido, este método retorna `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="60f6c-131">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="60f6c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60f6c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60f6c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60f6c-133">Request</span></span>
<span data-ttu-id="60f6c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60f6c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60f6c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="60f6c-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="60f6c-136">C#</span><span class="sxs-lookup"><span data-stu-id="60f6c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60f6c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="60f6c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60f6c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="60f6c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="60f6c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f6c-139">Response</span></span>

<span data-ttu-id="60f6c-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60f6c-140">Here is an example of the response.</span></span>
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
