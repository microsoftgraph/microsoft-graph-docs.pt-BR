---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 02356e8c0eb061d33653477bc4497cbe99c6a209
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269906"
---
# <a name="send-mail"></a><span data-ttu-id="00fea-104">Enviar email</span><span class="sxs-lookup"><span data-stu-id="00fea-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00fea-p102">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="00fea-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="00fea-107">Na mesma chamada de ação de **sendmail** , você pode:</span><span class="sxs-lookup"><span data-stu-id="00fea-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="00fea-108">Incluir um [anexo](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="00fea-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="00fea-109">Usar uma [menção](../resources/mention.md) para chamar outro usuário na nova mensagem</span><span class="sxs-lookup"><span data-stu-id="00fea-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="00fea-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="00fea-110">Permissions</span></span>
<span data-ttu-id="00fea-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00fea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="00fea-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00fea-113">Permission type</span></span>      | <span data-ttu-id="00fea-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00fea-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00fea-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00fea-115">Delegated (work or school account)</span></span> | <span data-ttu-id="00fea-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="00fea-116">Mail.Send</span></span>    |
|<span data-ttu-id="00fea-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00fea-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00fea-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="00fea-118">Mail.Send</span></span>    |
|<span data-ttu-id="00fea-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00fea-119">Application</span></span> | <span data-ttu-id="00fea-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="00fea-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="00fea-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00fea-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="00fea-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00fea-122">Request headers</span></span>
| <span data-ttu-id="00fea-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00fea-123">Header</span></span>       | <span data-ttu-id="00fea-124">Valor</span><span class="sxs-lookup"><span data-stu-id="00fea-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00fea-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="00fea-125">Authorization</span></span>  | <span data-ttu-id="00fea-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00fea-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="00fea-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00fea-128">Content-Type</span></span>  | <span data-ttu-id="00fea-129">application/json</span><span class="sxs-lookup"><span data-stu-id="00fea-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00fea-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00fea-130">Request body</span></span>
<span data-ttu-id="00fea-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00fea-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="00fea-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="00fea-132">Parameter</span></span>    | <span data-ttu-id="00fea-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="00fea-133">Type</span></span>   |<span data-ttu-id="00fea-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="00fea-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00fea-135">Message</span><span class="sxs-lookup"><span data-stu-id="00fea-135">Message</span></span>|[<span data-ttu-id="00fea-136">Message</span><span class="sxs-lookup"><span data-stu-id="00fea-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="00fea-p105">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00fea-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="00fea-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="00fea-139">SaveToSentItems</span></span>|<span data-ttu-id="00fea-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="00fea-140">Boolean</span></span>|<span data-ttu-id="00fea-p106">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="00fea-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="00fea-144">Se você quiser usar **menção** para chamar outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="00fea-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="00fea-145">Inclua a propriedade \*\*\*\* Required ToRecipients, a \*\*\*\* Propriedade mencionas e qualquer propriedade gravável de mensagem no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00fea-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="00fea-146">Para cada menção na propriedade **menciona** , você deve especificar a propriedade **mencionado** .</span><span class="sxs-lookup"><span data-stu-id="00fea-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="00fea-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="00fea-147">Response</span></span>

<span data-ttu-id="00fea-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00fea-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00fea-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00fea-150">Example</span></span>
<span data-ttu-id="00fea-151">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="00fea-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="00fea-152">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="00fea-152">Request 1</span></span>
<span data-ttu-id="00fea-153">Aqui está um exemplo da solicitação para criar e enviar uma mensagem instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="00fea-153">Here is an example of the request to create and send a message on the fly.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="00fea-154">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="00fea-154">Response 1</span></span>
<span data-ttu-id="00fea-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00fea-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="00fea-156">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="00fea-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="00fea-157">C#</span><span class="sxs-lookup"><span data-stu-id="00fea-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00fea-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="00fea-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="00fea-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00fea-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_sendmail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a><span data-ttu-id="00fea-160">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="00fea-160">Request 2</span></span>
<span data-ttu-id="00fea-161">O exemplo a seguir mostra uma mensagem pelo usuário conectado ao estande de Paula.</span><span class="sxs-lookup"><span data-stu-id="00fea-161">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="00fea-162">A mensagem também inclui uma menção de outro usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="00fea-162">The message also includes a mention of another user, Dana Swope.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="00fea-163">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="00fea-163">Response 2</span></span>
<span data-ttu-id="00fea-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00fea-164">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="00fea-165">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="00fea-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="00fea-166">C#</span><span class="sxs-lookup"><span data-stu-id="00fea-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail_with_mentions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00fea-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="00fea-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail_with_mentions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="00fea-168">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00fea-168">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_sendmail_with_mentions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-3"></a><span data-ttu-id="00fea-169">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="00fea-169">Request 3</span></span>
<span data-ttu-id="00fea-170">O exemplo a seguir cria uma mensagem com cabeçalhos personalizados de mensagem da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="00fea-170">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-3"></a><span data-ttu-id="00fea-171">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="00fea-171">Response 3</span></span>
<span data-ttu-id="00fea-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00fea-172">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="00fea-173">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="00fea-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="00fea-174">C#</span><span class="sxs-lookup"><span data-stu-id="00fea-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00fea-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="00fea-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="00fea-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00fea-176">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_sendmail_with_headers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
