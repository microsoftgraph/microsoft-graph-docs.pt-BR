---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3e722ea2ee069f5ea18f27c26e658847dfdfabdd
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107350"
---
# <a name="send-mail"></a><span data-ttu-id="91b99-104">Enviar email</span><span class="sxs-lookup"><span data-stu-id="91b99-104">Send mail</span></span>

<span data-ttu-id="91b99-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b99-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b99-p102">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="91b99-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="91b99-108">Na mesma chamada de ação de **sendmail** , você pode:</span><span class="sxs-lookup"><span data-stu-id="91b99-108">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="91b99-109">Incluir um [anexo](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="91b99-109">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="91b99-110">Usar uma [menção](../resources/mention.md) para chamar outro usuário na nova mensagem</span><span class="sxs-lookup"><span data-stu-id="91b99-110">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="91b99-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="91b99-111">Permissions</span></span>
<span data-ttu-id="91b99-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91b99-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="91b99-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91b99-114">Permission type</span></span>      | <span data-ttu-id="91b99-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91b99-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91b99-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91b99-116">Delegated (work or school account)</span></span> | <span data-ttu-id="91b99-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="91b99-117">Mail.Send</span></span>    |
|<span data-ttu-id="91b99-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91b99-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b99-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="91b99-119">Mail.Send</span></span>    |
|<span data-ttu-id="91b99-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91b99-120">Application</span></span> | <span data-ttu-id="91b99-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="91b99-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="91b99-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91b99-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="91b99-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91b99-123">Request headers</span></span>
| <span data-ttu-id="91b99-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91b99-124">Header</span></span>       | <span data-ttu-id="91b99-125">Valor</span><span class="sxs-lookup"><span data-stu-id="91b99-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91b99-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="91b99-126">Authorization</span></span>  | <span data-ttu-id="91b99-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91b99-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91b99-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91b99-129">Content-Type</span></span>  | <span data-ttu-id="91b99-130">application/json</span><span class="sxs-lookup"><span data-stu-id="91b99-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91b99-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91b99-131">Request body</span></span>
<span data-ttu-id="91b99-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91b99-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="91b99-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="91b99-133">Parameter</span></span>    | <span data-ttu-id="91b99-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="91b99-134">Type</span></span>   |<span data-ttu-id="91b99-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b99-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91b99-136">Message</span><span class="sxs-lookup"><span data-stu-id="91b99-136">Message</span></span>|[<span data-ttu-id="91b99-137">Message</span><span class="sxs-lookup"><span data-stu-id="91b99-137">Message</span></span>](../resources/message.md)|<span data-ttu-id="91b99-p105">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91b99-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="91b99-140">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="91b99-140">SaveToSentItems</span></span>|<span data-ttu-id="91b99-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="91b99-141">Boolean</span></span>|<span data-ttu-id="91b99-p106">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="91b99-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="91b99-145">Se você quiser usar **menção** para chamar outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="91b99-145">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="91b99-146">Inclua a propriedade Required **ToRecipients** , a propriedade **mencionas** e qualquer propriedade gravável de mensagem no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91b99-146">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="91b99-147">Para cada menção na propriedade **menciona** , você deve especificar a propriedade **mencionado** .</span><span class="sxs-lookup"><span data-stu-id="91b99-147">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="91b99-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b99-148">Response</span></span>

<span data-ttu-id="91b99-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b99-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91b99-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91b99-151">Example</span></span>
<span data-ttu-id="91b99-152">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="91b99-152">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="91b99-153">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="91b99-153">Request 1</span></span>
<span data-ttu-id="91b99-154">Aqui está um exemplo da solicitação para criar e enviar uma mensagem instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="91b99-154">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="http"></a>[<span data-ttu-id="91b99-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="91b99-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 512

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
          "address": "samanthab@contoso.onmicrosoft.com"
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
# <a name="c"></a>[<span data-ttu-id="91b99-156">C#</span><span class="sxs-lookup"><span data-stu-id="91b99-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91b99-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91b99-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91b99-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91b99-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="91b99-159">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="91b99-159">Response 1</span></span>
<span data-ttu-id="91b99-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b99-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="91b99-161">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="91b99-161">Request 2</span></span>
<span data-ttu-id="91b99-162">O exemplo a seguir mostra uma mensagem pelo usuário conectado ao estande de Paula.</span><span class="sxs-lookup"><span data-stu-id="91b99-162">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="91b99-163">A mensagem também inclui uma menção de outro usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="91b99-163">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="http"></a>[<span data-ttu-id="91b99-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="91b99-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_mentions"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
Content-type: application/json
Content-length: 344

{
  "Message": {
    "subject": "Project kickoff",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="91b99-165">C#</span><span class="sxs-lookup"><span data-stu-id="91b99-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91b99-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91b99-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91b99-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91b99-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="91b99-168">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="91b99-168">Response 2</span></span>
<span data-ttu-id="91b99-169">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b99-169">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="91b99-170">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="91b99-170">Request 3</span></span>
<span data-ttu-id="91b99-171">O exemplo a seguir cria uma mensagem com cabeçalhos personalizados de mensagem da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="91b99-171">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="http"></a>[<span data-ttu-id="91b99-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="91b99-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_headers"
}-->
```http
POST https://graph.microsoft.com/beta/me/sendMail
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
# <a name="c"></a>[<span data-ttu-id="91b99-173">C#</span><span class="sxs-lookup"><span data-stu-id="91b99-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91b99-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91b99-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91b99-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91b99-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="91b99-176">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="91b99-176">Response 3</span></span>
<span data-ttu-id="91b99-177">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b99-177">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-4"></a><span data-ttu-id="91b99-178">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="91b99-178">Request 4</span></span>

<span data-ttu-id="91b99-179">O exemplo a seguir cria uma mensagem com cabeçalhos personalizados de mensagem da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="91b99-179">The next example creates a message with a file attachment and sends the message.</span></span>


# <a name="http"></a>[<span data-ttu-id="91b99-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="91b99-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_sendmail_with_attachment"
}-->

```http
POST https://graph.microsoft.com/beta/me/sendMail
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
# <a name="c"></a>[<span data-ttu-id="91b99-181">C#</span><span class="sxs-lookup"><span data-stu-id="91b99-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91b99-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91b99-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91b99-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91b99-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-4"></a><span data-ttu-id="91b99-184">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="91b99-184">Response 4</span></span>

<span data-ttu-id="91b99-185">Este é um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b99-185">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
