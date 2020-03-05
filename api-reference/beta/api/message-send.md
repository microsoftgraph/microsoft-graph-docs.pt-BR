---
title: 'message: send'
description: Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser o rascunho de uma mensagem nova, rascunho de resposta, rascunho de resposta a todos ou
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 76e58203640a8d5e392208a56e478ab8c29fa767
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456864"
---
# <a name="message-send"></a><span data-ttu-id="24543-104">message: send</span><span class="sxs-lookup"><span data-stu-id="24543-104">message: send</span></span>

<span data-ttu-id="24543-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="24543-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24543-p102">Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="24543-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="24543-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="24543-109">Permissions</span></span>

<span data-ttu-id="24543-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24543-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24543-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24543-112">Permission type</span></span>      | <span data-ttu-id="24543-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24543-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24543-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24543-114">Delegated (work or school account)</span></span> | <span data-ttu-id="24543-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24543-115">Mail.Send</span></span>    |
|<span data-ttu-id="24543-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24543-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24543-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24543-117">Mail.Send</span></span>    |
|<span data-ttu-id="24543-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24543-118">Application</span></span> | <span data-ttu-id="24543-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24543-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="24543-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24543-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="24543-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24543-121">Request headers</span></span>

| <span data-ttu-id="24543-122">Nome</span><span class="sxs-lookup"><span data-stu-id="24543-122">Name</span></span>       | <span data-ttu-id="24543-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="24543-123">Type</span></span> | <span data-ttu-id="24543-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="24543-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24543-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="24543-125">Authorization</span></span>  | <span data-ttu-id="24543-126">string</span><span class="sxs-lookup"><span data-stu-id="24543-126">string</span></span>  | <span data-ttu-id="24543-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24543-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24543-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="24543-129">Content-Length</span></span> | <span data-ttu-id="24543-130">number</span><span class="sxs-lookup"><span data-stu-id="24543-130">number</span></span> | <span data-ttu-id="24543-131">0. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24543-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24543-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24543-132">Request body</span></span>

## <a name="response"></a><span data-ttu-id="24543-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="24543-133">Response</span></span>

<span data-ttu-id="24543-p105">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24543-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24543-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24543-136">Example</span></span>

<span data-ttu-id="24543-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="24543-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24543-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24543-138">Request</span></span>

<span data-ttu-id="24543-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24543-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="24543-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="24543-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="24543-141">C#</span><span class="sxs-lookup"><span data-stu-id="24543-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24543-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24543-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24543-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24543-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="24543-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="24543-144">Response</span></span>

<span data-ttu-id="24543-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24543-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
