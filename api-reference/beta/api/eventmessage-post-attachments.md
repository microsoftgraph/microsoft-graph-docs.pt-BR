---
title: Adicionar anexo
description: Use esta API para criar um novo Anexo.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a047967c1b6d1aaadaef56f22390ac8f1b2a1d31
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787004"
---
# <a name="add-attachment"></a><span data-ttu-id="53b3b-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="53b3b-103">Add attachment</span></span>

<span data-ttu-id="53b3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53b3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53b3b-105">Use esta API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="53b3b-105">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="53b3b-106">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="53b3b-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="53b3b-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="53b3b-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="53b3b-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="53b3b-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="53b3b-109">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="53b3b-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="53b3b-110">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="53b3b-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="53b3b-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="53b3b-111">Permissions</span></span>
<span data-ttu-id="53b3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b3b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53b3b-114">Permission type</span></span>      | <span data-ttu-id="53b3b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53b3b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53b3b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53b3b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="53b3b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53b3b-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53b3b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53b3b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53b3b-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53b3b-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53b3b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53b3b-120">Application</span></span> | <span data-ttu-id="53b3b-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53b3b-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="53b3b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53b3b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="53b3b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53b3b-123">Request headers</span></span>
| <span data-ttu-id="53b3b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="53b3b-124">Name</span></span>       | <span data-ttu-id="53b3b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="53b3b-125">Type</span></span> | <span data-ttu-id="53b3b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="53b3b-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53b3b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="53b3b-127">Authorization</span></span>  | <span data-ttu-id="53b3b-128">string</span><span class="sxs-lookup"><span data-stu-id="53b3b-128">string</span></span>  | <span data-ttu-id="53b3b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53b3b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53b3b-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53b3b-131">Content-Type</span></span> | <span data-ttu-id="53b3b-132">string</span><span class="sxs-lookup"><span data-stu-id="53b3b-132">string</span></span>  | <span data-ttu-id="53b3b-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53b3b-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53b3b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53b3b-135">Request body</span></span>
<span data-ttu-id="53b3b-136">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="53b3b-136">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="53b3b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b3b-137">Response</span></span>

<span data-ttu-id="53b3b-138">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53b3b-138">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="53b3b-139">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="53b3b-139">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="53b3b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53b3b-140">Request</span></span>
<span data-ttu-id="53b3b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53b3b-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53b3b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b3b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```
# <a name="c"></a>[<span data-ttu-id="53b3b-143">C#</span><span class="sxs-lookup"><span data-stu-id="53b3b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53b3b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b3b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53b3b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b3b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53b3b-146">Java</span><span class="sxs-lookup"><span data-stu-id="53b3b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53b3b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b3b-147">Response</span></span>
<span data-ttu-id="53b3b-p104">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="53b3b-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="53b3b-150">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="53b3b-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="53b3b-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53b3b-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="53b3b-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b3b-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": {
    "@odata.type": "microsoft.graph.message"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="53b3b-153">C#</span><span class="sxs-lookup"><span data-stu-id="53b3b-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53b3b-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b3b-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53b3b-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b3b-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53b3b-156">Java</span><span class="sxs-lookup"><span data-stu-id="53b3b-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-item-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53b3b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b3b-157">Response</span></span>
<span data-ttu-id="53b3b-p105">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="53b3b-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


