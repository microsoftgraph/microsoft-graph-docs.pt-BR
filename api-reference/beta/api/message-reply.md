---
title: 'message: reply'
description: Responder ao remetente de uma mensagem usando o formato JSON ou MIME.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5a9cab87389f41c795268a1d7964a7d8e987269
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870497"
---
# <a name="message-reply"></a><span data-ttu-id="f0aa3-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="f0aa3-103">message: reply</span></span>

<span data-ttu-id="f0aa3-104">Namespace: microsoft.graph.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-104">Namespace: microsoft.graph.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0aa3-105">Responder ao remetente de uma mensagem [usando](../resources/message.md) o formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-105">Reply to the sender of a [message](../resources/message.md) using either JSON or MIME format.</span></span>

<span data-ttu-id="f0aa3-106">Ao usar o formato JSON:</span><span class="sxs-lookup"><span data-stu-id="f0aa3-106">When using JSON format:</span></span>
- <span data-ttu-id="f0aa3-107">Especifique um comentário ou **a propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="f0aa3-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="f0aa3-109">Se a mensagem original especificar um destinatário na propriedade **replyTo,** por Formato de Mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), envie a resposta aos destinatários em **replyTo** e não ao destinatário na propriedade **from.**</span><span class="sxs-lookup"><span data-stu-id="f0aa3-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span>

<span data-ttu-id="f0aa3-110">Ao utilizar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="f0aa3-110">When using MIME format:</span></span>
- <span data-ttu-id="f0aa3-111">Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="f0aa3-112">Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="f0aa3-113">Este método salva a mensagem na pasta **Itens Enviados**.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-113">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="f0aa3-114">Como alternativa, [crie um rascunho para responder a uma mensagem](../api/message-createreply.md)e [envie-a](../api/message-send.md) mais tarde.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-114">Alternatively, [create a draft to reply to a message](../api/message-createreply.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0aa3-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0aa3-115">Permissions</span></span>
<span data-ttu-id="f0aa3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0aa3-p102">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0aa3-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0aa3-118">Permission type</span></span>      | <span data-ttu-id="f0aa3-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0aa3-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0aa3-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0aa3-120">Delegated (work or school account)</span></span> | <span data-ttu-id="f0aa3-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f0aa3-121">Mail.Send</span></span>    |
|<span data-ttu-id="f0aa3-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0aa3-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0aa3-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f0aa3-123">Mail.Send</span></span>    |
|<span data-ttu-id="f0aa3-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0aa3-124">Application</span></span> | <span data-ttu-id="f0aa3-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f0aa3-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0aa3-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0aa3-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```

## <a name="request-headers"></a><span data-ttu-id="f0aa3-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aa3-127">Request headers</span></span>
| <span data-ttu-id="f0aa3-128">Nome</span><span class="sxs-lookup"><span data-stu-id="f0aa3-128">Name</span></span>       | <span data-ttu-id="f0aa3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0aa3-129">Type</span></span> | <span data-ttu-id="f0aa3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0aa3-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f0aa3-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0aa3-131">Authorization</span></span>  | <span data-ttu-id="f0aa3-132">string</span><span class="sxs-lookup"><span data-stu-id="f0aa3-132">string</span></span>  | <span data-ttu-id="f0aa3-133">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-133">Bearer {token}.</span></span> <span data-ttu-id="f0aa3-134">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f0aa3-134">Required</span></span> |
| <span data-ttu-id="f0aa3-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0aa3-135">Content-Type</span></span> | <span data-ttu-id="f0aa3-136">string</span><span class="sxs-lookup"><span data-stu-id="f0aa3-136">string</span></span>  | <span data-ttu-id="f0aa3-137">Natureza dos dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-137">Nature of the data in the body of an entity.</span></span> <span data-ttu-id="f0aa3-138">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f0aa3-138">Required</span></span> <br/> <span data-ttu-id="f0aa3-139">Usar `application/json` para um objeto JSON e para conteúdo `text/plain` MIME</span><span class="sxs-lookup"><span data-stu-id="f0aa3-139">Use `application/json` for a JSON object and `text/plain` for MIME content</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0aa3-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aa3-140">Request body</span></span>
<span data-ttu-id="f0aa3-141">Ao usar o formato JSON, inclua um objeto JSON com os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-141">When using JSON format, include a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f0aa3-142">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f0aa3-142">Parameter</span></span>    | <span data-ttu-id="f0aa3-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0aa3-143">Type</span></span>   |<span data-ttu-id="f0aa3-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0aa3-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0aa3-145">comment</span><span class="sxs-lookup"><span data-stu-id="f0aa3-145">comment</span></span>|<span data-ttu-id="f0aa3-146">String</span><span class="sxs-lookup"><span data-stu-id="f0aa3-146">String</span></span>|<span data-ttu-id="f0aa3-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f0aa3-149">mensagem</span><span class="sxs-lookup"><span data-stu-id="f0aa3-149">message</span></span>|[<span data-ttu-id="f0aa3-150">message</span><span class="sxs-lookup"><span data-stu-id="f0aa3-150">message</span></span>](../resources/message.md) | <span data-ttu-id="f0aa3-151">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-151">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="f0aa3-152">Ao especificar o corpo no formato MIME, forneça o conteúdo MIME com os headers de mensagem da Internet aplicáveis, todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-152">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span> <span data-ttu-id="f0aa3-153">Este método usa o remetente da mensagem original como destinatário.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-153">This method uses the sender of the original message as recipient.</span></span>

## <a name="response"></a><span data-ttu-id="f0aa3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0aa3-154">Response</span></span>

<span data-ttu-id="f0aa3-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="f0aa3-157">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="f0aa3-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="f0aa3-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0aa3-158">Examples</span></span>
### <a name="example-1-reply-to-a-message-in-json-format"></a><span data-ttu-id="f0aa3-159">Exemplo 1: Responder a uma mensagem no formato JSON</span><span class="sxs-lookup"><span data-stu-id="f0aa3-159">Example 1: Reply to a message in JSON format</span></span>
<span data-ttu-id="f0aa3-160">O exemplo a seguir inclui um comentário e adiciona um destinatário à mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-160">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="f0aa3-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aa3-161">Request</span></span>
<span data-ttu-id="f0aa3-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0aa3-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0aa3-163">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "message_reply_beta",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}

```

# <a name="c"></a>[<span data-ttu-id="f0aa3-164">C#</span><span class="sxs-lookup"><span data-stu-id="f0aa3-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0aa3-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0aa3-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0aa3-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0aa3-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0aa3-167">Java</span><span class="sxs-lookup"><span data-stu-id="f0aa3-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f0aa3-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0aa3-168">Response</span></span>
<span data-ttu-id="f0aa3-169">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-169">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reply-to-a-message-in-mime-format"></a><span data-ttu-id="f0aa3-170">Exemplo 2: Responder a uma mensagem no formato MIME</span><span class="sxs-lookup"><span data-stu-id="f0aa3-170">Example 2: Reply to a message in MIME format</span></span>
##### <a name="request"></a><span data-ttu-id="f0aa3-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aa3-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_reply_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: text/plain

UmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSBieSAKY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoIE1pY3Jvc29mdCAKU01UUCBTZXJ2ZXIgKHZlcnNpb249VExTMV8yLCAKY2lwaGVyPVRMU19FQ0RIRV9SU0FfV0lUSF9BRVNfMjU2X0NCQ19TSEEzODRfUDI1NikgaW

```

##### <a name="response"></a><span data-ttu-id="f0aa3-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0aa3-172">Response</span></span>
<span data-ttu-id="f0aa3-173">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-173">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="f0aa3-174">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="f0aa3-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
