---
title: 'message: forward'
description: 'Encaminhar uma mensagem, adicionar um comentário ou modificar qualquer propriedade atualizável  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9b4e9ee3e2b0c97971e12143263a33e2241f876c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346923"
---
# <a name="message-forward"></a><span data-ttu-id="42d22-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="42d22-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42d22-104">Encaminhar uma mensagem, adicionar um comentário ou modificar qualquer propriedade atualizável</span><span class="sxs-lookup"><span data-stu-id="42d22-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="42d22-105">tudo em uma \*\*\*\* chamada de encaminhamento.</span><span class="sxs-lookup"><span data-stu-id="42d22-105">all in one **forward** call.</span></span> <span data-ttu-id="42d22-106">A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="42d22-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="42d22-107">Outra opção é primeiro [criar um rascunho de mensagem de encaminhamento](../api/message-createforward.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="42d22-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="42d22-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="42d22-108">**Note**</span></span>

- <span data-ttu-id="42d22-109">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="42d22-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="42d22-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="42d22-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="42d22-111">Você deve especificar o `toRecipients` parâmetro ou a propriedade ToRecipients do \*\*\*\* `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="42d22-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="42d22-112">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="42d22-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="42d22-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="42d22-113">Permissions</span></span>
<span data-ttu-id="42d22-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42d22-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42d22-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42d22-116">Permission type</span></span>      | <span data-ttu-id="42d22-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42d22-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42d22-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42d22-118">Delegated (work or school account)</span></span> | <span data-ttu-id="42d22-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="42d22-119">Mail.Send</span></span>    |
|<span data-ttu-id="42d22-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42d22-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42d22-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="42d22-121">Mail.Send</span></span>    |
|<span data-ttu-id="42d22-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42d22-122">Application</span></span> | <span data-ttu-id="42d22-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="42d22-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="42d22-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42d22-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="42d22-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42d22-125">Request headers</span></span>
| <span data-ttu-id="42d22-126">Nome</span><span class="sxs-lookup"><span data-stu-id="42d22-126">Name</span></span>       | <span data-ttu-id="42d22-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="42d22-127">Type</span></span> | <span data-ttu-id="42d22-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d22-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42d22-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="42d22-129">Authorization</span></span>  | <span data-ttu-id="42d22-130">string</span><span class="sxs-lookup"><span data-stu-id="42d22-130">string</span></span>  | <span data-ttu-id="42d22-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42d22-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42d22-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42d22-133">Content-Type</span></span> | <span data-ttu-id="42d22-134">string</span><span class="sxs-lookup"><span data-stu-id="42d22-134">string</span></span>  | <span data-ttu-id="42d22-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42d22-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42d22-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42d22-137">Request body</span></span>
<span data-ttu-id="42d22-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42d22-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="42d22-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="42d22-139">Parameter</span></span>    | <span data-ttu-id="42d22-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="42d22-140">Type</span></span>   |<span data-ttu-id="42d22-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d22-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42d22-142">comment</span><span class="sxs-lookup"><span data-stu-id="42d22-142">comment</span></span>|<span data-ttu-id="42d22-143">String</span><span class="sxs-lookup"><span data-stu-id="42d22-143">String</span></span>|<span data-ttu-id="42d22-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="42d22-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="42d22-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="42d22-146">toRecipients</span></span>|<span data-ttu-id="42d22-147">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="42d22-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="42d22-148">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="42d22-148">The list of recipients.</span></span>|
|<span data-ttu-id="42d22-149">message</span><span class="sxs-lookup"><span data-stu-id="42d22-149">message</span></span>|[<span data-ttu-id="42d22-150">message</span><span class="sxs-lookup"><span data-stu-id="42d22-150">message</span></span>](../resources/message.md)|<span data-ttu-id="42d22-151">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="42d22-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="42d22-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d22-152">Response</span></span>

<span data-ttu-id="42d22-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42d22-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42d22-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42d22-155">Example</span></span>
<span data-ttu-id="42d22-156">O exemplo a seguir define a propriedade **isDeliveryReceiptRequested** como true, adiciona um comentário e encaminha a mensagem.</span><span class="sxs-lookup"><span data-stu-id="42d22-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="42d22-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42d22-157">Request</span></span>
<span data-ttu-id="42d22-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42d22-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="42d22-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="42d22-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this." 
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42d22-160">C#</span><span class="sxs-lookup"><span data-stu-id="42d22-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42d22-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42d22-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42d22-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="42d22-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="42d22-163">Java</span><span class="sxs-lookup"><span data-stu-id="42d22-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="42d22-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d22-164">Response</span></span>
<span data-ttu-id="42d22-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42d22-165">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
