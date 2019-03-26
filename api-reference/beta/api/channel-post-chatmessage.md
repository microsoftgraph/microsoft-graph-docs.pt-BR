---
title: Enviar uma mensagem em um canal
description: Enviar uma nova mensagem no canal especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 960c5d8164f2681b71bb2c3b46383bb210240bb2
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799981"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="08b28-103">Enviar uma mensagem para um canal</span><span class="sxs-lookup"><span data-stu-id="08b28-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08b28-104">Criar uma nova [mensagem](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="08b28-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08b28-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="08b28-105">Permissions</span></span>
<span data-ttu-id="08b28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08b28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08b28-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08b28-108">Permission type</span></span>      | <span data-ttu-id="08b28-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08b28-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08b28-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08b28-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08b28-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08b28-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="08b28-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08b28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08b28-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08b28-113">Not supported.</span></span>    |
|<span data-ttu-id="08b28-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08b28-114">Application</span></span> | <span data-ttu-id="08b28-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08b28-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08b28-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08b28-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="08b28-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08b28-117">Request headers</span></span>
| <span data-ttu-id="08b28-118">Nome</span><span class="sxs-lookup"><span data-stu-id="08b28-118">Name</span></span>       | <span data-ttu-id="08b28-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="08b28-119">Type</span></span> | <span data-ttu-id="08b28-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="08b28-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08b28-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="08b28-121">Authorization</span></span>  | <span data-ttu-id="08b28-122">string</span><span class="sxs-lookup"><span data-stu-id="08b28-122">string</span></span>  | <span data-ttu-id="08b28-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08b28-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08b28-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08b28-125">Request body</span></span>
<span data-ttu-id="08b28-126">No corpo da solicitação, forneça uma representação JSON de um objeto [Message](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="08b28-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="08b28-127">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="08b28-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="08b28-128">Observação: não há suporte para o envio de mensagens com anexos e imagens.</span><span class="sxs-lookup"><span data-stu-id="08b28-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="08b28-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="08b28-129">Response</span></span>

<span data-ttu-id="08b28-130">Se bem-sucedido, este método retorna `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.</span><span class="sxs-lookup"><span data-stu-id="08b28-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="08b28-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="08b28-131">Examples</span></span> 

### <a name="example-1-hello-world"></a><span data-ttu-id="08b28-132">Exemplo 1: Olá mundo</span><span class="sxs-lookup"><span data-stu-id="08b28-132">Example 1: Hello World</span></span>

##### <a name="request"></a><span data-ttu-id="08b28-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08b28-133">Request</span></span>
<span data-ttu-id="08b28-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08b28-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="08b28-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="08b28-135">Response</span></span>

<span data-ttu-id="08b28-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08b28-136">Here is an example of the response.</span></span>
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

### <a name="example-2-mentions"></a><span data-ttu-id="08b28-137">Exemplo 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="08b28-137">Example 2: @mentions</span></span>

##### <a name="request"></a><span data-ttu-id="08b28-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08b28-138">Request</span></span>
<span data-ttu-id="08b28-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08b28-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="08b28-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="08b28-140">Response</span></span>

<span data-ttu-id="08b28-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08b28-141">Here is an example of the response.</span></span>
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
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

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
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
