---
title: 'message: forward'
description: Encaminhar uma mensagem usando o formato JSON ou MIME
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 021d17d930e76a7696ab8e4484d1f43c20c84fd4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870630"
---
# <a name="message-forward"></a><span data-ttu-id="20ef5-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="20ef5-103">message: forward</span></span>

<span data-ttu-id="20ef5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20ef5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20ef5-105">Encaminhar uma mensagem usando o formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="20ef5-105">Forward a message using either JSON or MIME format.</span></span>

<span data-ttu-id="20ef5-106">Ao usar o formato JSON, você pode:</span><span class="sxs-lookup"><span data-stu-id="20ef5-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="20ef5-107">Especifique um comentário ou **a propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="20ef5-107">Specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="20ef5-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="20ef5-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="20ef5-109">Especifique `toRecipients` o parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="20ef5-109">Specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="20ef5-110">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="20ef5-110">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

<span data-ttu-id="20ef5-111">Ao utilizar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="20ef5-111">When using MIME format:</span></span>
- <span data-ttu-id="20ef5-112">Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20ef5-112">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="20ef5-113">Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="20ef5-113">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="20ef5-114">Este método salva a mensagem na pasta **Itens Enviados**.</span><span class="sxs-lookup"><span data-stu-id="20ef5-114">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="20ef5-115">Como alternativa, [crie um rascunho para encaminhar uma mensagem](../api/message-createforward.md)e [enviá-la](../api/message-send.md) posteriormente.</span><span class="sxs-lookup"><span data-stu-id="20ef5-115">Alternatively, [create a draft to forward a message](../api/message-createforward.md), and [send](../api/message-send.md) it later.</span></span>

## <a name="permissions"></a><span data-ttu-id="20ef5-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="20ef5-116">Permissions</span></span>
<span data-ttu-id="20ef5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20ef5-p103">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20ef5-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20ef5-119">Permission type</span></span>      | <span data-ttu-id="20ef5-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20ef5-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20ef5-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20ef5-121">Delegated (work or school account)</span></span> | <span data-ttu-id="20ef5-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="20ef5-122">Mail.Send</span></span>    |
|<span data-ttu-id="20ef5-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20ef5-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20ef5-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="20ef5-124">Mail.Send</span></span>    |
|<span data-ttu-id="20ef5-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20ef5-125">Application</span></span> | <span data-ttu-id="20ef5-126">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="20ef5-126">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="20ef5-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20ef5-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="20ef5-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20ef5-128">Request headers</span></span>
| <span data-ttu-id="20ef5-129">Nome</span><span class="sxs-lookup"><span data-stu-id="20ef5-129">Name</span></span>       | <span data-ttu-id="20ef5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="20ef5-130">Type</span></span> | <span data-ttu-id="20ef5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="20ef5-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="20ef5-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="20ef5-132">Authorization</span></span>  | <span data-ttu-id="20ef5-133">string</span><span class="sxs-lookup"><span data-stu-id="20ef5-133">string</span></span>  | <span data-ttu-id="20ef5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20ef5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20ef5-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20ef5-136">Content-Type</span></span> | <span data-ttu-id="20ef5-137">string</span><span class="sxs-lookup"><span data-stu-id="20ef5-137">string</span></span>  | <span data-ttu-id="20ef5-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20ef5-p105">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="20ef5-140">Use `application/json` para um objeto JSON e `text/plain` para conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="20ef5-140">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20ef5-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20ef5-141">Request body</span></span>
<span data-ttu-id="20ef5-142">Ao usar o formato JSON, forneça um objeto JSON com os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="20ef5-142">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20ef5-143">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20ef5-143">Parameter</span></span>    | <span data-ttu-id="20ef5-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="20ef5-144">Type</span></span>   |<span data-ttu-id="20ef5-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="20ef5-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20ef5-146">comment</span><span class="sxs-lookup"><span data-stu-id="20ef5-146">comment</span></span>|<span data-ttu-id="20ef5-147">String</span><span class="sxs-lookup"><span data-stu-id="20ef5-147">String</span></span>|<span data-ttu-id="20ef5-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="20ef5-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="20ef5-150">toRecipients</span><span class="sxs-lookup"><span data-stu-id="20ef5-150">toRecipients</span></span>|<span data-ttu-id="20ef5-151">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="20ef5-151">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="20ef5-152">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="20ef5-152">The list of recipients.</span></span>|
|<span data-ttu-id="20ef5-153">mensagem</span><span class="sxs-lookup"><span data-stu-id="20ef5-153">message</span></span>|[<span data-ttu-id="20ef5-154">message</span><span class="sxs-lookup"><span data-stu-id="20ef5-154">message</span></span>](../resources/message.md)|<span data-ttu-id="20ef5-155">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="20ef5-155">Any writeable properties to update in the reply message.</span></span>|

<span data-ttu-id="20ef5-156">Ao especificar o corpo no formato MIME, forneça ao conteúdo MIME os cabeçalhos de mensagem da Internet aplicáveis ("Para", "CC", "CCO", "Assunto"), todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20ef5-156">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="20ef5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ef5-157">Response</span></span>

<span data-ttu-id="20ef5-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20ef5-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="20ef5-160">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="20ef5-160">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="20ef5-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20ef5-161">Examples</span></span>
### <a name="example-1-forward-a-message-using-json-format"></a><span data-ttu-id="20ef5-162">Exemplo 1: encaminhar uma mensagem usando o formato JSON</span><span class="sxs-lookup"><span data-stu-id="20ef5-162">Example 1: Forward a message using JSON format</span></span>
<span data-ttu-id="20ef5-163">O exemplo a seguir define a **propriedade isDeliveryReceiptRequested** como true, adiciona um comentário e encaminha a mensagem.</span><span class="sxs-lookup"><span data-stu-id="20ef5-163">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="20ef5-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20ef5-164">Request</span></span>
<span data-ttu-id="20ef5-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20ef5-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20ef5-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="20ef5-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this." 
}
```
# <a name="c"></a>[<span data-ttu-id="20ef5-167">C#</span><span class="sxs-lookup"><span data-stu-id="20ef5-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20ef5-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20ef5-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20ef5-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20ef5-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20ef5-170">Java</span><span class="sxs-lookup"><span data-stu-id="20ef5-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="20ef5-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ef5-171">Response</span></span>
<span data-ttu-id="20ef5-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20ef5-172">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-forward-a-message-using-mime-format"></a><span data-ttu-id="20ef5-173">Exemplo 2: encaminhar uma mensagem usando o formato MIME</span><span class="sxs-lookup"><span data-stu-id="20ef5-173">Example 2: Forward a message using MIME format</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_forward_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np...

```


##### <a name="response"></a><span data-ttu-id="20ef5-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ef5-174">Response</span></span>
<span data-ttu-id="20ef5-175">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20ef5-175">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted

```

<span data-ttu-id="20ef5-176">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="20ef5-176">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
