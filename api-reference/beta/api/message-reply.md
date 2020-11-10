---
title: 'message: reply'
description: 'Responda ao remetente de uma mensagem, adicione um comentário ou modifique todas as propriedades atualizáveis em uma única chamada **reply**. '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7b9ea1532eb932e99325b22e8c664879089b0f1d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967403"
---
# <a name="message-reply"></a><span data-ttu-id="e9fc8-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="e9fc8-103">message: reply</span></span>

<span data-ttu-id="e9fc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9fc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9fc8-105">Responda ao remetente de uma mensagem, adicione um comentário ou modifique todas as propriedades atualizáveis em uma única chamada **reply**.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-105">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="e9fc8-106">A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-106">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="e9fc8-107">Outra opção é primeiro [criar um rascunho de mensagem de resposta](../api/message-createreply.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-107">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="e9fc8-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="e9fc8-108">**Note**</span></span>

- <span data-ttu-id="e9fc8-109">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="e9fc8-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="e9fc8-111">Se a propriedade **ReplyTo** for especificada na mensagem original, por formato de mensagem da Internet ( [RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários em **ReplyTo** e não ao destinatário na propriedade **from** .</span><span class="sxs-lookup"><span data-stu-id="e9fc8-111">If the **replyTo** property is specified in the original message, per Internet Message Format ( [RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="e9fc8-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9fc8-112">Permissions</span></span>
<span data-ttu-id="e9fc8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9fc8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9fc8-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9fc8-115">Permission type</span></span>      | <span data-ttu-id="e9fc8-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9fc8-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9fc8-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9fc8-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e9fc8-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e9fc8-118">Mail.Send</span></span>    |
|<span data-ttu-id="e9fc8-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9fc8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9fc8-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e9fc8-120">Mail.Send</span></span>    |
|<span data-ttu-id="e9fc8-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9fc8-121">Application</span></span> | <span data-ttu-id="e9fc8-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="e9fc8-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9fc8-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9fc8-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="e9fc8-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fc8-124">Request headers</span></span>
| <span data-ttu-id="e9fc8-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e9fc8-125">Name</span></span>       | <span data-ttu-id="e9fc8-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9fc8-126">Type</span></span> | <span data-ttu-id="e9fc8-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9fc8-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9fc8-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9fc8-128">Authorization</span></span>  | <span data-ttu-id="e9fc8-129">string</span><span class="sxs-lookup"><span data-stu-id="e9fc8-129">string</span></span>  | <span data-ttu-id="e9fc8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9fc8-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9fc8-132">Content-Type</span></span> | <span data-ttu-id="e9fc8-133">string</span><span class="sxs-lookup"><span data-stu-id="e9fc8-133">string</span></span>  | <span data-ttu-id="e9fc8-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9fc8-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fc8-136">Request body</span></span>
<span data-ttu-id="e9fc8-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9fc8-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e9fc8-138">Parameter</span></span>    | <span data-ttu-id="e9fc8-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9fc8-139">Type</span></span>   |<span data-ttu-id="e9fc8-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9fc8-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9fc8-141">comment</span><span class="sxs-lookup"><span data-stu-id="e9fc8-141">comment</span></span>|<span data-ttu-id="e9fc8-142">String</span><span class="sxs-lookup"><span data-stu-id="e9fc8-142">String</span></span>|<span data-ttu-id="e9fc8-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="e9fc8-145">message</span><span class="sxs-lookup"><span data-stu-id="e9fc8-145">message</span></span>|[<span data-ttu-id="e9fc8-146">message</span><span class="sxs-lookup"><span data-stu-id="e9fc8-146">message</span></span>](../resources/message.md)|<span data-ttu-id="e9fc8-147">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="e9fc8-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9fc8-148">Response</span></span>

<span data-ttu-id="e9fc8-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9fc8-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9fc8-151">Example</span></span>
<span data-ttu-id="e9fc8-152">O exemplo a seguir inclui um comentário e adiciona um destinatário à mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-152">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="e9fc8-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fc8-153">Request</span></span>
<span data-ttu-id="e9fc8-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9fc8-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9fc8-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_reply_beta",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}
```
# <a name="c"></a>[<span data-ttu-id="e9fc8-156">C#</span><span class="sxs-lookup"><span data-stu-id="e9fc8-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9fc8-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9fc8-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9fc8-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9fc8-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9fc8-159">Java</span><span class="sxs-lookup"><span data-stu-id="e9fc8-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e9fc8-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9fc8-160">Response</span></span>
<span data-ttu-id="e9fc8-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fc8-161">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


