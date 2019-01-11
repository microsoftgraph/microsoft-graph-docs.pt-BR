---
title: Enviar email
description: Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 9187601787fce5b173ce6d22006bc56bec9b83fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872146"
---
# <a name="send-mail"></a><span data-ttu-id="0d13d-104">Enviar email</span><span class="sxs-lookup"><span data-stu-id="0d13d-104">Send mail</span></span>

<span data-ttu-id="0d13d-p102">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="0d13d-p102">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="0d13d-107">Você pode incluir um [anexo de arquivo](../resources/fileattachment.md) na mesma chamada de ação de **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="0d13d-107">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d13d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d13d-108">Permissions</span></span>
<span data-ttu-id="0d13d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d13d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0d13d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d13d-111">Permission type</span></span>      | <span data-ttu-id="0d13d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d13d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d13d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d13d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0d13d-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0d13d-114">Mail.Send</span></span>    |
|<span data-ttu-id="0d13d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d13d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d13d-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0d13d-116">Mail.Send</span></span>    |
|<span data-ttu-id="0d13d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d13d-117">Application</span></span> | <span data-ttu-id="0d13d-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="0d13d-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d13d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d13d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="0d13d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d13d-120">Request headers</span></span>
| <span data-ttu-id="0d13d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d13d-121">Header</span></span>       | <span data-ttu-id="0d13d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0d13d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d13d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d13d-123">Authorization</span></span>  | <span data-ttu-id="0d13d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d13d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d13d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d13d-126">Content-Type</span></span>  | <span data-ttu-id="0d13d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0d13d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d13d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d13d-128">Request body</span></span>
<span data-ttu-id="0d13d-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d13d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0d13d-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0d13d-130">Parameter</span></span>    | <span data-ttu-id="0d13d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d13d-131">Type</span></span>   |<span data-ttu-id="0d13d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d13d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d13d-133">message</span><span class="sxs-lookup"><span data-stu-id="0d13d-133">message</span></span>|[<span data-ttu-id="0d13d-134">Message</span><span class="sxs-lookup"><span data-stu-id="0d13d-134">Message</span></span>](../resources/message.md)|<span data-ttu-id="0d13d-p105">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d13d-p105">The message to send. Required.</span></span>|
|<span data-ttu-id="0d13d-137">saveToSentItems</span><span class="sxs-lookup"><span data-stu-id="0d13d-137">saveToSentItems</span></span>|<span data-ttu-id="0d13d-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d13d-138">Boolean</span></span>|<span data-ttu-id="0d13d-p106">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="0d13d-p106">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0d13d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d13d-142">Response</span></span>

<span data-ttu-id="0d13d-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d13d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d13d-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d13d-145">Example</span></span>
<span data-ttu-id="0d13d-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0d13d-146">Here is an example of how to call this API.</span></span>
##### <a name="request-1"></a><span data-ttu-id="0d13d-147">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="0d13d-147">Request 1</span></span>
<span data-ttu-id="0d13d-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d13d-148">Here is an example of the request.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="0d13d-149">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="0d13d-149">Response 1</span></span>
<span data-ttu-id="0d13d-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d13d-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="request-2"></a><span data-ttu-id="0d13d-151">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="0d13d-151">Request 2</span></span>
<span data-ttu-id="0d13d-152">O próximo exemplo cria uma mensagem com cabeçalhos de mensagem personalizados da Internet e envia a mensagem.</span><span class="sxs-lookup"><span data-stu-id="0d13d-152">The next example creates a message with custom Internet message headers and sends the message.</span></span>
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

##### <a name="response-2"></a><span data-ttu-id="0d13d-153">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="0d13d-153">Response 2</span></span>
<span data-ttu-id="0d13d-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d13d-154">Here is an example of the response.</span></span>
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
