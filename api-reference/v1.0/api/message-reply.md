---
title: 'message: reply'
description: 'Responder ao remetente de uma mensagem usando o formato JSON ou MIME. '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b5b288f91a4f8657a17be1c26ed3d8407446c23f
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645270"
---
# <a name="message-reply"></a><span data-ttu-id="e6d87-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="e6d87-103">message: reply</span></span>

<span data-ttu-id="e6d87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6d87-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6d87-105">Responder ao remetente de uma mensagem [usando](../resources/message.md) o formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="e6d87-105">Reply to the sender of a [message](../resources/message.md) using either JSON or MIME format.</span></span>

<span data-ttu-id="e6d87-106">Ao usar o formato JSON:</span><span class="sxs-lookup"><span data-stu-id="e6d87-106">When using JSON format:</span></span>
- <span data-ttu-id="e6d87-107">Especifique um comentário ou **a propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e6d87-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="e6d87-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="e6d87-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="e6d87-109">Se a mensagem original especificar um destinatário na propriedade **replyTo,** por Formato de Mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), envie a resposta aos destinatários em **replyTo** e não ao destinatário na propriedade **from.**</span><span class="sxs-lookup"><span data-stu-id="e6d87-109">If the original message specifies a recipient in the **replyTo** property, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span>

<span data-ttu-id="e6d87-110">Ao usar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="e6d87-110">When using MIME format:</span></span>
- <span data-ttu-id="e6d87-111">Forneça os [headers](https://tools.ietf.org/html/rfc2076) de mensagens da Internet aplicáveis e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045), todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6d87-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="e6d87-112">Adicione quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="e6d87-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="e6d87-113">Este método salva a mensagem na pasta **Itens** Enviados.</span><span class="sxs-lookup"><span data-stu-id="e6d87-113">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="e6d87-114">Como alternativa, [crie um rascunho para responder a uma mensagem existente](../api/message-createreply.md) e [enviá-la](../api/message-send.md) mais tarde.</span><span class="sxs-lookup"><span data-stu-id="e6d87-114">Alternatively, [create a draft to reply to an existing message](../api/message-createreply.md) and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6d87-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6d87-115">Permissions</span></span>
<span data-ttu-id="e6d87-116">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e6d87-116">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="e6d87-117">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6d87-117">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6d87-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6d87-118">Permission type</span></span>      | <span data-ttu-id="e6d87-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6d87-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6d87-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6d87-120">Delegated (work or school account)</span></span> | <span data-ttu-id="e6d87-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e6d87-121">Mail.Send</span></span>    |
|<span data-ttu-id="e6d87-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6d87-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6d87-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e6d87-123">Mail.Send</span></span>    |
|<span data-ttu-id="e6d87-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6d87-124">Application</span></span> | <span data-ttu-id="e6d87-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e6d87-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6d87-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6d87-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="e6d87-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6d87-127">Request headers</span></span>
| <span data-ttu-id="e6d87-128">Nome</span><span class="sxs-lookup"><span data-stu-id="e6d87-128">Name</span></span>       | <span data-ttu-id="e6d87-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6d87-129">Type</span></span> | <span data-ttu-id="e6d87-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6d87-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6d87-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6d87-131">Authorization</span></span>  | <span data-ttu-id="e6d87-132">string</span><span class="sxs-lookup"><span data-stu-id="e6d87-132">string</span></span>  | <span data-ttu-id="e6d87-133">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="e6d87-133">Bearer {token}.</span></span> <span data-ttu-id="e6d87-134">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e6d87-134">Required</span></span> |
| <span data-ttu-id="e6d87-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6d87-135">Content-Type</span></span> | <span data-ttu-id="e6d87-136">string</span><span class="sxs-lookup"><span data-stu-id="e6d87-136">string</span></span>  | <span data-ttu-id="e6d87-137">Natureza dos dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="e6d87-137">Nature of the data in the body of an entity.</span></span> <span data-ttu-id="e6d87-138">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e6d87-138">Required</span></span> <br/> <span data-ttu-id="e6d87-139">Use `application/json` para um objeto JSON e para conteúdo `text/plain` MIME.</span><span class="sxs-lookup"><span data-stu-id="e6d87-139">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6d87-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6d87-140">Request body</span></span>
<span data-ttu-id="e6d87-141">Ao usar o formato JSON, forneça um objeto JSON no corpo da solicitação com os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e6d87-141">When using JSON format, provide a JSON object in the request body with the following parameters.</span></span>

| <span data-ttu-id="e6d87-142">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6d87-142">Parameter</span></span>    | <span data-ttu-id="e6d87-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6d87-143">Type</span></span>   | <span data-ttu-id="e6d87-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6d87-144">Description</span></span> |
|---------------|-------|---------|
| <span data-ttu-id="e6d87-145">comment</span><span class="sxs-lookup"><span data-stu-id="e6d87-145">comment</span></span> | <span data-ttu-id="e6d87-146">String</span><span class="sxs-lookup"><span data-stu-id="e6d87-146">String</span></span> | <span data-ttu-id="e6d87-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="e6d87-p105">A comment to include. Can be an empty string.</span></span> |
| <span data-ttu-id="e6d87-149">mensagem</span><span class="sxs-lookup"><span data-stu-id="e6d87-149">message</span></span> | [<span data-ttu-id="e6d87-150">message</span><span class="sxs-lookup"><span data-stu-id="e6d87-150">message</span></span>](../resources/message.md) | <span data-ttu-id="e6d87-151">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6d87-151">Any writeable properties to update in the reply message.</span></span> |

<span data-ttu-id="e6d87-152">Ao especificar o corpo no formato MIME, forneça o conteúdo MIME com os headers de mensagem da Internet aplicáveis, todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6d87-152">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers, all encoded in **base64** format in the request body.</span></span> <span data-ttu-id="e6d87-153">Este método usa o remetente da mensagem original como destinatário.</span><span class="sxs-lookup"><span data-stu-id="e6d87-153">This method uses the sender of the original message as recipient.</span></span>

## <a name="response"></a><span data-ttu-id="e6d87-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6d87-154">Response</span></span>

<span data-ttu-id="e6d87-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6d87-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="e6d87-157">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará e a seguinte mensagem de erro: "Cadeia de caracteres `400 Bad request` base64 inválida para conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="e6d87-157">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="e6d87-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e6d87-158">Examples</span></span>
### <a name="example-1-reply-in-json-format-to-an-existing-message"></a><span data-ttu-id="e6d87-159">Exemplo 1: Responder no formato JSON a uma mensagem existente</span><span class="sxs-lookup"><span data-stu-id="e6d87-159">Example 1: Reply in JSON format to an existing message</span></span>
<span data-ttu-id="e6d87-160">O exemplo a seguir inclui um comentário e adiciona um destinatário à mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6d87-160">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="e6d87-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6d87-161">Request</span></span>
<span data-ttu-id="e6d87-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6d87-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6d87-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6d87-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply_v1",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
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
# <a name="c"></a>[<span data-ttu-id="e6d87-164">C#</span><span class="sxs-lookup"><span data-stu-id="e6d87-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6d87-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6d87-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6d87-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6d87-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6d87-167">Java</span><span class="sxs-lookup"><span data-stu-id="e6d87-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e6d87-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6d87-168">Response</span></span>
<span data-ttu-id="e6d87-169">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6d87-169">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="exaxmple-2-reply-in-mime-format-to-an-existing-message"></a><span data-ttu-id="e6d87-170">Exaxmple 2: Responder no formato MIME para uma mensagem existente</span><span class="sxs-lookup"><span data-stu-id="e6d87-170">Exaxmple 2: Reply in MIME format to an existing message</span></span>
##### <a name="request"></a><span data-ttu-id="e6d87-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6d87-171">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np
```
##### <a name="response"></a><span data-ttu-id="e6d87-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6d87-172">Response</span></span>
<span data-ttu-id="e6d87-173">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6d87-173">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="e6d87-174">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="e6d87-174">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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

