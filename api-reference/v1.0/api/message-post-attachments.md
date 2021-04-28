---
title: Adicionar anexo
description: 'Use esta API para adicionar um anexo a uma mensagem. '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0d282afb127dba1222f208d0660e6ff584c22834
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052233"
---
# <a name="add-attachment"></a><span data-ttu-id="571ba-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="571ba-103">Add attachment</span></span>

<span data-ttu-id="571ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="571ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="571ba-105">Use esta API para adicionar um [anexo](../resources/attachment.md) a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="571ba-105">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="571ba-106">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="571ba-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="571ba-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="571ba-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="571ba-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="571ba-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="571ba-109">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="571ba-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="571ba-110">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="571ba-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="571ba-111">Você pode adicionar um anexo a uma mensagem existente postando na seu coleção de anexos, ou pode adicionar um anexo a uma mensagem que está sendo [criada e enviada dinamicamente](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="571ba-111">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="571ba-112">Essa operação limita o tamanho do anexo que você pode adicionar a menos de 3 MB.</span><span class="sxs-lookup"><span data-stu-id="571ba-112">This operation limits the size of the attachment you can add to under 3 MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="571ba-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="571ba-113">Permissions</span></span>
<span data-ttu-id="571ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="571ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="571ba-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="571ba-116">Permission type</span></span>      | <span data-ttu-id="571ba-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="571ba-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="571ba-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="571ba-118">Delegated (work or school account)</span></span> | <span data-ttu-id="571ba-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="571ba-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="571ba-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="571ba-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="571ba-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="571ba-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="571ba-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="571ba-122">Application</span></span> | <span data-ttu-id="571ba-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="571ba-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="571ba-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="571ba-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="571ba-125">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="571ba-125">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="571ba-126">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="571ba-126">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="571ba-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante. </span><span class="sxs-lookup"><span data-stu-id="571ba-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="571ba-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="571ba-129">Request headers</span></span>
| <span data-ttu-id="571ba-130">Nome</span><span class="sxs-lookup"><span data-stu-id="571ba-130">Name</span></span>       | <span data-ttu-id="571ba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="571ba-131">Type</span></span> | <span data-ttu-id="571ba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="571ba-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="571ba-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="571ba-133">Authorization</span></span>  | <span data-ttu-id="571ba-134">string</span><span class="sxs-lookup"><span data-stu-id="571ba-134">string</span></span>  | <span data-ttu-id="571ba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="571ba-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="571ba-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="571ba-137">Content-Type</span></span> | <span data-ttu-id="571ba-138">string</span><span class="sxs-lookup"><span data-stu-id="571ba-138">string</span></span>  | <span data-ttu-id="571ba-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="571ba-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="571ba-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="571ba-141">Request body</span></span>
<span data-ttu-id="571ba-142">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="571ba-142">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="571ba-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="571ba-143">Response</span></span>

<span data-ttu-id="571ba-144">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="571ba-144">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="571ba-145">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="571ba-145">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="571ba-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="571ba-146">Request</span></span>
<span data-ttu-id="571ba-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="571ba-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="571ba-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="571ba-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_file_attachment_from_message_v1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```
# <a name="c"></a>[<span data-ttu-id="571ba-149">C#</span><span class="sxs-lookup"><span data-stu-id="571ba-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="571ba-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="571ba-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="571ba-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="571ba-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="571ba-152">Java</span><span class="sxs-lookup"><span data-stu-id="571ba-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-message-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="571ba-153">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="571ba-153">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="571ba-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="571ba-154">Response</span></span>
<span data-ttu-id="571ba-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="571ba-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_message_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 202

{
    "id": "AAMkADNkN2R",
    "lastModifiedDateTime": "2017-01-26T08:48:28Z",
    "name": "smile",
    "contentType": "image/gif",
    "size": 1008,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="571ba-156">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="571ba-156">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="571ba-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="571ba-157">Request</span></span>
<span data-ttu-id="571ba-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="571ba-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "create_item_attachment_from_message_v1"
}-->

```
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 200

{
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
      "dateTime": "2016-12-02T18:00:00",
      "timeZone": "Pacific Standard Time"
    },
    "end": {
      "dateTime": "2016-12-02T19:00:00",
      "timeZone": "Pacific Standard Time"
    }
  }
}
```


##### <a name="response"></a><span data-ttu-id="571ba-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="571ba-159">Response</span></span>
<span data-ttu-id="571ba-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="571ba-160">Here is an example of the response.</span></span> <span data-ttu-id="571ba-161">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="571ba-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_message_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "id":"AAMkADNkNJp5JVnQIe9r0=",
  "lastModifiedDateTime":"2016-12-01T22:27:13Z",
  "name":"Holiday event",
  "contentType":null,
  "size":2473,
  "isInline":false
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
  ]
}-->

