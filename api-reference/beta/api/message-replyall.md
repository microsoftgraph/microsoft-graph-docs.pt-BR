---
title: 'message: replyAll'
description: 'Responder a todos os destinatários de uma mensagem especificando um comentário e modificando qualquer propriedade atualizável '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 49065615cc34d6f6d09c863aac213344ef743968
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456885"
---
# <a name="message-replyall"></a><span data-ttu-id="d1154-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="d1154-103">message: replyAll</span></span>

<span data-ttu-id="d1154-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d1154-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1154-105">Responda a todos os destinatários de uma mensagem especificando um comentário e modificando as propriedades atualizáveis da resposta, tudo usando o método **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="d1154-105">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="d1154-106">A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="d1154-106">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="d1154-107">Como alternativa, você pode primeiro [criar um rascunho de mensagem de resposta](../api/message-createreplyall.md) para incluir um comentário ou atualizar quaisquer propriedades de mensagem e, em seguida, [Enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1154-107">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="d1154-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="d1154-108">**Note**</span></span>

- <span data-ttu-id="d1154-109">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d1154-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="d1154-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="d1154-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="d1154-111">Se a propriedade **ReplyTo** for especificada na mensagem original, por formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários no</span><span class="sxs-lookup"><span data-stu-id="d1154-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="d1154-112">as propriedades **ReplyTo** e **ToRecipients** e não os destinatários nas propriedades **from** e **ToRecipients** .</span><span class="sxs-lookup"><span data-stu-id="d1154-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d1154-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1154-113">Permissions</span></span>
<span data-ttu-id="d1154-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1154-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1154-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1154-116">Permission type</span></span>      | <span data-ttu-id="d1154-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1154-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1154-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1154-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d1154-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1154-119">Mail.Send</span></span>    |
|<span data-ttu-id="d1154-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1154-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1154-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1154-121">Mail.Send</span></span>    |
|<span data-ttu-id="d1154-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1154-122">Application</span></span> | <span data-ttu-id="d1154-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d1154-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1154-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1154-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="d1154-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1154-125">Request headers</span></span>
| <span data-ttu-id="d1154-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d1154-126">Name</span></span>       | <span data-ttu-id="d1154-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1154-127">Type</span></span> | <span data-ttu-id="d1154-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1154-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d1154-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1154-129">Authorization</span></span>  | <span data-ttu-id="d1154-130">string</span><span class="sxs-lookup"><span data-stu-id="d1154-130">string</span></span>  | <span data-ttu-id="d1154-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1154-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1154-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1154-133">Content-Type</span></span> | <span data-ttu-id="d1154-134">string</span><span class="sxs-lookup"><span data-stu-id="d1154-134">string</span></span>  | <span data-ttu-id="d1154-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1154-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1154-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1154-137">Request body</span></span>
<span data-ttu-id="d1154-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1154-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1154-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d1154-139">Parameter</span></span>    | <span data-ttu-id="d1154-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1154-140">Type</span></span>   |<span data-ttu-id="d1154-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1154-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1154-142">comment</span><span class="sxs-lookup"><span data-stu-id="d1154-142">comment</span></span>|<span data-ttu-id="d1154-143">String</span><span class="sxs-lookup"><span data-stu-id="d1154-143">String</span></span>|<span data-ttu-id="d1154-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="d1154-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="d1154-146">message</span><span class="sxs-lookup"><span data-stu-id="d1154-146">message</span></span>|[<span data-ttu-id="d1154-147">message</span><span class="sxs-lookup"><span data-stu-id="d1154-147">message</span></span>](../resources/message.md)|<span data-ttu-id="d1154-148">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1154-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="d1154-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1154-149">Response</span></span>

<span data-ttu-id="d1154-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1154-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1154-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1154-152">Example</span></span>
<span data-ttu-id="d1154-153">O exemplo a seguir inclui um comentário e adiciona um anexo à mensagem de resposta a todos.</span><span class="sxs-lookup"><span data-stu-id="d1154-153">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="d1154-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1154-154">Request</span></span>
<span data-ttu-id="d1154-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1154-155">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1154-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1154-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="d1154-157">C#</span><span class="sxs-lookup"><span data-stu-id="d1154-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1154-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1154-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1154-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1154-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="d1154-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1154-160">Response</span></span>
<span data-ttu-id="d1154-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1154-161">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
