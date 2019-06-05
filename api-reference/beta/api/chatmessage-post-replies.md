---
title: Criar uma resposta chat em um canal
description: Cria um novo objeto chat em resposta a um objeto chat existente.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6b09efa8b0d35b2377b9980c456b794954445a3e
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720855"
---
# <a name="create-chatmessage-reply-in-a-channel"></a><span data-ttu-id="6a336-103">Criar uma resposta chat em um canal</span><span class="sxs-lookup"><span data-stu-id="6a336-103">Create chatMessage reply in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a336-104">Cria um novo objeto [chat](../resources/chatmessage.md) em resposta a um objeto [chat](../resources/chatmessage.md) existente.</span><span class="sxs-lookup"><span data-stu-id="6a336-104">Creates a new [chatMessage](../resources/chatmessage.md) object in reply to an existing [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a336-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a336-105">Permissions</span></span>

<span data-ttu-id="6a336-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a336-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a336-108">Permission type</span></span>                        | <span data-ttu-id="6a336-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a336-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a336-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a336-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a336-111">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a336-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="6a336-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a336-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a336-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a336-113">Not supported.</span></span> |
| <span data-ttu-id="6a336-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a336-114">Application</span></span>                            | <span data-ttu-id="6a336-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a336-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a336-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a336-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages/{id}/replies
POST /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="6a336-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a336-117">Request headers</span></span>

| <span data-ttu-id="6a336-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6a336-118">Name</span></span>          | <span data-ttu-id="6a336-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a336-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6a336-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a336-120">Authorization</span></span> | <span data-ttu-id="6a336-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6a336-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a336-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a336-122">Request body</span></span>

<span data-ttu-id="6a336-123">No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="6a336-123">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6a336-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a336-124">Response</span></span>

<span data-ttu-id="6a336-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a336-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a336-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a336-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a336-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a336-127">Request</span></span>

<span data-ttu-id="6a336-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a336-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a336-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a336-129">Response</span></span>

<span data-ttu-id="6a336-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a336-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="6a336-131">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6a336-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6a336-132">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a336-132">All the properties will be returned from an actual call.</span></span>

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