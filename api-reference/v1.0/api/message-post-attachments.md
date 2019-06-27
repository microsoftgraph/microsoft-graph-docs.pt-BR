---
title: Adicionar anexo
description: 'Use esta API para adicionar um anexo a uma mensagem. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1b68777b98a3f956b0032318070531db2bf9c627
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276787"
---
# <a name="add-attachment"></a><span data-ttu-id="f30f9-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="f30f9-103">Add attachment</span></span>

<span data-ttu-id="f30f9-104">Use esta API para adicionar um [anexo](../resources/attachment.md) a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="f30f9-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="f30f9-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="f30f9-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="f30f9-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f30f9-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="f30f9-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f30f9-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="f30f9-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="f30f9-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="f30f9-109">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f30f9-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="f30f9-110">Você pode adicionar um anexo a uma mensagem existente postando na seu coleção de anexos, ou pode adicionar um anexo a uma mensagem que está sendo [criada e enviada dinamicamente](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="f30f9-110">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="f30f9-111">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="f30f9-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="f30f9-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="f30f9-112">Permissions</span></span>
<span data-ttu-id="f30f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f30f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f30f9-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f30f9-115">Permission type</span></span>      | <span data-ttu-id="f30f9-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f30f9-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f30f9-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f30f9-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f30f9-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30f9-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f30f9-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f30f9-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f30f9-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30f9-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f30f9-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f30f9-121">Application</span></span> | <span data-ttu-id="f30f9-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30f9-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f30f9-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f30f9-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f30f9-124">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="f30f9-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="f30f9-125">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f30f9-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="f30f9-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="f30f9-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f30f9-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f30f9-128">Request headers</span></span>
| <span data-ttu-id="f30f9-129">Nome</span><span class="sxs-lookup"><span data-stu-id="f30f9-129">Name</span></span>       | <span data-ttu-id="f30f9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f30f9-130">Type</span></span> | <span data-ttu-id="f30f9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f30f9-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f30f9-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="f30f9-132">Authorization</span></span>  | <span data-ttu-id="f30f9-133">string</span><span class="sxs-lookup"><span data-stu-id="f30f9-133">string</span></span>  | <span data-ttu-id="f30f9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f30f9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f30f9-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f30f9-136">Content-Type</span></span> | <span data-ttu-id="f30f9-137">string</span><span class="sxs-lookup"><span data-stu-id="f30f9-137">string</span></span>  | <span data-ttu-id="f30f9-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f30f9-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f30f9-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f30f9-140">Request body</span></span>
<span data-ttu-id="f30f9-141">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f30f9-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f30f9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f30f9-142">Response</span></span>

<span data-ttu-id="f30f9-143">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f30f9-143">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="f30f9-144">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="f30f9-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f30f9-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f30f9-145">Request</span></span>
<span data-ttu-id="f30f9-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f30f9-146">Here is an example of the request.</span></span>
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

<span data-ttu-id="f30f9-147">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f30f9-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f30f9-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f30f9-148">Response</span></span>
<span data-ttu-id="f30f9-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f30f9-149">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f30f9-150">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f30f9-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f30f9-151">C#</span><span class="sxs-lookup"><span data-stu-id="f30f9-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f30f9-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="f30f9-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f30f9-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f30f9-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="f30f9-154">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="f30f9-154">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="f30f9-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f30f9-155">Request</span></span>
<span data-ttu-id="f30f9-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f30f9-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_item_attachment_from_message"
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

##### <a name="response"></a><span data-ttu-id="f30f9-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="f30f9-157">Response</span></span>
<span data-ttu-id="f30f9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f30f9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
