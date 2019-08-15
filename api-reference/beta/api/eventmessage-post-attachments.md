---
title: Adicionar anexo
description: Use esta API para criar um novo Anexo.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a6a3aebc1873e2a7b79948a130c783f68f466401
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419815"
---
# <a name="add-attachment"></a><span data-ttu-id="b75bf-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="b75bf-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b75bf-104">Use esta API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="b75bf-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="b75bf-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="b75bf-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="b75bf-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="b75bf-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="b75bf-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="b75bf-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="b75bf-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="b75bf-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="b75bf-109">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b75bf-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b75bf-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b75bf-110">Permissions</span></span>
<span data-ttu-id="b75bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b75bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b75bf-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b75bf-113">Permission type</span></span>      | <span data-ttu-id="b75bf-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b75bf-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b75bf-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b75bf-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b75bf-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b75bf-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b75bf-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b75bf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b75bf-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b75bf-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b75bf-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b75bf-119">Application</span></span> | <span data-ttu-id="b75bf-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b75bf-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b75bf-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b75bf-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="b75bf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b75bf-122">Request headers</span></span>
| <span data-ttu-id="b75bf-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b75bf-123">Name</span></span>       | <span data-ttu-id="b75bf-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b75bf-124">Type</span></span> | <span data-ttu-id="b75bf-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b75bf-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b75bf-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b75bf-126">Authorization</span></span>  | <span data-ttu-id="b75bf-127">string</span><span class="sxs-lookup"><span data-stu-id="b75bf-127">string</span></span>  | <span data-ttu-id="b75bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b75bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b75bf-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b75bf-130">Content-Type</span></span> | <span data-ttu-id="b75bf-131">string</span><span class="sxs-lookup"><span data-stu-id="b75bf-131">string</span></span>  | <span data-ttu-id="b75bf-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b75bf-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b75bf-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b75bf-134">Request body</span></span>
<span data-ttu-id="b75bf-135">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b75bf-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b75bf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b75bf-136">Response</span></span>

<span data-ttu-id="b75bf-137">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b75bf-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="b75bf-138">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="b75bf-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="b75bf-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b75bf-139">Request</span></span>
<span data-ttu-id="b75bf-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b75bf-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b75bf-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b75bf-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b75bf-142">C#</span><span class="sxs-lookup"><span data-stu-id="b75bf-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b75bf-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b75bf-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b75bf-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b75bf-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b75bf-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b75bf-145">Response</span></span>
<span data-ttu-id="b75bf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b75bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="b75bf-149">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="b75bf-149">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="b75bf-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b75bf-150">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b75bf-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="b75bf-151">HTTP</span></span>](#tab/http)
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
  "item": "message or event entity"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b75bf-152">C#</span><span class="sxs-lookup"><span data-stu-id="b75bf-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b75bf-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b75bf-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b75bf-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b75bf-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b75bf-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b75bf-155">Response</span></span>
<span data-ttu-id="b75bf-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b75bf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
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
