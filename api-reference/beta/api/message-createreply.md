---
title: 'message: createReply'
description: 'Criar um rascunho de uma mensagem de resposta para incluir um comentário ou atualizar as propriedades da mensagem '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d2943f5a822ce02c3fc4c8fd1e6ae34e6d6f7b98
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134726"
---
# <a name="message-createreply"></a><span data-ttu-id="4d846-103">message: createReply</span><span class="sxs-lookup"><span data-stu-id="4d846-103">message: createReply</span></span>

<span data-ttu-id="4d846-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d846-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d846-105">Crie uma mensagem de resposta de rascunho para incluir um comentário ou atualizar todas as propriedades da mensagem em uma chamada **createReply**.</span><span class="sxs-lookup"><span data-stu-id="4d846-105">Create a draft of a reply message to include a comment or update any message properties all in one **createReply** call.</span></span> <span data-ttu-id="4d846-106">Em seguida, você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) esse rascunho.</span><span class="sxs-lookup"><span data-stu-id="4d846-106">You can then [update](../api/message-update.md) or [send](../api/message-send.md) the draft.</span></span>

<span data-ttu-id="4d846-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="4d846-107">**Note**</span></span>

- <span data-ttu-id="4d846-108">Você pode especificar um comentário ou a **propriedade do** corpo do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4d846-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="4d846-109">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="4d846-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="4d846-110">Se **replyTo** for especificado na mensagem original, por Formato de Mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta para os destinatários em **replyTo**, e não os destinatários de **.**</span><span class="sxs-lookup"><span data-stu-id="4d846-110">If **replyTo** is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo**, and not the recipients in **from**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4d846-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d846-111">Permissions</span></span>
<span data-ttu-id="4d846-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d846-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d846-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d846-114">Permission type</span></span>      | <span data-ttu-id="4d846-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d846-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d846-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d846-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4d846-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d846-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4d846-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d846-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d846-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d846-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4d846-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d846-120">Application</span></span> | <span data-ttu-id="4d846-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d846-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d846-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d846-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="4d846-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d846-123">Request headers</span></span>
| <span data-ttu-id="4d846-124">Nome</span><span class="sxs-lookup"><span data-stu-id="4d846-124">Name</span></span>       | <span data-ttu-id="4d846-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d846-125">Type</span></span> | <span data-ttu-id="4d846-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d846-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d846-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d846-127">Authorization</span></span>  | <span data-ttu-id="4d846-128">string</span><span class="sxs-lookup"><span data-stu-id="4d846-128">string</span></span>  | <span data-ttu-id="4d846-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d846-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d846-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d846-131">Content-Type</span></span> | <span data-ttu-id="4d846-132">string</span><span class="sxs-lookup"><span data-stu-id="4d846-132">string</span></span>  | <span data-ttu-id="4d846-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d846-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d846-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d846-135">Request body</span></span>
<span data-ttu-id="4d846-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d846-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d846-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4d846-137">Parameter</span></span>    | <span data-ttu-id="4d846-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d846-138">Type</span></span>   |<span data-ttu-id="4d846-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d846-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d846-140">comment</span><span class="sxs-lookup"><span data-stu-id="4d846-140">comment</span></span>|<span data-ttu-id="4d846-141">String</span><span class="sxs-lookup"><span data-stu-id="4d846-141">String</span></span>|<span data-ttu-id="4d846-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="4d846-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="4d846-144">message</span><span class="sxs-lookup"><span data-stu-id="4d846-144">message</span></span>|[<span data-ttu-id="4d846-145">message</span><span class="sxs-lookup"><span data-stu-id="4d846-145">message</span></span>](../resources/message.md)|<span data-ttu-id="4d846-146">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d846-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="4d846-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d846-147">Response</span></span>

<span data-ttu-id="4d846-148">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d846-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d846-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d846-149">Example</span></span>
<span data-ttu-id="4d846-150">O exemplo a seguir cria um rascunho de resposta, adiciona um comentário e um destinatário no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d846-150">The following example creates a reply draft, adds a comment and a recipient in the request body.</span></span>
##### <a name="request"></a><span data-ttu-id="4d846-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d846-151">Request</span></span>
<span data-ttu-id="4d846-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d846-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4d846-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d846-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4d846-154">C#</span><span class="sxs-lookup"><span data-stu-id="4d846-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d846-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d846-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d846-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d846-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d846-157">Java</span><span class="sxs-lookup"><span data-stu-id="4d846-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4d846-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d846-158">Response</span></span>
<span data-ttu-id="4d846-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d846-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
  ]
}
-->


