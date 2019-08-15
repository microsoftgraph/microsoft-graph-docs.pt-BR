---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fe255a3f4e314d6624948a28c504236a589e81a3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421824"
---
# <a name="send-mail"></a><span data-ttu-id="3a054-104">Enviar email</span><span class="sxs-lookup"><span data-stu-id="3a054-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a054-p102">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="3a054-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="3a054-107">Na mesma chamada de ação de **sendmail** , você pode:</span><span class="sxs-lookup"><span data-stu-id="3a054-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="3a054-108">Incluir um [anexo](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="3a054-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="3a054-109">Usar uma [menção](../resources/mention.md) para chamar outro usuário na nova mensagem</span><span class="sxs-lookup"><span data-stu-id="3a054-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="3a054-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a054-110">Permissions</span></span>
<span data-ttu-id="3a054-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a054-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3a054-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a054-113">Permission type</span></span>      | <span data-ttu-id="3a054-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a054-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a054-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a054-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3a054-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3a054-116">Mail.Send</span></span>    |
|<span data-ttu-id="3a054-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a054-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a054-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3a054-118">Mail.Send</span></span>    |
|<span data-ttu-id="3a054-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a054-119">Application</span></span> | <span data-ttu-id="3a054-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3a054-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a054-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a054-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="3a054-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a054-122">Request headers</span></span>
| <span data-ttu-id="3a054-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a054-123">Header</span></span>       | <span data-ttu-id="3a054-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3a054-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a054-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a054-125">Authorization</span></span>  | <span data-ttu-id="3a054-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a054-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a054-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a054-128">Content-Type</span></span>  | <span data-ttu-id="3a054-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3a054-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a054-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a054-130">Request body</span></span>
<span data-ttu-id="3a054-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a054-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a054-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3a054-132">Parameter</span></span>    | <span data-ttu-id="3a054-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a054-133">Type</span></span>   |<span data-ttu-id="3a054-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a054-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a054-135">Message</span><span class="sxs-lookup"><span data-stu-id="3a054-135">Message</span></span>|[<span data-ttu-id="3a054-136">Message</span><span class="sxs-lookup"><span data-stu-id="3a054-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="3a054-p105">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a054-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="3a054-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="3a054-139">SaveToSentItems</span></span>|<span data-ttu-id="3a054-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a054-140">Boolean</span></span>|<span data-ttu-id="3a054-p106">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="3a054-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="3a054-144">Se você quiser usar **menção** para chamar outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="3a054-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="3a054-145">Inclua a propriedade \*\*\*\* Required ToRecipients, a \*\*\*\* Propriedade mencionas e qualquer propriedade gravável de mensagem no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a054-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="3a054-146">Para cada menção na propriedade **menciona** , você deve especificar a propriedade **mencionado** .</span><span class="sxs-lookup"><span data-stu-id="3a054-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="3a054-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a054-147">Response</span></span>

<span data-ttu-id="3a054-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a054-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a054-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a054-150">Example</span></span>
<span data-ttu-id="3a054-151">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3a054-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="3a054-152">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="3a054-152">Request 1</span></span>
<span data-ttu-id="3a054-153">Aqui está um exemplo da solicitação para criar e enviar uma mensagem instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="3a054-153">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3a054-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a054-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3a054-155">C#</span><span class="sxs-lookup"><span data-stu-id="3a054-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a054-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a054-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3a054-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3a054-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="3a054-158">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="3a054-158">Response 1</span></span>
<span data-ttu-id="3a054-159">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a054-159">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="3a054-160">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="3a054-160">Request 2</span></span>
<span data-ttu-id="3a054-161">O exemplo a seguir mostra uma mensagem pelo usuário conectado ao estande de Paula.</span><span class="sxs-lookup"><span data-stu-id="3a054-161">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="3a054-162">A mensagem também inclui uma menção de outro usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="3a054-162">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3a054-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a054-163">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3a054-164">C#</span><span class="sxs-lookup"><span data-stu-id="3a054-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a054-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a054-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3a054-166">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3a054-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="3a054-167">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="3a054-167">Response 2</span></span>
<span data-ttu-id="3a054-168">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a054-168">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="3a054-169">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="3a054-169">Request 3</span></span>
<span data-ttu-id="3a054-170">O exemplo a seguir cria uma mensagem com cabeçalhos personalizados de mensagem da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="3a054-170">The next example creates a message with custom Internet message headers and sends the message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3a054-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a054-171">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3a054-172">C#</span><span class="sxs-lookup"><span data-stu-id="3a054-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a054-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a054-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3a054-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3a054-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-3"></a><span data-ttu-id="3a054-175">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="3a054-175">Response 3</span></span>
<span data-ttu-id="3a054-176">Este é um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a054-176">Here is an example of the response.</span></span>
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
