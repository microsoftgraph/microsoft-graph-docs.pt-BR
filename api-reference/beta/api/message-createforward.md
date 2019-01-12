---
title: 'message: createForward'
description: 'Criar uma mensagem de rascunho sequencial para incluir um comentário ou atualizar as propriedades de mensagem  '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 56f73ac798ef3440b66cb4c0de1192d3248d3a61
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949070"
---
# <a name="message-createforward"></a><span data-ttu-id="5c28d-103">message: createForward</span><span class="sxs-lookup"><span data-stu-id="5c28d-103">message: createForward</span></span>

> <span data-ttu-id="5c28d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5c28d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c28d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5c28d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c28d-106">Criar uma mensagem de rascunho sequencial para incluir um comentário ou atualizar as propriedades de mensagem</span><span class="sxs-lookup"><span data-stu-id="5c28d-106">Create a draft forward message to include a comment or update any message properties</span></span>  
<span data-ttu-id="5c28d-107">tudo isso em um **createForward** chamada.</span><span class="sxs-lookup"><span data-stu-id="5c28d-107">all in one **createForward** call.</span></span> <span data-ttu-id="5c28d-108">Você pode então [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="5c28d-108">You can then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="5c28d-109">**Observação**</span><span class="sxs-lookup"><span data-stu-id="5c28d-109">**Note**</span></span>

- <span data-ttu-id="5c28d-110">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5c28d-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="5c28d-111">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="5c28d-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="5c28d-112">Você deve especificar o `toRecipients` parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5c28d-112">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="5c28d-113">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="5c28d-113">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c28d-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c28d-114">Permissions</span></span>
<span data-ttu-id="5c28d-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c28d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c28d-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c28d-117">Permission type</span></span>      | <span data-ttu-id="5c28d-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c28d-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c28d-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c28d-119">Delegated (work or school account)</span></span> | <span data-ttu-id="5c28d-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c28d-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5c28d-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c28d-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c28d-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c28d-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5c28d-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c28d-123">Application</span></span> | <span data-ttu-id="5c28d-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c28d-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c28d-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c28d-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="5c28d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c28d-126">Request headers</span></span>
| <span data-ttu-id="5c28d-127">Nome</span><span class="sxs-lookup"><span data-stu-id="5c28d-127">Name</span></span>       | <span data-ttu-id="5c28d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c28d-128">Type</span></span> | <span data-ttu-id="5c28d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c28d-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c28d-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c28d-130">Authorization</span></span>  | <span data-ttu-id="5c28d-131">string</span><span class="sxs-lookup"><span data-stu-id="5c28d-131">string</span></span>  | <span data-ttu-id="5c28d-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c28d-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c28d-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c28d-134">Content-Type</span></span> | <span data-ttu-id="5c28d-135">string</span><span class="sxs-lookup"><span data-stu-id="5c28d-135">string</span></span>  | <span data-ttu-id="5c28d-p107">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c28d-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c28d-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c28d-138">Request body</span></span>
<span data-ttu-id="5c28d-139">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c28d-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c28d-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c28d-140">Parameter</span></span>    | <span data-ttu-id="5c28d-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c28d-141">Type</span></span>   |<span data-ttu-id="5c28d-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c28d-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c28d-143">comment</span><span class="sxs-lookup"><span data-stu-id="5c28d-143">comment</span></span>|<span data-ttu-id="5c28d-144">String</span><span class="sxs-lookup"><span data-stu-id="5c28d-144">String</span></span>|<span data-ttu-id="5c28d-p108">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="5c28d-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="5c28d-147">toRecipients</span><span class="sxs-lookup"><span data-stu-id="5c28d-147">toRecipients</span></span>|<span data-ttu-id="5c28d-148">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="5c28d-148">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="5c28d-149">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="5c28d-149">The list of recipients.</span></span>|
|<span data-ttu-id="5c28d-150">message</span><span class="sxs-lookup"><span data-stu-id="5c28d-150">message</span></span>|[<span data-ttu-id="5c28d-151">message</span><span class="sxs-lookup"><span data-stu-id="5c28d-151">message</span></span>](../resources/message.md)|<span data-ttu-id="5c28d-152">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c28d-152">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="5c28d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c28d-153">Response</span></span>

<span data-ttu-id="5c28d-154">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c28d-154">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c28d-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c28d-155">Example</span></span>
<span data-ttu-id="5c28d-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5c28d-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c28d-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c28d-157">Request</span></span>
<span data-ttu-id="5c28d-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c28d-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5c28d-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c28d-159">Response</span></span>
<span data-ttu-id="5c28d-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c28d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
