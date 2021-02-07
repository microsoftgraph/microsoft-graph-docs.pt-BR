---
title: 'message: forward'
description: Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bf50b58b215eb4ec277c79d15c89e159882ee831
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128383"
---
# <a name="message-forward"></a><span data-ttu-id="b9315-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="b9315-104">message: forward</span></span>

<span data-ttu-id="b9315-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9315-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9315-p102">Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="b9315-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9315-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9315-108">Permissions</span></span>
<span data-ttu-id="b9315-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9315-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9315-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9315-111">Permission type</span></span>      | <span data-ttu-id="b9315-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9315-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9315-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9315-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b9315-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b9315-114">Mail.Send</span></span>    |
|<span data-ttu-id="b9315-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9315-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9315-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b9315-116">Mail.Send</span></span>    |
|<span data-ttu-id="b9315-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9315-117">Application</span></span> | <span data-ttu-id="b9315-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b9315-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9315-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9315-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="b9315-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9315-120">Request headers</span></span>
| <span data-ttu-id="b9315-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b9315-121">Name</span></span>       | <span data-ttu-id="b9315-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9315-122">Type</span></span> | <span data-ttu-id="b9315-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9315-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9315-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9315-124">Authorization</span></span>  | <span data-ttu-id="b9315-125">string</span><span class="sxs-lookup"><span data-stu-id="b9315-125">string</span></span>  | <span data-ttu-id="b9315-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9315-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9315-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9315-128">Content-Type</span></span> | <span data-ttu-id="b9315-129">string</span><span class="sxs-lookup"><span data-stu-id="b9315-129">string</span></span>  | <span data-ttu-id="b9315-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9315-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9315-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9315-132">Request body</span></span>
<span data-ttu-id="b9315-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9315-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9315-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9315-134">Parameter</span></span>    | <span data-ttu-id="b9315-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9315-135">Type</span></span>   |<span data-ttu-id="b9315-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9315-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9315-137">comment</span><span class="sxs-lookup"><span data-stu-id="b9315-137">comment</span></span>|<span data-ttu-id="b9315-138">String</span><span class="sxs-lookup"><span data-stu-id="b9315-138">String</span></span>|<span data-ttu-id="b9315-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="b9315-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="b9315-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="b9315-141">toRecipients</span></span>|<span data-ttu-id="b9315-142">Coleção [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="b9315-142">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="b9315-143">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="b9315-143">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="b9315-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9315-144">Response</span></span>

<span data-ttu-id="b9315-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9315-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9315-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9315-147">Example</span></span>
<span data-ttu-id="b9315-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b9315-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9315-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9315-149">Request</span></span>
<span data-ttu-id="b9315-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9315-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9315-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9315-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9315-152">C#</span><span class="sxs-lookup"><span data-stu-id="b9315-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9315-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9315-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9315-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9315-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9315-155">Java</span><span class="sxs-lookup"><span data-stu-id="b9315-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b9315-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9315-156">Response</span></span>
##### <a name="response"></a><span data-ttu-id="b9315-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9315-157">Response</span></span>
<span data-ttu-id="b9315-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9315-158">Here is an example of the response.</span></span>
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

