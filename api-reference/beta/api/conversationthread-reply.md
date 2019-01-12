---
title: 'conversationThread: reply'
description: 'Responder a um segmento em uma conversa de grupo e adicionar uma nova postagem a ela. Você pode especificar a conversa pai '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7662a8bcc2ba61d37b279b4ae1cc04cf14171f6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956491"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="4ccc5-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="4ccc5-104">conversationThread: reply</span></span>

> <span data-ttu-id="4ccc5-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ccc5-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ccc5-p103">Responde a um thread em uma conversa de grupo e adicione uma nova postagem a ele. Você pode especificar a conversa pai na solicitação ou apenas o thread, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-p103">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ccc5-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ccc5-109">Permissions</span></span>
<span data-ttu-id="4ccc5-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ccc5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ccc5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ccc5-112">Permission type</span></span>      | <span data-ttu-id="4ccc5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ccc5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ccc5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ccc5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4ccc5-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ccc5-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ccc5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ccc5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ccc5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-117">Not supported.</span></span>    |
|<span data-ttu-id="4ccc5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ccc5-118">Application</span></span> | <span data-ttu-id="4ccc5-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-119">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="4ccc5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ccc5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="4ccc5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ccc5-121">Request headers</span></span>
| <span data-ttu-id="4ccc5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ccc5-122">Header</span></span>       | <span data-ttu-id="4ccc5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4ccc5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ccc5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ccc5-124">Authorization</span></span>  | <span data-ttu-id="4ccc5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4ccc5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ccc5-127">Content-Type</span></span>  | <span data-ttu-id="4ccc5-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ccc5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ccc5-130">Request body</span></span>
<span data-ttu-id="4ccc5-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4ccc5-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4ccc5-132">Parameter</span></span>    | <span data-ttu-id="4ccc5-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ccc5-133">Type</span></span>   |<span data-ttu-id="4ccc5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ccc5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ccc5-135">post</span><span class="sxs-lookup"><span data-stu-id="4ccc5-135">post</span></span>|[<span data-ttu-id="4ccc5-136">post</span><span class="sxs-lookup"><span data-stu-id="4ccc5-136">post</span></span>](../resources/post.md)|<span data-ttu-id="4ccc5-137">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-137">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="4ccc5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ccc5-138">Response</span></span>

<span data-ttu-id="4ccc5-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ccc5-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ccc5-141">Example</span></span>
<span data-ttu-id="4ccc5-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ccc5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ccc5-143">Request</span></span>
<span data-ttu-id="4ccc5-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/reply
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

##### <a name="response"></a><span data-ttu-id="4ccc5-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ccc5-145">Response</span></span>
<span data-ttu-id="4ccc5-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ccc5-146">Here is an example of the response.</span></span>
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
