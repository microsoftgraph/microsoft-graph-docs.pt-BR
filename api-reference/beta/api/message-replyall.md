---
title: 'message: replyAll'
description: 'Responder a todos os destinatários de uma mensagem especificando um comentário e modificar quaisquer propriedades atualizáveis '
author: angelgolfer-ms
ms.openlocfilehash: 035212224bca5cb6d173be9ea447cf16406ebf36
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307186"
---
# <a name="message-replyall"></a><span data-ttu-id="85801-103">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="85801-103">message: replyAll</span></span>

> <span data-ttu-id="85801-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="85801-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85801-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="85801-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85801-106">Responder a todos os destinatários de uma mensagem especificando um comentário e modificar quaisquer propriedades atualizáveis para a resposta, tudo usando o método **replyAll** .</span><span class="sxs-lookup"><span data-stu-id="85801-106">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="85801-107">Em seguida, a mensagem será salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="85801-107">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="85801-108">Como alternativa, você pode primeiro [criar uma mensagem de responder a todos de rascunho](../api/message-createreplyall.md) para incluir um comentário ou atualizar qualquer propriedades da mensagem e, em seguida, [Enviar](../api/message-send.md) a resposta.</span><span class="sxs-lookup"><span data-stu-id="85801-108">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="85801-109">**Observação**</span><span class="sxs-lookup"><span data-stu-id="85801-109">**Note**</span></span>

- <span data-ttu-id="85801-110">Você pode especificar um comentário ou a propriedade **body** do `message` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="85801-110">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="85801-111">Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="85801-111">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="85801-112">Se a propriedade **replyTo** for especificada na mensagem original, por um formato de mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), você deve enviar a resposta aos destinatários no</span><span class="sxs-lookup"><span data-stu-id="85801-112">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="85801-113">propriedades **replyTo** e **toRecipients** e não os destinatários nas propriedades **do** e **toRecipients** .</span><span class="sxs-lookup"><span data-stu-id="85801-113">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="85801-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="85801-114">Permissions</span></span>
<span data-ttu-id="85801-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85801-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85801-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85801-117">Permission type</span></span>      | <span data-ttu-id="85801-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85801-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85801-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85801-119">Delegated (work or school account)</span></span> | <span data-ttu-id="85801-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85801-120">Mail.Send</span></span>    |
|<span data-ttu-id="85801-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85801-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85801-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85801-122">Mail.Send</span></span>    |
|<span data-ttu-id="85801-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85801-123">Application</span></span> | <span data-ttu-id="85801-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85801-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="85801-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85801-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="85801-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85801-126">Request headers</span></span>
| <span data-ttu-id="85801-127">Nome</span><span class="sxs-lookup"><span data-stu-id="85801-127">Name</span></span>       | <span data-ttu-id="85801-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="85801-128">Type</span></span> | <span data-ttu-id="85801-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="85801-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85801-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="85801-130">Authorization</span></span>  | <span data-ttu-id="85801-131">string</span><span class="sxs-lookup"><span data-stu-id="85801-131">string</span></span>  | <span data-ttu-id="85801-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85801-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85801-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85801-134">Content-Type</span></span> | <span data-ttu-id="85801-135">string</span><span class="sxs-lookup"><span data-stu-id="85801-135">string</span></span>  | <span data-ttu-id="85801-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85801-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85801-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85801-138">Request body</span></span>
<span data-ttu-id="85801-139">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85801-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="85801-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="85801-140">Parameter</span></span>    | <span data-ttu-id="85801-141">Type</span><span class="sxs-lookup"><span data-stu-id="85801-141">Type</span></span>   |<span data-ttu-id="85801-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="85801-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85801-143">comment</span><span class="sxs-lookup"><span data-stu-id="85801-143">comment</span></span>|<span data-ttu-id="85801-144">String</span><span class="sxs-lookup"><span data-stu-id="85801-144">String</span></span>|<span data-ttu-id="85801-p107">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="85801-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="85801-147">message</span><span class="sxs-lookup"><span data-stu-id="85801-147">message</span></span>|[<span data-ttu-id="85801-148">message</span><span class="sxs-lookup"><span data-stu-id="85801-148">message</span></span>](../resources/message.md)|<span data-ttu-id="85801-149">Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="85801-149">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="85801-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="85801-150">Response</span></span>

<span data-ttu-id="85801-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85801-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85801-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85801-153">Example</span></span>
<span data-ttu-id="85801-154">O exemplo a seguir inclui um comentário e adiciona um anexo à mensagem de resposta a todos.</span><span class="sxs-lookup"><span data-stu-id="85801-154">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="85801-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85801-155">Request</span></span>
<span data-ttu-id="85801-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85801-156">Here is an example of the request.</span></span>
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


##### <a name="response"></a><span data-ttu-id="85801-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="85801-157">Response</span></span>
<span data-ttu-id="85801-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85801-158">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
