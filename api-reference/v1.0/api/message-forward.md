---
title: 'message: forward'
description: Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c14b19f7e5b377b12cadb745718f6712d7da291d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069677"
---
# <a name="message-forward"></a><span data-ttu-id="85727-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="85727-104">message: forward</span></span>

<span data-ttu-id="85727-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85727-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85727-p102">Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="85727-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="85727-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="85727-108">Permissions</span></span>
<span data-ttu-id="85727-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85727-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85727-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85727-111">Permission type</span></span>      | <span data-ttu-id="85727-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85727-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85727-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85727-113">Delegated (work or school account)</span></span> | <span data-ttu-id="85727-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85727-114">Mail.Send</span></span>    |
|<span data-ttu-id="85727-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85727-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85727-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85727-116">Mail.Send</span></span>    |
|<span data-ttu-id="85727-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85727-117">Application</span></span> | <span data-ttu-id="85727-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="85727-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="85727-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85727-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="85727-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85727-120">Request headers</span></span>
| <span data-ttu-id="85727-121">Nome</span><span class="sxs-lookup"><span data-stu-id="85727-121">Name</span></span>       | <span data-ttu-id="85727-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="85727-122">Type</span></span> | <span data-ttu-id="85727-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="85727-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85727-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="85727-124">Authorization</span></span>  | <span data-ttu-id="85727-125">string</span><span class="sxs-lookup"><span data-stu-id="85727-125">string</span></span>  | <span data-ttu-id="85727-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85727-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85727-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85727-128">Content-Type</span></span> | <span data-ttu-id="85727-129">string</span><span class="sxs-lookup"><span data-stu-id="85727-129">string</span></span>  | <span data-ttu-id="85727-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85727-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85727-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85727-132">Request body</span></span>
<span data-ttu-id="85727-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85727-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="85727-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="85727-134">Parameter</span></span>    | <span data-ttu-id="85727-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="85727-135">Type</span></span>   |<span data-ttu-id="85727-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="85727-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85727-137">comment</span><span class="sxs-lookup"><span data-stu-id="85727-137">comment</span></span>|<span data-ttu-id="85727-138">String</span><span class="sxs-lookup"><span data-stu-id="85727-138">String</span></span>|<span data-ttu-id="85727-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="85727-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="85727-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="85727-141">toRecipients</span></span>|<span data-ttu-id="85727-142">Coleção [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="85727-142">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="85727-143">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="85727-143">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="85727-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="85727-144">Response</span></span>

<span data-ttu-id="85727-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85727-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85727-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85727-147">Example</span></span>
<span data-ttu-id="85727-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="85727-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85727-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85727-149">Request</span></span>
<span data-ttu-id="85727-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85727-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85727-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="85727-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="85727-152">C#</span><span class="sxs-lookup"><span data-stu-id="85727-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85727-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85727-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85727-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85727-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85727-155">Java</span><span class="sxs-lookup"><span data-stu-id="85727-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85727-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="85727-156">Response</span></span>
##### <a name="response"></a><span data-ttu-id="85727-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="85727-157">Response</span></span>
<span data-ttu-id="85727-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85727-158">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

