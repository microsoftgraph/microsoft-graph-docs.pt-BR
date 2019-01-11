---
title: 'conversationThread: reply'
description: 'Responder a um segmento em uma conversa de grupo e adicionar uma nova postagem a ela. Você pode especificar a conversa pai '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: e9990e97b4d22e5d2374dfd007446fb114d9c6f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845651"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="d8634-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="d8634-104">conversationThread: reply</span></span>

<span data-ttu-id="d8634-p102">Responde a um thread em uma conversa de grupo e adicione uma nova postagem a ele. Você pode especificar a conversa pai na solicitação ou apenas o thread, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="d8634-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8634-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8634-107">Permissions</span></span>
<span data-ttu-id="d8634-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8634-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8634-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8634-110">Permission type</span></span>      | <span data-ttu-id="d8634-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8634-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8634-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8634-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8634-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8634-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8634-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8634-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8634-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8634-115">Not supported.</span></span>    |
|<span data-ttu-id="d8634-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8634-116">Application</span></span> | <span data-ttu-id="d8634-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8634-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8634-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8634-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="d8634-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8634-119">Request headers</span></span>
| <span data-ttu-id="d8634-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8634-120">Header</span></span>       | <span data-ttu-id="d8634-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d8634-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8634-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8634-122">Authorization</span></span>  | <span data-ttu-id="d8634-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8634-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d8634-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8634-125">Content-Type</span></span>  | <span data-ttu-id="d8634-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8634-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8634-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8634-128">Request body</span></span>
<span data-ttu-id="d8634-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8634-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d8634-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d8634-130">Parameter</span></span>    | <span data-ttu-id="d8634-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8634-131">Type</span></span>   |<span data-ttu-id="d8634-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8634-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8634-133">post</span><span class="sxs-lookup"><span data-stu-id="d8634-133">post</span></span>|[<span data-ttu-id="d8634-134">post</span><span class="sxs-lookup"><span data-stu-id="d8634-134">post</span></span>](../resources/post.md)|<span data-ttu-id="d8634-135">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="d8634-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="d8634-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8634-136">Response</span></span>

<span data-ttu-id="d8634-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8634-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8634-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8634-139">Example</span></span>
<span data-ttu-id="d8634-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d8634-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d8634-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8634-141">Request</span></span>
<span data-ttu-id="d8634-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8634-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="d8634-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8634-143">Response</span></span>
<span data-ttu-id="d8634-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8634-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
