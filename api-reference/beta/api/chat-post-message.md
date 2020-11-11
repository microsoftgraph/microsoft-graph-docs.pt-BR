---
title: Enviar chat em um chat
description: Envie um novo chat em um chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e11602181e50c2d6a190e45622c6bc7d4cd323f
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993938"
---
# <a name="send-chatmessage-in-a-chat"></a><span data-ttu-id="1f187-103">Enviar chat em um chat</span><span class="sxs-lookup"><span data-stu-id="1f187-103">Send chatMessage in a chat</span></span>

<span data-ttu-id="1f187-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f187-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f187-105">Criar um novo [chat](../resources/chatmessage.md) no [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1f187-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="1f187-106">Esta API não pode criar um novo chat; Você deve usar o método [list chats](chat-list.md) para recuperar a ID de um chat existente antes de criar uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="1f187-106">This API cannot create a new chat; you must use the [list chats](chat-list.md) method to retrieve the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="1f187-107">**Observação** : não é recomendável usar essa API para a migração de dados.</span><span class="sxs-lookup"><span data-stu-id="1f187-107">**Note** : We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="1f187-108">Ele não tem a taxa de transferência necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="1f187-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="1f187-109">**Observação** : trata-se de uma violação dos [termos de uso](/legal/microsoft-apis/terms-of-use) para usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="1f187-109">**Note** : It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="1f187-110">Só envie mensagens que as pessoas lerám.</span><span class="sxs-lookup"><span data-stu-id="1f187-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f187-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f187-111">Permissions</span></span>

<span data-ttu-id="1f187-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f187-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f187-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f187-114">Permission type</span></span>                        | <span data-ttu-id="1f187-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f187-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f187-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f187-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f187-117">Chat. Send, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f187-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="1f187-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f187-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f187-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f187-119">Not supported.</span></span> |
| <span data-ttu-id="1f187-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f187-120">Application</span></span>                            | <span data-ttu-id="1f187-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f187-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f187-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f187-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="1f187-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f187-123">Request headers</span></span>

| <span data-ttu-id="1f187-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1f187-124">Name</span></span>          | <span data-ttu-id="1f187-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f187-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1f187-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f187-126">Authorization</span></span> | <span data-ttu-id="1f187-127">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="1f187-127">Bearer {code}.</span></span> <span data-ttu-id="1f187-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f187-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f187-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f187-129">Request body</span></span>

<span data-ttu-id="1f187-130">No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="1f187-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1f187-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f187-131">Response</span></span>

<span data-ttu-id="1f187-132">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f187-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f187-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1f187-133">Examples</span></span>

<span data-ttu-id="1f187-134">Para obter uma lista mais abrangente de exemplos, consulte [criar chat em um canal ou em um chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="1f187-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="1f187-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f187-135">Request</span></span>

<span data-ttu-id="1f187-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f187-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f187-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f187-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
     "content": "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="1f187-138">C#</span><span class="sxs-lookup"><span data-stu-id="1f187-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f187-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f187-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f187-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f187-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f187-141">Java</span><span class="sxs-lookup"><span data-stu-id="1f187-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f187-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f187-142">Response</span></span>

<span data-ttu-id="1f187-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1f187-143">The following is an example of the response.</span></span>

> <span data-ttu-id="1f187-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f187-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
