---
title: 'message: createForward'
description: 'Criar um rascunho de mensagem de encaminhamento para incluir um comentário ou atualizar quaisquer propriedades de mensagem  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0b1ce182e58d5e2033b1e9cac0f1025df1dd6e89
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448275"
---
# <a name="message-createforward"></a><span data-ttu-id="7ce2b-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="7ce2b-103">message: createForward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ce2b-104">Criar um rascunho de mensagem de encaminhamento para incluir um comentário ou atualizar quaisquer propriedades de mensagem</span><span class="sxs-lookup"><span data-stu-id="7ce2b-104">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="7ce2b-105">tudo em uma \*\*\*\* chamada de createforward.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-105">all in one **createForward** call.</span></span> <span data-ttu-id="7ce2b-106">Você pode então [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-106">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="7ce2b-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="7ce2b-107">**Note**</span></span>

- <span data-ttu-id="7ce2b-108">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="7ce2b-109">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="7ce2b-110">Você deve especificar o `toRecipients` parâmetro ou a propriedade ToRecipients do \*\*\*\* `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-110">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="7ce2b-111">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-111">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ce2b-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ce2b-112">Permissions</span></span>
<span data-ttu-id="7ce2b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ce2b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ce2b-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ce2b-115">Permission type</span></span>      | <span data-ttu-id="7ce2b-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ce2b-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ce2b-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ce2b-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7ce2b-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce2b-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7ce2b-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ce2b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ce2b-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce2b-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7ce2b-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ce2b-121">Application</span></span> | <span data-ttu-id="7ce2b-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce2b-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ce2b-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ce2b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="7ce2b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce2b-124">Request headers</span></span>
| <span data-ttu-id="7ce2b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="7ce2b-125">Name</span></span>       | <span data-ttu-id="7ce2b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ce2b-126">Type</span></span> | <span data-ttu-id="7ce2b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ce2b-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ce2b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ce2b-128">Authorization</span></span>  | <span data-ttu-id="7ce2b-129">string</span><span class="sxs-lookup"><span data-stu-id="7ce2b-129">string</span></span>  | <span data-ttu-id="7ce2b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ce2b-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ce2b-132">Content-Type</span></span> | <span data-ttu-id="7ce2b-133">string</span><span class="sxs-lookup"><span data-stu-id="7ce2b-133">string</span></span>  | <span data-ttu-id="7ce2b-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ce2b-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce2b-136">Request body</span></span>
<span data-ttu-id="7ce2b-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7ce2b-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7ce2b-138">Parameter</span></span>    | <span data-ttu-id="7ce2b-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ce2b-139">Type</span></span>   |<span data-ttu-id="7ce2b-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ce2b-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ce2b-141">comment</span><span class="sxs-lookup"><span data-stu-id="7ce2b-141">comment</span></span>|<span data-ttu-id="7ce2b-142">String</span><span class="sxs-lookup"><span data-stu-id="7ce2b-142">String</span></span>|<span data-ttu-id="7ce2b-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="7ce2b-145">toRecipients</span><span class="sxs-lookup"><span data-stu-id="7ce2b-145">toRecipients</span></span>|<span data-ttu-id="7ce2b-146">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="7ce2b-146">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="7ce2b-147">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-147">The list of recipients.</span></span>|
|<span data-ttu-id="7ce2b-148">message</span><span class="sxs-lookup"><span data-stu-id="7ce2b-148">message</span></span>|[<span data-ttu-id="7ce2b-149">message</span><span class="sxs-lookup"><span data-stu-id="7ce2b-149">message</span></span>](../resources/message.md)|<span data-ttu-id="7ce2b-150">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-150">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="7ce2b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ce2b-151">Response</span></span>

<span data-ttu-id="7ce2b-152">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-152">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ce2b-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ce2b-153">Example</span></span>
<span data-ttu-id="7ce2b-154">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7ce2b-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ce2b-155">Request</span></span>
<span data-ttu-id="7ce2b-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7ce2b-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ce2b-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ce2b-158">C#</span><span class="sxs-lookup"><span data-stu-id="7ce2b-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ce2b-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ce2b-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ce2b-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7ce2b-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ce2b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ce2b-161">Response</span></span>
<span data-ttu-id="7ce2b-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ce2b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKqAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DQ\"",
  "id": "AAMkADA1MTAAAH5JKqAAA=",
  "subject": "FW: Let's start a group",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>\r\nDana, just want to make sure you get this; you'll need this if the project gets approved.\r\n<b>From:</b> Admin<br>\r\n<b>Sent:</b> Tuesday, March 15, 2016 6:47:54 AM<br>\r\n<b>To:</b> Samantha Booth; Randi Welch<br>\r\n<b>Subject:</b> RE: Let's start a group</body>\r\n</html>\r\n"
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
        "name": "Dana Swope",
        "address": "danas@contoso.onmicrosoft.com"
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
