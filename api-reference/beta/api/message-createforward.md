---
title: 'message: createForward'
description: 'Criar um rascunho de mensagem de encaminhamento para incluir um comentário ou atualizar quaisquer propriedades de mensagem  '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 42115aaedd5de84b0fbbdd898267a18da0d75e37
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981591"
---
# <a name="message-createforward"></a><span data-ttu-id="efb2b-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="efb2b-103">message: createForward</span></span>

<span data-ttu-id="efb2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efb2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efb2b-105">Criar um rascunho de mensagem de encaminhamento para incluir um comentário ou atualizar quaisquer propriedades de mensagem</span><span class="sxs-lookup"><span data-stu-id="efb2b-105">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="efb2b-106">tudo em uma chamada de **createforward** .</span><span class="sxs-lookup"><span data-stu-id="efb2b-106">all in one **createForward** call.</span></span> <span data-ttu-id="efb2b-107">Você pode então [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="efb2b-107">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="efb2b-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="efb2b-108">**Note**</span></span>

- <span data-ttu-id="efb2b-109">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="efb2b-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="efb2b-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="efb2b-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="efb2b-111">Você deve especificar o `toRecipients` parâmetro ou a propriedade **ToRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="efb2b-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="efb2b-112">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="efb2b-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="efb2b-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="efb2b-113">Permissions</span></span>
<span data-ttu-id="efb2b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efb2b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb2b-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efb2b-116">Permission type</span></span>      | <span data-ttu-id="efb2b-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efb2b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efb2b-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efb2b-118">Delegated (work or school account)</span></span> | <span data-ttu-id="efb2b-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efb2b-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="efb2b-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efb2b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efb2b-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efb2b-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="efb2b-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efb2b-122">Application</span></span> | <span data-ttu-id="efb2b-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efb2b-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="efb2b-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efb2b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="efb2b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efb2b-125">Request headers</span></span>
| <span data-ttu-id="efb2b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="efb2b-126">Name</span></span>       | <span data-ttu-id="efb2b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="efb2b-127">Type</span></span> | <span data-ttu-id="efb2b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb2b-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efb2b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="efb2b-129">Authorization</span></span>  | <span data-ttu-id="efb2b-130">string</span><span class="sxs-lookup"><span data-stu-id="efb2b-130">string</span></span>  | <span data-ttu-id="efb2b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efb2b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="efb2b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="efb2b-133">Content-Type</span></span> | <span data-ttu-id="efb2b-134">string</span><span class="sxs-lookup"><span data-stu-id="efb2b-134">string</span></span>  | <span data-ttu-id="efb2b-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efb2b-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efb2b-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efb2b-137">Request body</span></span>
<span data-ttu-id="efb2b-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efb2b-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="efb2b-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="efb2b-139">Parameter</span></span>    | <span data-ttu-id="efb2b-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="efb2b-140">Type</span></span>   |<span data-ttu-id="efb2b-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb2b-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efb2b-142">comment</span><span class="sxs-lookup"><span data-stu-id="efb2b-142">comment</span></span>|<span data-ttu-id="efb2b-143">String</span><span class="sxs-lookup"><span data-stu-id="efb2b-143">String</span></span>|<span data-ttu-id="efb2b-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="efb2b-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="efb2b-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="efb2b-146">toRecipients</span></span>|<span data-ttu-id="efb2b-147">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="efb2b-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="efb2b-148">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="efb2b-148">The list of recipients.</span></span>|
|<span data-ttu-id="efb2b-149">message</span><span class="sxs-lookup"><span data-stu-id="efb2b-149">message</span></span>|[<span data-ttu-id="efb2b-150">message</span><span class="sxs-lookup"><span data-stu-id="efb2b-150">message</span></span>](../resources/message.md)|<span data-ttu-id="efb2b-151">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="efb2b-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="efb2b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="efb2b-152">Response</span></span>

<span data-ttu-id="efb2b-153">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efb2b-153">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb2b-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efb2b-154">Example</span></span>
<span data-ttu-id="efb2b-155">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="efb2b-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="efb2b-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efb2b-156">Request</span></span>
<span data-ttu-id="efb2b-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efb2b-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="efb2b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="efb2b-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="efb2b-159">C#</span><span class="sxs-lookup"><span data-stu-id="efb2b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efb2b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efb2b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efb2b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efb2b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efb2b-162">Java</span><span class="sxs-lookup"><span data-stu-id="efb2b-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="efb2b-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="efb2b-163">Response</span></span>
<span data-ttu-id="efb2b-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efb2b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


