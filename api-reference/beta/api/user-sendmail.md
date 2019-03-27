---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 47cdb200f7de493c6fcc83b3d77be2af1824ef65
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869425"
---
# <a name="send-mail"></a><span data-ttu-id="6360e-104">Enviar email</span><span class="sxs-lookup"><span data-stu-id="6360e-104">Send mail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6360e-p102">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="6360e-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="6360e-107">Na mesma chamada de ação de **sendmail** , você pode:</span><span class="sxs-lookup"><span data-stu-id="6360e-107">In the same **sendMail** action call, you can:</span></span>

- <span data-ttu-id="6360e-108">Incluir um [anexo](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="6360e-108">Include an [attachment](../resources/attachment.md)</span></span>
- <span data-ttu-id="6360e-109">Usar uma [menção](../resources/mention.md) para chamar outro usuário na nova mensagem</span><span class="sxs-lookup"><span data-stu-id="6360e-109">Use a [mention](../resources/mention.md) to call out another user in the new message</span></span>

## <a name="permissions"></a><span data-ttu-id="6360e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="6360e-110">Permissions</span></span>
<span data-ttu-id="6360e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6360e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6360e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6360e-113">Permission type</span></span>      | <span data-ttu-id="6360e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6360e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6360e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6360e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6360e-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6360e-116">Mail.Send</span></span>    |
|<span data-ttu-id="6360e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6360e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6360e-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6360e-118">Mail.Send</span></span>    |
|<span data-ttu-id="6360e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6360e-119">Application</span></span> | <span data-ttu-id="6360e-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="6360e-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="6360e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6360e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/sendMail
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="6360e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6360e-122">Request headers</span></span>
| <span data-ttu-id="6360e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6360e-123">Header</span></span>       | <span data-ttu-id="6360e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6360e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6360e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6360e-125">Authorization</span></span>  | <span data-ttu-id="6360e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6360e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6360e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6360e-128">Content-Type</span></span>  | <span data-ttu-id="6360e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6360e-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6360e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6360e-130">Request body</span></span>
<span data-ttu-id="6360e-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6360e-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6360e-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6360e-132">Parameter</span></span>    | <span data-ttu-id="6360e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6360e-133">Type</span></span>   |<span data-ttu-id="6360e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6360e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6360e-135">Message</span><span class="sxs-lookup"><span data-stu-id="6360e-135">Message</span></span>|[<span data-ttu-id="6360e-136">Message</span><span class="sxs-lookup"><span data-stu-id="6360e-136">Message</span></span>](../resources/message.md)|<span data-ttu-id="6360e-p105">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6360e-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="6360e-139">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="6360e-139">SaveToSentItems</span></span>|<span data-ttu-id="6360e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="6360e-140">Boolean</span></span>|<span data-ttu-id="6360e-p106">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="6360e-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span>|

<span data-ttu-id="6360e-144">Se você quiser usar **menção** para chamar outro usuário na nova mensagem:</span><span class="sxs-lookup"><span data-stu-id="6360e-144">If you want to use **mention** to call out another user in the new message:</span></span>

- <span data-ttu-id="6360e-145">Inclua a propriedade \*\*\*\* Required ToRecipients, a \*\*\*\* Propriedade mencionas e qualquer propriedade gravável de mensagem no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6360e-145">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="6360e-146">Para cada menção na propriedade **menciona** , você deve especificar a propriedade **mencionado** .</span><span class="sxs-lookup"><span data-stu-id="6360e-146">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

## <a name="response"></a><span data-ttu-id="6360e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6360e-147">Response</span></span>

<span data-ttu-id="6360e-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6360e-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6360e-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6360e-150">Example</span></span>
<span data-ttu-id="6360e-151">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6360e-151">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="6360e-152">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="6360e-152">Request 1</span></span>
<span data-ttu-id="6360e-153">Aqui está um exemplo da solicitação para criar e enviar uma mensagem instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="6360e-153">Here is an example of the request to create and send a message on the fly.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="6360e-154">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="6360e-154">Response 1</span></span>
<span data-ttu-id="6360e-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6360e-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


##### <a name="request-2"></a><span data-ttu-id="6360e-156">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="6360e-156">Request 2</span></span>
<span data-ttu-id="6360e-157">O exemplo a seguir mostra uma mensagem pelo usuário conectado ao estande de Paula.</span><span class="sxs-lookup"><span data-stu-id="6360e-157">The next example shows a message by the signed-in user to Samantha Booth.</span></span> <span data-ttu-id="6360e-158">A mensagem também inclui uma menção de outro usuário, Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="6360e-158">The message also includes a mention of another user, Dana Swope.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="6360e-159">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="6360e-159">Response 2</span></span>
<span data-ttu-id="6360e-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6360e-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-3"></a><span data-ttu-id="6360e-161">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="6360e-161">Request 3</span></span>
<span data-ttu-id="6360e-162">O próximo exemplo cria uma mensagem com cabeçalhos de mensagem da Internet personalizada e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="6360e-162">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-3"></a><span data-ttu-id="6360e-163">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="6360e-163">Response 3</span></span>
<span data-ttu-id="6360e-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6360e-164">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/user-sendmail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
