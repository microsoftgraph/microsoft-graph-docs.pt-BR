---
title: 'message: reply'
description: Responder ao remetente de uma mensagem. A mensagem é então salva na pasta Itens Enviados.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 825c7bec04254c2b1efc950c44fc0b3cf78ddeb3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374712"
---
# <a name="message-reply"></a><span data-ttu-id="9baa5-104">message: reply</span><span class="sxs-lookup"><span data-stu-id="9baa5-104">message: reply</span></span>

<span data-ttu-id="9baa5-p102">Responder ao remetente de uma mensagem. A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="9baa5-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9baa5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9baa5-107">Permissions</span></span>
<span data-ttu-id="9baa5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9baa5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9baa5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9baa5-110">Permission type</span></span>      | <span data-ttu-id="9baa5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9baa5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9baa5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9baa5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9baa5-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9baa5-113">Mail.Send</span></span>    |
|<span data-ttu-id="9baa5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9baa5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9baa5-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9baa5-115">Mail.Send</span></span>    |
|<span data-ttu-id="9baa5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9baa5-116">Application</span></span> | <span data-ttu-id="9baa5-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9baa5-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9baa5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9baa5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="9baa5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9baa5-119">Request headers</span></span>
| <span data-ttu-id="9baa5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9baa5-120">Name</span></span>       | <span data-ttu-id="9baa5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9baa5-121">Type</span></span> | <span data-ttu-id="9baa5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9baa5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9baa5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9baa5-123">Authorization</span></span>  | <span data-ttu-id="9baa5-124">string</span><span class="sxs-lookup"><span data-stu-id="9baa5-124">string</span></span>  | <span data-ttu-id="9baa5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9baa5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9baa5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9baa5-127">Content-Type</span></span> | <span data-ttu-id="9baa5-128">string</span><span class="sxs-lookup"><span data-stu-id="9baa5-128">string</span></span>  | <span data-ttu-id="9baa5-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9baa5-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9baa5-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9baa5-131">Request body</span></span>
<span data-ttu-id="9baa5-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9baa5-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9baa5-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9baa5-133">Parameter</span></span>    | <span data-ttu-id="9baa5-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9baa5-134">Type</span></span>   |<span data-ttu-id="9baa5-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9baa5-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9baa5-136">comment</span><span class="sxs-lookup"><span data-stu-id="9baa5-136">comment</span></span>|<span data-ttu-id="9baa5-137">String</span><span class="sxs-lookup"><span data-stu-id="9baa5-137">String</span></span>|<span data-ttu-id="9baa5-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="9baa5-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="9baa5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9baa5-140">Response</span></span>

<span data-ttu-id="9baa5-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9baa5-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9baa5-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9baa5-143">Example</span></span>
<span data-ttu-id="9baa5-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9baa5-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9baa5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9baa5-145">Request</span></span>
<span data-ttu-id="9baa5-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9baa5-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9baa5-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="9baa5-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9baa5-148">C#</span><span class="sxs-lookup"><span data-stu-id="9baa5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9baa5-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9baa5-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9baa5-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9baa5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9baa5-151">Java</span><span class="sxs-lookup"><span data-stu-id="9baa5-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9baa5-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9baa5-152">Response</span></span>
##### <a name="response"></a><span data-ttu-id="9baa5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9baa5-153">Response</span></span>
<span data-ttu-id="9baa5-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9baa5-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
