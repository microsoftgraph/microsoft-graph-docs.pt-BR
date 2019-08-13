---
title: 'message: replyAll'
description: Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2596dfcf93895dc152673bc2e7e89a3f7380b322
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374684"
---
# <a name="message-replyall"></a><span data-ttu-id="59679-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="59679-104">message: replyAll</span></span>

<span data-ttu-id="59679-p102">Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="59679-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="59679-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="59679-107">Permissions</span></span>
<span data-ttu-id="59679-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59679-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59679-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59679-110">Permission type</span></span>      | <span data-ttu-id="59679-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59679-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59679-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59679-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59679-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="59679-113">Mail.Send</span></span>    |
|<span data-ttu-id="59679-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59679-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59679-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="59679-115">Mail.Send</span></span>    |
|<span data-ttu-id="59679-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59679-116">Application</span></span> | <span data-ttu-id="59679-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="59679-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="59679-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59679-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="59679-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59679-119">Request headers</span></span>
| <span data-ttu-id="59679-120">Nome</span><span class="sxs-lookup"><span data-stu-id="59679-120">Name</span></span>       | <span data-ttu-id="59679-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="59679-121">Type</span></span> | <span data-ttu-id="59679-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="59679-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="59679-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59679-123">Authorization</span></span>  | <span data-ttu-id="59679-124">string</span><span class="sxs-lookup"><span data-stu-id="59679-124">string</span></span>  | <span data-ttu-id="59679-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59679-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59679-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59679-127">Content-Type</span></span> | <span data-ttu-id="59679-128">string</span><span class="sxs-lookup"><span data-stu-id="59679-128">string</span></span>  | <span data-ttu-id="59679-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59679-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59679-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59679-131">Request body</span></span>
<span data-ttu-id="59679-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59679-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59679-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59679-133">Parameter</span></span>    | <span data-ttu-id="59679-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="59679-134">Type</span></span>   |<span data-ttu-id="59679-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="59679-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59679-136">comment</span><span class="sxs-lookup"><span data-stu-id="59679-136">comment</span></span>|<span data-ttu-id="59679-137">String</span><span class="sxs-lookup"><span data-stu-id="59679-137">String</span></span>|<span data-ttu-id="59679-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="59679-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="59679-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="59679-140">Response</span></span>

<span data-ttu-id="59679-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59679-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59679-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59679-143">Example</span></span>
<span data-ttu-id="59679-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="59679-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="59679-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59679-145">Request</span></span>
<span data-ttu-id="59679-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59679-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59679-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="59679-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="59679-148">C#</span><span class="sxs-lookup"><span data-stu-id="59679-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59679-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59679-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59679-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="59679-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="59679-151">Java</span><span class="sxs-lookup"><span data-stu-id="59679-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="59679-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="59679-152">Response</span></span>
<span data-ttu-id="59679-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59679-153">Here is an example of the response.</span></span>
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
