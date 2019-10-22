---
title: Adicionar anexo
description: Adicionar um anexo ao criar uma postagem de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9cef56cbe87db5923accb362804434b1501c32d1
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "36633766"
---
# <a name="add-attachment"></a><span data-ttu-id="21b41-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="21b41-103">Add attachment</span></span>

<span data-ttu-id="21b41-104">Adicionar um [anexo](../resources/attachment.md) ao criar uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="21b41-104">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span>

<span data-ttu-id="21b41-105">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="21b41-105">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="21b41-106">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="21b41-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="21b41-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="21b41-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="21b41-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="21b41-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="21b41-109">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="21b41-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="21b41-110">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="21b41-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="21b41-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="21b41-111">Permissions</span></span>
<span data-ttu-id="21b41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21b41-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21b41-114">Permission type</span></span>      | <span data-ttu-id="21b41-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21b41-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21b41-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21b41-116">Delegated (work or school account)</span></span> | <span data-ttu-id="21b41-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b41-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="21b41-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21b41-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21b41-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21b41-119">Not supported.</span></span>    |
|<span data-ttu-id="21b41-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21b41-120">Application</span></span> | <span data-ttu-id="21b41-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b41-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21b41-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21b41-122">HTTP request</span></span>
<span data-ttu-id="21b41-123">Incluir um anexo ao criar uma [postagem](../resources/post.md) em um [conversationThread](../resources/conversationthread.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="21b41-123">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="21b41-124">A especificação da [conversa](../resources/conversation.md) pai é opcional.</span><span class="sxs-lookup"><span data-stu-id="21b41-124">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="21b41-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21b41-125">Request headers</span></span>
| <span data-ttu-id="21b41-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21b41-126">Header</span></span>       | <span data-ttu-id="21b41-127">Valor</span><span class="sxs-lookup"><span data-stu-id="21b41-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21b41-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="21b41-128">Authorization</span></span>  | <span data-ttu-id="21b41-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21b41-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21b41-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21b41-131">Request body</span></span>
<span data-ttu-id="21b41-132">No corpo da solicitação, forneça um objeto JSON que inclui um parâmetro **post** .</span><span class="sxs-lookup"><span data-stu-id="21b41-132">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="21b41-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="21b41-133">Parameter</span></span>    | <span data-ttu-id="21b41-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="21b41-134">Type</span></span>   |<span data-ttu-id="21b41-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b41-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21b41-136">post</span><span class="sxs-lookup"><span data-stu-id="21b41-136">post</span></span>|[<span data-ttu-id="21b41-137">post</span><span class="sxs-lookup"><span data-stu-id="21b41-137">post</span></span>](../resources/post.md)|<span data-ttu-id="21b41-138">A nova postagem que está sendo respondida, que inclui um ou mais anexos em uma coleção de [anexos](../resources/attachment.md) .</span><span class="sxs-lookup"><span data-stu-id="21b41-138">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="21b41-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="21b41-139">Response</span></span>

<span data-ttu-id="21b41-p104">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21b41-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21b41-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="21b41-142">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="21b41-143">Exemplo 1: incluir um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="21b41-143">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="21b41-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21b41-144">Request</span></span>
<span data-ttu-id="21b41-145">Veja a seguir um exemplo de uma solicitação que inclui um arquivo como um anexo ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="21b41-145">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21b41-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="21b41-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="21b41-147">C#</span><span class="sxs-lookup"><span data-stu-id="21b41-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21b41-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21b41-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21b41-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21b41-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="21b41-150">Java</span><span class="sxs-lookup"><span data-stu-id="21b41-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-with-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="21b41-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="21b41-151">Response</span></span>
<span data-ttu-id="21b41-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21b41-152">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="21b41-153">Exemplo 2: incluir um anexo de item</span><span class="sxs-lookup"><span data-stu-id="21b41-153">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="21b41-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21b41-154">Request</span></span>
<span data-ttu-id="21b41-155">Veja a seguir um exemplo de uma solicitação que inclui um evento como um anexo ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="21b41-155">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
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


#### <a name="response"></a><span data-ttu-id="21b41-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="21b41-156">Response</span></span>
<span data-ttu-id="21b41-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21b41-157">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="21b41-158">Exemplo 3: incluir um anexo de referência</span><span class="sxs-lookup"><span data-stu-id="21b41-158">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="21b41-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21b41-159">Request</span></span>
<span data-ttu-id="21b41-160">Veja a seguir um exemplo de uma solicitação que inclui um anexo de referência ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="21b41-160">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="21b41-161">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="21b41-161">The attachment points to a folder on OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="21b41-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="21b41-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_with_post",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJUdfolA=="]
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="21b41-163">C#</span><span class="sxs-lookup"><span data-stu-id="21b41-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21b41-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21b41-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21b41-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21b41-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="21b41-166">Java</span><span class="sxs-lookup"><span data-stu-id="21b41-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-with-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21b41-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="21b41-167">Response</span></span>
<span data-ttu-id="21b41-168">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21b41-168">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
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
