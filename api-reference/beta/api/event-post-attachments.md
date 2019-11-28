---
title: Adicionar anexo
description: Use esta API para adicionar um anexo a um evento. Desde lá
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e382b778819c7c1c68d445ee9691a0206bbd76e5
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636817"
---
# <a name="add-attachment"></a><span data-ttu-id="7f504-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="7f504-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f504-105">Use esta API para adicionar um [anexo](../resources/attachment.md) a um [evento](../resources/event.md)existente.</span><span class="sxs-lookup"><span data-stu-id="7f504-105">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="7f504-106">Esta operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="7f504-106">This operation limits the size of the attachment you can add to under 4 MB.</span></span>

<span data-ttu-id="7f504-107">Se um organizador adicionar um anexo a um evento de reunião, o organizador poderá, subsequentemente, [Atualizar](event-update.md) o evento para enviar o anexo e também atualizar o evento para cada participante.</span><span class="sxs-lookup"><span data-stu-id="7f504-107">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f504-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f504-108">Permissions</span></span>

<span data-ttu-id="7f504-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f504-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f504-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f504-111">Permission type</span></span>      | <span data-ttu-id="7f504-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f504-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f504-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f504-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7f504-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f504-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7f504-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f504-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f504-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f504-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7f504-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f504-117">Application</span></span> | <span data-ttu-id="7f504-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f504-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f504-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f504-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="7f504-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f504-120">Request headers</span></span>

| <span data-ttu-id="7f504-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7f504-121">Name</span></span>       | <span data-ttu-id="7f504-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f504-122">Type</span></span> | <span data-ttu-id="7f504-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f504-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f504-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f504-124">Authorization</span></span>  | <span data-ttu-id="7f504-125">string</span><span class="sxs-lookup"><span data-stu-id="7f504-125">string</span></span>  | <span data-ttu-id="7f504-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f504-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f504-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f504-128">Content-Type</span></span> | <span data-ttu-id="7f504-129">string</span><span class="sxs-lookup"><span data-stu-id="7f504-129">string</span></span>  | <span data-ttu-id="7f504-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f504-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f504-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f504-132">Request body</span></span>

<span data-ttu-id="7f504-133">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="7f504-133">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7f504-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f504-134">Response</span></span>

<span data-ttu-id="7f504-135">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f504-135">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="7f504-136">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="7f504-136">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="7f504-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f504-137">Request</span></span>

<span data-ttu-id="7f504-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f504-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7f504-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f504-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event_beta"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f504-140">C#</span><span class="sxs-lookup"><span data-stu-id="7f504-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f504-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f504-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f504-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f504-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="7f504-143">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="7f504-143">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="7f504-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f504-144">Response</span></span>

<span data-ttu-id="7f504-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f504-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_event_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
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

## <a name="example-item-attachment"></a><span data-ttu-id="7f504-148">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="7f504-148">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="7f504-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f504-149">Request</span></span>

<span data-ttu-id="7f504-150">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="7f504-150">Here is an example which attaches an event with another event as an item attachment.</span></span>

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


### <a name="response"></a><span data-ttu-id="7f504-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f504-151">Response</span></span>

<span data-ttu-id="7f504-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f504-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
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

## <a name="example-reference-attachment"></a><span data-ttu-id="7f504-155">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="7f504-155">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="7f504-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f504-156">Request</span></span>

<span data-ttu-id="7f504-157">Veja um exemplo de uma solicitação que adiciona um anexo de referência a um evento existente.</span><span class="sxs-lookup"><span data-stu-id="7f504-157">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="7f504-158">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7f504-158">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7f504-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f504-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f504-160">C#</span><span class="sxs-lookup"><span data-stu-id="7f504-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f504-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f504-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f504-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f504-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f504-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f504-163">Response</span></span>

<span data-ttu-id="7f504-164">Veja um exemplo de resposta completa.</span><span class="sxs-lookup"><span data-stu-id="7f504-164">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_from_event",
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
  "tocPath": ""
}
-->
