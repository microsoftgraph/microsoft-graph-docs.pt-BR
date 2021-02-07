---
title: 'message: replyAll'
description: Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3e6509b2d580406410b4c78742b38a2019405bd2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137575"
---
# <a name="message-replyall"></a><span data-ttu-id="668cc-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="668cc-104">message: replyAll</span></span>

<span data-ttu-id="668cc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="668cc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="668cc-p102">Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="668cc-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="668cc-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="668cc-108">Permissions</span></span>
<span data-ttu-id="668cc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="668cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="668cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="668cc-111">Permission type</span></span>      | <span data-ttu-id="668cc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="668cc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="668cc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="668cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="668cc-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="668cc-114">Mail.Send</span></span>    |
|<span data-ttu-id="668cc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="668cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="668cc-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="668cc-116">Mail.Send</span></span>    |
|<span data-ttu-id="668cc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="668cc-117">Application</span></span> | <span data-ttu-id="668cc-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="668cc-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="668cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="668cc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="668cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="668cc-120">Request headers</span></span>
| <span data-ttu-id="668cc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="668cc-121">Name</span></span>       | <span data-ttu-id="668cc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="668cc-122">Type</span></span> | <span data-ttu-id="668cc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="668cc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="668cc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="668cc-124">Authorization</span></span>  | <span data-ttu-id="668cc-125">string</span><span class="sxs-lookup"><span data-stu-id="668cc-125">string</span></span>  | <span data-ttu-id="668cc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="668cc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="668cc-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="668cc-128">Content-Type</span></span> | <span data-ttu-id="668cc-129">string</span><span class="sxs-lookup"><span data-stu-id="668cc-129">string</span></span>  | <span data-ttu-id="668cc-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="668cc-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="668cc-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="668cc-132">Request body</span></span>
<span data-ttu-id="668cc-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="668cc-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="668cc-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="668cc-134">Parameter</span></span>    | <span data-ttu-id="668cc-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="668cc-135">Type</span></span>   |<span data-ttu-id="668cc-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="668cc-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="668cc-137">comment</span><span class="sxs-lookup"><span data-stu-id="668cc-137">comment</span></span>|<span data-ttu-id="668cc-138">String</span><span class="sxs-lookup"><span data-stu-id="668cc-138">String</span></span>|<span data-ttu-id="668cc-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="668cc-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="668cc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="668cc-141">Response</span></span>

<span data-ttu-id="668cc-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="668cc-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="668cc-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="668cc-144">Example</span></span>
<span data-ttu-id="668cc-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="668cc-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="668cc-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="668cc-146">Request</span></span>
<span data-ttu-id="668cc-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="668cc-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="668cc-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="668cc-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```
# <a name="c"></a>[<span data-ttu-id="668cc-149">C#</span><span class="sxs-lookup"><span data-stu-id="668cc-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="668cc-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="668cc-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="668cc-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="668cc-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="668cc-152">Java</span><span class="sxs-lookup"><span data-stu-id="668cc-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="668cc-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="668cc-153">Response</span></span>
<span data-ttu-id="668cc-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="668cc-154">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

