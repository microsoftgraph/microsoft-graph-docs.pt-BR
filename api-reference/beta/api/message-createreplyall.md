---
title: 'message: createReplyAll'
description: 'Crie um rascunho de uma mensagem de resposta-tudo para incluir um comentário ou atualizar quaisquer propriedades de mensagem, '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ac0e9047933d51773601d64aff8970758f36a171
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052156"
---
# <a name="message-createreplyall"></a><span data-ttu-id="848dc-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="848dc-103">message: createReplyAll</span></span>

<span data-ttu-id="848dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="848dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="848dc-105">Crie uma mensagem para responder a todos de rascunho para incluir um comentário ou atualizar todas as propriedades da mensagem em uma chamada **createReplyAll**.</span><span class="sxs-lookup"><span data-stu-id="848dc-105">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call.</span></span> <span data-ttu-id="848dc-106">Em seguida, você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) esse rascunho.</span><span class="sxs-lookup"><span data-stu-id="848dc-106">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="848dc-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="848dc-107">**Note**</span></span>

- <span data-ttu-id="848dc-108">Você pode especificar um comentário ou a **propriedade body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="848dc-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="848dc-109">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="848dc-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="848dc-110">Se a **propriedade replyTo** for especificada na mensagem original, por Formato de Mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deverá enviar a resposta aos destinatários no</span><span class="sxs-lookup"><span data-stu-id="848dc-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="848dc-111">**propriedades replyTo** **e toRecipients,** e não os destinatários nas propriedades **from** **e toRecipients.**</span><span class="sxs-lookup"><span data-stu-id="848dc-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="848dc-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="848dc-112">Permissions</span></span>
<span data-ttu-id="848dc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="848dc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="848dc-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="848dc-115">Permission type</span></span>      | <span data-ttu-id="848dc-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="848dc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="848dc-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="848dc-117">Delegated (work or school account)</span></span> | <span data-ttu-id="848dc-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="848dc-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="848dc-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="848dc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="848dc-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="848dc-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="848dc-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="848dc-121">Application</span></span> | <span data-ttu-id="848dc-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="848dc-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="848dc-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="848dc-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="848dc-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="848dc-124">Request headers</span></span>
| <span data-ttu-id="848dc-125">Nome</span><span class="sxs-lookup"><span data-stu-id="848dc-125">Name</span></span>       | <span data-ttu-id="848dc-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="848dc-126">Type</span></span> | <span data-ttu-id="848dc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="848dc-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="848dc-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="848dc-128">Authorization</span></span>  | <span data-ttu-id="848dc-129">string</span><span class="sxs-lookup"><span data-stu-id="848dc-129">string</span></span>  | <span data-ttu-id="848dc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="848dc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="848dc-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="848dc-132">Content-Type</span></span> | <span data-ttu-id="848dc-133">string</span><span class="sxs-lookup"><span data-stu-id="848dc-133">string</span></span>  | <span data-ttu-id="848dc-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="848dc-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="848dc-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="848dc-136">Request body</span></span>
<span data-ttu-id="848dc-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="848dc-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="848dc-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="848dc-138">Parameter</span></span>    | <span data-ttu-id="848dc-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="848dc-139">Type</span></span>   |<span data-ttu-id="848dc-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="848dc-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="848dc-141">comment</span><span class="sxs-lookup"><span data-stu-id="848dc-141">comment</span></span>|<span data-ttu-id="848dc-142">String</span><span class="sxs-lookup"><span data-stu-id="848dc-142">String</span></span>|<span data-ttu-id="848dc-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="848dc-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="848dc-145">message</span><span class="sxs-lookup"><span data-stu-id="848dc-145">message</span></span>|[<span data-ttu-id="848dc-146">message</span><span class="sxs-lookup"><span data-stu-id="848dc-146">message</span></span>](../resources/message.md)|<span data-ttu-id="848dc-147">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta a todos.</span><span class="sxs-lookup"><span data-stu-id="848dc-147">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="848dc-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="848dc-148">Response</span></span>

<span data-ttu-id="848dc-149">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="848dc-149">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="848dc-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="848dc-150">Example</span></span>
<span data-ttu-id="848dc-151">O exemplo a seguir cria um rascunho para responder a todos e adiciona um anexo e um comentário em **uma chamada createReplyAll.**</span><span class="sxs-lookup"><span data-stu-id="848dc-151">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="848dc-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="848dc-152">Request</span></span>
<span data-ttu-id="848dc-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="848dc-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="848dc-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="848dc-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll
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
    "comment": "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[<span data-ttu-id="848dc-155">C#</span><span class="sxs-lookup"><span data-stu-id="848dc-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="848dc-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="848dc-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="848dc-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="848dc-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="848dc-158">Java</span><span class="sxs-lookup"><span data-stu-id="848dc-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="848dc-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="848dc-159">Response</span></span>
<span data-ttu-id="848dc-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="848dc-160">Here is an example of the response.</span></span> <span data-ttu-id="848dc-161">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="848dc-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKpAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DP\"",
  "id": "AAMkADA1MTAAAH5JKpAAA=",
  "subject": "RE: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body dir=\"ltr\">\r\nif the project gets approved, please take a look at the attached guidelines before you decide on the name.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:36:32 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group\r\n<div>Samantha, Randi, would you name the group please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n</body>\r\n</html>"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress": {
        "name": "Randi Welch",
        "address": "randiw@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


