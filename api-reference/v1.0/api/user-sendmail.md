---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9792261c9e7bb513a99165533bc13661e45c5e6d
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774342"
---
# <a name="send-mail"></a><span data-ttu-id="c3633-104">Enviar email</span><span class="sxs-lookup"><span data-stu-id="c3633-104">Send mail</span></span>

<span data-ttu-id="c3633-p102">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="c3633-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="c3633-107">Você pode incluir um [anexo de arquivo](../resources/fileattachment.md) na mesma chamada de ação de **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="c3633-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3633-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3633-108">Permissions</span></span>
<span data-ttu-id="c3633-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3633-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c3633-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3633-111">Permission type</span></span>      | <span data-ttu-id="c3633-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3633-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3633-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3633-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c3633-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3633-114">Mail.Send</span></span>    |
|<span data-ttu-id="c3633-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3633-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3633-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3633-116">Mail.Send</span></span>    |
|<span data-ttu-id="c3633-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3633-117">Application</span></span> | <span data-ttu-id="c3633-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3633-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3633-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3633-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="c3633-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3633-120">Request headers</span></span>
| <span data-ttu-id="c3633-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3633-121">Header</span></span>       | <span data-ttu-id="c3633-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c3633-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3633-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3633-123">Authorization</span></span>  | <span data-ttu-id="c3633-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3633-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c3633-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3633-126">Content-Type</span></span>  | <span data-ttu-id="c3633-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c3633-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3633-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3633-128">Request body</span></span>
<span data-ttu-id="c3633-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3633-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c3633-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c3633-130">Parameter</span></span>    | <span data-ttu-id="c3633-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3633-131">Type</span></span>   |<span data-ttu-id="c3633-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3633-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3633-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="c3633-133">message</span></span>|[<span data-ttu-id="c3633-134">Message</span><span class="sxs-lookup"><span data-stu-id="c3633-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="c3633-p105">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3633-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="c3633-137">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="c3633-137">saveToSentItems</span></span>|<span data-ttu-id="c3633-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3633-138">Boolean</span></span>|<span data-ttu-id="c3633-p106">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3633-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c3633-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3633-142">Response</span></span>

<span data-ttu-id="c3633-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3633-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3633-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3633-145">Example</span></span>
<span data-ttu-id="c3633-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c3633-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="c3633-147">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="c3633-147">Request 1</span></span>
<span data-ttu-id="c3633-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3633-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3633-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3633-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3633-150">C#</span><span class="sxs-lookup"><span data-stu-id="c3633-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3633-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3633-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3633-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3633-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3633-153">Java</span><span class="sxs-lookup"><span data-stu-id="c3633-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="c3633-154">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="c3633-154">Response 1</span></span>
<span data-ttu-id="c3633-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3633-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="c3633-156">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="c3633-156">Request 2</span></span>
<span data-ttu-id="c3633-157">O exemplo a seguir cria uma mensagem com cabeçalhos personalizados de mensagem da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="c3633-157">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3633-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3633-158">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3633-159">C#</span><span class="sxs-lookup"><span data-stu-id="c3633-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3633-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3633-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3633-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3633-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3633-162">Java</span><span class="sxs-lookup"><span data-stu-id="c3633-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="c3633-163">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="c3633-163">Response 2</span></span>
<span data-ttu-id="c3633-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3633-164">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="c3633-165">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="c3633-165">Request 3</span></span>

<span data-ttu-id="c3633-166">O exemplo a seguir cria uma mensagem com cabeçalhos personalizados de mensagem da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="c3633-166">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3633-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3633-167">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3633-168">C#</span><span class="sxs-lookup"><span data-stu-id="c3633-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3633-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3633-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3633-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3633-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3633-171">Java</span><span class="sxs-lookup"><span data-stu-id="c3633-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="c3633-172">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="c3633-172">Response 3</span></span>

<span data-ttu-id="c3633-173">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3633-173">Here is an example of the response.</span></span>
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
