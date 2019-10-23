---
title: Adicionar anexo
description: 'Use esta API para adicionar um anexo a uma mensagem. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 05cdbdbc5cc044f30a3dd2f8ea63dcf6fac50222
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637564"
---
# <a name="add-attachment"></a><span data-ttu-id="fa034-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="fa034-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa034-104">Use esta API para adicionar um [anexo](../resources/attachment.md) a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="fa034-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="fa034-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="fa034-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="fa034-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="fa034-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="fa034-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="fa034-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="fa034-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="fa034-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="fa034-109">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="fa034-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="fa034-110">Você pode adicionar um anexo a uma [mensagem](../resources/message.md) existente postando na coleção Attachments ou em uma nova mensagem que está sendo [rascunho](../api/user-post-messages.md), ou [criada e enviada em tempo real](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="fa034-110">You can add an attachment to an existing [message](../resources/message.md) by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

><span data-ttu-id="fa034-111">**Observação**: esta operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="fa034-111">**Note**: This operation limits the size of the attachment you can add to under 4 MB.</span></span>
>
> <span data-ttu-id="fa034-112">No entanto, se estiver anexando a uma mensagem um arquivo entre 3 MB e 150MB, você pode [criar uma sessão de carregamento](attachment-createuploadsession.md) e carregar de forma iterativa os intervalos do arquivo para anexá-lo.</span><span class="sxs-lookup"><span data-stu-id="fa034-112">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="fa034-113">Consulte [anexar arquivos grandes às mensagens do Outlook](/graph/outlook-large-attachments) para obter um exemplo.</span><span class="sxs-lookup"><span data-stu-id="fa034-113">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa034-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa034-114">Permissions</span></span>
<span data-ttu-id="fa034-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa034-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa034-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa034-117">Permission type</span></span>      | <span data-ttu-id="fa034-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa034-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa034-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa034-119">Delegated (work or school account)</span></span> | <span data-ttu-id="fa034-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa034-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fa034-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa034-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa034-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa034-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fa034-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa034-123">Application</span></span> | <span data-ttu-id="fa034-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa034-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa034-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa034-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="fa034-126">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="fa034-126">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="fa034-127">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="fa034-127">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="fa034-p103">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante. </span><span class="sxs-lookup"><span data-stu-id="fa034-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fa034-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa034-130">Request headers</span></span>
| <span data-ttu-id="fa034-131">Nome</span><span class="sxs-lookup"><span data-stu-id="fa034-131">Name</span></span>       | <span data-ttu-id="fa034-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa034-132">Type</span></span> | <span data-ttu-id="fa034-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa034-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fa034-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa034-134">Authorization</span></span>  | <span data-ttu-id="fa034-135">string</span><span class="sxs-lookup"><span data-stu-id="fa034-135">string</span></span>  | <span data-ttu-id="fa034-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa034-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa034-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa034-138">Content-Type</span></span> | <span data-ttu-id="fa034-139">string</span><span class="sxs-lookup"><span data-stu-id="fa034-139">string</span></span>  | <span data-ttu-id="fa034-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa034-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa034-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa034-142">Request body</span></span>
<span data-ttu-id="fa034-143">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="fa034-143">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fa034-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa034-144">Response</span></span>

<span data-ttu-id="fa034-145">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa034-145">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="fa034-146">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="fa034-146">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="fa034-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa034-147">Request</span></span>
<span data-ttu-id="fa034-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa034-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa034-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa034-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa034-150">C#</span><span class="sxs-lookup"><span data-stu-id="fa034-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa034-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa034-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa034-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa034-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="fa034-153">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="fa034-153">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fa034-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa034-154">Response</span></span>
<span data-ttu-id="fa034-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa034-155">Here is an example of the response.</span></span> 
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

## <a name="example-item-attachment"></a><span data-ttu-id="fa034-156">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="fa034-156">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="fa034-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa034-157">Request</span></span>
<span data-ttu-id="fa034-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa034-158">Here is an example of the request.</span></span>

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


##### <a name="response"></a><span data-ttu-id="fa034-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa034-159">Response</span></span>
<span data-ttu-id="fa034-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa034-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="fa034-163">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="fa034-163">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="fa034-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa034-164">Request</span></span>
<span data-ttu-id="fa034-165">Veja um exemplo de uma solicitação que adiciona um anexo de referência a uma mensagem existente.</span><span class="sxs-lookup"><span data-stu-id="fa034-165">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="fa034-166">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fa034-166">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa034-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa034-167">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa034-168">C#</span><span class="sxs-lookup"><span data-stu-id="fa034-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa034-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa034-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa034-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa034-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fa034-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa034-171">Response</span></span>
<span data-ttu-id="fa034-172">Veja um exemplo de resposta completa.</span><span class="sxs-lookup"><span data-stu-id="fa034-172">Here is an example of a full response.</span></span>
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
