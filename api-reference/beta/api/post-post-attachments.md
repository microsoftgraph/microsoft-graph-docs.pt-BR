---
title: Adicionar anexo
description: Use essa API para adicionar um anexo a uma publicação. Desde daí
author: dkershaw10
ms.openlocfilehash: 67e219c7ffd95a41926be97323a2215625b30d2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328340"
---
# <a name="add-attachment"></a><span data-ttu-id="f20f6-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="f20f6-104">Add attachment</span></span>

> <span data-ttu-id="f20f6-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f20f6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f20f6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f20f6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f20f6-p103">Use esta API para adicionar um [attachment](../resources/attachment.md) a uma postagem. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="f20f6-p103">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="f20f6-109">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="f20f6-109">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="f20f6-110">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f20f6-110">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="f20f6-111">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f20f6-111">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="f20f6-112">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f20f6-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="f20f6-113">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f20f6-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f20f6-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="f20f6-114">Permissions</span></span>
<span data-ttu-id="f20f6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f20f6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f20f6-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f20f6-117">Permission type</span></span>      | <span data-ttu-id="f20f6-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f20f6-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f20f6-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f20f6-119">Delegated (work or school account)</span></span> | <span data-ttu-id="f20f6-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f20f6-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f20f6-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f20f6-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f20f6-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f20f6-122">Not supported.</span></span>    |
|<span data-ttu-id="f20f6-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f20f6-123">Application</span></span> | <span data-ttu-id="f20f6-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f20f6-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f20f6-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f20f6-125">HTTP request</span></span>
<span data-ttu-id="f20f6-126"><!-- { "blockType": "ignored" } -->Anexos de uma [postagem](../resources/post.md) em um [segmento](../resources/conversationthread.md) pertencente a uma [conversa](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="f20f6-126"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="f20f6-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f20f6-127">Request headers</span></span>
| <span data-ttu-id="f20f6-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f20f6-128">Header</span></span>       | <span data-ttu-id="f20f6-129">Valor</span><span class="sxs-lookup"><span data-stu-id="f20f6-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f20f6-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="f20f6-130">Authorization</span></span>  | <span data-ttu-id="f20f6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f20f6-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f20f6-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f20f6-133">Request body</span></span>
<span data-ttu-id="f20f6-134">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f20f6-134">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f20f6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f20f6-135">Response</span></span>

<span data-ttu-id="f20f6-136">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f20f6-136">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f20f6-137">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="f20f6-137">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f20f6-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f20f6-138">Request</span></span>
<span data-ttu-id="f20f6-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f20f6-139">Here is an example of the request.</span></span>
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

<span data-ttu-id="f20f6-140">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f20f6-140">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f20f6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f20f6-141">Response</span></span>
<span data-ttu-id="f20f6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f20f6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="f20f6-145">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="f20f6-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f20f6-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f20f6-146">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="f20f6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f20f6-147">Response</span></span>
<span data-ttu-id="f20f6-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f20f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="example-reference-attachment"></a><span data-ttu-id="f20f6-151">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="f20f6-151">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f20f6-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f20f6-152">Request</span></span>
<span data-ttu-id="f20f6-153">Aqui está um exemplo de uma solicitação que adiciona um anexo de referência a uma postagem existente.</span><span class="sxs-lookup"><span data-stu-id="f20f6-153">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="f20f6-154">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f20f6-154">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f20f6-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="f20f6-155">Response</span></span>
<span data-ttu-id="f20f6-156">Aqui está um exemplo de uma resposta completa.</span><span class="sxs-lookup"><span data-stu-id="f20f6-156">Here is an example of a full response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
