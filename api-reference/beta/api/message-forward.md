---
title: 'message: forward'
description: 'Encaminhar uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis  '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fb90daf582c1697dbab8f8d50e68885c91af28d3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130337"
---
# <a name="message-forward"></a><span data-ttu-id="5c770-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="5c770-103">message: forward</span></span>

<span data-ttu-id="5c770-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c770-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c770-105">Encaminhar uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis</span><span class="sxs-lookup"><span data-stu-id="5c770-105">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="5c770-106">tudo em uma **chamada** de encaminhamento.</span><span class="sxs-lookup"><span data-stu-id="5c770-106">all in one **forward** call.</span></span> <span data-ttu-id="5c770-107">A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="5c770-107">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="5c770-108">Outra opção é primeiro [criar um rascunho de mensagem de encaminhamento](../api/message-createforward.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="5c770-108">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="5c770-109">**Observação**</span><span class="sxs-lookup"><span data-stu-id="5c770-109">**Note**</span></span>

- <span data-ttu-id="5c770-110">Você pode especificar um comentário ou a **propriedade do** corpo do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5c770-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="5c770-111">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="5c770-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="5c770-112">Você deve especificar o `toRecipients` parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5c770-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="5c770-113">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="5c770-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c770-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c770-114">Permissions</span></span>
<span data-ttu-id="5c770-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c770-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c770-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c770-117">Permission type</span></span>      | <span data-ttu-id="5c770-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c770-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c770-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c770-119">Delegated (work or school account)</span></span> | <span data-ttu-id="5c770-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5c770-120">Mail.Send</span></span>    |
|<span data-ttu-id="5c770-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c770-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c770-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5c770-122">Mail.Send</span></span>    |
|<span data-ttu-id="5c770-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c770-123">Application</span></span> | <span data-ttu-id="5c770-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5c770-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c770-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c770-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="5c770-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c770-126">Request headers</span></span>
| <span data-ttu-id="5c770-127">Nome</span><span class="sxs-lookup"><span data-stu-id="5c770-127">Name</span></span>       | <span data-ttu-id="5c770-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c770-128">Type</span></span> | <span data-ttu-id="5c770-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c770-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c770-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c770-130">Authorization</span></span>  | <span data-ttu-id="5c770-131">string</span><span class="sxs-lookup"><span data-stu-id="5c770-131">string</span></span>  | <span data-ttu-id="5c770-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c770-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c770-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c770-134">Content-Type</span></span> | <span data-ttu-id="5c770-135">string</span><span class="sxs-lookup"><span data-stu-id="5c770-135">string</span></span>  | <span data-ttu-id="5c770-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c770-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c770-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c770-138">Request body</span></span>
<span data-ttu-id="5c770-139">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c770-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c770-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c770-140">Parameter</span></span>    | <span data-ttu-id="5c770-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c770-141">Type</span></span>   |<span data-ttu-id="5c770-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c770-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c770-143">comment</span><span class="sxs-lookup"><span data-stu-id="5c770-143">comment</span></span>|<span data-ttu-id="5c770-144">String</span><span class="sxs-lookup"><span data-stu-id="5c770-144">String</span></span>|<span data-ttu-id="5c770-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="5c770-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="5c770-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="5c770-147">toRecipients</span></span>|<span data-ttu-id="5c770-148">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="5c770-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="5c770-149">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="5c770-149">The list of recipients.</span></span>|
|<span data-ttu-id="5c770-150">message</span><span class="sxs-lookup"><span data-stu-id="5c770-150">message</span></span>|[<span data-ttu-id="5c770-151">message</span><span class="sxs-lookup"><span data-stu-id="5c770-151">message</span></span>](../resources/message.md)|<span data-ttu-id="5c770-152">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c770-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="5c770-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c770-153">Response</span></span>

<span data-ttu-id="5c770-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c770-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c770-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c770-156">Example</span></span>
<span data-ttu-id="5c770-157">O exemplo a seguir define a **propriedade isDeliveryReceiptRequested** como true, adiciona um comentário e encaminha a mensagem.</span><span class="sxs-lookup"><span data-stu-id="5c770-157">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="5c770-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c770-158">Request</span></span>
<span data-ttu-id="5c770-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c770-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c770-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c770-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c770-161">C#</span><span class="sxs-lookup"><span data-stu-id="5c770-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c770-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c770-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c770-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c770-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c770-164">Java</span><span class="sxs-lookup"><span data-stu-id="5c770-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5c770-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c770-165">Response</span></span>
<span data-ttu-id="5c770-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c770-166">Here is an example of the response.</span></span>
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


