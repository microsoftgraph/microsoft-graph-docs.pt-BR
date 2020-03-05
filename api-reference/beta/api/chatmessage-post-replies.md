---
title: Criar uma resposta chatMessage em um canal
description: Cria um novo objeto chat em resposta a um objeto chat existente.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 00d1f9d6d2197f1e265c59a795ef66941c0a5c60
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438299"
---
# <a name="create-chatmessage-reply-in-a-channel"></a><span data-ttu-id="4d500-103">Criar uma resposta chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="4d500-103">Create chatMessage reply in a channel</span></span>

<span data-ttu-id="4d500-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4d500-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d500-105">Cria um novo objeto [chat](../resources/chatmessage.md) em resposta a um objeto [chat](../resources/chatmessage.md) existente.</span><span class="sxs-lookup"><span data-stu-id="4d500-105">Creates a new [chatMessage](../resources/chatmessage.md) object in reply to an existing [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d500-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d500-106">Permissions</span></span>

<span data-ttu-id="4d500-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d500-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d500-109">Permission type</span></span>                        | <span data-ttu-id="4d500-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d500-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4d500-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d500-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d500-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d500-112">Chat.ReadWrite</span></span> |
| <span data-ttu-id="4d500-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d500-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d500-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d500-114">Not supported.</span></span> |
| <span data-ttu-id="4d500-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d500-115">Application</span></span>                            | <span data-ttu-id="4d500-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d500-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d500-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d500-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="4d500-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d500-118">Request headers</span></span>

| <span data-ttu-id="4d500-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4d500-119">Name</span></span>          | <span data-ttu-id="4d500-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d500-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d500-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d500-121">Authorization</span></span> | <span data-ttu-id="4d500-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4d500-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d500-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d500-123">Request body</span></span>

<span data-ttu-id="4d500-124">No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="4d500-124">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d500-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d500-125">Response</span></span>

<span data-ttu-id="4d500-126">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d500-126">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d500-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4d500-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d500-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d500-128">Request</span></span>

<span data-ttu-id="4d500-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d500-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d500-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d500-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chatmessage"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4d500-131">C#</span><span class="sxs-lookup"><span data-stu-id="4d500-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chatmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d500-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d500-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chatmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d500-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d500-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chatmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d500-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d500-134">Response</span></span>

<span data-ttu-id="4d500-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d500-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4d500-136">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4d500-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4d500-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d500-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "87ea812c-8816-40e9-b770-5c165fa31397",
      "displayName": "Test User"
    }
  },
  "messageType": "message",
  "body": {
     "content": "Hello world",
     "contentType": "text"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
