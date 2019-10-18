---
title: 'message: send'
description: Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser o rascunho de uma mensagem nova, rascunho de resposta, rascunho de resposta a todos ou
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 124992e2481209debecf9edc9e10f54ebc3a8f5a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374670"
---
# <a name="message-send"></a><span data-ttu-id="a7e78-104">message: send</span><span class="sxs-lookup"><span data-stu-id="a7e78-104">message: send</span></span>

<span data-ttu-id="a7e78-p102">Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="a7e78-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7e78-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7e78-108">Permissions</span></span>

<span data-ttu-id="a7e78-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7e78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7e78-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7e78-111">Permission type</span></span>      | <span data-ttu-id="a7e78-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7e78-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7e78-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7e78-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a7e78-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a7e78-114">Mail.Send</span></span>    |
|<span data-ttu-id="a7e78-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7e78-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7e78-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a7e78-116">Mail.Send</span></span>    |
|<span data-ttu-id="a7e78-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7e78-117">Application</span></span> | <span data-ttu-id="a7e78-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a7e78-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7e78-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7e78-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="a7e78-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7e78-120">Request headers</span></span>

| <span data-ttu-id="a7e78-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a7e78-121">Name</span></span>       | <span data-ttu-id="a7e78-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7e78-122">Type</span></span> | <span data-ttu-id="a7e78-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7e78-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a7e78-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7e78-124">Authorization</span></span>  | <span data-ttu-id="a7e78-125">string</span><span class="sxs-lookup"><span data-stu-id="a7e78-125">string</span></span>  | <span data-ttu-id="a7e78-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7e78-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7e78-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="a7e78-128">Content-Length</span></span> | <span data-ttu-id="a7e78-129">number</span><span class="sxs-lookup"><span data-stu-id="a7e78-129">number</span></span> | <span data-ttu-id="a7e78-130">0. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7e78-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7e78-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7e78-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a7e78-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7e78-132">Response</span></span>

<span data-ttu-id="a7e78-p105">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7e78-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7e78-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7e78-135">Example</span></span>

<span data-ttu-id="a7e78-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a7e78-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a7e78-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7e78-137">Request</span></span>

<span data-ttu-id="a7e78-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7e78-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7e78-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7e78-139">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7e78-140">C#</span><span class="sxs-lookup"><span data-stu-id="a7e78-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7e78-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7e78-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7e78-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7e78-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a7e78-143">Java</span><span class="sxs-lookup"><span data-stu-id="a7e78-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a7e78-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7e78-144">Response</span></span>

<span data-ttu-id="a7e78-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7e78-145">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
