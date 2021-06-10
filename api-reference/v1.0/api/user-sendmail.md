---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação usando o formato JSON ou MIME.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 460e09371869fec98b24bd81dc5ab44cc8b199b8
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870385"
---
# <a name="send-mail"></a><span data-ttu-id="586d1-103">Enviar email</span><span class="sxs-lookup"><span data-stu-id="586d1-103">Send mail</span></span>

<span data-ttu-id="586d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="586d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="586d1-105">Enviar a mensagem especificada no corpo da solicitação usando o formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="586d1-105">Send the message specified in the request body using either JSON or MIME format.</span></span>

<span data-ttu-id="586d1-106">Ao usar o formato JSON, você pode incluir um [anexo de arquivo](../resources/fileattachment.md) na mesma chamada de ação **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="586d1-106">When using JSON format you can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

<span data-ttu-id="586d1-107">Ao utilizar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="586d1-107">When using MIME format:</span></span>
- <span data-ttu-id="586d1-108">Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="586d1-108">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="586d1-109">Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="586d1-109">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="586d1-110">Este método salva a mensagem na pasta **Itens Enviados**.</span><span class="sxs-lookup"><span data-stu-id="586d1-110">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="586d1-111">Alternativamente, [criar um rascunho da mensagem](../api/user-post-messages.md) para enviar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="586d1-111">Alternatively, [create a draft message](../api/user-post-messages.md) to send later.</span></span>

## <a name="permissions"></a><span data-ttu-id="586d1-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="586d1-112">Permissions</span></span>
<span data-ttu-id="586d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="586d1-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="586d1-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="586d1-115">Permission type</span></span>      | <span data-ttu-id="586d1-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="586d1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="586d1-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="586d1-117">Delegated (work or school account)</span></span> | <span data-ttu-id="586d1-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="586d1-118">Mail.Send</span></span>    |
|<span data-ttu-id="586d1-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="586d1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="586d1-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="586d1-120">Mail.Send</span></span>    |
|<span data-ttu-id="586d1-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="586d1-121">Application</span></span> | <span data-ttu-id="586d1-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="586d1-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="586d1-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="586d1-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```

## <a name="request-headers"></a><span data-ttu-id="586d1-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="586d1-124">Request headers</span></span>
| <span data-ttu-id="586d1-125">Nome</span><span class="sxs-lookup"><span data-stu-id="586d1-125">Name</span></span>       | <span data-ttu-id="586d1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="586d1-126">Type</span></span> | <span data-ttu-id="586d1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="586d1-127">Description</span></span>| 
|:---------------|:--------|:----------
| <span data-ttu-id="586d1-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="586d1-128">Authorization</span></span>  | <span data-ttu-id="586d1-129">string</span><span class="sxs-lookup"><span data-stu-id="586d1-129">string</span></span>  | <span data-ttu-id="586d1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="586d1-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="586d1-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="586d1-132">Content-Type</span></span> | <span data-ttu-id="586d1-133">string</span><span class="sxs-lookup"><span data-stu-id="586d1-133">string</span></span>  | <span data-ttu-id="586d1-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="586d1-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="586d1-136">Use `application/json` para um objeto JSON e `text/plain` para conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="586d1-136">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="586d1-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="586d1-137">Request body</span></span>
<span data-ttu-id="586d1-138">Ao usar o formato JSON, forneça um objeto JSON com os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="586d1-138">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="586d1-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="586d1-139">Parameter</span></span>    | <span data-ttu-id="586d1-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="586d1-140">Type</span></span>   |<span data-ttu-id="586d1-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="586d1-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="586d1-142">mensagem</span><span class="sxs-lookup"><span data-stu-id="586d1-142">message</span></span>|[<span data-ttu-id="586d1-143">Message</span><span class="sxs-lookup"><span data-stu-id="586d1-143">Message</span></span>](../resources/message.md)|<span data-ttu-id="586d1-p104">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="586d1-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="586d1-146">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="586d1-146">saveToSentItems</span></span>|<span data-ttu-id="586d1-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="586d1-147">Boolean</span></span>|<span data-ttu-id="586d1-p105">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="586d1-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

