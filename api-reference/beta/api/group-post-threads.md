---
title: Criar thread de conversas
description: 'Inicie uma nova conversa em grupo criando primeiro um thread. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b47f23d8162728089934e95d9d0c4a1babc8a2a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984567"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="a6e0c-103">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="a6e0c-103">Create conversation thread</span></span>

> <span data-ttu-id="a6e0c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6e0c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6e0c-106">Inicie uma nova conversa em grupo criando primeiro um thread.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-106">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="a6e0c-p102">Uma nova conversa, thread de conversas e posts são criados no grupo. Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais naquele thread.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-p102">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="a6e0c-109">Observação: também é possível [iniciar um novo thread em uma conversa existente](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="a6e0c-109">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a6e0c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6e0c-110">Permissions</span></span>
<span data-ttu-id="a6e0c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6e0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6e0c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6e0c-113">Permission type</span></span>      | <span data-ttu-id="a6e0c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6e0c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6e0c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6e0c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a6e0c-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e0c-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6e0c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6e0c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6e0c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-118">Not supported.</span></span>    |
|<span data-ttu-id="a6e0c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6e0c-119">Application</span></span> | <span data-ttu-id="a6e0c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6e0c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e0c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="a6e0c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e0c-122">Request headers</span></span>
| <span data-ttu-id="a6e0c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6e0c-123">Header</span></span>       | <span data-ttu-id="a6e0c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a6e0c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a6e0c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6e0c-125">Authorization</span></span>  | <span data-ttu-id="a6e0c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a6e0c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6e0c-128">Content-Type</span></span>  | <span data-ttu-id="a6e0c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a6e0c-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6e0c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e0c-130">Request body</span></span>
<span data-ttu-id="a6e0c-131">No corpo da solicitação, forneça uma representação JSON do objeto [conversationThread](../resources/conversationthread.md) que contém um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="a6e0c-131">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="a6e0c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e0c-132">Response</span></span>
<span data-ttu-id="a6e0c-133">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-133">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6e0c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6e0c-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a6e0c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6e0c-135">Request</span></span>
<span data-ttu-id="a6e0c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```

#### <a name="response"></a><span data-ttu-id="a6e0c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6e0c-137">Response</span></span>
<span data-ttu-id="a6e0c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-138">The following is an example of the response.</span></span>
><span data-ttu-id="a6e0c-139">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a6e0c-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6e0c-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
