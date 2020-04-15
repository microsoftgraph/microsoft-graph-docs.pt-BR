---
title: Atualizar eventMessage
description: Atualize as propriedades de um objeto eventMessage.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dc0955b6d0490f5eb499916fef1bc682f6652500
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461514"
---
# <a name="update-eventmessage"></a><span data-ttu-id="d47a4-103">Atualizar eventMessage</span><span class="sxs-lookup"><span data-stu-id="d47a4-103">Update eventMessage</span></span>

<span data-ttu-id="d47a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d47a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d47a4-105">Atualize as propriedades de um objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="d47a4-105">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d47a4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d47a4-106">Permissions</span></span>
<span data-ttu-id="d47a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d47a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d47a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d47a4-109">Permission type</span></span>      | <span data-ttu-id="d47a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d47a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d47a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d47a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d47a4-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47a4-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d47a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d47a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d47a4-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47a4-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d47a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d47a4-115">Application</span></span> | <span data-ttu-id="d47a4-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47a4-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d47a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d47a4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d47a4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d47a4-118">Request headers</span></span>
| <span data-ttu-id="d47a4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d47a4-119">Name</span></span>       | <span data-ttu-id="d47a4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d47a4-120">Type</span></span> | <span data-ttu-id="d47a4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d47a4-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d47a4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d47a4-122">Authorization</span></span>  | <span data-ttu-id="d47a4-123">string</span><span class="sxs-lookup"><span data-stu-id="d47a4-123">string</span></span>  | <span data-ttu-id="d47a4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d47a4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d47a4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d47a4-126">Content-Type</span></span> | <span data-ttu-id="d47a4-127">string</span><span class="sxs-lookup"><span data-stu-id="d47a4-127">string</span></span>  | <span data-ttu-id="d47a4-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d47a4-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="d47a4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d47a4-130">Request body</span></span>
<span data-ttu-id="d47a4-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="d47a4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="d47a4-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d47a4-135">Property</span></span>     | <span data-ttu-id="d47a4-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d47a4-136">Type</span></span>   |<span data-ttu-id="d47a4-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d47a4-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d47a4-138">categories</span><span class="sxs-lookup"><span data-stu-id="d47a4-138">categories</span></span>|<span data-ttu-id="d47a4-139">String</span><span class="sxs-lookup"><span data-stu-id="d47a4-139">String</span></span>|<span data-ttu-id="d47a4-140">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="d47a4-140">The categories associated with the message.</span></span>|
|<span data-ttu-id="d47a4-141">importância</span><span class="sxs-lookup"><span data-stu-id="d47a4-141">importance</span></span>|<span data-ttu-id="d47a4-142">String</span><span class="sxs-lookup"><span data-stu-id="d47a4-142">String</span></span>|<span data-ttu-id="d47a4-143">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="d47a4-143">The importance of the message.</span></span> <span data-ttu-id="d47a4-144">Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="d47a4-144">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="d47a4-145">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d47a4-145">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="d47a4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47a4-146">Boolean</span></span>|<span data-ttu-id="d47a4-147">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d47a4-147">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="d47a4-148">isRead</span><span class="sxs-lookup"><span data-stu-id="d47a4-148">isRead</span></span>|<span data-ttu-id="d47a4-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47a4-149">Boolean</span></span>|<span data-ttu-id="d47a4-150">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="d47a4-150">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="d47a4-151">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d47a4-151">isReadReceiptRequested</span></span>|<span data-ttu-id="d47a4-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47a4-152">Boolean</span></span>|<span data-ttu-id="d47a4-153">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d47a4-153">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="d47a4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d47a4-154">Response</span></span>

<span data-ttu-id="d47a4-155">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d47a4-155">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d47a4-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d47a4-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d47a4-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d47a4-157">Request</span></span>
<span data-ttu-id="d47a4-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d47a4-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d47a4-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="d47a4-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
# <a name="c"></a>[<span data-ttu-id="d47a4-160">C#</span><span class="sxs-lookup"><span data-stu-id="d47a4-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d47a4-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d47a4-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d47a4-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d47a4-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d47a4-163">Java</span><span class="sxs-lookup"><span data-stu-id="d47a4-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d47a4-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="d47a4-164">Response</span></span>
<span data-ttu-id="d47a4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d47a4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
