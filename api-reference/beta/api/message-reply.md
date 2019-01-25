---
title: 'message: reply'
description: 'Responda ao remetente de uma mensagem, adicione um comentário ou modifique qualquer **propriedade atualizável** tudo em uma única chamada Resposta. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6461d9735459ff9cf956820b00bb61a4d42d1ec0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519007"
---
# <a name="message-reply"></a><span data-ttu-id="68a6d-103">message: reply</span><span class="sxs-lookup"><span data-stu-id="68a6d-103">message: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68a6d-104">Responda ao remetente de uma mensagem, adicione um comentário ou modifique qualquer **propriedade atualizável** tudo em uma única chamada Resposta.</span><span class="sxs-lookup"><span data-stu-id="68a6d-104">Reply to the sender of a message, add a comment or modify any updateable properties all in one **reply** call.</span></span> <span data-ttu-id="68a6d-105">Em seguida, a mensagem será salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="68a6d-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="68a6d-106">Outra opção é primeiro [criar um rascunho de mensagem de resposta](../api/message-createreply.md) para incluir um comentário ou atualizar quaisquer propriedades da mensagem e, em seguida, [enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="68a6d-106">Alternatively, you can first [create a draft reply message](../api/message-createreply.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="68a6d-107">**Observação**</span><span class="sxs-lookup"><span data-stu-id="68a6d-107">**Note**</span></span>

- <span data-ttu-id="68a6d-108">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="68a6d-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="68a6d-109">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="68a6d-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="68a6d-110">Se a propriedade **replyTo** for especificada na mensagem original, por um formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta para os destinatários em **replyTo** e não o destinatário na propriedade **da** .</span><span class="sxs-lookup"><span data-stu-id="68a6d-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in **replyTo** and not the recipient in the **from** property.</span></span> 


## <a name="permissions"></a><span data-ttu-id="68a6d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="68a6d-111">Permissions</span></span>
<span data-ttu-id="68a6d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68a6d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68a6d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68a6d-114">Permission type</span></span>      | <span data-ttu-id="68a6d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68a6d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68a6d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68a6d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="68a6d-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="68a6d-117">Mail.Send</span></span>    |
|<span data-ttu-id="68a6d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68a6d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68a6d-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="68a6d-119">Mail.Send</span></span>    |
|<span data-ttu-id="68a6d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68a6d-120">Application</span></span> | <span data-ttu-id="68a6d-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="68a6d-121">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="68a6d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68a6d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="68a6d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68a6d-123">Request headers</span></span>
| <span data-ttu-id="68a6d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="68a6d-124">Name</span></span>       | <span data-ttu-id="68a6d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="68a6d-125">Type</span></span> | <span data-ttu-id="68a6d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="68a6d-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="68a6d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="68a6d-127">Authorization</span></span>  | <span data-ttu-id="68a6d-128">string</span><span class="sxs-lookup"><span data-stu-id="68a6d-128">string</span></span>  | <span data-ttu-id="68a6d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68a6d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="68a6d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68a6d-131">Content-Type</span></span> | <span data-ttu-id="68a6d-132">string</span><span class="sxs-lookup"><span data-stu-id="68a6d-132">string</span></span>  | <span data-ttu-id="68a6d-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68a6d-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68a6d-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68a6d-135">Request body</span></span>
<span data-ttu-id="68a6d-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68a6d-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="68a6d-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="68a6d-137">Parameter</span></span>    | <span data-ttu-id="68a6d-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="68a6d-138">Type</span></span>   |<span data-ttu-id="68a6d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="68a6d-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68a6d-140">comment</span><span class="sxs-lookup"><span data-stu-id="68a6d-140">comment</span></span>|<span data-ttu-id="68a6d-141">String</span><span class="sxs-lookup"><span data-stu-id="68a6d-141">String</span></span>|<span data-ttu-id="68a6d-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="68a6d-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="68a6d-144">message</span><span class="sxs-lookup"><span data-stu-id="68a6d-144">message</span></span>|[<span data-ttu-id="68a6d-145">message</span><span class="sxs-lookup"><span data-stu-id="68a6d-145">message</span></span>](../resources/message.md)|<span data-ttu-id="68a6d-146">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="68a6d-146">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="68a6d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a6d-147">Response</span></span>

<span data-ttu-id="68a6d-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68a6d-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68a6d-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68a6d-150">Example</span></span>
<span data-ttu-id="68a6d-151">O exemplo a seguir inclui um comentário e adiciona um destinatário à mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="68a6d-151">The following example includes a comment and adds a recipient to the reply message.</span></span>
##### <a name="request"></a><span data-ttu-id="68a6d-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68a6d-152">Request</span></span>
<span data-ttu-id="68a6d-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68a6d-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="68a6d-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a6d-154">Response</span></span>
<span data-ttu-id="68a6d-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68a6d-155">Here is an example of the response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/message-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
