---
title: Criar thread
description: 'Crie um novo thread na conversa especificada. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6887b27a32f561d005b2c86eeb71eaeda9abb8a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566168"
---
# <a name="create-thread"></a><span data-ttu-id="c2690-103">Criar thread</span><span class="sxs-lookup"><span data-stu-id="c2690-103">Create thread</span></span>

<span data-ttu-id="c2690-104">Crie um novo thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="c2690-104">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="c2690-p101">Um thread e uma postagem são criados conforme especificado. Use [responder ao thread](conversationthread-reply.md) para incluir postagens adicionais no thread. Ou, se receber a ID de postagem, você também poderá [responder](post-reply.md) a essa postagem no thread.</span><span class="sxs-lookup"><span data-stu-id="c2690-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="c2690-108">Observação: Você também pode [Iniciar uma nova conversa criando primeiro um thread](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="c2690-108">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2690-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2690-109">Permissions</span></span>
<span data-ttu-id="c2690-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2690-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2690-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2690-112">Permission type</span></span>      | <span data-ttu-id="c2690-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2690-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2690-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2690-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c2690-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2690-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2690-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2690-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2690-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2690-117">Not supported.</span></span>    |
|<span data-ttu-id="c2690-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2690-118">Application</span></span> | <span data-ttu-id="c2690-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2690-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2690-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2690-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="c2690-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2690-121">Request headers</span></span>
| <span data-ttu-id="c2690-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c2690-122">Name</span></span>       | <span data-ttu-id="c2690-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2690-123">Type</span></span> | <span data-ttu-id="c2690-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2690-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2690-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2690-125">Authorization</span></span>  | <span data-ttu-id="c2690-126">string</span><span class="sxs-lookup"><span data-stu-id="c2690-126">string</span></span>  | <span data-ttu-id="c2690-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2690-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2690-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2690-129">Request body</span></span>
<span data-ttu-id="c2690-130">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="c2690-130">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c2690-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2690-131">Response</span></span>

<span data-ttu-id="c2690-132">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2690-132">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2690-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2690-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2690-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2690-134">Request</span></span>
<span data-ttu-id="c2690-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2690-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="c2690-136">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="c2690-136">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c2690-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2690-137">Response</span></span>

<span data-ttu-id="c2690-p104">Se for bem-sucedido, este método retornará um código de resposta `201 Created` e o `id` do novo thread no corpo da resposta. Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2690-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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
