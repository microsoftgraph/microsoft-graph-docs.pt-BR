---
title: 'message: replyAll'
description: Responder a todos os destinatários de uma mensagem usando o formato JSON ou MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a20827d2ea6c58339f5c1563c2d61354fa6c52d1
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870490"
---
# <a name="message-replyall"></a><span data-ttu-id="72f54-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="72f54-103">message: replyAll</span></span>

<span data-ttu-id="72f54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72f54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72f54-105">Responder a todos os destinatários de uma [mensagem usando](../resources/message.md) o formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="72f54-105">Reply to all recipients of a [message](../resources/message.md) using either JSON or MIME format.</span></span>

<span data-ttu-id="72f54-106">Ao usar o formato JSON:</span><span class="sxs-lookup"><span data-stu-id="72f54-106">When using JSON format:</span></span>
- <span data-ttu-id="72f54-107">Especifique um comentário ou **a propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="72f54-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="72f54-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="72f54-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="72f54-109">Se a mensagem original especificar um destinatário na propriedade **replyTo,** por Formato de Mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), envie a resposta aos destinatários em **replyTo** e não ao destinatário na propriedade **from.**</span><span class="sxs-lookup"><span data-stu-id="72f54-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span>

<span data-ttu-id="72f54-110">Ao utilizar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="72f54-110">When using MIME format:</span></span>
- <span data-ttu-id="72f54-111">Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72f54-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="72f54-112">Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="72f54-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="72f54-113">Este método salva a mensagem na pasta **Itens Enviados**.</span><span class="sxs-lookup"><span data-stu-id="72f54-113">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="72f54-114">Como alternativa, [crie um rascunho para responder tudo a uma mensagem](../api/message-createreplyall.md)e [envie-a](../api/message-send.md) mais tarde.</span><span class="sxs-lookup"><span data-stu-id="72f54-114">Alternatively, [create a draft to reply-all to a message](../api/message-createreplyall.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="72f54-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="72f54-115">Permissions</span></span>
<span data-ttu-id="72f54-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72f54-p102">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72f54-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72f54-118">Permission type</span></span>      | <span data-ttu-id="72f54-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72f54-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72f54-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72f54-120">Delegated (work or school account)</span></span> | <span data-ttu-id="72f54-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="72f54-121">Mail.Send</span></span>    |
|<span data-ttu-id="72f54-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72f54-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72f54-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="72f54-123">Mail.Send</span></span>    |
|<span data-ttu-id="72f54-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72f54-124">Application</span></span> | <span data-ttu-id="72f54-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="72f54-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="72f54-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72f54-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="72f54-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72f54-127">Request headers</span></span>
| <span data-ttu-id="72f54-128">Nome</span><span class="sxs-lookup"><span data-stu-id="72f54-128">Name</span></span>       | <span data-ttu-id="72f54-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="72f54-129">Type</span></span> | <span data-ttu-id="72f54-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="72f54-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="72f54-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="72f54-131">Authorization</span></span>  | <span data-ttu-id="72f54-132">string</span><span class="sxs-lookup"><span data-stu-id="72f54-132">string</span></span>  | <span data-ttu-id="72f54-133">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="72f54-133">Bearer {token}.</span></span> <span data-ttu-id="72f54-134">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="72f54-134">Required</span></span>|
| <span data-ttu-id="72f54-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72f54-135">Content-Type</span></span> | <span data-ttu-id="72f54-136">string</span><span class="sxs-lookup"><span data-stu-id="72f54-136">string</span></span>  | <span data-ttu-id="72f54-137">Natureza dos dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="72f54-137">Nature of the data in the body of an entity.</span></span> <span data-ttu-id="72f54-138">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="72f54-138">Required</span></span> <br/> <span data-ttu-id="72f54-139">Usar `application/json` para um objeto JSON e para conteúdo `text/plain` MIME</span><span class="sxs-lookup"><span data-stu-id="72f54-139">Use `application/json` for a JSON object and `text/plain` for MIME content</span></span> |

## <a name="request-body"></a><span data-ttu-id="72f54-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72f54-140">Request body</span></span>
<span data-ttu-id="72f54-141">Ao usar o formato JSON, forneça um objeto JSON com os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="72f54-141">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="72f54-142">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="72f54-142">Parameter</span></span>    | <span data-ttu-id="72f54-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="72f54-143">Type</span></span>   |<span data-ttu-id="72f54-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="72f54-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72f54-145">comment</span><span class="sxs-lookup"><span data-stu-id="72f54-145">comment</span></span>|<span data-ttu-id="72f54-146">String</span><span class="sxs-lookup"><span data-stu-id="72f54-146">String</span></span>|<span data-ttu-id="72f54-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="72f54-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="72f54-149">mensagem</span><span class="sxs-lookup"><span data-stu-id="72f54-149">message</span></span>|[<span data-ttu-id="72f54-150">message</span><span class="sxs-lookup"><span data-stu-id="72f54-150">message</span></span>](../resources/message.md)|<span data-ttu-id="72f54-151">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="72f54-151">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="72f54-152">Ao especificar o corpo no formato MIME, forneça o conteúdo MIME com os headers de mensagem da Internet aplicáveis, todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72f54-152">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span> <span data-ttu-id="72f54-153">Este método carrega o remetente e todos os destinatários da mensagem original como destinatários da nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="72f54-153">This method loads the sender and all recipients of the original message as recipients of the new message.</span></span>

## <a name="response"></a><span data-ttu-id="72f54-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="72f54-154">Response</span></span>

<span data-ttu-id="72f54-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72f54-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="72f54-157">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="72f54-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="72f54-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72f54-158">Examples</span></span>
### <a name="example-1-reply-all-to-a-message-in-json-format"></a><span data-ttu-id="72f54-159">Exemplo 1: Responder tudo a uma mensagem no formato JSON</span><span class="sxs-lookup"><span data-stu-id="72f54-159">Example 1: Reply-all to a message in JSON format</span></span>
<span data-ttu-id="72f54-160">O exemplo a seguir inclui um comentário e adiciona um anexo à mensagem de resposta a todos.</span><span class="sxs-lookup"><span data-stu-id="72f54-160">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="72f54-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72f54-161">Request</span></span>
<span data-ttu-id="72f54-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72f54-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72f54-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="72f54-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="72f54-164">C#</span><span class="sxs-lookup"><span data-stu-id="72f54-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72f54-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72f54-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72f54-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72f54-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72f54-167">Java</span><span class="sxs-lookup"><span data-stu-id="72f54-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="72f54-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="72f54-168">Response</span></span>
<span data-ttu-id="72f54-169">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72f54-169">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reply-all-to-a-message-in-mime-format"></a><span data-ttu-id="72f54-170">Exemplo 2: Responder-tudo a uma mensagem no formato MIME</span><span class="sxs-lookup"><span data-stu-id="72f54-170">Example 2: Reply-all to a message in MIME format</span></span>
##### <a name="request"></a><span data-ttu-id="72f54-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72f54-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_replyAll_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/replyAll
Content-Type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM...

```

##### <a name="response"></a><span data-ttu-id="72f54-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="72f54-172">Response</span></span>
<span data-ttu-id="72f54-173">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72f54-173">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="72f54-174">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="72f54-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


