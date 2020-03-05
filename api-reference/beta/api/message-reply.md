---
title: 'message: reply'
description: 'Responda ao remetente de uma mensagem, adicione um comentário ou modifique todas as propriedades atualizáveis em uma única chamada **reply**. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4beb56d4ea37c4dd8e71418d491fafd7f54b69a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456884"
---
# <a name="message-reply"></a><span data-ttu-id="dd1be-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="dd1be-103">message: reply</span></span>

<span data-ttu-id="dd1be-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd1be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd1be-105">Responda ao remetente de uma mensagem, adicione um comentário ou modifique todas as propriedades atualizáveis em uma única chamada **reply**.</span><span class="sxs-lookup"><span data-stu-id="dd1be-105">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="dd1be-106">A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="dd1be-106">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="dd1be-107">Outra opção é primeiro [criar um rascunho de mensagem de resposta](../api/message-createreply.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="dd1be-107">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="dd1be-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="dd1be-108">**Note**</span></span>

- <span data-ttu-id="dd1be-109">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="dd1be-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="dd1be-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="dd1be-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="dd1be-111">Se a propriedade **ReplyTo** for especificada na mensagem original, por formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários em **ReplyTo** e não ao destinatário na propriedade **from** .</span><span class="sxs-lookup"><span data-stu-id="dd1be-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="dd1be-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd1be-112">Permissions</span></span>
<span data-ttu-id="dd1be-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd1be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd1be-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd1be-115">Permission type</span></span>      | <span data-ttu-id="dd1be-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd1be-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd1be-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd1be-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dd1be-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dd1be-118">Mail.Send</span></span>    |
|<span data-ttu-id="dd1be-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd1be-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd1be-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dd1be-120">Mail.Send</span></span>    |
|<span data-ttu-id="dd1be-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd1be-121">Application</span></span> | <span data-ttu-id="dd1be-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="dd1be-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd1be-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd1be-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="dd1be-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd1be-124">Request headers</span></span>
| <span data-ttu-id="dd1be-125">Nome</span><span class="sxs-lookup"><span data-stu-id="dd1be-125">Name</span></span>       | <span data-ttu-id="dd1be-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd1be-126">Type</span></span> | <span data-ttu-id="dd1be-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd1be-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd1be-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd1be-128">Authorization</span></span>  | <span data-ttu-id="dd1be-129">string</span><span class="sxs-lookup"><span data-stu-id="dd1be-129">string</span></span>  | <span data-ttu-id="dd1be-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd1be-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd1be-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd1be-132">Content-Type</span></span> | <span data-ttu-id="dd1be-133">string</span><span class="sxs-lookup"><span data-stu-id="dd1be-133">string</span></span>  | <span data-ttu-id="dd1be-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd1be-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd1be-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd1be-136">Request body</span></span>
<span data-ttu-id="dd1be-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd1be-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd1be-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dd1be-138">Parameter</span></span>    | <span data-ttu-id="dd1be-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd1be-139">Type</span></span>   |<span data-ttu-id="dd1be-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd1be-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd1be-141">comment</span><span class="sxs-lookup"><span data-stu-id="dd1be-141">comment</span></span>|<span data-ttu-id="dd1be-142">String</span><span class="sxs-lookup"><span data-stu-id="dd1be-142">String</span></span>|<span data-ttu-id="dd1be-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="dd1be-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="dd1be-145">message</span><span class="sxs-lookup"><span data-stu-id="dd1be-145">message</span></span>|[<span data-ttu-id="dd1be-146">message</span><span class="sxs-lookup"><span data-stu-id="dd1be-146">message</span></span>](../resources/message.md)|<span data-ttu-id="dd1be-147">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd1be-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="dd1be-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd1be-148">Response</span></span>

<span data-ttu-id="dd1be-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd1be-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd1be-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd1be-151">Example</span></span>
<span data-ttu-id="dd1be-152">O exemplo a seguir inclui um comentário e adiciona um destinatário à mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd1be-152">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="dd1be-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd1be-153">Request</span></span>
<span data-ttu-id="dd1be-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd1be-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd1be-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd1be-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dd1be-156">C#</span><span class="sxs-lookup"><span data-stu-id="dd1be-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd1be-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd1be-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd1be-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd1be-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd1be-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd1be-159">Response</span></span>
<span data-ttu-id="dd1be-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd1be-160">Here is an example of the response.</span></span>
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
