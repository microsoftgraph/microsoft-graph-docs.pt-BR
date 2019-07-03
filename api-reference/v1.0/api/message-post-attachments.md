---
title: Adicionar anexo
description: 'Use esta API para adicionar um anexo a uma mensagem. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4dcbfed0e1401591083876baf29c2e87a4c935d1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443942"
---
# <a name="add-attachment"></a><span data-ttu-id="b8954-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="b8954-103">Add attachment</span></span>

<span data-ttu-id="b8954-104">Use esta API para adicionar um [anexo](../resources/attachment.md) a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b8954-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="b8954-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="b8954-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="b8954-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="b8954-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="b8954-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="b8954-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="b8954-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="b8954-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="b8954-109">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b8954-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="b8954-110">Você pode adicionar um anexo a uma mensagem existente postando na seu coleção de anexos, ou pode adicionar um anexo a uma mensagem que está sendo [criada e enviada dinamicamente](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="b8954-110">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="b8954-111">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="b8954-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8954-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8954-112">Permissions</span></span>
<span data-ttu-id="b8954-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8954-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8954-115">Permission type</span></span>      | <span data-ttu-id="b8954-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8954-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8954-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8954-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b8954-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8954-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8954-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8954-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8954-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8954-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8954-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8954-121">Application</span></span> | <span data-ttu-id="b8954-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8954-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8954-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8954-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b8954-124">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="b8954-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="b8954-125">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b8954-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="b8954-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="b8954-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b8954-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8954-128">Request headers</span></span>
| <span data-ttu-id="b8954-129">Nome</span><span class="sxs-lookup"><span data-stu-id="b8954-129">Name</span></span>       | <span data-ttu-id="b8954-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8954-130">Type</span></span> | <span data-ttu-id="b8954-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8954-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8954-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8954-132">Authorization</span></span>  | <span data-ttu-id="b8954-133">string</span><span class="sxs-lookup"><span data-stu-id="b8954-133">string</span></span>  | <span data-ttu-id="b8954-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8954-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8954-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8954-136">Content-Type</span></span> | <span data-ttu-id="b8954-137">string</span><span class="sxs-lookup"><span data-stu-id="b8954-137">string</span></span>  | <span data-ttu-id="b8954-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8954-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8954-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8954-140">Request body</span></span>
<span data-ttu-id="b8954-141">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b8954-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b8954-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8954-142">Response</span></span>

<span data-ttu-id="b8954-143">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8954-143">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="b8954-144">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="b8954-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="b8954-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8954-145">Request</span></span>
<span data-ttu-id="b8954-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8954-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8954-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8954-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "base64R0lGODdhEAYEAA7"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8954-148">C#</span><span class="sxs-lookup"><span data-stu-id="b8954-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8954-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="b8954-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8954-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b8954-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="b8954-151">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b8954-151">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b8954-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8954-152">Response</span></span>
<span data-ttu-id="b8954-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8954-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
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
    "contentBytes": "base64R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="b8954-154">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="b8954-154">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="b8954-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8954-155">Request</span></span>
<span data-ttu-id="b8954-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8954-156">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->

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


##### <a name="response"></a><span data-ttu-id="b8954-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8954-157">Response</span></span>
<span data-ttu-id="b8954-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8954-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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
