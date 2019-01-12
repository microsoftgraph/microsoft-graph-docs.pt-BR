---
title: 'message: forward'
description: 'Encaminhar uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 18394c29d57c090811bca9a70371c451b090fb26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971484"
---
# <a name="message-forward"></a><span data-ttu-id="8b7a6-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="8b7a6-103">message: forward</span></span>

> <span data-ttu-id="8b7a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b7a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b7a6-106">Encaminhar uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis</span><span class="sxs-lookup"><span data-stu-id="8b7a6-106">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="8b7a6-107">tudo em um **Encaminhar** chamadas.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-107">all in one **forward** call.</span></span> <span data-ttu-id="8b7a6-108">A mensagem será salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-108">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="8b7a6-109">Outra opção é primeiro [criar um rascunho de mensagem de encaminhamento](../api/message-createforward.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-109">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="8b7a6-110">**Observação**</span><span class="sxs-lookup"><span data-stu-id="8b7a6-110">**Note**</span></span>

- <span data-ttu-id="8b7a6-111">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-111">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="8b7a6-112">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-112">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="8b7a6-113">Você deve especificar o `toRecipients` parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-113">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="8b7a6-114">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-114">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b7a6-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b7a6-115">Permissions</span></span>
<span data-ttu-id="8b7a6-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b7a6-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b7a6-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b7a6-118">Permission type</span></span>      | <span data-ttu-id="8b7a6-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b7a6-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b7a6-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b7a6-120">Delegated (work or school account)</span></span> | <span data-ttu-id="8b7a6-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8b7a6-121">Mail.Send</span></span>    |
|<span data-ttu-id="8b7a6-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b7a6-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b7a6-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8b7a6-123">Mail.Send</span></span>    |
|<span data-ttu-id="8b7a6-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b7a6-124">Application</span></span> | <span data-ttu-id="8b7a6-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8b7a6-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b7a6-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b7a6-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="8b7a6-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b7a6-127">Request headers</span></span>
| <span data-ttu-id="8b7a6-128">Nome</span><span class="sxs-lookup"><span data-stu-id="8b7a6-128">Name</span></span>       | <span data-ttu-id="8b7a6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b7a6-129">Type</span></span> | <span data-ttu-id="8b7a6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b7a6-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8b7a6-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b7a6-131">Authorization</span></span>  | <span data-ttu-id="8b7a6-132">string</span><span class="sxs-lookup"><span data-stu-id="8b7a6-132">string</span></span>  | <span data-ttu-id="8b7a6-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b7a6-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b7a6-135">Content-Type</span></span> | <span data-ttu-id="8b7a6-136">string</span><span class="sxs-lookup"><span data-stu-id="8b7a6-136">string</span></span>  | <span data-ttu-id="8b7a6-p107">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b7a6-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b7a6-139">Request body</span></span>
<span data-ttu-id="8b7a6-140">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b7a6-141">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8b7a6-141">Parameter</span></span>    | <span data-ttu-id="8b7a6-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b7a6-142">Type</span></span>   |<span data-ttu-id="8b7a6-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b7a6-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b7a6-144">comment</span><span class="sxs-lookup"><span data-stu-id="8b7a6-144">comment</span></span>|<span data-ttu-id="8b7a6-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b7a6-145">String</span></span>|<span data-ttu-id="8b7a6-p108">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="8b7a6-148">toRecipients</span><span class="sxs-lookup"><span data-stu-id="8b7a6-148">toRecipients</span></span>|<span data-ttu-id="8b7a6-149">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="8b7a6-149">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="8b7a6-150">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-150">The list of recipients.</span></span>|
|<span data-ttu-id="8b7a6-151">message</span><span class="sxs-lookup"><span data-stu-id="8b7a6-151">message</span></span>|[<span data-ttu-id="8b7a6-152">message</span><span class="sxs-lookup"><span data-stu-id="8b7a6-152">message</span></span>](../resources/message.md)|<span data-ttu-id="8b7a6-153">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-153">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="8b7a6-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b7a6-154">Response</span></span>

<span data-ttu-id="8b7a6-p109">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-p109">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b7a6-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b7a6-157">Example</span></span>
<span data-ttu-id="8b7a6-158">O exemplo a seguir define a propriedade **isDeliveryReceiptRequested** como true, adiciona um comentário e encaminha a mensagem.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-158">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="8b7a6-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b7a6-159">Request</span></span>
<span data-ttu-id="8b7a6-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8b7a6-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b7a6-161">Response</span></span>
<span data-ttu-id="8b7a6-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b7a6-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
