---
title: 'message: forward'
description: Encaminhar uma mensagem usando o formato JSON ou MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3e0004bae41d7b700ae3a337bce27b214ba209cb
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870399"
---
# <a name="message-forward"></a><span data-ttu-id="63a5b-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="63a5b-103">message: forward</span></span>

<span data-ttu-id="63a5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63a5b-105">Encaminhar uma mensagem usando o formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="63a5b-105">Forward a message using either JSON or MIME format.</span></span>

<span data-ttu-id="63a5b-106">Ao usar o formato JSON, você pode:</span><span class="sxs-lookup"><span data-stu-id="63a5b-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="63a5b-107">Especifique um comentário ou **a propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="63a5b-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="63a5b-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="63a5b-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="63a5b-109">Especifique `toRecipients` o parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="63a5b-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="63a5b-110">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="63a5b-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

<span data-ttu-id="63a5b-111">Ao utilizar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="63a5b-111">When using MIME format:</span></span>
- <span data-ttu-id="63a5b-112">Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63a5b-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="63a5b-113">Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="63a5b-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="63a5b-114">Este método salva a mensagem na pasta **Itens Enviados**.</span><span class="sxs-lookup"><span data-stu-id="63a5b-114">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="63a5b-115">Como alternativa, [crie um rascunho para encaminhar uma mensagem](../api/message-createforward.md)e [enviá-la](../api/message-send.md) posteriormente.</span><span class="sxs-lookup"><span data-stu-id="63a5b-115">Alternatively, [create a draft to forward a message](../api/message-createforward.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="63a5b-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="63a5b-116">Permissions</span></span>
<span data-ttu-id="63a5b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63a5b-p103">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63a5b-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63a5b-119">Permission type</span></span>      | <span data-ttu-id="63a5b-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63a5b-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63a5b-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63a5b-121">Delegated (work or school account)</span></span> | <span data-ttu-id="63a5b-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="63a5b-122">Mail.Send</span></span>    |
|<span data-ttu-id="63a5b-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63a5b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63a5b-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="63a5b-124">Mail.Send</span></span>    |
|<span data-ttu-id="63a5b-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63a5b-125">Application</span></span> | <span data-ttu-id="63a5b-126">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="63a5b-126">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="63a5b-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63a5b-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="63a5b-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63a5b-128">Request headers</span></span>
| <span data-ttu-id="63a5b-129">Nome</span><span class="sxs-lookup"><span data-stu-id="63a5b-129">Name</span></span>       | <span data-ttu-id="63a5b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="63a5b-130">Type</span></span> | <span data-ttu-id="63a5b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="63a5b-131">Description</span></span>| 
|:---------------|:--------|:----------|
| <span data-ttu-id="63a5b-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="63a5b-132">Authorization</span></span>  | <span data-ttu-id="63a5b-133">string</span><span class="sxs-lookup"><span data-stu-id="63a5b-133">string</span></span>  | <span data-ttu-id="63a5b-134">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="63a5b-134">Bearer {token}.</span></span> <span data-ttu-id="63a5b-135">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="63a5b-135">Required</span></span> |
| <span data-ttu-id="63a5b-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63a5b-136">Content-Type</span></span> | <span data-ttu-id="63a5b-137">string</span><span class="sxs-lookup"><span data-stu-id="63a5b-137">string</span></span>  | <span data-ttu-id="63a5b-138">Natureza dos dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="63a5b-138">Nature of the data in the body of an entity.</span></span>  <span data-ttu-id="63a5b-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63a5b-139">Required.</span></span> <br/> <span data-ttu-id="63a5b-140">Use `application/json` para um objeto JSON e `text/plain` para conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="63a5b-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63a5b-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63a5b-141">Request body</span></span>
<span data-ttu-id="63a5b-142">Ao usar o formato JSON, forneça um objeto JSON no corpo da solicitação com os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="63a5b-142">When using JSON format, provide a JSON object in the request body with the following parameters.</span></span>

| <span data-ttu-id="63a5b-143">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="63a5b-143">Parameter</span></span>    | <span data-ttu-id="63a5b-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="63a5b-144">Type</span></span>   |<span data-ttu-id="63a5b-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="63a5b-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63a5b-146">comment</span><span class="sxs-lookup"><span data-stu-id="63a5b-146">comment</span></span>|<span data-ttu-id="63a5b-147">String</span><span class="sxs-lookup"><span data-stu-id="63a5b-147">String</span></span>|<span data-ttu-id="63a5b-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="63a5b-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="63a5b-150">toRecipients</span><span class="sxs-lookup"><span data-stu-id="63a5b-150">toRecipients</span></span>|<span data-ttu-id="63a5b-151">Coleção [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="63a5b-151">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="63a5b-152">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="63a5b-152">The list of recipients.</span></span>|

<span data-ttu-id="63a5b-153">Ao especificar o corpo no formato MIME, forneça ao conteúdo MIME os cabeçalhos de mensagem da Internet aplicáveis ("Para", "CC", "CCO", "Assunto"), todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63a5b-153">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="63a5b-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="63a5b-154">Response</span></span>

<span data-ttu-id="63a5b-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63a5b-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="63a5b-157">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="63a5b-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="63a5b-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="63a5b-158">Examples</span></span>
### <a name="example-1-forward-a-message-using-json-format"></a><span data-ttu-id="63a5b-159">Exemplo 1: encaminhar uma mensagem usando o formato JSON</span><span class="sxs-lookup"><span data-stu-id="63a5b-159">Example 1: Forward a message using JSON format</span></span>
<span data-ttu-id="63a5b-160">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="63a5b-160">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63a5b-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63a5b-161">Request</span></span>
<span data-ttu-id="63a5b-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63a5b-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63a5b-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="63a5b-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="63a5b-164">C#</span><span class="sxs-lookup"><span data-stu-id="63a5b-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63a5b-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63a5b-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63a5b-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63a5b-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63a5b-167">Java</span><span class="sxs-lookup"><span data-stu-id="63a5b-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="63a5b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="63a5b-168">Response</span></span>
<span data-ttu-id="63a5b-169">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63a5b-169">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

### <a name="example-2-forward-a-message-using-mime-content"></a><span data-ttu-id="63a5b-170">Exemplo 2: encaminhar uma mensagem usando conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="63a5b-170">Example 2: Forward a message using MIME content</span></span>
##### <a name="request"></a><span data-ttu-id="63a5b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63a5b-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_forward_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/forward
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np
```

##### <a name="response"></a><span data-ttu-id="63a5b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="63a5b-172">Response</span></span>
<span data-ttu-id="63a5b-173">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63a5b-173">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="63a5b-174">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="63a5b-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
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

