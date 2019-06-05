---
title: Criar chat
description: Use esta API para criar um novo chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 22ee0d1e4b2822f26a4892fb354bdc8c90663d21
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720859"
---
# <a name="create-chatmessage"></a><span data-ttu-id="55e77-103">Criar chat</span><span class="sxs-lookup"><span data-stu-id="55e77-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55e77-104">Criar uma nova [mensagem](../resources/chatmessage.md) no [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="55e77-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="55e77-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="55e77-105">Permissions</span></span>

<span data-ttu-id="55e77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55e77-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55e77-108">Permission type</span></span>                        | <span data-ttu-id="55e77-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55e77-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="55e77-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55e77-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="55e77-111">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55e77-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="55e77-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55e77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55e77-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55e77-113">Not supported.</span></span> |
| <span data-ttu-id="55e77-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55e77-114">Application</span></span>                            | <span data-ttu-id="55e77-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55e77-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55e77-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55e77-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="55e77-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55e77-117">Request headers</span></span>

| <span data-ttu-id="55e77-118">Nome</span><span class="sxs-lookup"><span data-stu-id="55e77-118">Name</span></span>          | <span data-ttu-id="55e77-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="55e77-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="55e77-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="55e77-120">Authorization</span></span> | <span data-ttu-id="55e77-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="55e77-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="55e77-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55e77-122">Request body</span></span>

<span data-ttu-id="55e77-123">No corpo da solicitação, forneça uma representação JSON do objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="55e77-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="55e77-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="55e77-124">Response</span></span>

<span data-ttu-id="55e77-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55e77-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55e77-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55e77-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55e77-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55e77-127">Request</span></span>

<span data-ttu-id="55e77-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55e77-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```

### <a name="response"></a><span data-ttu-id="55e77-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="55e77-129">Response</span></span>

<span data-ttu-id="55e77-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55e77-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="55e77-131">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55e77-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55e77-132">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55e77-132">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->