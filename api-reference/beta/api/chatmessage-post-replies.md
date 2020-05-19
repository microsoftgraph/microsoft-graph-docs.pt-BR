---
title: Criar uma resposta chatMessage em um canal
description: Cria um novo objeto chat em resposta a um objeto chat existente.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6c18d20ba85d7d25c961a517df577cd13996c607
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287056"
---
# <a name="create-chatmessage-reply-in-a-channel"></a><span data-ttu-id="66ace-103">Criar uma resposta chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="66ace-103">Create chatMessage reply in a channel</span></span>

<span data-ttu-id="66ace-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ace-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66ace-105">Cria um novo objeto [chat](../resources/chatmessage.md) em resposta a um objeto [chat](../resources/chatmessage.md) existente.</span><span class="sxs-lookup"><span data-stu-id="66ace-105">Creates a new [chatMessage](../resources/chatmessage.md) object in reply to an existing [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66ace-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66ace-106">Permissions</span></span>

<span data-ttu-id="66ace-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66ace-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66ace-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66ace-109">Permission type</span></span>                        | <span data-ttu-id="66ace-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66ace-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66ace-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66ace-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="66ace-112">Chat. Send, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66ace-112">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="66ace-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66ace-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66ace-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66ace-114">Not supported.</span></span> |
| <span data-ttu-id="66ace-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66ace-115">Application</span></span>                            | <span data-ttu-id="66ace-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66ace-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66ace-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66ace-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="66ace-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66ace-118">Request headers</span></span>

| <span data-ttu-id="66ace-119">Nome</span><span class="sxs-lookup"><span data-stu-id="66ace-119">Name</span></span>          | <span data-ttu-id="66ace-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="66ace-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="66ace-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66ace-121">Authorization</span></span> | <span data-ttu-id="66ace-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="66ace-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="66ace-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66ace-123">Request body</span></span>

<span data-ttu-id="66ace-124">No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="66ace-124">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66ace-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="66ace-125">Response</span></span>

<span data-ttu-id="66ace-126">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66ace-126">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66ace-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="66ace-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66ace-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66ace-128">Request</span></span>

<span data-ttu-id="66ace-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66ace-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66ace-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="66ace-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="66ace-131">C#</span><span class="sxs-lookup"><span data-stu-id="66ace-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chatmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66ace-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66ace-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chatmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66ace-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66ace-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chatmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="66ace-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="66ace-134">Response</span></span>

<span data-ttu-id="66ace-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66ace-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="66ace-136">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="66ace-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="66ace-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66ace-137">All the properties will be returned from an actual call.</span></span>

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
