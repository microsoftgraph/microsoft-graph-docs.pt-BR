---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.
ms.openlocfilehash: 8103a1f0b4004e602c23d114e199b60fa96c15e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040300"
---
# <a name="send-mail"></a><span data-ttu-id="f2d47-104">Enviar email</span><span class="sxs-lookup"><span data-stu-id="f2d47-104">Send mail</span></span>

> <span data-ttu-id="f2d47-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2d47-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2d47-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2d47-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2d47-p103">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="f2d47-p103">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="f2d47-109">Na mesma chamada de ação **sendMail** , você pode:</span><span class="sxs-lookup"><span data-stu-id="f2d47-109">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="f2d47-110">Incluir um [anexo](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="f2d47-110">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="f2d47-111">Use um [mencionar](../resources/mention.md) chamar check-out de outro usuário na nova mensagem</span><span class="sxs-lookup"><span data-stu-id="f2d47-111">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="f2d47-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="f2d47-112">Permissions</span></span>
<span data-ttu-id="f2d47-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2d47-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f2d47-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2d47-115">Permission type</span></span>      | <span data-ttu-id="f2d47-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2d47-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2d47-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2d47-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f2d47-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f2d47-118">Mail.Send</span></span>    |
|<span data-ttu-id="f2d47-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2d47-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2d47-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f2d47-120">Mail.Send</span></span>    |
|<span data-ttu-id="f2d47-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2d47-121">Application</span></span> | <span data-ttu-id="f2d47-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f2d47-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2d47-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2d47-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="f2d47-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2d47-124">Request headers</span></span>
| <span data-ttu-id="f2d47-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2d47-125">Header</span></span>       | <span data-ttu-id="f2d47-126">Valor</span><span class="sxs-lookup"><span data-stu-id="f2d47-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2d47-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2d47-127">Authorization</span></span>  | <span data-ttu-id="f2d47-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2d47-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f2d47-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2d47-130">Content-Type</span></span>  | <span data-ttu-id="f2d47-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f2d47-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2d47-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2d47-132">Request body</span></span>
<span data-ttu-id="f2d47-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2d47-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f2d47-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f2d47-134">Parameter</span></span>    | <span data-ttu-id="f2d47-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2d47-135">Type</span></span>   |<span data-ttu-id="f2d47-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2d47-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2d47-137">Message</span><span class="sxs-lookup"><span data-stu-id="f2d47-137">Message</span></span>|[<span data-ttu-id="f2d47-138">Message</span><span class="sxs-lookup"><span data-stu-id="f2d47-138">Message</span></span>](../resources/message.md)|<span data-ttu-id="f2d47-p106">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2d47-p106">The message to send. Required.</span></span>|
|<span data-ttu-id="f2d47-141">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="f2d47-141">SaveToSentItems</span></span>|<span data-ttu-id="f2d47-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="f2d47-142">Boolean</span></span>|<span data-ttu-id="f2d47-p107">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="f2d47-p107">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="f2d47-146">Se você quiser usar **mencionar** chamar check-out de outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="f2d47-146">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="f2d47-147">Inclua a propriedade necessários **toRecipients** , a propriedade **menções** e propriedades de qualquer mensagem graváveis no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2d47-147">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="f2d47-148">Para cada mencionam na propriedade **menções** , você deve especificar a propriedade **mencionado** .</span><span class="sxs-lookup"><span data-stu-id="f2d47-148">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="f2d47-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2d47-149">Response</span></span>

<span data-ttu-id="f2d47-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2d47-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2d47-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2d47-152">Example</span></span>
<span data-ttu-id="f2d47-153">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f2d47-153">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="f2d47-154">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="f2d47-154">Request 1</span></span>
<span data-ttu-id="f2d47-155">Aqui está um exemplo da solicitação para criar e enviar uma mensagem dinamicamente.</span><span class="sxs-lookup"><span data-stu-id="f2d47-155">Here is an example of the request to create and send a message on the fly.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="f2d47-156">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="f2d47-156">Response 1</span></span>
<span data-ttu-id="f2d47-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2d47-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="f2d47-158">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="f2d47-158">Request 2</span></span>
<span data-ttu-id="f2d47-159">O exemplo a seguir mostra uma mensagem pelo usuário conectado para Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="f2d47-159">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="f2d47-160">A mensagem também inclui um mencionam de outro usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="f2d47-160">The message also includes a mention of another user, Dana Swope.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="f2d47-161">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="f2d47-161">Response 2</span></span>
<span data-ttu-id="f2d47-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2d47-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="f2d47-163">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="f2d47-163">Request 3</span></span>
<span data-ttu-id="f2d47-164">O próximo exemplo cria uma mensagem com cabeçalhos de mensagem personalizados da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="f2d47-164">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-3"></a><span data-ttu-id="f2d47-165">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="f2d47-165">Response 3</span></span>
<span data-ttu-id="f2d47-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2d47-166">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
