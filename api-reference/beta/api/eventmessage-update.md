---
title: Atualizar eventMessage
description: Atualize as propriedades de um objeto eventMessage.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3684ec702a0fd0e1bcd55d4087fee2c75b7af3bc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43364145"
---
# <a name="update-eventmessage"></a><span data-ttu-id="03c36-103">Atualizar eventMessage</span><span class="sxs-lookup"><span data-stu-id="03c36-103">Update eventMessage</span></span>

<span data-ttu-id="03c36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03c36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03c36-105">Atualize as propriedades de um objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="03c36-105">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="03c36-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="03c36-106">Permissions</span></span>
<span data-ttu-id="03c36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03c36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03c36-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03c36-109">Permission type</span></span>      | <span data-ttu-id="03c36-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03c36-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03c36-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03c36-111">Delegated (work or school account)</span></span> | <span data-ttu-id="03c36-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03c36-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="03c36-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03c36-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03c36-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03c36-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="03c36-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03c36-115">Application</span></span> | <span data-ttu-id="03c36-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03c36-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="03c36-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03c36-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="03c36-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03c36-118">Request headers</span></span>
| <span data-ttu-id="03c36-119">Nome</span><span class="sxs-lookup"><span data-stu-id="03c36-119">Name</span></span>       | <span data-ttu-id="03c36-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="03c36-120">Type</span></span> | <span data-ttu-id="03c36-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="03c36-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="03c36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="03c36-122">Authorization</span></span>  | <span data-ttu-id="03c36-123">string</span><span class="sxs-lookup"><span data-stu-id="03c36-123">string</span></span>  | <span data-ttu-id="03c36-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03c36-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03c36-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03c36-126">Content-Type</span></span> | <span data-ttu-id="03c36-127">string</span><span class="sxs-lookup"><span data-stu-id="03c36-127">string</span></span>  | <span data-ttu-id="03c36-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03c36-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="03c36-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03c36-130">Request body</span></span>
<span data-ttu-id="03c36-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="03c36-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="03c36-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03c36-135">Property</span></span>     | <span data-ttu-id="03c36-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="03c36-136">Type</span></span>   |<span data-ttu-id="03c36-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="03c36-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03c36-138">categories</span><span class="sxs-lookup"><span data-stu-id="03c36-138">categories</span></span>|<span data-ttu-id="03c36-139">String</span><span class="sxs-lookup"><span data-stu-id="03c36-139">String</span></span>|<span data-ttu-id="03c36-140">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="03c36-140">The categories associated with the message.</span></span>|
|<span data-ttu-id="03c36-141">importância</span><span class="sxs-lookup"><span data-stu-id="03c36-141">importance</span></span>|<span data-ttu-id="03c36-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03c36-142">String</span></span>|<span data-ttu-id="03c36-p105">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="03c36-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="03c36-145">isAllDay</span><span class="sxs-lookup"><span data-stu-id="03c36-145">isAllDay</span></span> |<span data-ttu-id="03c36-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="03c36-146">Boolean</span></span>|<span data-ttu-id="03c36-147">Indica se o evento dura todo o dia.</span><span class="sxs-lookup"><span data-stu-id="03c36-147">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="03c36-148">Ajustar essa propriedade requer ajustar as propriedades **StartDateTime** e **EndDateTime** do evento também.</span><span class="sxs-lookup"><span data-stu-id="03c36-148">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="03c36-149">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="03c36-149">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="03c36-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="03c36-150">Boolean</span></span>|<span data-ttu-id="03c36-151">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="03c36-151">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="03c36-152">isRead</span><span class="sxs-lookup"><span data-stu-id="03c36-152">isRead</span></span>|<span data-ttu-id="03c36-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="03c36-153">Boolean</span></span>|<span data-ttu-id="03c36-154">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="03c36-154">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="03c36-155">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="03c36-155">isReadReceiptRequested</span></span>|<span data-ttu-id="03c36-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="03c36-156">Boolean</span></span>|<span data-ttu-id="03c36-157">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="03c36-157">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="03c36-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="03c36-158">Response</span></span>

<span data-ttu-id="03c36-159">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03c36-159">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03c36-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03c36-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03c36-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03c36-161">Request</span></span>
<span data-ttu-id="03c36-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03c36-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03c36-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="03c36-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
# <a name="c"></a>[<span data-ttu-id="03c36-164">C#</span><span class="sxs-lookup"><span data-stu-id="03c36-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03c36-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03c36-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03c36-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03c36-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03c36-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="03c36-167">Response</span></span>
<span data-ttu-id="03c36-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03c36-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
