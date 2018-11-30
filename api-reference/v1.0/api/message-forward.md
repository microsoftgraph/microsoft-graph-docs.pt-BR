---
title: 'message: forward'
description: Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.
ms.openlocfilehash: 862ce3c40d6e83595373c5530df94cfa18c14b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003917"
---
# <a name="message-forward"></a><span data-ttu-id="7d425-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="7d425-104">message: forward</span></span>

<span data-ttu-id="7d425-p102">Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="7d425-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d425-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d425-107">Permissions</span></span>
<span data-ttu-id="7d425-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d425-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d425-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d425-110">Permission type</span></span>      | <span data-ttu-id="7d425-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d425-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d425-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d425-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d425-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7d425-113">Mail.Send</span></span>    |
|<span data-ttu-id="7d425-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d425-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d425-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7d425-115">Mail.Send</span></span>    |
|<span data-ttu-id="7d425-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d425-116">Application</span></span> | <span data-ttu-id="7d425-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7d425-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d425-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d425-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="7d425-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d425-119">Request headers</span></span>
| <span data-ttu-id="7d425-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7d425-120">Name</span></span>       | <span data-ttu-id="7d425-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d425-121">Type</span></span> | <span data-ttu-id="7d425-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d425-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d425-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d425-123">Authorization</span></span>  | <span data-ttu-id="7d425-124">string</span><span class="sxs-lookup"><span data-stu-id="7d425-124">string</span></span>  | <span data-ttu-id="7d425-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d425-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d425-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d425-127">Content-Type</span></span> | <span data-ttu-id="7d425-128">string</span><span class="sxs-lookup"><span data-stu-id="7d425-128">string</span></span>  | <span data-ttu-id="7d425-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d425-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d425-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d425-131">Request body</span></span>
<span data-ttu-id="7d425-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d425-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d425-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7d425-133">Parameter</span></span>    | <span data-ttu-id="7d425-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d425-134">Type</span></span>   |<span data-ttu-id="7d425-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d425-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d425-136">comment</span><span class="sxs-lookup"><span data-stu-id="7d425-136">comment</span></span>|<span data-ttu-id="7d425-137">String</span><span class="sxs-lookup"><span data-stu-id="7d425-137">String</span></span>|<span data-ttu-id="7d425-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="7d425-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="7d425-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="7d425-140">toRecipients</span></span>|<span data-ttu-id="7d425-141">Coleção [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="7d425-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="7d425-142">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="7d425-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="7d425-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d425-143">Response</span></span>

<span data-ttu-id="7d425-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d425-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d425-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d425-146">Example</span></span>
<span data-ttu-id="7d425-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7d425-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d425-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d425-148">Request</span></span>
<span data-ttu-id="7d425-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d425-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="7d425-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d425-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="7d425-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d425-151">Response</span></span>
<span data-ttu-id="7d425-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d425-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
