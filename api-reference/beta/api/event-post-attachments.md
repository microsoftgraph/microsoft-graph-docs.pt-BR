---
title: Adicionar anexo
description: Use esta API para adicionar um anexo a um evento. Como não há
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ece15b579bae9e439eb9303c8b594631ce9b9b31
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464015"
---
# <a name="add-attachment"></a><span data-ttu-id="7826c-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="7826c-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7826c-p102">Use esta API para adicionar um [anexo](../resources/attachment.md) a um evento. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="7826c-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="7826c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7826c-107">Permissions</span></span>

<span data-ttu-id="7826c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7826c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7826c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7826c-110">Permission type</span></span>      | <span data-ttu-id="7826c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7826c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7826c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7826c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7826c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7826c-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7826c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7826c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7826c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7826c-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7826c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7826c-116">Application</span></span> | <span data-ttu-id="7826c-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7826c-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7826c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7826c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="7826c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7826c-119">Request headers</span></span>

| <span data-ttu-id="7826c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7826c-120">Name</span></span>       | <span data-ttu-id="7826c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7826c-121">Type</span></span> | <span data-ttu-id="7826c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7826c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7826c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7826c-123">Authorization</span></span>  | <span data-ttu-id="7826c-124">string</span><span class="sxs-lookup"><span data-stu-id="7826c-124">string</span></span>  | <span data-ttu-id="7826c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7826c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7826c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7826c-127">Content-Type</span></span> | <span data-ttu-id="7826c-128">string</span><span class="sxs-lookup"><span data-stu-id="7826c-128">string</span></span>  | <span data-ttu-id="7826c-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7826c-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7826c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7826c-131">Request body</span></span>

<span data-ttu-id="7826c-132">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="7826c-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7826c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7826c-133">Response</span></span>

<span data-ttu-id="7826c-134">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7826c-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="7826c-135">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="7826c-135">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="7826c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7826c-136">Request</span></span>

<span data-ttu-id="7826c-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7826c-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

<span data-ttu-id="7826c-138">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="7826c-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="7826c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7826c-139">Response</span></span>

<span data-ttu-id="7826c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7826c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP 201 Created
Content-Length: 735

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="7826c-143">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="7826c-143">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="7826c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7826c-144">Request</span></span>

<span data-ttu-id="7826c-145">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="7826c-145">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
Content-type: application/json
Content-length: 600

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

### <a name="response"></a><span data-ttu-id="7826c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7826c-146">Response</span></span>

<span data-ttu-id="7826c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7826c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/beta/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="7826c-150">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="7826c-150">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="7826c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7826c-151">Request</span></span>

<span data-ttu-id="7826c-152">Veja um exemplo de uma solicitação que adiciona um anexo de referência a um evento existente.</span><span class="sxs-lookup"><span data-stu-id="7826c-152">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="7826c-153">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7826c-153">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments
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

### <a name="response"></a><span data-ttu-id="7826c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7826c-154">Response</span></span>

<span data-ttu-id="7826c-155">Veja um exemplo de resposta completa.</span><span class="sxs-lookup"><span data-stu-id="7826c-155">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
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
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
