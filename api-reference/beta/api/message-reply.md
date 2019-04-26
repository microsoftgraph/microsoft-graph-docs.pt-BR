---
title: 'message: reply'
description: 'Responda ao remetente de uma mensagem, adicione um comentário ou modifique todas as propriedades atualizáveis em uma única chamada **reply**. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c745cfaab60aae9395e2b8d720852a1d2b2b2a39
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333192"
---
# <a name="message-reply"></a><span data-ttu-id="7d12f-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="7d12f-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d12f-104">Responda ao remetente de uma mensagem, adicione um comentário ou modifique todas as propriedades atualizáveis em uma única chamada **reply**.</span><span class="sxs-lookup"><span data-stu-id="7d12f-104">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="7d12f-105">A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="7d12f-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="7d12f-106">Outra opção é primeiro [criar um rascunho de mensagem de resposta](../api/message-createreply.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d12f-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="7d12f-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="7d12f-107">**Note**</span></span>

- <span data-ttu-id="7d12f-108">Você pode especificar um comentário ou a propriedade **Body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7d12f-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="7d12f-109">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="7d12f-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="7d12f-110">Se a \*\*\*\* Propriedade ReplyTo for especificada na mensagem original, por formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários em **ReplyTo** e não ao destinatário na propriedade **from** .</span><span class="sxs-lookup"><span data-stu-id="7d12f-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7d12f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d12f-111">Permissions</span></span>
<span data-ttu-id="7d12f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d12f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d12f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d12f-114">Permission type</span></span>      | <span data-ttu-id="7d12f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d12f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d12f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d12f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7d12f-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7d12f-117">Mail.Send</span></span>    |
|<span data-ttu-id="7d12f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d12f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d12f-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7d12f-119">Mail.Send</span></span>    |
|<span data-ttu-id="7d12f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d12f-120">Application</span></span> | <span data-ttu-id="7d12f-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7d12f-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d12f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d12f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="7d12f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d12f-123">Request headers</span></span>
| <span data-ttu-id="7d12f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7d12f-124">Name</span></span>       | <span data-ttu-id="7d12f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d12f-125">Type</span></span> | <span data-ttu-id="7d12f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d12f-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d12f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d12f-127">Authorization</span></span>  | <span data-ttu-id="7d12f-128">string</span><span class="sxs-lookup"><span data-stu-id="7d12f-128">string</span></span>  | <span data-ttu-id="7d12f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d12f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d12f-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d12f-131">Content-Type</span></span> | <span data-ttu-id="7d12f-132">string</span><span class="sxs-lookup"><span data-stu-id="7d12f-132">string</span></span>  | <span data-ttu-id="7d12f-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d12f-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d12f-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d12f-135">Request body</span></span>
<span data-ttu-id="7d12f-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d12f-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d12f-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7d12f-137">Parameter</span></span>    | <span data-ttu-id="7d12f-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d12f-138">Type</span></span>   |<span data-ttu-id="7d12f-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d12f-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d12f-140">comment</span><span class="sxs-lookup"><span data-stu-id="7d12f-140">comment</span></span>|<span data-ttu-id="7d12f-141">String</span><span class="sxs-lookup"><span data-stu-id="7d12f-141">String</span></span>|<span data-ttu-id="7d12f-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="7d12f-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="7d12f-144">mensagem</span><span class="sxs-lookup"><span data-stu-id="7d12f-144">message</span></span>|[<span data-ttu-id="7d12f-145">message</span><span class="sxs-lookup"><span data-stu-id="7d12f-145">message</span></span>](../resources/message.md)|<span data-ttu-id="7d12f-146">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d12f-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="7d12f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d12f-147">Response</span></span>

<span data-ttu-id="7d12f-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d12f-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d12f-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d12f-150">Example</span></span>
<span data-ttu-id="7d12f-151">O exemplo a seguir inclui um comentário e adiciona um destinatário à mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d12f-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="7d12f-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d12f-152">Request</span></span>
<span data-ttu-id="7d12f-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d12f-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7d12f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d12f-154">Response</span></span>
<span data-ttu-id="7d12f-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d12f-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