<span data-ttu-id="586d1-151">Ao especificar o corpo no formato MIME, forneça o conteúdo MIME como **uma cadeia de caracteres codificada em base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="586d1-151">When specifying the body in MIME format, provide the MIME content as **a base64-encoded string** in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="586d1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="586d1-152">Response</span></span>

<span data-ttu-id="586d1-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="586d1-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="586d1-155">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="586d1-155">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="586d1-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="586d1-156">Examples</span></span>
### <a name="example-1-send-a-new-email-using-json-format"></a><span data-ttu-id="586d1-157">Exemplo 1: Enviar um novo email utilizando o formato JSON</span><span class="sxs-lookup"><span data-stu-id="586d1-157">Example 1: Send a new email using JSON format</span></span>
<span data-ttu-id="586d1-158">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="586d1-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="586d1-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="586d1-159">Request</span></span>
<span data-ttu-id="586d1-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="586d1-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="586d1-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="586d1-161">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```
# <a name="c"></a>[<span data-ttu-id="586d1-162">C#</span><span class="sxs-lookup"><span data-stu-id="586d1-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="586d1-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="586d1-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="586d1-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="586d1-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="586d1-165">Java</span><span class="sxs-lookup"><span data-stu-id="586d1-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="586d1-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="586d1-166">Response</span></span>
<span data-ttu-id="586d1-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="586d1-167">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-create-a-message-with-custom-internet-message-headers-and-send-the-message"></a><span data-ttu-id="586d1-168">Exemplo 2: Criar uma mensagem com cabeçalhos de mensagens personalizadas na Internet e enviar a mensagem</span><span class="sxs-lookup"><span data-stu-id="586d1-168">Example 2: Create a message with custom Internet message headers and send the message</span></span>
#### <a name="request"></a><span data-ttu-id="586d1-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="586d1-169">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="586d1-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="586d1-170">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "9/9/2018: concert",
    "body": {
      "contentType": "HTML",
      "content": "The group represents Nevada."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    ],
    "internetMessageHeaders":[
      {
        "name":"x-custom-header-group-name",
        "value":"Nevada"
      },
      {
        "name":"x-custom-header-group-id",
        "value":"NV001"
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="586d1-171">C#</span><span class="sxs-lookup"><span data-stu-id="586d1-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="586d1-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="586d1-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="586d1-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="586d1-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="586d1-174">Java</span><span class="sxs-lookup"><span data-stu-id="586d1-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="586d1-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="586d1-175">Response</span></span>
<span data-ttu-id="586d1-176">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="586d1-176">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-3--create-a-message-with-a-file-attachment-and-send-the-message"></a><span data-ttu-id="586d1-177">Exemplo 3: Criar uma mensagem com um arquivo anexo e enviar a mensagem</span><span class="sxs-lookup"><span data-stu-id="586d1-177">Example 3:  Create a message with a file attachment and send the message</span></span>
#### <a name="request"></a><span data-ttu-id="586d1-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="586d1-178">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="586d1-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="586d1-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_attachment"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "meganb@contoso.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "#microsoft.graph.fileAttachment",
        "name": "attachment.txt",
        "contentType": "text/plain",
        "contentBytes": "SGVsbG8gV29ybGQh"
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="586d1-180">C#</span><span class="sxs-lookup"><span data-stu-id="586d1-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="586d1-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="586d1-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="586d1-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="586d1-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="586d1-183">Java</span><span class="sxs-lookup"><span data-stu-id="586d1-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="586d1-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="586d1-184">Response</span></span>
<span data-ttu-id="586d1-185">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="586d1-185">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-4-send-a-new-message-using-mime-format"></a><span data-ttu-id="586d1-186">Exemplo 4: Enviar uma nova mensagem utilizando o formato MIME</span><span class="sxs-lookup"><span data-stu-id="586d1-186">Example 4: Send a new message using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="586d1-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="586d1-187">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "message_send_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRvcjoKWC1NUy1Fe

```

#### <a name="response"></a><span data-ttu-id="586d1-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="586d1-188">Response</span></span>
<span data-ttu-id="586d1-189">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="586d1-189">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="586d1-190">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="586d1-190">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
