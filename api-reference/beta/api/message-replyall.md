---
title: 'message: replyAll'
description: 'Responder a todos os destinatários de uma mensagem especificando um comentário e modificando quaisquer propriedades atualizáveis '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5c2651d56b65d73548f30cc442f1a66500d5e956
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131135"
---
# <a name="message-replyall"></a><span data-ttu-id="c7365-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="c7365-103">message: replyAll</span></span>

<span data-ttu-id="c7365-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7365-105">Responda a todos os destinatários de uma mensagem especificando um comentário e modificando quaisquer propriedades atualizáveis para a resposta, tudo isso usando o **método replyAll.**</span><span class="sxs-lookup"><span data-stu-id="c7365-105">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="c7365-106">A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="c7365-106">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="c7365-107">Como alternativa, você pode primeiro [criar um rascunho](../api/message-createreplyall.md) de mensagem de resposta a todos para incluir um comentário ou atualizar as propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7365-107">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="c7365-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="c7365-108">**Note**</span></span>

- <span data-ttu-id="c7365-109">Você pode especificar um comentário ou a **propriedade do** corpo do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c7365-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="c7365-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="c7365-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="c7365-111">Se a **propriedade replyTo** for especificada na mensagem original, por Formato de Mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários no</span><span class="sxs-lookup"><span data-stu-id="c7365-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="c7365-112">**Propriedades replyTo** **e toRecipients,** e não os destinatários nas propriedades **from** **e toRecipients.**</span><span class="sxs-lookup"><span data-stu-id="c7365-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="c7365-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7365-113">Permissions</span></span>
<span data-ttu-id="c7365-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7365-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7365-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7365-116">Permission type</span></span>      | <span data-ttu-id="c7365-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7365-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7365-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7365-118">Delegated (work or school account)</span></span> | <span data-ttu-id="c7365-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c7365-119">Mail.Send</span></span>    |
|<span data-ttu-id="c7365-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7365-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7365-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c7365-121">Mail.Send</span></span>    |
|<span data-ttu-id="c7365-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7365-122">Application</span></span> | <span data-ttu-id="c7365-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c7365-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7365-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7365-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="c7365-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7365-125">Request headers</span></span>
| <span data-ttu-id="c7365-126">Nome</span><span class="sxs-lookup"><span data-stu-id="c7365-126">Name</span></span>       | <span data-ttu-id="c7365-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7365-127">Type</span></span> | <span data-ttu-id="c7365-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7365-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c7365-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7365-129">Authorization</span></span>  | <span data-ttu-id="c7365-130">string</span><span class="sxs-lookup"><span data-stu-id="c7365-130">string</span></span>  | <span data-ttu-id="c7365-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7365-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7365-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7365-133">Content-Type</span></span> | <span data-ttu-id="c7365-134">string</span><span class="sxs-lookup"><span data-stu-id="c7365-134">string</span></span>  | <span data-ttu-id="c7365-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7365-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7365-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7365-137">Request body</span></span>
<span data-ttu-id="c7365-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7365-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c7365-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c7365-139">Parameter</span></span>    | <span data-ttu-id="c7365-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7365-140">Type</span></span>   |<span data-ttu-id="c7365-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7365-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7365-142">comment</span><span class="sxs-lookup"><span data-stu-id="c7365-142">comment</span></span>|<span data-ttu-id="c7365-143">String</span><span class="sxs-lookup"><span data-stu-id="c7365-143">String</span></span>|<span data-ttu-id="c7365-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="c7365-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="c7365-146">message</span><span class="sxs-lookup"><span data-stu-id="c7365-146">message</span></span>|[<span data-ttu-id="c7365-147">message</span><span class="sxs-lookup"><span data-stu-id="c7365-147">message</span></span>](../resources/message.md)|<span data-ttu-id="c7365-148">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7365-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="c7365-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7365-149">Response</span></span>

<span data-ttu-id="c7365-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7365-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7365-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7365-152">Example</span></span>
<span data-ttu-id="c7365-153">O exemplo a seguir inclui um comentário e adiciona um anexo à mensagem de resposta a todos.</span><span class="sxs-lookup"><span data-stu-id="c7365-153">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="c7365-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7365-154">Request</span></span>
<span data-ttu-id="c7365-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7365-155">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7365-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7365-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c7365-157">C#</span><span class="sxs-lookup"><span data-stu-id="c7365-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7365-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7365-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7365-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7365-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7365-160">Java</span><span class="sxs-lookup"><span data-stu-id="c7365-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="c7365-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7365-161">Response</span></span>
<span data-ttu-id="c7365-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7365-162">Here is an example of the response.</span></span>
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


