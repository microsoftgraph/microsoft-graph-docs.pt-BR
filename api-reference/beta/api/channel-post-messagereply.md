---
title: Responder a uma mensagem em um canal
description: Responder a uma mensagem existente em um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 15e1bfffe7d7634092937a0605debfd5294b142b
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789673"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="21c37-103">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="21c37-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21c37-104">Criar uma nova resposta a uma [mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="21c37-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="21c37-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="21c37-105">Permissions</span></span>
<span data-ttu-id="21c37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21c37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21c37-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21c37-108">Permission type</span></span>      | <span data-ttu-id="21c37-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21c37-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21c37-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21c37-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21c37-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21c37-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="21c37-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21c37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21c37-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21c37-113">Not supported.</span></span>    |
|<span data-ttu-id="21c37-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21c37-114">Application</span></span> | <span data-ttu-id="21c37-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21c37-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21c37-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21c37-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="21c37-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21c37-117">Request headers</span></span>
| <span data-ttu-id="21c37-118">Nome</span><span class="sxs-lookup"><span data-stu-id="21c37-118">Name</span></span>       | <span data-ttu-id="21c37-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="21c37-119">Type</span></span> | <span data-ttu-id="21c37-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="21c37-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="21c37-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="21c37-121">Authorization</span></span>  | <span data-ttu-id="21c37-122">string</span><span class="sxs-lookup"><span data-stu-id="21c37-122">string</span></span>  | <span data-ttu-id="21c37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21c37-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21c37-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21c37-125">Request body</span></span>
<span data-ttu-id="21c37-126">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="21c37-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="21c37-127">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="21c37-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="21c37-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="21c37-128">Response</span></span>

<span data-ttu-id="21c37-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="21c37-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="21c37-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21c37-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21c37-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21c37-131">Request</span></span>
<span data-ttu-id="21c37-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21c37-132">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="21c37-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="21c37-133">Response</span></span>

<span data-ttu-id="21c37-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21c37-134">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/channel-post-reply_chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
