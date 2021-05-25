---
title: Enviar email
description: Envie a mensagem especificada no corpo da solicitação usando o formato JSON ou MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5ee3bc0682f6611a06cb5e24e66b2c665a0be123
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645637"
---
# <a name="send-mail"></a><span data-ttu-id="8c8ed-103">Enviar email</span><span class="sxs-lookup"><span data-stu-id="8c8ed-103">Send mail</span></span>

<span data-ttu-id="8c8ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c8ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c8ed-105">Envie a mensagem especificada no corpo da solicitação usando o formato JSON ou MIME.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-105">Send the message specified in the request body using either JSON or MIME format.</span></span>

<span data-ttu-id="8c8ed-106">Ao usar o formato JSON, você [](../resources/mention.md) pode incluir um [anexo](../resources/attachment.md) e usar uma menção para chamar outro usuário na nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-106">When using JSON format you can include an [attachment](../resources/attachment.md) and use a [mention](../resources/mention.md) to call out another user in the new message.</span></span>

<span data-ttu-id="8c8ed-107">Ao usar o formato MIME:</span><span class="sxs-lookup"><span data-stu-id="8c8ed-107">When using MIME format:</span></span>
- <span data-ttu-id="8c8ed-108">Forneça os [headers](https://tools.ietf.org/html/rfc2076) de mensagens da Internet aplicáveis e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045), todos codificados no **formato base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-108">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="8c8ed-109">Adicione quaisquer anexos e propriedades S/MIME ao conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-109">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="8c8ed-110">Este método salva a mensagem na pasta **Itens** Enviados.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-110">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="8c8ed-111">Como alternativa, [crie uma mensagem de rascunho](../api/user-post-messages.md) para enviar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-111">Alternatively, [create a draft message](../api/user-post-messages.md) to send later.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c8ed-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c8ed-112">Permissions</span></span>
<span data-ttu-id="8c8ed-113">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-113">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="8c8ed-114">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c8ed-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c8ed-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c8ed-115">Permission type</span></span>      | <span data-ttu-id="8c8ed-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c8ed-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c8ed-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c8ed-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8c8ed-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8c8ed-118">Mail.Send</span></span>    |
|<span data-ttu-id="8c8ed-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c8ed-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c8ed-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8c8ed-120">Mail.Send</span></span>    |
|<span data-ttu-id="8c8ed-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c8ed-121">Application</span></span> | <span data-ttu-id="8c8ed-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8c8ed-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c8ed-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c8ed-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```

## <a name="request-headers"></a><span data-ttu-id="8c8ed-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8ed-124">Request headers</span></span>
| <span data-ttu-id="8c8ed-125">Nome</span><span class="sxs-lookup"><span data-stu-id="8c8ed-125">Name</span></span>       | <span data-ttu-id="8c8ed-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c8ed-126">Type</span></span> | <span data-ttu-id="8c8ed-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c8ed-127">Description</span></span>| 
|:---------------|:--------|:----------
| <span data-ttu-id="8c8ed-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c8ed-128">Authorization</span></span>  | <span data-ttu-id="8c8ed-129">string</span><span class="sxs-lookup"><span data-stu-id="8c8ed-129">string</span></span>  | <span data-ttu-id="8c8ed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8c8ed-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c8ed-132">Content-Type</span></span> | <span data-ttu-id="8c8ed-133">string</span><span class="sxs-lookup"><span data-stu-id="8c8ed-133">string</span></span>  | <span data-ttu-id="8c8ed-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="8c8ed-136">Use `application/json` para um objeto JSON e para conteúdo `text/plain` MIME.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-136">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c8ed-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8ed-137">Request body</span></span>
<span data-ttu-id="8c8ed-138">Ao usar o formato JSON, forneça um objeto JSON com os seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-138">When using JSON format, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c8ed-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8c8ed-139">Parameter</span></span>    | <span data-ttu-id="8c8ed-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c8ed-140">Type</span></span>   |<span data-ttu-id="8c8ed-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c8ed-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c8ed-142">Message</span><span class="sxs-lookup"><span data-stu-id="8c8ed-142">Message</span></span>|[<span data-ttu-id="8c8ed-143">Message</span><span class="sxs-lookup"><span data-stu-id="8c8ed-143">Message</span></span>](../resources/message.md)|<span data-ttu-id="8c8ed-p104">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="8c8ed-146">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="8c8ed-146">SaveToSentItems</span></span>|<span data-ttu-id="8c8ed-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c8ed-147">Boolean</span></span>|<span data-ttu-id="8c8ed-p105">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="8c8ed-151">Para usar **a menção** para chamar outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="8c8ed-151">To use **mention** to call out another user in the new message:</span></span>
- <span data-ttu-id="8c8ed-152">Inclua a propriedade **required toRecipients,** a propriedade **mentions** e quaisquer propriedades de mensagem writable no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-152">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="8c8ed-153">Para cada menção na **propriedade mentions,** você deve especificar a **propriedade** mencionada.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-153">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="8c8ed-154">Ao especificar o corpo no formato MIME, forneça o conteúdo MIME como uma cadeia de caracteres codificada com **base64** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-154">When specifying the body in MIME format, provide the MIME content as **a base64-encoded string** in the request body.</span></span> <span data-ttu-id="8c8ed-155">Não inclua parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-155">Do not include parameters.</span></span>

## <a name="response"></a><span data-ttu-id="8c8ed-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c8ed-156">Response</span></span>

<span data-ttu-id="8c8ed-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="8c8ed-159">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará e a seguinte mensagem de erro: "Cadeia de caracteres `400 Bad request` base64 inválida para conteúdo MIME".</span><span class="sxs-lookup"><span data-stu-id="8c8ed-159">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="8c8ed-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8c8ed-160">Examples</span></span>
### <a name="example-1-send-a-new-email-using-json-format"></a><span data-ttu-id="8c8ed-161">Exemplo 1: Enviar um novo email usando o formato JSON</span><span class="sxs-lookup"><span data-stu-id="8c8ed-161">Example 1: Send a new email using JSON format</span></span>
<span data-ttu-id="8c8ed-162">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-162">Here is an example of how to call this API.</span></span>
#### <a name="request"></a><span data-ttu-id="8c8ed-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8ed-163">Request</span></span>
<span data-ttu-id="8c8ed-164">Aqui está um exemplo da solicitação para criar e enviar uma mensagem em tempo real.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-164">Here is an example of the request to create and send a message on the fly.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c8ed-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c8ed-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8c8ed-166">C#</span><span class="sxs-lookup"><span data-stu-id="8c8ed-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c8ed-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c8ed-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c8ed-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c8ed-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c8ed-169">Java</span><span class="sxs-lookup"><span data-stu-id="8c8ed-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8c8ed-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c8ed-170">Response</span></span>
<span data-ttu-id="8c8ed-171">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-171">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-send-a-message-that-includes-an--mention"></a><span data-ttu-id="8c8ed-172">Exemplo 2: Enviar uma mensagem que inclui uma @-mention</span><span class="sxs-lookup"><span data-stu-id="8c8ed-172">Example 2: Send a message that includes an @-mention</span></span>
#### <a name="request"></a><span data-ttu-id="8c8ed-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8ed-173">Request</span></span>
<span data-ttu-id="8c8ed-174">O próximo exemplo mostra uma mensagem do usuário in-lo como Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-174">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="8c8ed-175">A mensagem também inclui uma menção de outra usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-175">The message also includes a mention of another user, Dana Swope.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c8ed-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c8ed-176">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="8c8ed-177">C#</span><span class="sxs-lookup"><span data-stu-id="8c8ed-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c8ed-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c8ed-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c8ed-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c8ed-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c8ed-180">Java</span><span class="sxs-lookup"><span data-stu-id="8c8ed-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8c8ed-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c8ed-181">Response</span></span>
<span data-ttu-id="8c8ed-182">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-182">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-send-a-message-that-includes-custom-internet-message-headers"></a><span data-ttu-id="8c8ed-183">Exemplo 3: Enviar uma mensagem que inclua os headers de mensagens da Internet personalizados</span><span class="sxs-lookup"><span data-stu-id="8c8ed-183">Example 3: Send a message that includes custom Internet message headers</span></span> 
#### <a name="request"></a><span data-ttu-id="8c8ed-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8ed-184">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c8ed-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c8ed-185">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="8c8ed-186">C#</span><span class="sxs-lookup"><span data-stu-id="8c8ed-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c8ed-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c8ed-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c8ed-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c8ed-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c8ed-189">Java</span><span class="sxs-lookup"><span data-stu-id="8c8ed-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8c8ed-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c8ed-190">Response</span></span>
<span data-ttu-id="8c8ed-191">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-191">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-4-sends-a-message-with-a-file-attachment"></a><span data-ttu-id="8c8ed-192">Exemplo 4: envia uma mensagem com um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="8c8ed-192">Example 4: Sends a message with a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="8c8ed-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8ed-193">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c8ed-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c8ed-194">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8c8ed-195">C#</span><span class="sxs-lookup"><span data-stu-id="8c8ed-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-sendmail-with-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c8ed-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c8ed-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-sendmail-with-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c8ed-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c8ed-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-sendmail-with-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c8ed-198">Java</span><span class="sxs-lookup"><span data-stu-id="8c8ed-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-sendmail-with-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8c8ed-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c8ed-199">Response</span></span>

<span data-ttu-id="8c8ed-200">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-200">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```
### <a name="example-5-send-a-new-message-using-mime-format"></a><span data-ttu-id="8c8ed-201">Exemplo 5: Enviar uma nova mensagem usando o formato MIME</span><span class="sxs-lookup"><span data-stu-id="8c8ed-201">Example 5: Send a new message using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="8c8ed-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8ed-202">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "message_send_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/sendMail
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
#### <a name="response"></a><span data-ttu-id="8c8ed-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c8ed-203">Response</span></span>
<span data-ttu-id="8c8ed-204">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-204">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="8c8ed-205">Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="8c8ed-205">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
