---
title: 'message: replyAll'
description: 'Responder a todos os destinatários de uma mensagem especificando um comentário e modificando qualquer propriedade atualizável '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b49e4ac2b2d88ac7d5841f3adb39c5ce6efafba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342814"
---
# <a name="message-replyall"></a><span data-ttu-id="18de9-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="18de9-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18de9-104">Responda a todos os destinatários de uma mensagem especificando um comentário e modificando as propriedades atualizáveis da resposta, tudo usando o método **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="18de9-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="18de9-105">A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="18de9-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="18de9-106">Como alternativa, você pode primeiro [criar um rascunho de mensagem de resposta](../api/message-createreplyall.md) para incluir um comentário ou atualizar quaisquer propriedades de mensagem e, em seguida, [Enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="18de9-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="18de9-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="18de9-107">**Note**</span></span>

- <span data-ttu-id="18de9-108">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="18de9-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="18de9-109">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="18de9-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="18de9-110">Se a \*\*\*\* Propriedade ReplyTo for especificada na mensagem original, por formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários no</span><span class="sxs-lookup"><span data-stu-id="18de9-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="18de9-111">\*\*\*\* as propriedades ReplyTo e ToRecipients e não os destinatários nas propriedades **from** e \*\*\*\* ToRecipients. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="18de9-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="18de9-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="18de9-112">Permissions</span></span>
<span data-ttu-id="18de9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18de9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18de9-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18de9-115">Permission type</span></span>      | <span data-ttu-id="18de9-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18de9-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18de9-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18de9-117">Delegated (work or school account)</span></span> | <span data-ttu-id="18de9-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="18de9-118">Mail.Send</span></span>    |
|<span data-ttu-id="18de9-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18de9-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18de9-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="18de9-120">Mail.Send</span></span>    |
|<span data-ttu-id="18de9-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18de9-121">Application</span></span> | <span data-ttu-id="18de9-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="18de9-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="18de9-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18de9-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="18de9-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18de9-124">Request headers</span></span>
| <span data-ttu-id="18de9-125">Nome</span><span class="sxs-lookup"><span data-stu-id="18de9-125">Name</span></span>       | <span data-ttu-id="18de9-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="18de9-126">Type</span></span> | <span data-ttu-id="18de9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="18de9-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18de9-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="18de9-128">Authorization</span></span>  | <span data-ttu-id="18de9-129">string</span><span class="sxs-lookup"><span data-stu-id="18de9-129">string</span></span>  | <span data-ttu-id="18de9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18de9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18de9-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18de9-132">Content-Type</span></span> | <span data-ttu-id="18de9-133">string</span><span class="sxs-lookup"><span data-stu-id="18de9-133">string</span></span>  | <span data-ttu-id="18de9-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18de9-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18de9-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18de9-136">Request body</span></span>
<span data-ttu-id="18de9-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18de9-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18de9-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="18de9-138">Parameter</span></span>    | <span data-ttu-id="18de9-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="18de9-139">Type</span></span>   |<span data-ttu-id="18de9-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="18de9-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18de9-141">comment</span><span class="sxs-lookup"><span data-stu-id="18de9-141">comment</span></span>|<span data-ttu-id="18de9-142">String</span><span class="sxs-lookup"><span data-stu-id="18de9-142">String</span></span>|<span data-ttu-id="18de9-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="18de9-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="18de9-145">message</span><span class="sxs-lookup"><span data-stu-id="18de9-145">message</span></span>|[<span data-ttu-id="18de9-146">message</span><span class="sxs-lookup"><span data-stu-id="18de9-146">message</span></span>](../resources/message.md)|<span data-ttu-id="18de9-147">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="18de9-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="18de9-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="18de9-148">Response</span></span>

<span data-ttu-id="18de9-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18de9-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18de9-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18de9-151">Example</span></span>
<span data-ttu-id="18de9-152">O exemplo a seguir inclui um comentário e adiciona um anexo à mensagem de resposta a todos.</span><span class="sxs-lookup"><span data-stu-id="18de9-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="18de9-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18de9-153">Request</span></span>
<span data-ttu-id="18de9-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18de9-154">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18de9-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="18de9-155">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="18de9-156">C#</span><span class="sxs-lookup"><span data-stu-id="18de9-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18de9-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18de9-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18de9-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="18de9-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="18de9-159">Java</span><span class="sxs-lookup"><span data-stu-id="18de9-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="18de9-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="18de9-160">Response</span></span>
<span data-ttu-id="18de9-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18de9-161">Here is an example of the response.</span></span>
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
