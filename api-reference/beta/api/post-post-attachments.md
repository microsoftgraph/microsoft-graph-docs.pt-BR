---
title: Adicionar anexo
description: Adicionar um anexo ao criar uma postagem de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a8d45943ffc17c5cc949024029bd520d23895df5
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637382"
---
# <a name="add-attachment"></a><span data-ttu-id="a568c-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="a568c-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a568c-104">Adicionar um [anexo](../resources/attachment.md) ao criar uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="a568c-104">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span> 

<span data-ttu-id="a568c-105">Esta operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="a568c-105">This operation limits the size of the attachment you can add to under 4 MB.</span></span>

<span data-ttu-id="a568c-106">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="a568c-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="a568c-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="a568c-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="a568c-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="a568c-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="a568c-109">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="a568c-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="a568c-110">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="a568c-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a568c-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="a568c-111">Permissions</span></span>
<span data-ttu-id="a568c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a568c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a568c-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a568c-114">Permission type</span></span>      | <span data-ttu-id="a568c-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a568c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a568c-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a568c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a568c-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a568c-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a568c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a568c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a568c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a568c-119">Not supported.</span></span>    |
|<span data-ttu-id="a568c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a568c-120">Application</span></span> | <span data-ttu-id="a568c-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a568c-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a568c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a568c-122">HTTP request</span></span>
<span data-ttu-id="a568c-123">Incluir um anexo ao criar uma [postagem](../resources/post.md) em um [conversationThread](../resources/conversationthread.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="a568c-123">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="a568c-124">A especificação da [conversa](../resources/conversation.md) pai é opcional.</span><span class="sxs-lookup"><span data-stu-id="a568c-124">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="a568c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a568c-125">Request headers</span></span>
| <span data-ttu-id="a568c-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a568c-126">Header</span></span>       | <span data-ttu-id="a568c-127">Valor</span><span class="sxs-lookup"><span data-stu-id="a568c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a568c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a568c-128">Authorization</span></span>  | <span data-ttu-id="a568c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a568c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a568c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a568c-131">Request body</span></span>
<span data-ttu-id="a568c-132">No corpo da solicitação, forneça um objeto JSON que inclui um parâmetro **post** .</span><span class="sxs-lookup"><span data-stu-id="a568c-132">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="a568c-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a568c-133">Parameter</span></span>    | <span data-ttu-id="a568c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a568c-134">Type</span></span>   |<span data-ttu-id="a568c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a568c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a568c-136">post</span><span class="sxs-lookup"><span data-stu-id="a568c-136">post</span></span>|[<span data-ttu-id="a568c-137">post</span><span class="sxs-lookup"><span data-stu-id="a568c-137">post</span></span>](../resources/post.md)|<span data-ttu-id="a568c-138">A nova postagem que está sendo respondida, que inclui um ou mais anexos em uma coleção de [anexos](../resources/attachment.md) .</span><span class="sxs-lookup"><span data-stu-id="a568c-138">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="a568c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a568c-139">Response</span></span>

<span data-ttu-id="a568c-p104">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a568c-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a568c-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a568c-142">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="a568c-143">Exemplo 1: incluir um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="a568c-143">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="a568c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a568c-144">Request</span></span>
<span data-ttu-id="a568c-145">Veja a seguir um exemplo de uma solicitação que inclui um arquivo como um anexo ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="a568c-145">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a568c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a568c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "Which quarter does that file cover? See my attachment."
    },
    "attachments": [{
      "@odata.type": "#microsoft.graph.fileAttachment",
      "name": "Another file as attachment",
      "contentBytes": "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
    } ]
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a568c-147">C#</span><span class="sxs-lookup"><span data-stu-id="a568c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a568c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a568c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a568c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a568c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a568c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a568c-150">Response</span></span>
<span data-ttu-id="a568c-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a568c-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="a568c-152">Exemplo 2: incluir um anexo de item</span><span class="sxs-lookup"><span data-stu-id="a568c-152">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="a568c-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a568c-153">Request</span></span>
<span data-ttu-id="a568c-154">Veja a seguir um exemplo de uma solicitação que inclui um evento como um anexo ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="a568c-154">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "I attached an event."
    },
    "attachments": [{
      "@odata.type": "#microsoft.graph.itemAttachment",
      "name": "Holiday event", 
      "item": {
          "@odata.type": "microsoft.graph.event",
          "subject": "Discuss gifts for children",
          "body": {
              "contentType": "HTML",
              "content": "Let's look for funding!"
          },
          "start": {
              "dateTime": "2019-12-02T18:00:00",
              "timeZone": "Pacific Standard Time"
          },
          "end": {
              "dateTime": "2019-12-02T19:00:00",
              "timeZone": "Pacific Standard Time"
          }
      }
    } ]
  }
}
```


#### <a name="response"></a><span data-ttu-id="a568c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="a568c-155">Response</span></span>
<span data-ttu-id="a568c-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a568c-156">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="a568c-157">Exemplo 3: incluir um anexo de referência</span><span class="sxs-lookup"><span data-stu-id="a568c-157">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="a568c-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a568c-158">Request</span></span>
<span data-ttu-id="a568c-159">Veja a seguir um exemplo de uma solicitação que inclui um anexo de referência ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="a568c-159">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="a568c-160">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a568c-160">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a568c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="a568c-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/beta/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "text",
      "content": "I attached a reference to a file on OneDrive."
    },
    "attachments": [{
      "@odata.type": "#microsoft.graph.referenceAttachment", 
      "name": "Personal pictures", 
      "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
      "providerType": "oneDriveConsumer", 
      "permission": "Edit", 
      "isFolder": "True"
    } ]
  }
}
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="a568c-162">C#</span><span class="sxs-lookup"><span data-stu-id="a568c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a568c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a568c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a568c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a568c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a568c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a568c-165">Response</span></span>
<span data-ttu-id="a568c-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a568c-166">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
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
