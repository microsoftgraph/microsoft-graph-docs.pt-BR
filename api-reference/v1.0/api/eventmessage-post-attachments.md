---
title: Adicionar anexo
description: Use esta API para criar um novo Anexo.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c1b61c1a0f2cfc54760f6bcf6f2ad6781cabd8ae
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275912"
---
# <a name="add-attachment"></a><span data-ttu-id="f1a47-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="f1a47-103">Add attachment</span></span>

<span data-ttu-id="f1a47-104">Use esta API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="f1a47-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="f1a47-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="f1a47-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="f1a47-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f1a47-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="f1a47-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f1a47-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="f1a47-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f1a47-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="f1a47-109">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f1a47-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f1a47-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1a47-110">Permissions</span></span>
<span data-ttu-id="f1a47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a47-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1a47-113">Permission type</span></span>      | <span data-ttu-id="f1a47-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1a47-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1a47-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1a47-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f1a47-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1a47-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f1a47-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1a47-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a47-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1a47-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f1a47-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1a47-119">Application</span></span> | <span data-ttu-id="f1a47-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1a47-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1a47-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a47-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="f1a47-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a47-122">Request headers</span></span>
| <span data-ttu-id="f1a47-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f1a47-123">Name</span></span>       | <span data-ttu-id="f1a47-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1a47-124">Type</span></span> | <span data-ttu-id="f1a47-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1a47-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1a47-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1a47-126">Authorization</span></span>  | <span data-ttu-id="f1a47-127">string</span><span class="sxs-lookup"><span data-stu-id="f1a47-127">string</span></span>  | <span data-ttu-id="f1a47-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1a47-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1a47-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1a47-130">Content-Type</span></span> | <span data-ttu-id="f1a47-131">string</span><span class="sxs-lookup"><span data-stu-id="f1a47-131">string</span></span>  | <span data-ttu-id="f1a47-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1a47-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1a47-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a47-134">Request body</span></span>
<span data-ttu-id="f1a47-135">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f1a47-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f1a47-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a47-136">Response</span></span>

<span data-ttu-id="f1a47-137">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a47-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f1a47-138">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="f1a47-138">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="f1a47-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a47-139">Request</span></span>
<span data-ttu-id="f1a47-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1a47-140">Here is an example of the request.</span></span>
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

<span data-ttu-id="f1a47-141">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f1a47-141">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f1a47-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a47-142">Response</span></span>
<span data-ttu-id="f1a47-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1a47-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1a47-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f1a47-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1a47-147">C#</span><span class="sxs-lookup"><span data-stu-id="f1a47-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1a47-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1a47-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f1a47-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f1a47-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="f1a47-150">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="f1a47-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f1a47-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a47-151">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="f1a47-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a47-152">Response</span></span>
<span data-ttu-id="f1a47-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1a47-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f1a47-156">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f1a47-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f1a47-157">C#</span><span class="sxs-lookup"><span data-stu-id="f1a47-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1a47-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1a47-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f1a47-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f1a47-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
