---
title: Criar thread de conversas
description: 'Inicie uma nova conversa em grupo criando primeiro um thread. '
author: dkershaw10
ms.openlocfilehash: f3800d95604ff6c094ade7d5e4d567d19a57600f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355619"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="e4542-103">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="e4542-103">Create conversation thread</span></span>

> <span data-ttu-id="e4542-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4542-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4542-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4542-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4542-106">Inicie uma nova conversa em grupo criando primeiro um thread.</span><span class="sxs-lookup"><span data-stu-id="e4542-106">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="e4542-p102">Uma nova conversa, thread de conversas e posts são criados no grupo. Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais naquele thread.</span><span class="sxs-lookup"><span data-stu-id="e4542-p102">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="e4542-109">Observação: também é possível [iniciar um novo thread em uma conversa existente](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="e4542-109">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e4542-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4542-110">Permissions</span></span>
<span data-ttu-id="e4542-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4542-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4542-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4542-113">Permission type</span></span>      | <span data-ttu-id="e4542-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4542-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4542-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4542-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e4542-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4542-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4542-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4542-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4542-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4542-118">Not supported.</span></span>    |
|<span data-ttu-id="e4542-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4542-119">Application</span></span> | <span data-ttu-id="e4542-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4542-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4542-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4542-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="e4542-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4542-122">Request headers</span></span>
| <span data-ttu-id="e4542-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4542-123">Header</span></span>       | <span data-ttu-id="e4542-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e4542-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4542-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4542-125">Authorization</span></span>  | <span data-ttu-id="e4542-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4542-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e4542-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4542-128">Content-Type</span></span>  | <span data-ttu-id="e4542-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e4542-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4542-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4542-130">Request body</span></span>
<span data-ttu-id="e4542-131">No corpo da solicitação, forneça uma representação JSON do objeto [conversationThread](../resources/conversationthread.md) que contém um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="e4542-131">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="e4542-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4542-132">Response</span></span>
<span data-ttu-id="e4542-133">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4542-133">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4542-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4542-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e4542-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4542-135">Request</span></span>
<span data-ttu-id="e4542-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4542-136">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="e4542-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4542-137">Response</span></span>
<span data-ttu-id="e4542-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4542-138">The following is an example of the response.</span></span>
><span data-ttu-id="e4542-139">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e4542-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e4542-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4542-140">All the properties will be returned from an actual call.</span></span>
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
