---
title: 'message: reply'
description: Responder ao remetente de uma mensagem. A mensagem é então salva na pasta Itens Enviados.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d65dc2c3dc036322d130cdd81979fab11d3b7842
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274589"
---
# <a name="message-reply"></a><span data-ttu-id="3cf35-104">message: reply</span><span class="sxs-lookup"><span data-stu-id="3cf35-104">message: reply</span></span>

<span data-ttu-id="3cf35-p102">Responder ao remetente de uma mensagem. A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="3cf35-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cf35-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cf35-107">Permissions</span></span>
<span data-ttu-id="3cf35-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cf35-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cf35-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cf35-110">Permission type</span></span>      | <span data-ttu-id="3cf35-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cf35-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cf35-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cf35-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3cf35-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3cf35-113">Mail.Send</span></span>    |
|<span data-ttu-id="3cf35-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cf35-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf35-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3cf35-115">Mail.Send</span></span>    |
|<span data-ttu-id="3cf35-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cf35-116">Application</span></span> | <span data-ttu-id="3cf35-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3cf35-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cf35-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cf35-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="3cf35-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cf35-119">Request headers</span></span>
| <span data-ttu-id="3cf35-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3cf35-120">Name</span></span>       | <span data-ttu-id="3cf35-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cf35-121">Type</span></span> | <span data-ttu-id="3cf35-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cf35-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3cf35-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cf35-123">Authorization</span></span>  | <span data-ttu-id="3cf35-124">string</span><span class="sxs-lookup"><span data-stu-id="3cf35-124">string</span></span>  | <span data-ttu-id="3cf35-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cf35-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3cf35-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cf35-127">Content-Type</span></span> | <span data-ttu-id="3cf35-128">string</span><span class="sxs-lookup"><span data-stu-id="3cf35-128">string</span></span>  | <span data-ttu-id="3cf35-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cf35-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cf35-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cf35-131">Request body</span></span>
<span data-ttu-id="3cf35-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf35-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3cf35-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3cf35-133">Parameter</span></span>    | <span data-ttu-id="3cf35-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cf35-134">Type</span></span>   |<span data-ttu-id="3cf35-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cf35-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cf35-136">comment</span><span class="sxs-lookup"><span data-stu-id="3cf35-136">comment</span></span>|<span data-ttu-id="3cf35-137">String</span><span class="sxs-lookup"><span data-stu-id="3cf35-137">String</span></span>|<span data-ttu-id="3cf35-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="3cf35-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="3cf35-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cf35-140">Response</span></span>

<span data-ttu-id="3cf35-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cf35-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cf35-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cf35-143">Example</span></span>
<span data-ttu-id="3cf35-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3cf35-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3cf35-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cf35-145">Request</span></span>
<span data-ttu-id="3cf35-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cf35-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3cf35-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cf35-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="3cf35-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cf35-148">Response</span></span>
<span data-ttu-id="3cf35-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cf35-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3cf35-150">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3cf35-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3cf35-151">C#</span><span class="sxs-lookup"><span data-stu-id="3cf35-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cf35-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cf35-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_reply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3cf35-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3cf35-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_reply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
