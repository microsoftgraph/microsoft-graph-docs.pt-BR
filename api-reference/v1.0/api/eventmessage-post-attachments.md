---
title: Adicionar anexo
description: Use esta API para criar um novo Anexo.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dcf49756cfb62659b4125a0d10b52ddb804502dc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319178"
---
# <a name="add-attachment"></a><span data-ttu-id="c901a-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="c901a-103">Add attachment</span></span>

<span data-ttu-id="c901a-104">Use esta API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="c901a-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="c901a-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="c901a-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="c901a-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="c901a-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="c901a-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="c901a-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="c901a-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="c901a-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="c901a-109">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c901a-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c901a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c901a-110">Permissions</span></span>
<span data-ttu-id="c901a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c901a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c901a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c901a-113">Permission type</span></span>      | <span data-ttu-id="c901a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c901a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c901a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c901a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c901a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c901a-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c901a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c901a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c901a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c901a-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c901a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c901a-119">Application</span></span> | <span data-ttu-id="c901a-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c901a-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c901a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c901a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="c901a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c901a-122">Request headers</span></span>
| <span data-ttu-id="c901a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c901a-123">Name</span></span>       | <span data-ttu-id="c901a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c901a-124">Type</span></span> | <span data-ttu-id="c901a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c901a-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c901a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c901a-126">Authorization</span></span>  | <span data-ttu-id="c901a-127">string</span><span class="sxs-lookup"><span data-stu-id="c901a-127">string</span></span>  | <span data-ttu-id="c901a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c901a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c901a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c901a-130">Content-Type</span></span> | <span data-ttu-id="c901a-131">string</span><span class="sxs-lookup"><span data-stu-id="c901a-131">string</span></span>  | <span data-ttu-id="c901a-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c901a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c901a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c901a-134">Request body</span></span>
<span data-ttu-id="c901a-135">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c901a-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c901a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c901a-136">Response</span></span>

<span data-ttu-id="c901a-137">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c901a-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="c901a-138">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="c901a-138">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="c901a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c901a-139">Request</span></span>
<span data-ttu-id="c901a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c901a-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c901a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c901a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "base64-contentBytes-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c901a-142">C#</span><span class="sxs-lookup"><span data-stu-id="c901a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c901a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c901a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c901a-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c901a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c901a-145">Java</span><span class="sxs-lookup"><span data-stu-id="c901a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c901a-146">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c901a-146">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c901a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c901a-147">Response</span></span>
<span data-ttu-id="c901a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c901a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="c901a-151">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="c901a-151">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="c901a-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c901a-152">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c901a-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="c901a-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c901a-154">C#</span><span class="sxs-lookup"><span data-stu-id="c901a-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c901a-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c901a-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c901a-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c901a-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c901a-157">Java</span><span class="sxs-lookup"><span data-stu-id="c901a-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-item-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c901a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c901a-158">Response</span></span>
<span data-ttu-id="c901a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c901a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
