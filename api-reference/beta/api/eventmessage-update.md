---
title: Atualizar eventMessage
description: Atualize as propriedades de um objeto eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 33ad8199dfa7ebcc7544e2d4e0363a2973f3c170
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323546"
---
# <a name="update-eventmessage"></a><span data-ttu-id="00bd5-103">Atualizar eventMessage</span><span class="sxs-lookup"><span data-stu-id="00bd5-103">Update eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00bd5-104">Atualize as propriedades de um objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="00bd5-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="00bd5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="00bd5-105">Permissions</span></span>
<span data-ttu-id="00bd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00bd5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00bd5-108">Permission type</span></span>      | <span data-ttu-id="00bd5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00bd5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00bd5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00bd5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00bd5-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00bd5-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="00bd5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00bd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00bd5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00bd5-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="00bd5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00bd5-114">Application</span></span> | <span data-ttu-id="00bd5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00bd5-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="00bd5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00bd5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="00bd5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00bd5-117">Request headers</span></span>
| <span data-ttu-id="00bd5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="00bd5-118">Name</span></span>       | <span data-ttu-id="00bd5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="00bd5-119">Type</span></span> | <span data-ttu-id="00bd5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="00bd5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="00bd5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="00bd5-121">Authorization</span></span>  | <span data-ttu-id="00bd5-122">string</span><span class="sxs-lookup"><span data-stu-id="00bd5-122">string</span></span>  | <span data-ttu-id="00bd5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00bd5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00bd5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00bd5-125">Content-Type</span></span> | <span data-ttu-id="00bd5-126">string</span><span class="sxs-lookup"><span data-stu-id="00bd5-126">string</span></span>  | <span data-ttu-id="00bd5-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00bd5-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="00bd5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00bd5-129">Request body</span></span>
<span data-ttu-id="00bd5-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="00bd5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="00bd5-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00bd5-134">Property</span></span>     | <span data-ttu-id="00bd5-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="00bd5-135">Type</span></span>   |<span data-ttu-id="00bd5-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="00bd5-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00bd5-137">categories</span><span class="sxs-lookup"><span data-stu-id="00bd5-137">categories</span></span>|<span data-ttu-id="00bd5-138">String</span><span class="sxs-lookup"><span data-stu-id="00bd5-138">String</span></span>|<span data-ttu-id="00bd5-139">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="00bd5-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="00bd5-140">importance</span><span class="sxs-lookup"><span data-stu-id="00bd5-140">importance</span></span>|<span data-ttu-id="00bd5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00bd5-141">String</span></span>|<span data-ttu-id="00bd5-p105">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="00bd5-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="00bd5-144">isAllDay</span><span class="sxs-lookup"><span data-stu-id="00bd5-144">isAllDay</span></span> |<span data-ttu-id="00bd5-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="00bd5-145">Boolean</span></span>|<span data-ttu-id="00bd5-146">Indica se o evento dura todo o dia.</span><span class="sxs-lookup"><span data-stu-id="00bd5-146">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="00bd5-147">Ajustar essa propriedade requer ajustar as \*\*\*\* Propriedades StartDateTime e EndDateTime do evento também. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="00bd5-147">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="00bd5-148">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="00bd5-148">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="00bd5-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="00bd5-149">Boolean</span></span>|<span data-ttu-id="00bd5-150">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="00bd5-150">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="00bd5-151">isRead</span><span class="sxs-lookup"><span data-stu-id="00bd5-151">isRead</span></span>|<span data-ttu-id="00bd5-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="00bd5-152">Boolean</span></span>|<span data-ttu-id="00bd5-153">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="00bd5-153">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="00bd5-154">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="00bd5-154">isReadReceiptRequested</span></span>|<span data-ttu-id="00bd5-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="00bd5-155">Boolean</span></span>|<span data-ttu-id="00bd5-156">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="00bd5-156">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="00bd5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="00bd5-157">Response</span></span>

<span data-ttu-id="00bd5-158">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00bd5-158">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00bd5-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00bd5-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00bd5-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00bd5-160">Request</span></span>
<span data-ttu-id="00bd5-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00bd5-161">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="00bd5-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="00bd5-162">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="00bd5-163">C#</span><span class="sxs-lookup"><span data-stu-id="00bd5-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00bd5-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00bd5-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00bd5-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00bd5-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="00bd5-166">Java</span><span class="sxs-lookup"><span data-stu-id="00bd5-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="00bd5-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="00bd5-167">Response</span></span>
<span data-ttu-id="00bd5-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00bd5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
