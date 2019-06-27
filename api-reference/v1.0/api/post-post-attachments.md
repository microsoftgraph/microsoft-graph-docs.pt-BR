---
title: Adicionar anexo
description: Use esta API para adicionar um attachment a uma postagem. Desde lá
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 16b054b093a90f6017c073c77b5656ea56c8bbc3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275184"
---
# <a name="add-attachment"></a><span data-ttu-id="32e1c-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="32e1c-104">Add attachment</span></span>

<span data-ttu-id="32e1c-p102">Use esta API para adicionar um [attachment](../resources/attachment.md) a uma postagem. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="32e1c-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="32e1c-107">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="32e1c-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="32e1c-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="32e1c-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="32e1c-109">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="32e1c-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="32e1c-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="32e1c-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="32e1c-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="32e1c-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="32e1c-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="32e1c-112">Permissions</span></span>
<span data-ttu-id="32e1c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32e1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32e1c-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32e1c-115">Permission type</span></span>      | <span data-ttu-id="32e1c-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32e1c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32e1c-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32e1c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="32e1c-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32e1c-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="32e1c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32e1c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32e1c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32e1c-120">Not supported.</span></span>    |
|<span data-ttu-id="32e1c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32e1c-121">Application</span></span> | <span data-ttu-id="32e1c-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32e1c-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32e1c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32e1c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="32e1c-124">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="32e1c-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="32e1c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32e1c-125">Request headers</span></span>
| <span data-ttu-id="32e1c-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32e1c-126">Header</span></span>       | <span data-ttu-id="32e1c-127">Valor</span><span class="sxs-lookup"><span data-stu-id="32e1c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32e1c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="32e1c-128">Authorization</span></span>  | <span data-ttu-id="32e1c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32e1c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32e1c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32e1c-131">Request body</span></span>
<span data-ttu-id="32e1c-132">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="32e1c-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="32e1c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="32e1c-133">Response</span></span>

<span data-ttu-id="32e1c-134">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32e1c-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="32e1c-135">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="32e1c-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="32e1c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32e1c-136">Request</span></span>
<span data-ttu-id="32e1c-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32e1c-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="32e1c-138">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="32e1c-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="32e1c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="32e1c-139">Response</span></span>
<span data-ttu-id="32e1c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32e1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="32e1c-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="32e1c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="32e1c-144">C#</span><span class="sxs-lookup"><span data-stu-id="32e1c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32e1c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="32e1c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="32e1c-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="32e1c-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="32e1c-147">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="32e1c-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="32e1c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32e1c-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="32e1c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="32e1c-149">Response</span></span>
<span data-ttu-id="32e1c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32e1c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
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
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
