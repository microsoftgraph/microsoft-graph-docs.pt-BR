---
title: 'message: createReplyAll'
description: 'Criar um rascunho de uma mensagem de responder a todos para incluir um comentário ou atualizar as propriedades de mensagem, '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7f0b2631f02a94a7627e96e24308b135d70d20e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922168"
---
# <a name="message-createreplyall"></a><span data-ttu-id="46454-103">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="46454-103">message: createReplyAll</span></span>

> <span data-ttu-id="46454-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46454-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46454-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46454-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46454-106">Crie um rascunho de uma mensagem de responder a todos para incluir um comentário ou atualizar as propriedades de mensagem, todas em uma chamada de **createReplyAll** .</span><span class="sxs-lookup"><span data-stu-id="46454-106">Create a draft of a reply-all message to include a comment or update any message properties, all in one **createReplyAll** call.</span></span> <span data-ttu-id="46454-107">Em seguida, você pode [Atualizar](../api/message-update.md) ou [Enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="46454-107">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="46454-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="46454-108">**Note**</span></span>

- <span data-ttu-id="46454-109">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="46454-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="46454-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="46454-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="46454-111">Se a propriedade **replyTo** for especificada na mensagem original, por um formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários no</span><span class="sxs-lookup"><span data-stu-id="46454-111">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="46454-112">propriedades **replyTo** e **toRecipients** e não os destinatários nas propriedades **do** e **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="46454-112">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="46454-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="46454-113">Permissions</span></span>
<span data-ttu-id="46454-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46454-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46454-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46454-116">Permission type</span></span>      | <span data-ttu-id="46454-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46454-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46454-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46454-118">Delegated (work or school account)</span></span> | <span data-ttu-id="46454-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46454-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="46454-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46454-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46454-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46454-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="46454-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46454-122">Application</span></span> | <span data-ttu-id="46454-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46454-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="46454-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46454-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="46454-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46454-125">Request headers</span></span>
| <span data-ttu-id="46454-126">Nome</span><span class="sxs-lookup"><span data-stu-id="46454-126">Name</span></span>       | <span data-ttu-id="46454-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="46454-127">Type</span></span> | <span data-ttu-id="46454-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="46454-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46454-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="46454-129">Authorization</span></span>  | <span data-ttu-id="46454-130">string</span><span class="sxs-lookup"><span data-stu-id="46454-130">string</span></span>  | <span data-ttu-id="46454-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46454-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46454-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46454-133">Content-Type</span></span> | <span data-ttu-id="46454-134">string</span><span class="sxs-lookup"><span data-stu-id="46454-134">string</span></span>  | <span data-ttu-id="46454-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46454-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46454-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46454-137">Request body</span></span>
<span data-ttu-id="46454-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46454-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46454-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46454-139">Parameter</span></span>    | <span data-ttu-id="46454-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="46454-140">Type</span></span>   |<span data-ttu-id="46454-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="46454-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46454-142">comment</span><span class="sxs-lookup"><span data-stu-id="46454-142">comment</span></span>|<span data-ttu-id="46454-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46454-143">String</span></span>|<span data-ttu-id="46454-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="46454-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="46454-146">message</span><span class="sxs-lookup"><span data-stu-id="46454-146">message</span></span>|[<span data-ttu-id="46454-147">message</span><span class="sxs-lookup"><span data-stu-id="46454-147">message</span></span>](../resources/message.md)|<span data-ttu-id="46454-148">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta a todos.</span><span class="sxs-lookup"><span data-stu-id="46454-148">Any writeable properties to update in the reply-all message.</span></span>|

## <a name="response"></a><span data-ttu-id="46454-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="46454-149">Response</span></span>

<span data-ttu-id="46454-150">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46454-150">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46454-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46454-151">Example</span></span>
<span data-ttu-id="46454-152">O exemplo a seguir cria um rascunho para responder a todos e adiciona um anexo e o comentário todas em **createReplyAll** de uma chamada.</span><span class="sxs-lookup"><span data-stu-id="46454-152">The following example creates a draft to reply all, and adds an attachment and comment all in one **createReplyAll** call.</span></span>
##### <a name="request"></a><span data-ttu-id="46454-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46454-153">Request</span></span>
<span data-ttu-id="46454-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46454-154">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="46454-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="46454-155">Response</span></span>
<span data-ttu-id="46454-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46454-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
