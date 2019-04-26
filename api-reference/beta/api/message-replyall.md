---
title: 'message: replyAll'
description: 'Responder a todos os destinatários de uma mensagem especificando um comentário e modificando qualquer propriedade atualizável '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: deccb9d2fabdee0a85f292c9edf4443ab4f8b835
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338322"
---
# <a name="message-replyall"></a><span data-ttu-id="9c11f-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="9c11f-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c11f-104">Responda a todos os destinatários de uma mensagem especificando um comentário e modificando as propriedades atualizáveis da resposta, tudo usando o método **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="9c11f-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="9c11f-105">A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="9c11f-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="9c11f-106">Como alternativa, você pode primeiro [criar um rascunho de mensagem de resposta](../api/message-createreplyall.md) para incluir um comentário ou atualizar quaisquer propriedades de mensagem e, em seguida, [Enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="9c11f-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="9c11f-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="9c11f-107">**Note**</span></span>

- <span data-ttu-id="9c11f-108">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9c11f-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="9c11f-109">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="9c11f-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="9c11f-110">Se a \*\*\*\* Propriedade ReplyTo for especificada na mensagem original, por formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários no</span><span class="sxs-lookup"><span data-stu-id="9c11f-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="9c11f-111">\*\*\*\* as propriedades ReplyTo e ToRecipients e não os destinatários nas propriedades **from** e \*\*\*\* ToRecipients. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="9c11f-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="9c11f-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c11f-112">Permissions</span></span>
<span data-ttu-id="9c11f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c11f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c11f-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c11f-115">Permission type</span></span>      | <span data-ttu-id="9c11f-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c11f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c11f-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c11f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="9c11f-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c11f-118">Mail.Send</span></span>    |
|<span data-ttu-id="9c11f-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c11f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c11f-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c11f-120">Mail.Send</span></span>    |
|<span data-ttu-id="9c11f-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c11f-121">Application</span></span> | <span data-ttu-id="9c11f-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9c11f-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c11f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c11f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="9c11f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c11f-124">Request headers</span></span>
| <span data-ttu-id="9c11f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="9c11f-125">Name</span></span>       | <span data-ttu-id="9c11f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c11f-126">Type</span></span> | <span data-ttu-id="9c11f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c11f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c11f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c11f-128">Authorization</span></span>  | <span data-ttu-id="9c11f-129">string</span><span class="sxs-lookup"><span data-stu-id="9c11f-129">string</span></span>  | <span data-ttu-id="9c11f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c11f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c11f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c11f-132">Content-Type</span></span> | <span data-ttu-id="9c11f-133">string</span><span class="sxs-lookup"><span data-stu-id="9c11f-133">string</span></span>  | <span data-ttu-id="9c11f-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c11f-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c11f-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c11f-136">Request body</span></span>
<span data-ttu-id="9c11f-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c11f-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9c11f-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9c11f-138">Parameter</span></span>    | <span data-ttu-id="9c11f-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c11f-139">Type</span></span>   |<span data-ttu-id="9c11f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c11f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c11f-141">comment</span><span class="sxs-lookup"><span data-stu-id="9c11f-141">comment</span></span>|<span data-ttu-id="9c11f-142">String</span><span class="sxs-lookup"><span data-stu-id="9c11f-142">String</span></span>|<span data-ttu-id="9c11f-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="9c11f-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="9c11f-145">mensagem</span><span class="sxs-lookup"><span data-stu-id="9c11f-145">message</span></span>|[<span data-ttu-id="9c11f-146">message</span><span class="sxs-lookup"><span data-stu-id="9c11f-146">message</span></span>](../resources/message.md)|<span data-ttu-id="9c11f-147">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c11f-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="9c11f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c11f-148">Response</span></span>

<span data-ttu-id="9c11f-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c11f-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c11f-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c11f-151">Example</span></span>
<span data-ttu-id="9c11f-152">O exemplo a seguir inclui um comentário e adiciona um anexo à mensagem de resposta a todos.</span><span class="sxs-lookup"><span data-stu-id="9c11f-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="9c11f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c11f-153">Request</span></span>
<span data-ttu-id="9c11f-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c11f-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```


##### <a name="response"></a><span data-ttu-id="9c11f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c11f-155">Response</span></span>
<span data-ttu-id="9c11f-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c11f-156">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
