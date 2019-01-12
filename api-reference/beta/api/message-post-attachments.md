---
title: Adicionar anexo
description: 'Use esta API para adicionar um anexo a uma mensagem. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fc24c0a444c07dc8fb8e33814498fe5454b1b3fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991899"
---
# <a name="add-attachment"></a><span data-ttu-id="1fd6b-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="1fd6b-103">Add attachment</span></span>

> <span data-ttu-id="1fd6b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fd6b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1fd6b-106">Use esta API para adicionar um [anexo](../resources/attachment.md) a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-106">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="1fd6b-107">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="1fd6b-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="1fd6b-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="1fd6b-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="1fd6b-109">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="1fd6b-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="1fd6b-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="1fd6b-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="1fd6b-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="1fd6b-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="1fd6b-112">Você pode adicionar um anexo a uma mensagem existente pelo lançamento em sua coleção de anexos ou a uma nova mensagem que está sendo [escreveu](../api/user-post-messages.md)ou [criado e enviado dinamicamente](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="1fd6b-112">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="1fd6b-113">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-113">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="1fd6b-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fd6b-114">Permissions</span></span>
<span data-ttu-id="1fd6b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fd6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd6b-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fd6b-117">Permission type</span></span>      | <span data-ttu-id="1fd6b-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fd6b-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fd6b-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fd6b-119">Delegated (work or school account)</span></span> | <span data-ttu-id="1fd6b-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fd6b-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1fd6b-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fd6b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fd6b-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fd6b-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1fd6b-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fd6b-123">Application</span></span> | <span data-ttu-id="1fd6b-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fd6b-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fd6b-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd6b-125">HTTP request</span></span>
<span data-ttu-id="1fd6b-126"><!-- { "blockType": "ignored" } -->Anexos de uma [mensagem](../resources/message.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-126"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="1fd6b-127">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-127">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="1fd6b-p103">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1fd6b-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd6b-130">Request headers</span></span>
| <span data-ttu-id="1fd6b-131">Nome</span><span class="sxs-lookup"><span data-stu-id="1fd6b-131">Name</span></span>       | <span data-ttu-id="1fd6b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fd6b-132">Type</span></span> | <span data-ttu-id="1fd6b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fd6b-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fd6b-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fd6b-134">Authorization</span></span>  | <span data-ttu-id="1fd6b-135">string</span><span class="sxs-lookup"><span data-stu-id="1fd6b-135">string</span></span>  | <span data-ttu-id="1fd6b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fd6b-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fd6b-138">Content-Type</span></span> | <span data-ttu-id="1fd6b-139">string</span><span class="sxs-lookup"><span data-stu-id="1fd6b-139">string</span></span>  | <span data-ttu-id="1fd6b-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fd6b-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd6b-142">Request body</span></span>
<span data-ttu-id="1fd6b-143">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="1fd6b-143">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1fd6b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd6b-144">Response</span></span>

<span data-ttu-id="1fd6b-145">Se tiver êxito, este método retornará `201 Created` código de resposta e o objeto de [anexo](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-145">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="1fd6b-146">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="1fd6b-146">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="1fd6b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd6b-147">Request</span></span>
<span data-ttu-id="1fd6b-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-148">Here is an example of the request.</span></span>
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

<span data-ttu-id="1fd6b-149">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="1fd6b-149">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1fd6b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd6b-150">Response</span></span>
<span data-ttu-id="1fd6b-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-151">Here is an example of the response.</span></span> 
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

## <a name="example-item-attachment"></a><span data-ttu-id="1fd6b-152">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="1fd6b-152">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="1fd6b-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd6b-153">Request</span></span>
<span data-ttu-id="1fd6b-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-154">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1fd6b-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd6b-155">Response</span></span>
<span data-ttu-id="1fd6b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="1fd6b-159">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="1fd6b-159">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="1fd6b-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fd6b-160">Request</span></span>
<span data-ttu-id="1fd6b-161">Aqui está um exemplo de uma solicitação que adiciona um anexo de referência a uma mensagem existente.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-161">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="1fd6b-162">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-162">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1fd6b-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fd6b-163">Response</span></span>
<span data-ttu-id="1fd6b-164">Aqui está um exemplo de uma resposta completa.</span><span class="sxs-lookup"><span data-stu-id="1fd6b-164">Here is an example of a full response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
