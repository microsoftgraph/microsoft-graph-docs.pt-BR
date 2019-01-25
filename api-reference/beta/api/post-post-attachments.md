---
title: Adicionar anexo
description: Use essa API para adicionar um anexo a uma publicação. Desde daí
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4349673b5400674394db33540f09a407a0a6af33
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527889"
---
# <a name="add-attachment"></a><span data-ttu-id="f2de8-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="f2de8-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2de8-p102">Use esta API para adicionar um [attachment](../resources/attachment.md) a uma postagem. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="f2de8-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="f2de8-107">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="f2de8-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="f2de8-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f2de8-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="f2de8-109">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f2de8-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="f2de8-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f2de8-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="f2de8-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f2de8-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f2de8-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2de8-112">Permissions</span></span>
<span data-ttu-id="f2de8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2de8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2de8-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2de8-115">Permission type</span></span>      | <span data-ttu-id="f2de8-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2de8-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2de8-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2de8-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f2de8-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2de8-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2de8-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2de8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2de8-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2de8-120">Not supported.</span></span>    |
|<span data-ttu-id="f2de8-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2de8-121">Application</span></span> | <span data-ttu-id="f2de8-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2de8-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2de8-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2de8-123">HTTP request</span></span>
<span data-ttu-id="f2de8-124"><!-- { "blockType": "ignored" } -->Anexos de uma [postagem](../resources/post.md) em um [segmento](../resources/conversationthread.md) pertencente a uma [conversa](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="f2de8-124"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="f2de8-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2de8-125">Request headers</span></span>
| <span data-ttu-id="f2de8-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2de8-126">Header</span></span>       | <span data-ttu-id="f2de8-127">Valor</span><span class="sxs-lookup"><span data-stu-id="f2de8-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2de8-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2de8-128">Authorization</span></span>  | <span data-ttu-id="f2de8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2de8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2de8-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2de8-131">Request body</span></span>
<span data-ttu-id="f2de8-132">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f2de8-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f2de8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2de8-133">Response</span></span>

<span data-ttu-id="f2de8-134">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2de8-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f2de8-135">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="f2de8-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f2de8-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2de8-136">Request</span></span>
<span data-ttu-id="f2de8-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2de8-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="f2de8-138">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f2de8-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f2de8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2de8-139">Response</span></span>
<span data-ttu-id="f2de8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2de8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="f2de8-143">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="f2de8-143">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f2de8-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2de8-144">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="f2de8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2de8-145">Response</span></span>
<span data-ttu-id="f2de8-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2de8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="example-reference-attachment"></a><span data-ttu-id="f2de8-149">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="f2de8-149">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f2de8-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2de8-150">Request</span></span>
<span data-ttu-id="f2de8-151">Aqui está um exemplo de uma solicitação que adiciona um anexo de referência a uma postagem existente.</span><span class="sxs-lookup"><span data-stu-id="f2de8-151">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="f2de8-152">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f2de8-152">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f2de8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2de8-153">Response</span></span>
<span data-ttu-id="f2de8-154">Aqui está um exemplo de uma resposta completa.</span><span class="sxs-lookup"><span data-stu-id="f2de8-154">Here is an example of a full response.</span></span>
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
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
