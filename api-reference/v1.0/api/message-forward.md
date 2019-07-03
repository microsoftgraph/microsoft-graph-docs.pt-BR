---
title: 'message: forward'
description: Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 794668eb5aaddd73e33fdf31bbb36d305584839f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444145"
---
# <a name="message-forward"></a><span data-ttu-id="ce24a-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="ce24a-104">message: forward</span></span>

<span data-ttu-id="ce24a-p102">Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="ce24a-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce24a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce24a-107">Permissions</span></span>
<span data-ttu-id="ce24a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce24a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce24a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce24a-110">Permission type</span></span>      | <span data-ttu-id="ce24a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce24a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce24a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce24a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ce24a-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ce24a-113">Mail.Send</span></span>    |
|<span data-ttu-id="ce24a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce24a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce24a-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ce24a-115">Mail.Send</span></span>    |
|<span data-ttu-id="ce24a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce24a-116">Application</span></span> | <span data-ttu-id="ce24a-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ce24a-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce24a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce24a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="ce24a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce24a-119">Request headers</span></span>
| <span data-ttu-id="ce24a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ce24a-120">Name</span></span>       | <span data-ttu-id="ce24a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce24a-121">Type</span></span> | <span data-ttu-id="ce24a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce24a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ce24a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce24a-123">Authorization</span></span>  | <span data-ttu-id="ce24a-124">string</span><span class="sxs-lookup"><span data-stu-id="ce24a-124">string</span></span>  | <span data-ttu-id="ce24a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce24a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce24a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce24a-127">Content-Type</span></span> | <span data-ttu-id="ce24a-128">string</span><span class="sxs-lookup"><span data-stu-id="ce24a-128">string</span></span>  | <span data-ttu-id="ce24a-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce24a-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce24a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce24a-131">Request body</span></span>
<span data-ttu-id="ce24a-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce24a-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ce24a-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ce24a-133">Parameter</span></span>    | <span data-ttu-id="ce24a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce24a-134">Type</span></span>   |<span data-ttu-id="ce24a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce24a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce24a-136">comment</span><span class="sxs-lookup"><span data-stu-id="ce24a-136">comment</span></span>|<span data-ttu-id="ce24a-137">String</span><span class="sxs-lookup"><span data-stu-id="ce24a-137">String</span></span>|<span data-ttu-id="ce24a-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="ce24a-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ce24a-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="ce24a-140">toRecipients</span></span>|<span data-ttu-id="ce24a-141">Coleção [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="ce24a-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="ce24a-142">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="ce24a-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="ce24a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce24a-143">Response</span></span>

<span data-ttu-id="ce24a-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce24a-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce24a-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce24a-146">Example</span></span>
<span data-ttu-id="ce24a-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ce24a-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ce24a-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce24a-148">Request</span></span>
<span data-ttu-id="ce24a-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce24a-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ce24a-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce24a-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce24a-151">C#</span><span class="sxs-lookup"><span data-stu-id="ce24a-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce24a-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce24a-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce24a-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ce24a-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ce24a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce24a-154">Response</span></span>
##### <a name="response"></a><span data-ttu-id="ce24a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce24a-155">Response</span></span>
<span data-ttu-id="ce24a-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce24a-156">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
