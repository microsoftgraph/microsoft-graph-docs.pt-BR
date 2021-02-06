---
title: Adicionar anexo
description: 'Use esta API para adicionar um anexo a uma mensagem. '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 61776660883cdcf9ea8d6122e2e84c5b63505935
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131170"
---
# <a name="add-attachment"></a><span data-ttu-id="08dcd-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="08dcd-103">Add attachment</span></span>

<span data-ttu-id="08dcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08dcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08dcd-105">Use esta API para adicionar um [anexo](../resources/attachment.md) a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="08dcd-105">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="08dcd-106">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="08dcd-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="08dcd-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="08dcd-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="08dcd-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="08dcd-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="08dcd-109">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="08dcd-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="08dcd-110">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="08dcd-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="08dcd-111">Você pode adicionar um anexo [](../resources/message.md) a uma mensagem existente postando em sua coleção de anexos ou em uma nova mensagem que está sendo redigida [ou](../api/user-post-messages.md)criada e enviada em [tempo real.](../api/user-sendmail.md)</span><span class="sxs-lookup"><span data-stu-id="08dcd-111">You can add an attachment to an existing [message](../resources/message.md) by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

><span data-ttu-id="08dcd-112">**Observação:** essa operação limita o tamanho do anexo que você pode adicionar a menos de 3 MB.</span><span class="sxs-lookup"><span data-stu-id="08dcd-112">**Note**: This operation limits the size of the attachment you can add to under 3 MB.</span></span>
>
> <span data-ttu-id="08dcd-113">No entanto, se você estiver anexando a uma mensagem um arquivo entre 3 MB e 150 MB, poderá criar uma sessão de [upload](attachment-createuploadsession.md) e carregar iterativamente intervalos do arquivo para anexá-lo.</span><span class="sxs-lookup"><span data-stu-id="08dcd-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="08dcd-114">Veja [anexar arquivos grandes a mensagens do Outlook](/graph/outlook-large-attachments) para ver um exemplo.</span><span class="sxs-lookup"><span data-stu-id="08dcd-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>
## <a name="permissions"></a><span data-ttu-id="08dcd-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="08dcd-115">Permissions</span></span>
<span data-ttu-id="08dcd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08dcd-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08dcd-118">Permission type</span></span>      | <span data-ttu-id="08dcd-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08dcd-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08dcd-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08dcd-120">Delegated (work or school account)</span></span> | <span data-ttu-id="08dcd-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08dcd-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="08dcd-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08dcd-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08dcd-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08dcd-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="08dcd-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08dcd-124">Application</span></span> | <span data-ttu-id="08dcd-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08dcd-125">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="08dcd-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08dcd-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="08dcd-127">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="08dcd-127">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="08dcd-128">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="08dcd-128">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="08dcd-p103">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante. </span><span class="sxs-lookup"><span data-stu-id="08dcd-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="08dcd-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08dcd-131">Request headers</span></span>
| <span data-ttu-id="08dcd-132">Nome</span><span class="sxs-lookup"><span data-stu-id="08dcd-132">Name</span></span>       | <span data-ttu-id="08dcd-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="08dcd-133">Type</span></span> | <span data-ttu-id="08dcd-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="08dcd-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08dcd-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="08dcd-135">Authorization</span></span>  | <span data-ttu-id="08dcd-136">string</span><span class="sxs-lookup"><span data-stu-id="08dcd-136">string</span></span>  | <span data-ttu-id="08dcd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08dcd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08dcd-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08dcd-139">Content-Type</span></span> | <span data-ttu-id="08dcd-140">string</span><span class="sxs-lookup"><span data-stu-id="08dcd-140">string</span></span>  | <span data-ttu-id="08dcd-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08dcd-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08dcd-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08dcd-143">Request body</span></span>
<span data-ttu-id="08dcd-144">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="08dcd-144">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="08dcd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="08dcd-145">Response</span></span>

<span data-ttu-id="08dcd-146">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08dcd-146">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="08dcd-147">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="08dcd-147">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="08dcd-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08dcd-148">Request</span></span>
<span data-ttu-id="08dcd-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08dcd-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08dcd-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="08dcd-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message_beta"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "a0b1c76de9f7="
}
```
# <a name="c"></a>[<span data-ttu-id="08dcd-151">C#</span><span class="sxs-lookup"><span data-stu-id="08dcd-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08dcd-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08dcd-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08dcd-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08dcd-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08dcd-154">Java</span><span class="sxs-lookup"><span data-stu-id="08dcd-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-message-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="08dcd-155">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="08dcd-155">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="08dcd-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="08dcd-156">Response</span></span>
<span data-ttu-id="08dcd-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08dcd-157">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_message_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 201 Created
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
    "contentBytes": "a0b1c76de9f7="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="08dcd-158">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="08dcd-158">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="08dcd-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08dcd-159">Request</span></span>
<span data-ttu-id="08dcd-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08dcd-160">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message_beta"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
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


##### <a name="response"></a><span data-ttu-id="08dcd-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="08dcd-161">Response</span></span>
<span data-ttu-id="08dcd-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08dcd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_message_beta",
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

## <a name="example-reference-attachment"></a><span data-ttu-id="08dcd-165">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="08dcd-165">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="08dcd-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08dcd-166">Request</span></span>
<span data-ttu-id="08dcd-167">Aqui está um exemplo de uma solicitação que adiciona um anexo de referência a uma mensagem existente.</span><span class="sxs-lookup"><span data-stu-id="08dcd-167">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="08dcd-168">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="08dcd-168">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="08dcd-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="08dcd-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_message",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M88AADUv0uFAAA=/attachments
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
# <a name="c"></a>[<span data-ttu-id="08dcd-170">C#</span><span class="sxs-lookup"><span data-stu-id="08dcd-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08dcd-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08dcd-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08dcd-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08dcd-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08dcd-173">Java</span><span class="sxs-lookup"><span data-stu-id="08dcd-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-from-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08dcd-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="08dcd-174">Response</span></span>
<span data-ttu-id="08dcd-175">Aqui está um exemplo de uma resposta completa.</span><span class="sxs-lookup"><span data-stu-id="08dcd-175">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_from_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/messages/AAMkAGE1M88AADUv0uFAAA%3D/attachments/$entity",
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
  "tocPath": ""
}
-->


