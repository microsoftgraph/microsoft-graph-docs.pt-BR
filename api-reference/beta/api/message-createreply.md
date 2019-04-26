---
title: 'message: createReply'
description: 'Criar um rascunho de uma mensagem de resposta para incluir um comentário ou atualizar quaisquer propriedades de mensagem '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0705e4cfdb8b5e7a1aee90dece01f351f840c4c1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338597"
---
# <a name="message-createreply"></a><span data-ttu-id="ccd2a-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="ccd2a-103">message: createReply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccd2a-104">Crie uma mensagem de resposta de rascunho para incluir um comentário ou atualizar todas as propriedades da mensagem em uma chamada **createReply**.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-104">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call.</span></span> <span data-ttu-id="ccd2a-105">Em seguida, você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) esse rascunho.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-105">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="ccd2a-106">**Observação**</span><span class="sxs-lookup"><span data-stu-id="ccd2a-106">**Note**</span></span>

- <span data-ttu-id="ccd2a-107">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-107">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="ccd2a-108">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-108">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="ccd2a-109">Se **ReplyTo** for especificado na mensagem original, por formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários em **ReplyTo**, e não aos destinatários **de from**.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-109">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ccd2a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccd2a-110">Permissions</span></span>
<span data-ttu-id="ccd2a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd2a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd2a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccd2a-113">Permission type</span></span>      | <span data-ttu-id="ccd2a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccd2a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccd2a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccd2a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ccd2a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd2a-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ccd2a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccd2a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccd2a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd2a-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ccd2a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccd2a-119">Application</span></span> | <span data-ttu-id="ccd2a-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd2a-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccd2a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd2a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="ccd2a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd2a-122">Request headers</span></span>
| <span data-ttu-id="ccd2a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ccd2a-123">Name</span></span>       | <span data-ttu-id="ccd2a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccd2a-124">Type</span></span> | <span data-ttu-id="ccd2a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccd2a-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ccd2a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccd2a-126">Authorization</span></span>  | <span data-ttu-id="ccd2a-127">string</span><span class="sxs-lookup"><span data-stu-id="ccd2a-127">string</span></span>  | <span data-ttu-id="ccd2a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccd2a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccd2a-130">Content-Type</span></span> | <span data-ttu-id="ccd2a-131">string</span><span class="sxs-lookup"><span data-stu-id="ccd2a-131">string</span></span>  | <span data-ttu-id="ccd2a-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccd2a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd2a-134">Request body</span></span>
<span data-ttu-id="ccd2a-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ccd2a-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ccd2a-136">Parameter</span></span>    | <span data-ttu-id="ccd2a-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccd2a-137">Type</span></span>   |<span data-ttu-id="ccd2a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccd2a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccd2a-139">comment</span><span class="sxs-lookup"><span data-stu-id="ccd2a-139">comment</span></span>|<span data-ttu-id="ccd2a-140">String</span><span class="sxs-lookup"><span data-stu-id="ccd2a-140">String</span></span>|<span data-ttu-id="ccd2a-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ccd2a-143">mensagem</span><span class="sxs-lookup"><span data-stu-id="ccd2a-143">message</span></span>|[<span data-ttu-id="ccd2a-144">message</span><span class="sxs-lookup"><span data-stu-id="ccd2a-144">message</span></span>](../resources/message.md)|<span data-ttu-id="ccd2a-145">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-145">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="ccd2a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd2a-146">Response</span></span>

<span data-ttu-id="ccd2a-147">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-147">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd2a-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccd2a-148">Example</span></span>
<span data-ttu-id="ccd2a-149">O exemplo a seguir cria um rascunho de resposta, adiciona um comentário e um destinatário no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-149">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="ccd2a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd2a-150">Request</span></span>
<span data-ttu-id="ccd2a-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
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
  "comment": "Samantha, Randi, would you name the group if the project is approved, please?" 
}
```

##### <a name="response"></a><span data-ttu-id="ccd2a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd2a-152">Response</span></span>
<span data-ttu-id="ccd2a-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccd2a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKoAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DO\"",
  "id": "AAMkADA1MTAAAH5JKoAAA=",
  "subject": "RE: Let's start a group",
  "Body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>Samantha, Randi, would you name the group if the project is approved, please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n<p>That's a great idea!<br>\r\n</body>\r\n</html>"
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
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
