---
title: Responder a uma mensagem em um canal
description: Responder a uma mensagem existente em um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9353751562308c7c487fff8965024d90556ceb14
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635554"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="7424b-103">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="7424b-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7424b-104">Criar uma nova resposta a uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7424b-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7424b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7424b-105">Permissions</span></span>
<span data-ttu-id="7424b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7424b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7424b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7424b-108">Permission type</span></span>      | <span data-ttu-id="7424b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7424b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7424b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7424b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7424b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7424b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7424b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7424b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7424b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7424b-113">Not supported.</span></span>    |
|<span data-ttu-id="7424b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7424b-114">Application</span></span> | <span data-ttu-id="7424b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7424b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7424b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7424b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="7424b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7424b-117">Request headers</span></span>
| <span data-ttu-id="7424b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7424b-118">Name</span></span>       | <span data-ttu-id="7424b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7424b-119">Type</span></span> | <span data-ttu-id="7424b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7424b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7424b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7424b-121">Authorization</span></span>  | <span data-ttu-id="7424b-122">string</span><span class="sxs-lookup"><span data-stu-id="7424b-122">string</span></span>  | <span data-ttu-id="7424b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7424b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7424b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7424b-125">Request body</span></span>
<span data-ttu-id="7424b-126">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="7424b-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="7424b-127">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="7424b-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="7424b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7424b-128">Response</span></span>

<span data-ttu-id="7424b-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="7424b-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="7424b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7424b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7424b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7424b-131">Request</span></span>
<span data-ttu-id="7424b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7424b-132">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7424b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7424b-133">Response</span></span>

<span data-ttu-id="7424b-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7424b-134">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7424b-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7424b-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7424b-136">Basic</span><span class="sxs-lookup"><span data-stu-id="7424b-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_reply_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7424b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7424b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_reply_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/channel-post-messagereply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messagereply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
