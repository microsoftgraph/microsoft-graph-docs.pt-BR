---
title: 'message: createReply'
description: 'Criar um rascunho de uma mensagem de resposta para incluir um comentário ou atualizar as propriedades de mensagem '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 27e6aabe05cb732cd40242f3c17c822c920c062e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943736"
---
# <a name="message-createreply"></a><span data-ttu-id="b3db7-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="b3db7-103">message: createReply</span></span>

> <span data-ttu-id="b3db7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b3db7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3db7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b3db7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3db7-106">Crie um rascunho de uma mensagem de resposta para incluir um comentário ou atualizar as propriedades de mensagem todas em uma chamada de **createReply** .</span><span class="sxs-lookup"><span data-stu-id="b3db7-106">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call.</span></span> <span data-ttu-id="b3db7-107">Em seguida, você pode [Atualizar](../api/message-update.md) ou [Enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="b3db7-107">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="b3db7-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="b3db7-108">**Note**</span></span>

- <span data-ttu-id="b3db7-109">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b3db7-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="b3db7-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="b3db7-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="b3db7-111">Se **replyTo** for especificado na mensagem original, por um formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta para os destinatários na **replyTo**e não os destinatários **de**.</span><span class="sxs-lookup"><span data-stu-id="b3db7-111">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b3db7-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="b3db7-112">Permissions</span></span>
<span data-ttu-id="b3db7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3db7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3db7-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3db7-115">Permission type</span></span>      | <span data-ttu-id="b3db7-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3db7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3db7-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3db7-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b3db7-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3db7-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b3db7-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3db7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3db7-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3db7-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b3db7-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3db7-121">Application</span></span> | <span data-ttu-id="b3db7-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3db7-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3db7-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3db7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="b3db7-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3db7-124">Request headers</span></span>
| <span data-ttu-id="b3db7-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b3db7-125">Name</span></span>       | <span data-ttu-id="b3db7-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3db7-126">Type</span></span> | <span data-ttu-id="b3db7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3db7-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3db7-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3db7-128">Authorization</span></span>  | <span data-ttu-id="b3db7-129">string</span><span class="sxs-lookup"><span data-stu-id="b3db7-129">string</span></span>  | <span data-ttu-id="b3db7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3db7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3db7-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3db7-132">Content-Type</span></span> | <span data-ttu-id="b3db7-133">string</span><span class="sxs-lookup"><span data-stu-id="b3db7-133">string</span></span>  | <span data-ttu-id="b3db7-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3db7-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3db7-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3db7-136">Request body</span></span>
<span data-ttu-id="b3db7-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3db7-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3db7-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b3db7-138">Parameter</span></span>    | <span data-ttu-id="b3db7-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3db7-139">Type</span></span>   |<span data-ttu-id="b3db7-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3db7-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3db7-141">comment</span><span class="sxs-lookup"><span data-stu-id="b3db7-141">comment</span></span>|<span data-ttu-id="b3db7-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3db7-142">String</span></span>|<span data-ttu-id="b3db7-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="b3db7-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="b3db7-145">message</span><span class="sxs-lookup"><span data-stu-id="b3db7-145">message</span></span>|[<span data-ttu-id="b3db7-146">message</span><span class="sxs-lookup"><span data-stu-id="b3db7-146">message</span></span>](../resources/message.md)|<span data-ttu-id="b3db7-147">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3db7-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="b3db7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3db7-148">Response</span></span>

<span data-ttu-id="b3db7-149">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3db7-149">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3db7-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3db7-150">Example</span></span>
<span data-ttu-id="b3db7-151">O exemplo a seguir cria um rascunho de resposta, adiciona um comentário e um destinatário no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3db7-151">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="b3db7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3db7-152">Request</span></span>
<span data-ttu-id="b3db7-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3db7-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b3db7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3db7-154">Response</span></span>
<span data-ttu-id="b3db7-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3db7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
