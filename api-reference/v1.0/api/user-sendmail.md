---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cfb9fcd33a87b2112616241757a44f515f968df6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137211"
---
# <a name="send-mail"></a><span data-ttu-id="92d28-104">Enviar email</span><span class="sxs-lookup"><span data-stu-id="92d28-104">Send mail</span></span>

<span data-ttu-id="92d28-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92d28-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92d28-p102">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="92d28-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="92d28-108">Você pode incluir um [anexo de arquivo](../resources/fileattachment.md) na mesma chamada de ação de **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="92d28-108">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="92d28-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="92d28-109">Permissions</span></span>
<span data-ttu-id="92d28-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92d28-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="92d28-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92d28-112">Permission type</span></span>      | <span data-ttu-id="92d28-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92d28-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92d28-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92d28-114">Delegated (work or school account)</span></span> | <span data-ttu-id="92d28-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="92d28-115">Mail.Send</span></span>    |
|<span data-ttu-id="92d28-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92d28-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92d28-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="92d28-117">Mail.Send</span></span>    |
|<span data-ttu-id="92d28-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92d28-118">Application</span></span> | <span data-ttu-id="92d28-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="92d28-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="92d28-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92d28-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="92d28-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92d28-121">Request headers</span></span>
| <span data-ttu-id="92d28-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92d28-122">Header</span></span>       | <span data-ttu-id="92d28-123">Valor</span><span class="sxs-lookup"><span data-stu-id="92d28-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92d28-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="92d28-124">Authorization</span></span>  | <span data-ttu-id="92d28-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92d28-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="92d28-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92d28-127">Content-Type</span></span>  | <span data-ttu-id="92d28-128">application/json</span><span class="sxs-lookup"><span data-stu-id="92d28-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92d28-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92d28-129">Request body</span></span>
<span data-ttu-id="92d28-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92d28-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="92d28-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="92d28-131">Parameter</span></span>    | <span data-ttu-id="92d28-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="92d28-132">Type</span></span>   |<span data-ttu-id="92d28-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="92d28-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92d28-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="92d28-134">message</span></span>|[<span data-ttu-id="92d28-135">Message</span><span class="sxs-lookup"><span data-stu-id="92d28-135">Message</span></span>](../resources/message.md)|<span data-ttu-id="92d28-p105">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92d28-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="92d28-138">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="92d28-138">saveToSentItems</span></span>|<span data-ttu-id="92d28-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="92d28-139">Boolean</span></span>|<span data-ttu-id="92d28-p106">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="92d28-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="92d28-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="92d28-143">Response</span></span>

<span data-ttu-id="92d28-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92d28-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92d28-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92d28-146">Example</span></span>
<span data-ttu-id="92d28-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="92d28-147">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="92d28-148">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="92d28-148">Request 1</span></span>
<span data-ttu-id="92d28-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92d28-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92d28-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="92d28-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92d28-151">C#</span><span class="sxs-lookup"><span data-stu-id="92d28-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92d28-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92d28-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92d28-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92d28-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92d28-154">Java</span><span class="sxs-lookup"><span data-stu-id="92d28-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="92d28-155">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="92d28-155">Response 1</span></span>
<span data-ttu-id="92d28-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92d28-156">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="92d28-157">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="92d28-157">Request 2</span></span>
<span data-ttu-id="92d28-158">O exemplo a seguir cria uma mensagem com cabeçalhos personalizados de mensagem da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="92d28-158">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="http"></a>[<span data-ttu-id="92d28-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="92d28-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92d28-160">C#</span><span class="sxs-lookup"><span data-stu-id="92d28-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92d28-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92d28-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92d28-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92d28-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92d28-163">Java</span><span class="sxs-lookup"><span data-stu-id="92d28-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="92d28-164">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="92d28-164">Response 2</span></span>
<span data-ttu-id="92d28-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92d28-165">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="92d28-166">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="92d28-166">Request 3</span></span>

<span data-ttu-id="92d28-167">O exemplo a seguir cria uma mensagem com cabeçalhos personalizados de mensagem da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="92d28-167">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="http"></a>[<span data-ttu-id="92d28-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="92d28-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92d28-169">C#</span><span class="sxs-lookup"><span data-stu-id="92d28-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92d28-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92d28-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92d28-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92d28-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92d28-172">Java</span><span class="sxs-lookup"><span data-stu-id="92d28-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="92d28-173">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="92d28-173">Response 3</span></span>

<span data-ttu-id="92d28-174">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92d28-174">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
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

