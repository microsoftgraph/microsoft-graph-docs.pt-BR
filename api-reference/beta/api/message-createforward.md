---
title: 'message: createForward'
description: 'Criar um rascunho de mensagem de encaminhamento para incluir um comentário ou atualizar quaisquer propriedades de mensagem  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2c750ac0dd8f6a6226161701950bd879025f9641
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540536"
---
# <a name="message-createforward"></a><span data-ttu-id="74bb3-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="74bb3-103">message: createForward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74bb3-104">Criar um rascunho de mensagem de encaminhamento para incluir um comentário ou atualizar quaisquer propriedades de mensagem</span><span class="sxs-lookup"><span data-stu-id="74bb3-104">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="74bb3-105">tudo em uma \*\*\*\* chamada de createforward.</span><span class="sxs-lookup"><span data-stu-id="74bb3-105">all in one **createForward** call.</span></span> <span data-ttu-id="74bb3-106">Você pode então [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="74bb3-106">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="74bb3-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="74bb3-107">**Note**</span></span>

- <span data-ttu-id="74bb3-108">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="74bb3-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="74bb3-109">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="74bb3-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="74bb3-110">Você deve especificar o `toRecipients` parâmetro ou a propriedade ToRecipients do \*\*\*\* `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="74bb3-110">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="74bb3-111">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="74bb3-111">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="74bb3-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="74bb3-112">Permissions</span></span>
<span data-ttu-id="74bb3-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74bb3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74bb3-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74bb3-115">Permission type</span></span>      | <span data-ttu-id="74bb3-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74bb3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74bb3-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74bb3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="74bb3-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74bb3-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="74bb3-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74bb3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74bb3-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74bb3-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="74bb3-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74bb3-121">Application</span></span> | <span data-ttu-id="74bb3-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74bb3-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="74bb3-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74bb3-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="74bb3-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74bb3-124">Request headers</span></span>
| <span data-ttu-id="74bb3-125">Nome</span><span class="sxs-lookup"><span data-stu-id="74bb3-125">Name</span></span>       | <span data-ttu-id="74bb3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="74bb3-126">Type</span></span> | <span data-ttu-id="74bb3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="74bb3-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74bb3-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="74bb3-128">Authorization</span></span>  | <span data-ttu-id="74bb3-129">string</span><span class="sxs-lookup"><span data-stu-id="74bb3-129">string</span></span>  | <span data-ttu-id="74bb3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74bb3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74bb3-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74bb3-132">Content-Type</span></span> | <span data-ttu-id="74bb3-133">string</span><span class="sxs-lookup"><span data-stu-id="74bb3-133">string</span></span>  | <span data-ttu-id="74bb3-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74bb3-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74bb3-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74bb3-136">Request body</span></span>
<span data-ttu-id="74bb3-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74bb3-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74bb3-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="74bb3-138">Parameter</span></span>    | <span data-ttu-id="74bb3-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="74bb3-139">Type</span></span>   |<span data-ttu-id="74bb3-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="74bb3-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74bb3-141">comment</span><span class="sxs-lookup"><span data-stu-id="74bb3-141">comment</span></span>|<span data-ttu-id="74bb3-142">String</span><span class="sxs-lookup"><span data-stu-id="74bb3-142">String</span></span>|<span data-ttu-id="74bb3-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="74bb3-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="74bb3-145">toRecipients</span><span class="sxs-lookup"><span data-stu-id="74bb3-145">toRecipients</span></span>|<span data-ttu-id="74bb3-146">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="74bb3-146">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="74bb3-147">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="74bb3-147">The list of recipients.</span></span>|
|<span data-ttu-id="74bb3-148">message</span><span class="sxs-lookup"><span data-stu-id="74bb3-148">message</span></span>|[<span data-ttu-id="74bb3-149">mensagem</span><span class="sxs-lookup"><span data-stu-id="74bb3-149">message</span></span>](../resources/message.md)|<span data-ttu-id="74bb3-150">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="74bb3-150">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="74bb3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="74bb3-151">Response</span></span>

<span data-ttu-id="74bb3-152">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74bb3-152">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74bb3-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74bb3-153">Example</span></span>
<span data-ttu-id="74bb3-154">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="74bb3-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74bb3-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74bb3-155">Request</span></span>
<span data-ttu-id="74bb3-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74bb3-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="74bb3-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="74bb3-157">Response</span></span>
<span data-ttu-id="74bb3-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74bb3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/message-createforward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
