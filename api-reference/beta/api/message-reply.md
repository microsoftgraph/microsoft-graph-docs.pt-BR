---
title: 'message: reply'
description: 'Responder ao remetente de uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis todas em uma **resposta** de chamada. '
ms.openlocfilehash: 93130e8a877b9a7bdc553646037f583fd8da84fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037793"
---
# <a name="message-reply"></a><span data-ttu-id="455b4-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="455b4-103">message: reply</span></span>

> <span data-ttu-id="455b4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="455b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="455b4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="455b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="455b4-106">Responder ao remetente de uma mensagem, adicionar um comentário ou modificar quaisquer propriedades atualizáveis todas em uma **resposta** de chamada.</span><span class="sxs-lookup"><span data-stu-id="455b4-106">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="455b4-107">Em seguida, a mensagem será salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="455b4-107">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="455b4-108">Outra opção é primeiro [criar um rascunho de mensagem de resposta](../api/message-createreply.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="455b4-108">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="455b4-109">**Observação**</span><span class="sxs-lookup"><span data-stu-id="455b4-109">**Note**</span></span>

- <span data-ttu-id="455b4-110">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="455b4-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="455b4-111">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="455b4-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="455b4-112">Se a propriedade **replyTo** for especificada na mensagem original, por um formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta para os destinatários em **replyTo** e não o destinatário na propriedade **da** .</span><span class="sxs-lookup"><span data-stu-id="455b4-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="455b4-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="455b4-113">Permissions</span></span>
<span data-ttu-id="455b4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="455b4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="455b4-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="455b4-116">Permission type</span></span>      | <span data-ttu-id="455b4-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="455b4-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="455b4-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="455b4-118">Delegated (work or school account)</span></span> | <span data-ttu-id="455b4-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="455b4-119">Mail.Send</span></span>    |
|<span data-ttu-id="455b4-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="455b4-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="455b4-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="455b4-121">Mail.Send</span></span>    |
|<span data-ttu-id="455b4-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="455b4-122">Application</span></span> | <span data-ttu-id="455b4-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="455b4-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="455b4-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="455b4-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="455b4-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="455b4-125">Request headers</span></span>
| <span data-ttu-id="455b4-126">Nome</span><span class="sxs-lookup"><span data-stu-id="455b4-126">Name</span></span>       | <span data-ttu-id="455b4-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="455b4-127">Type</span></span> | <span data-ttu-id="455b4-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="455b4-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="455b4-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="455b4-129">Authorization</span></span>  | <span data-ttu-id="455b4-130">string</span><span class="sxs-lookup"><span data-stu-id="455b4-130">string</span></span>  | <span data-ttu-id="455b4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="455b4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="455b4-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="455b4-133">Content-Type</span></span> | <span data-ttu-id="455b4-134">string</span><span class="sxs-lookup"><span data-stu-id="455b4-134">string</span></span>  | <span data-ttu-id="455b4-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="455b4-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="455b4-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="455b4-137">Request body</span></span>
<span data-ttu-id="455b4-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="455b4-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="455b4-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="455b4-139">Parameter</span></span>    | <span data-ttu-id="455b4-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="455b4-140">Type</span></span>   |<span data-ttu-id="455b4-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="455b4-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="455b4-142">comment</span><span class="sxs-lookup"><span data-stu-id="455b4-142">comment</span></span>|<span data-ttu-id="455b4-143">String</span><span class="sxs-lookup"><span data-stu-id="455b4-143">String</span></span>|<span data-ttu-id="455b4-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="455b4-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="455b4-146">message</span><span class="sxs-lookup"><span data-stu-id="455b4-146">message</span></span>|[<span data-ttu-id="455b4-147">message</span><span class="sxs-lookup"><span data-stu-id="455b4-147">message</span></span>](../resources/message.md)|<span data-ttu-id="455b4-148">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="455b4-148">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="455b4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="455b4-149">Response</span></span>

<span data-ttu-id="455b4-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="455b4-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="455b4-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="455b4-152">Example</span></span>
<span data-ttu-id="455b4-153">O exemplo a seguir inclui um comentário e adiciona um destinatário à mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="455b4-153">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="455b4-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="455b4-154">Request</span></span>
<span data-ttu-id="455b4-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="455b4-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
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
  "comment": "Samantha, Randi, would you name the group please?" 
}
```

##### <a name="response"></a><span data-ttu-id="455b4-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="455b4-156">Response</span></span>
<span data-ttu-id="455b4-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="455b4-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
