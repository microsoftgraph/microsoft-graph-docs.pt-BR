---
title: Atualizar eventMessage
description: Atualize as propriedades de um objeto eventMessage.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6b523e12da00d4b0883d9e337edd288ded13bde2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052394"
---
# <a name="update-eventmessage"></a><span data-ttu-id="4fdc7-103">Atualizar eventMessage</span><span class="sxs-lookup"><span data-stu-id="4fdc7-103">Update eventMessage</span></span>

<span data-ttu-id="4fdc7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fdc7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4fdc7-105">Atualize as propriedades de um objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="4fdc7-105">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4fdc7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4fdc7-106">Permissions</span></span>
<span data-ttu-id="4fdc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fdc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fdc7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fdc7-109">Permission type</span></span>      | <span data-ttu-id="4fdc7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4fdc7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fdc7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fdc7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4fdc7-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fdc7-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4fdc7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fdc7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fdc7-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fdc7-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4fdc7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fdc7-115">Application</span></span> | <span data-ttu-id="4fdc7-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fdc7-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fdc7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fdc7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4fdc7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fdc7-118">Request headers</span></span>
| <span data-ttu-id="4fdc7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4fdc7-119">Name</span></span>       | <span data-ttu-id="4fdc7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fdc7-120">Type</span></span> | <span data-ttu-id="4fdc7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fdc7-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4fdc7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fdc7-122">Authorization</span></span>  | <span data-ttu-id="4fdc7-123">string</span><span class="sxs-lookup"><span data-stu-id="4fdc7-123">string</span></span>  | <span data-ttu-id="4fdc7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4fdc7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4fdc7-126">Content-Type</span></span> | <span data-ttu-id="4fdc7-127">string</span><span class="sxs-lookup"><span data-stu-id="4fdc7-127">string</span></span>  | <span data-ttu-id="4fdc7-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="4fdc7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fdc7-130">Request body</span></span>
<span data-ttu-id="4fdc7-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="4fdc7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="4fdc7-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fdc7-135">Property</span></span>     | <span data-ttu-id="4fdc7-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fdc7-136">Type</span></span>   |<span data-ttu-id="4fdc7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fdc7-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fdc7-138">categories</span><span class="sxs-lookup"><span data-stu-id="4fdc7-138">categories</span></span>|<span data-ttu-id="4fdc7-139">String</span><span class="sxs-lookup"><span data-stu-id="4fdc7-139">String</span></span>|<span data-ttu-id="4fdc7-140">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-140">The categories associated with the message.</span></span>|
|<span data-ttu-id="4fdc7-141">importância</span><span class="sxs-lookup"><span data-stu-id="4fdc7-141">importance</span></span>|<span data-ttu-id="4fdc7-142">String</span><span class="sxs-lookup"><span data-stu-id="4fdc7-142">String</span></span>|<span data-ttu-id="4fdc7-143">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-143">The importance of the message.</span></span> <span data-ttu-id="4fdc7-144">Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-144">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="4fdc7-145">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="4fdc7-145">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="4fdc7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdc7-146">Boolean</span></span>|<span data-ttu-id="4fdc7-147">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-147">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="4fdc7-148">isRead</span><span class="sxs-lookup"><span data-stu-id="4fdc7-148">isRead</span></span>|<span data-ttu-id="4fdc7-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdc7-149">Boolean</span></span>|<span data-ttu-id="4fdc7-150">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-150">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="4fdc7-151">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="4fdc7-151">isReadReceiptRequested</span></span>|<span data-ttu-id="4fdc7-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fdc7-152">Boolean</span></span>|<span data-ttu-id="4fdc7-153">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-153">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="4fdc7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fdc7-154">Response</span></span>

<span data-ttu-id="4fdc7-155">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-155">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4fdc7-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fdc7-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fdc7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fdc7-157">Request</span></span>
<span data-ttu-id="4fdc7-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4fdc7-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fdc7-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": true,
}
```
# <a name="c"></a>[<span data-ttu-id="4fdc7-160">C#</span><span class="sxs-lookup"><span data-stu-id="4fdc7-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4fdc7-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fdc7-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fdc7-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fdc7-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4fdc7-163">Java</span><span class="sxs-lookup"><span data-stu-id="4fdc7-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4fdc7-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fdc7-164">Response</span></span>
<span data-ttu-id="4fdc7-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-165">Here is an example of the response.</span></span> <span data-ttu-id="4fdc7-166">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4fdc7-166">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

