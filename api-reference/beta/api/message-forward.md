---
title: 'message: forward'
description: 'Encaminhar uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis  '
localization_priority: Normal
ms.openlocfilehash: b601ea1152e9f5b0c5796779967393b956fd2da0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864677"
---
# <a name="message-forward"></a><span data-ttu-id="a26b1-103">message: forward</span><span class="sxs-lookup"><span data-stu-id="a26b1-103">message: forward</span></span>

> <span data-ttu-id="a26b1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a26b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a26b1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a26b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a26b1-106">Encaminhar uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis</span><span class="sxs-lookup"><span data-stu-id="a26b1-106">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="a26b1-107">tudo em um **Encaminhar** chamadas.</span><span class="sxs-lookup"><span data-stu-id="a26b1-107">all in one **forward** call.</span></span> <span data-ttu-id="a26b1-108">A mensagem será salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="a26b1-108">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="a26b1-109">Outra opção é primeiro [criar um rascunho de mensagem de encaminhamento](../api/message-createforward.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) o rascunho da mensagem.</span><span class="sxs-lookup"><span data-stu-id="a26b1-109">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="a26b1-110">**Observação**</span><span class="sxs-lookup"><span data-stu-id="a26b1-110">**Note**</span></span>

- <span data-ttu-id="a26b1-111">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a26b1-111">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="a26b1-112">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="a26b1-112">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="a26b1-113">Você deve especificar o `toRecipients` parâmetro ou a propriedade **toRecipients** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a26b1-113">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="a26b1-114">Especificar ambos ou nenhum retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="a26b1-114">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="a26b1-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="a26b1-115">Permissions</span></span>
<span data-ttu-id="a26b1-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a26b1-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a26b1-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a26b1-118">Permission type</span></span>      | <span data-ttu-id="a26b1-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a26b1-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a26b1-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a26b1-120">Delegated (work or school account)</span></span> | <span data-ttu-id="a26b1-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a26b1-121">Mail.Send</span></span>    |
|<span data-ttu-id="a26b1-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a26b1-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a26b1-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a26b1-123">Mail.Send</span></span>    |
|<span data-ttu-id="a26b1-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a26b1-124">Application</span></span> | <span data-ttu-id="a26b1-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a26b1-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="a26b1-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a26b1-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="a26b1-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a26b1-127">Request headers</span></span>
| <span data-ttu-id="a26b1-128">Nome</span><span class="sxs-lookup"><span data-stu-id="a26b1-128">Name</span></span>       | <span data-ttu-id="a26b1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a26b1-129">Type</span></span> | <span data-ttu-id="a26b1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a26b1-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a26b1-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="a26b1-131">Authorization</span></span>  | <span data-ttu-id="a26b1-132">string</span><span class="sxs-lookup"><span data-stu-id="a26b1-132">string</span></span>  | <span data-ttu-id="a26b1-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a26b1-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a26b1-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a26b1-135">Content-Type</span></span> | <span data-ttu-id="a26b1-136">string</span><span class="sxs-lookup"><span data-stu-id="a26b1-136">string</span></span>  | <span data-ttu-id="a26b1-p107">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a26b1-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a26b1-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a26b1-139">Request body</span></span>
<span data-ttu-id="a26b1-140">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a26b1-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a26b1-141">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a26b1-141">Parameter</span></span>    | <span data-ttu-id="a26b1-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="a26b1-142">Type</span></span>   |<span data-ttu-id="a26b1-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a26b1-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a26b1-144">comment</span><span class="sxs-lookup"><span data-stu-id="a26b1-144">comment</span></span>|<span data-ttu-id="a26b1-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a26b1-145">String</span></span>|<span data-ttu-id="a26b1-p108">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="a26b1-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="a26b1-148">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a26b1-148">toRecipients</span></span>|<span data-ttu-id="a26b1-149">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a26b1-149">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="a26b1-150">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="a26b1-150">The list of recipients.</span></span>|
|<span data-ttu-id="a26b1-151">message</span><span class="sxs-lookup"><span data-stu-id="a26b1-151">message</span></span>|[<span data-ttu-id="a26b1-152">message</span><span class="sxs-lookup"><span data-stu-id="a26b1-152">message</span></span>](../resources/message.md)|<span data-ttu-id="a26b1-153">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="a26b1-153">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="a26b1-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="a26b1-154">Response</span></span>

<span data-ttu-id="a26b1-p109">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a26b1-p109">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a26b1-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a26b1-157">Example</span></span>
<span data-ttu-id="a26b1-158">O exemplo a seguir define a propriedade **isDeliveryReceiptRequested** como true, adiciona um comentário e encaminha a mensagem.</span><span class="sxs-lookup"><span data-stu-id="a26b1-158">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="a26b1-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a26b1-159">Request</span></span>
<span data-ttu-id="a26b1-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a26b1-160">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a26b1-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="a26b1-161">Response</span></span>
<span data-ttu-id="a26b1-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a26b1-162">Here is an example of the response.</span></span>
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
