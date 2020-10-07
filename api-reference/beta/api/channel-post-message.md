---
title: Criar chatMessage em um canal
description: Criar novo chat no canal especificado.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 91f200cbd1f2aace02ecb932f54359f3639f67e7
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372030"
---
# <a name="create-chatmessage-in-channel"></a><span data-ttu-id="82cf1-103">Criar chat no canal</span><span class="sxs-lookup"><span data-stu-id="82cf1-103">Create chatMessage in channel</span></span>

<span data-ttu-id="82cf1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82cf1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82cf1-105">Criar um novo [chat](../resources/chatmessage.md) no [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="82cf1-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="82cf1-106">**Observação**: não é recomendável usar essa API para a migração de dados.</span><span class="sxs-lookup"><span data-stu-id="82cf1-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="82cf1-107">Ele não tem a taxa de transferência necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="82cf1-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="82cf1-108">**Observação**: trata-se de uma violação dos [termos de uso](/legal/microsoft-apis/terms-of-use) para usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="82cf1-108">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="82cf1-109">Só envie mensagens que as pessoas lerám.</span><span class="sxs-lookup"><span data-stu-id="82cf1-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="82cf1-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="82cf1-110">Permissions</span></span>

<span data-ttu-id="82cf1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82cf1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82cf1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82cf1-113">Permission type</span></span>                        | <span data-ttu-id="82cf1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82cf1-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82cf1-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82cf1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="82cf1-116">ChannelMessage. Send, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="82cf1-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="82cf1-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82cf1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82cf1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82cf1-118">Not supported.</span></span> |
| <span data-ttu-id="82cf1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82cf1-119">Application</span></span>                            | <span data-ttu-id="82cf1-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82cf1-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82cf1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82cf1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="82cf1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82cf1-122">Request headers</span></span>

| <span data-ttu-id="82cf1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="82cf1-123">Name</span></span>          | <span data-ttu-id="82cf1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="82cf1-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="82cf1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="82cf1-125">Authorization</span></span> | <span data-ttu-id="82cf1-126">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="82cf1-126">Bearer {code}.</span></span> <span data-ttu-id="82cf1-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82cf1-127">Required.</span></span> |
| <span data-ttu-id="82cf1-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="82cf1-128">Content-type</span></span> | <span data-ttu-id="82cf1-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82cf1-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82cf1-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82cf1-131">Request body</span></span>

<span data-ttu-id="82cf1-132">No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="82cf1-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="82cf1-133">Somente a Propriedade Body é obrigatória, outras propriedades são opcionais.</span><span class="sxs-lookup"><span data-stu-id="82cf1-133">Only the body property is mandatory, other properties are optional.</span></span>


## <a name="response"></a><span data-ttu-id="82cf1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="82cf1-134">Response</span></span>

<span data-ttu-id="82cf1-135">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82cf1-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82cf1-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="82cf1-136">Examples</span></span>

<span data-ttu-id="82cf1-137">Para obter uma lista mais abrangente de exemplos, consulte [criar chat em um canal ou em um chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="82cf1-137">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="82cf1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82cf1-138">Request</span></span>
<span data-ttu-id="82cf1-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="82cf1-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82cf1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="82cf1-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="82cf1-141">C#</span><span class="sxs-lookup"><span data-stu-id="82cf1-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82cf1-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82cf1-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82cf1-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82cf1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82cf1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="82cf1-144">Response</span></span>

<span data-ttu-id="82cf1-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="82cf1-145">The following is an example of the response.</span></span>

> <span data-ttu-id="82cf1-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82cf1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
