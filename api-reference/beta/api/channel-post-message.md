---
title: Criar chatMessage em um canal
description: Criar um novo chat no canal especificado.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ade0014f24abd169d71ca2d0b0ea6b9fffc2517
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630377"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="7c858-103">Criar chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="7c858-103">Create chatMessage in a channel</span></span>

<span data-ttu-id="7c858-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c858-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c858-105">Criar um novo [chat](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7c858-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

<span data-ttu-id="7c858-106">*Não é recomendável usar essa API para a migração de dados. Ele não tem a taxa de transferência necessária para uma migração típica.*</span><span class="sxs-lookup"><span data-stu-id="7c858-106">*We don't recommend that you use this API for data migration. It does not have the throughput necessary for a typical migration.*</span></span>

> <span data-ttu-id="7c858-107">**Observação**: trata-se de uma violação dos [termos de uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) para usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="7c858-107">**Note**: It is a violation of the [terms of use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="7c858-108">Só envie mensagens que as pessoas lerám.</span><span class="sxs-lookup"><span data-stu-id="7c858-108">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c858-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c858-109">Permissions</span></span>

<span data-ttu-id="7c858-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c858-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c858-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c858-112">Permission type</span></span>                        | <span data-ttu-id="7c858-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c858-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7c858-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c858-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c858-115">ChannelMessage. Send, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7c858-115">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7c858-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c858-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c858-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c858-117">Not supported.</span></span> |
| <span data-ttu-id="7c858-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c858-118">Application</span></span>                            | <span data-ttu-id="7c858-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c858-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c858-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c858-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="7c858-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c858-121">Request headers</span></span>

| <span data-ttu-id="7c858-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7c858-122">Name</span></span>          | <span data-ttu-id="7c858-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c858-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7c858-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c858-124">Authorization</span></span> | <span data-ttu-id="7c858-125">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="7c858-125">Bearer {code}.</span></span> <span data-ttu-id="7c858-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c858-126">Required.</span></span> |
| <span data-ttu-id="7c858-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="7c858-127">Content-type</span></span> | <span data-ttu-id="7c858-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c858-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c858-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c858-130">Request body</span></span>

<span data-ttu-id="7c858-131">No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="7c858-131">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="7c858-132">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="7c858-132">Only the body property is mandatory, other properties are optional.</span></span>


## <a name="response"></a><span data-ttu-id="7c858-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c858-133">Response</span></span>

<span data-ttu-id="7c858-134">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c858-134">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c858-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7c858-135">Examples</span></span>

<span data-ttu-id="7c858-136">Para obter uma lista mais abrangente de exemplos, consulte [criar chat em um canal ou em um chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="7c858-136">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="7c858-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c858-137">Request</span></span>
<span data-ttu-id="7c858-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c858-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c858-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c858-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7c858-140">C#</span><span class="sxs-lookup"><span data-stu-id="7c858-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c858-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c858-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c858-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c858-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7c858-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c858-143">Response</span></span>

<span data-ttu-id="7c858-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c858-144">The following is an example of the response.</span></span>

> <span data-ttu-id="7c858-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c858-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
