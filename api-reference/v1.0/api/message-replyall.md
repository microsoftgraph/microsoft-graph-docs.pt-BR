---
title: 'message: replyAll'
description: Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: dffebfa65c2b8949c7ee8b132a9f1869672b51e0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455291"
---
# <a name="message-replyall"></a><span data-ttu-id="99df0-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="99df0-104">message: replyAll</span></span>

<span data-ttu-id="99df0-p102">Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="99df0-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="99df0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="99df0-107">Permissions</span></span>
<span data-ttu-id="99df0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99df0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99df0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99df0-110">Permission type</span></span>      | <span data-ttu-id="99df0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99df0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99df0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99df0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99df0-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="99df0-113">Mail.Send</span></span>    |
|<span data-ttu-id="99df0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99df0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99df0-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="99df0-115">Mail.Send</span></span>    |
|<span data-ttu-id="99df0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99df0-116">Application</span></span> | <span data-ttu-id="99df0-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="99df0-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="99df0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99df0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="99df0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99df0-119">Request headers</span></span>
| <span data-ttu-id="99df0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="99df0-120">Name</span></span>       | <span data-ttu-id="99df0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="99df0-121">Type</span></span> | <span data-ttu-id="99df0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="99df0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="99df0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="99df0-123">Authorization</span></span>  | <span data-ttu-id="99df0-124">string</span><span class="sxs-lookup"><span data-stu-id="99df0-124">string</span></span>  | <span data-ttu-id="99df0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99df0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99df0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99df0-127">Content-Type</span></span> | <span data-ttu-id="99df0-128">string</span><span class="sxs-lookup"><span data-stu-id="99df0-128">string</span></span>  | <span data-ttu-id="99df0-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99df0-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99df0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99df0-131">Request body</span></span>
<span data-ttu-id="99df0-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99df0-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99df0-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="99df0-133">Parameter</span></span>    | <span data-ttu-id="99df0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="99df0-134">Type</span></span>   |<span data-ttu-id="99df0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="99df0-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99df0-136">comment</span><span class="sxs-lookup"><span data-stu-id="99df0-136">comment</span></span>|<span data-ttu-id="99df0-137">String</span><span class="sxs-lookup"><span data-stu-id="99df0-137">String</span></span>|<span data-ttu-id="99df0-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="99df0-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="99df0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="99df0-140">Response</span></span>

<span data-ttu-id="99df0-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99df0-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99df0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99df0-143">Example</span></span>
<span data-ttu-id="99df0-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="99df0-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99df0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99df0-145">Request</span></span>
<span data-ttu-id="99df0-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99df0-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99df0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="99df0-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="99df0-148">C#</span><span class="sxs-lookup"><span data-stu-id="99df0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99df0-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="99df0-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99df0-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="99df0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="99df0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="99df0-151">Response</span></span>
<span data-ttu-id="99df0-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99df0-152">Here is an example of the response.</span></span>
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
