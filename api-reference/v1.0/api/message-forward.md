---
title: 'message: forward'
description: Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1becc0bc31b15c1393dde2c9aa8c7ec4fc2a921
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976665"
---
# <a name="message-forward"></a><span data-ttu-id="46b60-104">message: forward</span><span class="sxs-lookup"><span data-stu-id="46b60-104">message: forward</span></span>

<span data-ttu-id="46b60-p102">Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="46b60-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="46b60-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="46b60-107">Permissions</span></span>
<span data-ttu-id="46b60-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46b60-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46b60-110">Permission type</span></span>      | <span data-ttu-id="46b60-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46b60-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46b60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46b60-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46b60-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="46b60-113">Mail.Send</span></span>    |
|<span data-ttu-id="46b60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46b60-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46b60-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="46b60-115">Mail.Send</span></span>    |
|<span data-ttu-id="46b60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46b60-116">Application</span></span> | <span data-ttu-id="46b60-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="46b60-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="46b60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46b60-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="46b60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46b60-119">Request headers</span></span>
| <span data-ttu-id="46b60-120">Nome</span><span class="sxs-lookup"><span data-stu-id="46b60-120">Name</span></span>       | <span data-ttu-id="46b60-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="46b60-121">Type</span></span> | <span data-ttu-id="46b60-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="46b60-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46b60-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="46b60-123">Authorization</span></span>  | <span data-ttu-id="46b60-124">string</span><span class="sxs-lookup"><span data-stu-id="46b60-124">string</span></span>  | <span data-ttu-id="46b60-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46b60-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46b60-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46b60-127">Content-Type</span></span> | <span data-ttu-id="46b60-128">string</span><span class="sxs-lookup"><span data-stu-id="46b60-128">string</span></span>  | <span data-ttu-id="46b60-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46b60-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46b60-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46b60-131">Request body</span></span>
<span data-ttu-id="46b60-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46b60-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46b60-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46b60-133">Parameter</span></span>    | <span data-ttu-id="46b60-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="46b60-134">Type</span></span>   |<span data-ttu-id="46b60-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="46b60-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46b60-136">comment</span><span class="sxs-lookup"><span data-stu-id="46b60-136">comment</span></span>|<span data-ttu-id="46b60-137">String</span><span class="sxs-lookup"><span data-stu-id="46b60-137">String</span></span>|<span data-ttu-id="46b60-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="46b60-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="46b60-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="46b60-140">toRecipients</span></span>|<span data-ttu-id="46b60-141">Coleção [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="46b60-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="46b60-142">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="46b60-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="46b60-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b60-143">Response</span></span>

<span data-ttu-id="46b60-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46b60-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b60-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46b60-146">Example</span></span>
<span data-ttu-id="46b60-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="46b60-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46b60-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46b60-148">Request</span></span>
<span data-ttu-id="46b60-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46b60-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46b60-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="46b60-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="46b60-151">C#</span><span class="sxs-lookup"><span data-stu-id="46b60-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46b60-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="46b60-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46b60-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="46b60-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46b60-154">Java</span><span class="sxs-lookup"><span data-stu-id="46b60-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="46b60-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b60-155">Response</span></span>
##### <a name="response"></a><span data-ttu-id="46b60-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b60-156">Response</span></span>
<span data-ttu-id="46b60-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46b60-157">Here is an example of the response.</span></span>
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
