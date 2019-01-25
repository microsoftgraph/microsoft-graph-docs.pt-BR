---
title: 'message: forward'
description: 'Encaminhar uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed3d51c28e6fe0404b5cb26fb17f6d8ed3bba212
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508885"
---
# <a name="message-forward"></a><span data-ttu-id="b6570-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="b6570-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6570-104">Encaminhar uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis</span><span class="sxs-lookup"><span data-stu-id="b6570-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="b6570-105">tudo em um **Encaminhar** chamadas.</span><span class="sxs-lookup"><span data-stu-id="b6570-105">all in one **forward** call.</span></span> <span data-ttu-id="b6570-106">A mensagem será salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="b6570-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="b6570-107">Outra opção é primeiro [criar um rascunho de mensagem de encaminhamento](../api/message-createforward.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b6570-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="b6570-108">**Observação**</span><span class="sxs-lookup"><span data-stu-id="b6570-108">**Note**</span></span>

- <span data-ttu-id="b6570-109">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b6570-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="b6570-110">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="b6570-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="b6570-111">Você deve especificar o `toRecipients` parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b6570-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="b6570-112">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="b6570-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6570-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6570-113">Permissions</span></span>
<span data-ttu-id="b6570-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6570-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6570-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6570-116">Permission type</span></span>      | <span data-ttu-id="b6570-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6570-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6570-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6570-118">Delegated (work or school account)</span></span> | <span data-ttu-id="b6570-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b6570-119">Mail.Send</span></span>    |
|<span data-ttu-id="b6570-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6570-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6570-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b6570-121">Mail.Send</span></span>    |
|<span data-ttu-id="b6570-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6570-122">Application</span></span> | <span data-ttu-id="b6570-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b6570-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6570-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6570-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="b6570-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6570-125">Request headers</span></span>
| <span data-ttu-id="b6570-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b6570-126">Name</span></span>       | <span data-ttu-id="b6570-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6570-127">Type</span></span> | <span data-ttu-id="b6570-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6570-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6570-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6570-129">Authorization</span></span>  | <span data-ttu-id="b6570-130">string</span><span class="sxs-lookup"><span data-stu-id="b6570-130">string</span></span>  | <span data-ttu-id="b6570-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6570-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6570-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6570-133">Content-Type</span></span> | <span data-ttu-id="b6570-134">string</span><span class="sxs-lookup"><span data-stu-id="b6570-134">string</span></span>  | <span data-ttu-id="b6570-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6570-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6570-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6570-137">Request body</span></span>
<span data-ttu-id="b6570-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6570-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b6570-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b6570-139">Parameter</span></span>    | <span data-ttu-id="b6570-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6570-140">Type</span></span>   |<span data-ttu-id="b6570-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6570-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6570-142">comment</span><span class="sxs-lookup"><span data-stu-id="b6570-142">comment</span></span>|<span data-ttu-id="b6570-143">String</span><span class="sxs-lookup"><span data-stu-id="b6570-143">String</span></span>|<span data-ttu-id="b6570-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="b6570-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="b6570-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="b6570-146">toRecipients</span></span>|<span data-ttu-id="b6570-147">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="b6570-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="b6570-148">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="b6570-148">The list of recipients.</span></span>|
|<span data-ttu-id="b6570-149">message</span><span class="sxs-lookup"><span data-stu-id="b6570-149">message</span></span>|[<span data-ttu-id="b6570-150">message</span><span class="sxs-lookup"><span data-stu-id="b6570-150">message</span></span>](../resources/message.md)|<span data-ttu-id="b6570-151">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6570-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="b6570-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6570-152">Response</span></span>

<span data-ttu-id="b6570-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6570-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6570-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6570-155">Example</span></span>
<span data-ttu-id="b6570-156">O exemplo a seguir define a propriedade **IsDeliveryReceiptRequested** como verdadeira, adiciona um comentário e encaminha uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b6570-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="b6570-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6570-157">Request</span></span>
<span data-ttu-id="b6570-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6570-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
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
  "comment": "Dana, just want to make sure you get this." 
}
```

##### <a name="response"></a><span data-ttu-id="b6570-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6570-159">Response</span></span>
<span data-ttu-id="b6570-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6570-160">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
