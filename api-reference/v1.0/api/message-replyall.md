---
title: 'message: replyAll'
description: Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 15a0587fc1749ecf168711f204f8a6397efe648d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612325"
---
# <a name="message-replyall"></a><span data-ttu-id="9c496-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="9c496-104">message: replyAll</span></span>

<span data-ttu-id="9c496-p102">Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="9c496-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c496-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c496-107">Permissions</span></span>
<span data-ttu-id="9c496-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c496-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c496-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c496-110">Permission type</span></span>      | <span data-ttu-id="9c496-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c496-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c496-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c496-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c496-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c496-113">Mail.Send</span></span>    |
|<span data-ttu-id="9c496-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c496-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c496-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c496-115">Mail.Send</span></span>    |
|<span data-ttu-id="9c496-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c496-116">Application</span></span> | <span data-ttu-id="9c496-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c496-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c496-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c496-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="9c496-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c496-119">Request headers</span></span>
| <span data-ttu-id="9c496-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9c496-120">Name</span></span>       | <span data-ttu-id="9c496-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c496-121">Type</span></span> | <span data-ttu-id="9c496-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c496-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c496-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c496-123">Authorization</span></span>  | <span data-ttu-id="9c496-124">string</span><span class="sxs-lookup"><span data-stu-id="9c496-124">string</span></span>  | <span data-ttu-id="9c496-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c496-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c496-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c496-127">Content-Type</span></span> | <span data-ttu-id="9c496-128">string</span><span class="sxs-lookup"><span data-stu-id="9c496-128">string</span></span>  | <span data-ttu-id="9c496-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c496-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c496-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c496-131">Request body</span></span>
<span data-ttu-id="9c496-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c496-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9c496-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9c496-133">Parameter</span></span>    | <span data-ttu-id="9c496-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c496-134">Type</span></span>   |<span data-ttu-id="9c496-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c496-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c496-136">comment</span><span class="sxs-lookup"><span data-stu-id="9c496-136">comment</span></span>|<span data-ttu-id="9c496-137">String</span><span class="sxs-lookup"><span data-stu-id="9c496-137">String</span></span>|<span data-ttu-id="9c496-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="9c496-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="9c496-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c496-140">Response</span></span>

<span data-ttu-id="9c496-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c496-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c496-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c496-143">Example</span></span>
<span data-ttu-id="9c496-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9c496-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9c496-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c496-145">Request</span></span>
<span data-ttu-id="9c496-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c496-146">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="9c496-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c496-147">Response</span></span>
<span data-ttu-id="9c496-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c496-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9c496-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9c496-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9c496-150">Basic</span><span class="sxs-lookup"><span data-stu-id="9c496-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_replyall-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c496-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c496-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_replyall-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-replyall.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
