---
title: Adicionar anexo
description: 'Use esta API para adicionar um anexo a uma mensagem. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 56693a04d6f0579d043b4d745fe53ae61536b82e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540461"
---
# <a name="add-attachment"></a><span data-ttu-id="dd840-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="dd840-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd840-104">Use esta API para adicionar um [anexo](../resources/attachment.md) a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd840-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="dd840-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="dd840-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="dd840-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="dd840-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="dd840-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="dd840-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="dd840-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="dd840-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="dd840-109">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="dd840-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="dd840-110">Você pode adicionar um anexo a uma mensagem existente postando na coleção Attachments ou em uma nova mensagem que está sendo [rascunho](../api/user-post-messages.md), ou [criada e enviada em tempo real](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="dd840-110">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="dd840-111">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="dd840-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd840-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd840-112">Permissions</span></span>
<span data-ttu-id="dd840-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd840-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd840-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd840-115">Permission type</span></span>      | <span data-ttu-id="dd840-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd840-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd840-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd840-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dd840-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd840-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd840-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd840-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd840-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd840-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dd840-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd840-121">Application</span></span> | <span data-ttu-id="dd840-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd840-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd840-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd840-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="dd840-124">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="dd840-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="dd840-125">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="dd840-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="dd840-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="dd840-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dd840-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd840-128">Request headers</span></span>
| <span data-ttu-id="dd840-129">Nome</span><span class="sxs-lookup"><span data-stu-id="dd840-129">Name</span></span>       | <span data-ttu-id="dd840-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd840-130">Type</span></span> | <span data-ttu-id="dd840-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd840-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd840-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd840-132">Authorization</span></span>  | <span data-ttu-id="dd840-133">string</span><span class="sxs-lookup"><span data-stu-id="dd840-133">string</span></span>  | <span data-ttu-id="dd840-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd840-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd840-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd840-136">Content-Type</span></span> | <span data-ttu-id="dd840-137">string</span><span class="sxs-lookup"><span data-stu-id="dd840-137">string</span></span>  | <span data-ttu-id="dd840-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd840-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd840-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd840-140">Request body</span></span>
<span data-ttu-id="dd840-141">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="dd840-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dd840-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd840-142">Response</span></span>

<span data-ttu-id="dd840-143">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd840-143">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="dd840-144">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="dd840-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="dd840-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd840-145">Request</span></span>
<span data-ttu-id="dd840-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd840-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="dd840-147">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="dd840-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dd840-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd840-148">Response</span></span>
<span data-ttu-id="dd840-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd840-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
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
    "contentBytes": "R0lGODdhEAYEAA7"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="dd840-150">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="dd840-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="dd840-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd840-151">Request</span></span>
<span data-ttu-id="dd840-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd840-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message"
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

##### <a name="response"></a><span data-ttu-id="dd840-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd840-153">Response</span></span>
<span data-ttu-id="dd840-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd840-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="dd840-157">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="dd840-157">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="dd840-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd840-158">Request</span></span>
<span data-ttu-id="dd840-159">Veja um exemplo de uma solicitação que adiciona um anexo de referência a uma mensagem existente.</span><span class="sxs-lookup"><span data-stu-id="dd840-159">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="dd840-160">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="dd840-160">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dd840-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd840-161">Response</span></span>
<span data-ttu-id="dd840-162">Veja um exemplo de resposta completa.</span><span class="sxs-lookup"><span data-stu-id="dd840-162">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
