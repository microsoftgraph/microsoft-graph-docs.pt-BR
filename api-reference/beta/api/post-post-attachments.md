---
title: Adicionar anexo
description: Adicionar um anexo ao criar uma postagem de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 62fe2fdc347c7c74eaedd57e844978ea87c2f275
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455461"
---
# <a name="add-attachment"></a><span data-ttu-id="4903a-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="4903a-103">Add attachment</span></span>

<span data-ttu-id="4903a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4903a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4903a-105">Adicionar um [anexo](../resources/attachment.md) ao criar uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="4903a-105">Add an [attachment](../resources/attachment.md) when creating a group post.</span></span> 

<span data-ttu-id="4903a-106">Esta operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="4903a-106">This operation limits the size of the attachment you can add to under 4 MB.</span></span>

<span data-ttu-id="4903a-107">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="4903a-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="4903a-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4903a-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="4903a-109">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4903a-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="4903a-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4903a-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="4903a-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="4903a-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4903a-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="4903a-112">Permissions</span></span>
<span data-ttu-id="4903a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4903a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4903a-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4903a-115">Permission type</span></span>      | <span data-ttu-id="4903a-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4903a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4903a-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4903a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4903a-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4903a-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4903a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4903a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4903a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4903a-120">Not supported.</span></span>    |
|<span data-ttu-id="4903a-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4903a-121">Application</span></span> | <span data-ttu-id="4903a-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4903a-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4903a-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4903a-123">HTTP request</span></span>
<span data-ttu-id="4903a-124">Incluir um anexo ao criar uma [postagem](../resources/post.md) em um [conversationThread](../resources/conversationthread.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="4903a-124">Include an attachment when creating a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="4903a-125">A especificação da [conversa](../resources/conversation.md) pai é opcional.</span><span class="sxs-lookup"><span data-stu-id="4903a-125">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="4903a-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4903a-126">Request headers</span></span>
| <span data-ttu-id="4903a-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4903a-127">Header</span></span>       | <span data-ttu-id="4903a-128">Valor</span><span class="sxs-lookup"><span data-stu-id="4903a-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4903a-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="4903a-129">Authorization</span></span>  | <span data-ttu-id="4903a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4903a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4903a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4903a-132">Request body</span></span>
<span data-ttu-id="4903a-133">No corpo da solicitação, forneça um objeto JSON que inclui um parâmetro **post** .</span><span class="sxs-lookup"><span data-stu-id="4903a-133">In the request body, provide a JSON object that includes a **post** parameter.</span></span>

| <span data-ttu-id="4903a-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4903a-134">Parameter</span></span>    | <span data-ttu-id="4903a-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="4903a-135">Type</span></span>   |<span data-ttu-id="4903a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="4903a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4903a-137">post</span><span class="sxs-lookup"><span data-stu-id="4903a-137">post</span></span>|[<span data-ttu-id="4903a-138">post</span><span class="sxs-lookup"><span data-stu-id="4903a-138">post</span></span>](../resources/post.md)|<span data-ttu-id="4903a-139">A nova postagem que está sendo respondida, que inclui um ou mais anexos em uma coleção de [anexos](../resources/attachment.md) .</span><span class="sxs-lookup"><span data-stu-id="4903a-139">The new post that is being replied with, which includes one or more attachments in an [attachment](../resources/attachment.md) collection.</span></span>|

## <a name="response"></a><span data-ttu-id="4903a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4903a-140">Response</span></span>

<span data-ttu-id="4903a-p104">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4903a-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4903a-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4903a-143">Examples</span></span>
### <a name="example-1-include-a-file-attachment"></a><span data-ttu-id="4903a-144">Exemplo 1: incluir um anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="4903a-144">Example 1: Include a file attachment</span></span>
#### <a name="request"></a><span data-ttu-id="4903a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4903a-145">Request</span></span>
<span data-ttu-id="4903a-146">Veja a seguir um exemplo de uma solicitação que inclui um arquivo como um anexo ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="4903a-146">Here is an example of a request that includes a file as an attachment when creating a post.</span></span>

# <a name="http"></a>[<span data-ttu-id="4903a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="4903a-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4903a-148">C#</span><span class="sxs-lookup"><span data-stu-id="4903a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4903a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4903a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4903a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4903a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4903a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="4903a-151">Response</span></span>
<span data-ttu-id="4903a-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4903a-152">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accpted
```

### <a name="example-2-include-an-item-attachment"></a><span data-ttu-id="4903a-153">Exemplo 2: incluir um anexo de item</span><span class="sxs-lookup"><span data-stu-id="4903a-153">Example 2: Include an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4903a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4903a-154">Request</span></span>
<span data-ttu-id="4903a-155">Veja a seguir um exemplo de uma solicitação que inclui um evento como um anexo ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="4903a-155">Here is an example of a request that includes an event as an attachment when creating a post.</span></span>

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


#### <a name="response"></a><span data-ttu-id="4903a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="4903a-156">Response</span></span>
<span data-ttu-id="4903a-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4903a-157">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_with_post"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-3-include-a-reference-attachment"></a><span data-ttu-id="4903a-158">Exemplo 3: incluir um anexo de referência</span><span class="sxs-lookup"><span data-stu-id="4903a-158">Example 3: Include a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="4903a-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4903a-159">Request</span></span>
<span data-ttu-id="4903a-160">Veja a seguir um exemplo de uma solicitação que inclui um anexo de referência ao criar uma postagem.</span><span class="sxs-lookup"><span data-stu-id="4903a-160">Here is an example of a request that includes a reference attachment when creating a post.</span></span>
<span data-ttu-id="4903a-161">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4903a-161">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="4903a-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="4903a-162">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="4903a-163">C#</span><span class="sxs-lookup"><span data-stu-id="4903a-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-with-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4903a-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4903a-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-with-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4903a-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4903a-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-with-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4903a-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4903a-166">Response</span></span>
<span data-ttu-id="4903a-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4903a-167">Here is an example of the response.</span></span>
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
