---
title: Adicionar anexo
description: Use esta API para adicionar um attachment a uma postagem. Desde lá
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ffcbc9984774f0e0e59fc2953ddb86d3cc3ce195
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594965"
---
# <a name="add-attachment"></a><span data-ttu-id="9daf4-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="9daf4-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9daf4-p102">Use esta API para adicionar um [attachment](../resources/attachment.md) a uma postagem. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="9daf4-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="9daf4-107">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="9daf4-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="9daf4-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="9daf4-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="9daf4-109">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="9daf4-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="9daf4-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="9daf4-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="9daf4-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9daf4-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9daf4-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="9daf4-112">Permissions</span></span>
<span data-ttu-id="9daf4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9daf4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9daf4-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9daf4-115">Permission type</span></span>      | <span data-ttu-id="9daf4-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9daf4-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9daf4-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9daf4-117">Delegated (work or school account)</span></span> | <span data-ttu-id="9daf4-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9daf4-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9daf4-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9daf4-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9daf4-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9daf4-120">Not supported.</span></span>    |
|<span data-ttu-id="9daf4-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9daf4-121">Application</span></span> | <span data-ttu-id="9daf4-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9daf4-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9daf4-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9daf4-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9daf4-124">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="9daf4-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="9daf4-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9daf4-125">Request headers</span></span>
| <span data-ttu-id="9daf4-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9daf4-126">Header</span></span>       | <span data-ttu-id="9daf4-127">Valor</span><span class="sxs-lookup"><span data-stu-id="9daf4-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9daf4-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9daf4-128">Authorization</span></span>  | <span data-ttu-id="9daf4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9daf4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9daf4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9daf4-131">Request body</span></span>
<span data-ttu-id="9daf4-132">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9daf4-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9daf4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9daf4-133">Response</span></span>

<span data-ttu-id="9daf4-134">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9daf4-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="9daf4-135">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="9daf4-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9daf4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9daf4-136">Request</span></span>
<span data-ttu-id="9daf4-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9daf4-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="9daf4-138">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9daf4-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="9daf4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9daf4-139">Response</span></span>
<span data-ttu-id="9daf4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9daf4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9daf4-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9daf4-143">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9daf4-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9daf4-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="9daf4-145">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="9daf4-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9daf4-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9daf4-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="9daf4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9daf4-147">Response</span></span>
<span data-ttu-id="9daf4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9daf4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9daf4-151">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9daf4-151">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9daf4-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9daf4-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="example-reference-attachment"></a><span data-ttu-id="9daf4-153">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="9daf4-153">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9daf4-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9daf4-154">Request</span></span>
<span data-ttu-id="9daf4-155">Veja um exemplo de uma solicitação que adiciona um anexo de referência a uma postagem existente.</span><span class="sxs-lookup"><span data-stu-id="9daf4-155">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="9daf4-156">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9daf4-156">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_post",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments
Content-type: application/json
Content-length: 319

{ 
    "@odata.type": "#microsoft.graph.referenceAttachment", 
    "name": "Personal pictures", 
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    "providerType": "oneDriveConsumer", 
    "permission": "Edit", 
    "isFolder": "True" 
} 
```

##### <a name="response"></a><span data-ttu-id="9daf4-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9daf4-157">Response</span></span>
<span data-ttu-id="9daf4-158">Veja um exemplo de resposta completa.</span><span class="sxs-lookup"><span data-stu-id="9daf4-158">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PICVGCc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9daf4-159">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9daf4-159">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9daf4-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9daf4-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
