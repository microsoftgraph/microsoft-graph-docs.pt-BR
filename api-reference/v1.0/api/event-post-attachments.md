---
title: Adicionar anexo
description: Use esta API para adicionar um anexo a um evento. Desde lá
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 14d62182f4d21618dae5d8009c4376404fff66eb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473810"
---
# <a name="add-attachment"></a><span data-ttu-id="902d2-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="902d2-104">Add attachment</span></span>

<span data-ttu-id="902d2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="902d2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="902d2-106">Use essa API para adicionar um [anexo](../resources/attachment.md) a um evento [existente.](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="902d2-106">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="902d2-107">Essa operação limita o tamanho do anexo que você pode adicionar a menos de 3 MB.</span><span class="sxs-lookup"><span data-stu-id="902d2-107">This operation limits the size of the attachment you can add to under 3 MB.</span></span>

<span data-ttu-id="902d2-108">Se um organizador adiciona um anexo a um [](event-update.md) evento de reunião, o organizador pode atualizar o evento posteriormente para enviar o anexo e atualizar o evento para cada participante também.</span><span class="sxs-lookup"><span data-stu-id="902d2-108">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="902d2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="902d2-109">Permissions</span></span>
<span data-ttu-id="902d2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="902d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="902d2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="902d2-112">Permission type</span></span>      | <span data-ttu-id="902d2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="902d2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="902d2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="902d2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="902d2-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="902d2-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="902d2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="902d2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="902d2-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="902d2-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="902d2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="902d2-118">Application</span></span> | <span data-ttu-id="902d2-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="902d2-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="902d2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="902d2-120">HTTP request</span></span>
<span data-ttu-id="902d2-121">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="902d2-121">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="902d2-122">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="902d2-122">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="902d2-123">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="902d2-123">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="902d2-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="902d2-124">Request headers</span></span>
| <span data-ttu-id="902d2-125">Nome</span><span class="sxs-lookup"><span data-stu-id="902d2-125">Name</span></span>       | <span data-ttu-id="902d2-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="902d2-126">Type</span></span> | <span data-ttu-id="902d2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="902d2-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="902d2-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="902d2-128">Authorization</span></span>  | <span data-ttu-id="902d2-129">string</span><span class="sxs-lookup"><span data-stu-id="902d2-129">string</span></span>  | <span data-ttu-id="902d2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="902d2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="902d2-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="902d2-132">Content-Type</span></span> | <span data-ttu-id="902d2-133">string</span><span class="sxs-lookup"><span data-stu-id="902d2-133">string</span></span>  | <span data-ttu-id="902d2-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="902d2-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="902d2-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="902d2-136">Request body</span></span>
<span data-ttu-id="902d2-137">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="902d2-137">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="902d2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="902d2-138">Response</span></span>

<span data-ttu-id="902d2-139">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="902d2-139">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="902d2-140">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="902d2-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="902d2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="902d2-141">Request</span></span>
<span data-ttu-id="902d2-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="902d2-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="902d2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="902d2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_file_attachment_from_event_v1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```
# <a name="c"></a>[<span data-ttu-id="902d2-144">C#</span><span class="sxs-lookup"><span data-stu-id="902d2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="902d2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="902d2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="902d2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="902d2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="902d2-147">Java</span><span class="sxs-lookup"><span data-stu-id="902d2-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-event-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="902d2-148">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="902d2-148">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="902d2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="902d2-149">Response</span></span>
<span data-ttu-id="902d2-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="902d2-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_event_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
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

## <a name="example-item-attachment"></a><span data-ttu-id="902d2-151">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="902d2-151">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="902d2-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="902d2-152">Request</span></span>

<span data-ttu-id="902d2-153">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="902d2-153">Here is an example which attaches an event with another event as an item attachment.</span></span>


# <a name="http"></a>[<span data-ttu-id="902d2-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="902d2-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
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
# <a name="c"></a>[<span data-ttu-id="902d2-155">C#</span><span class="sxs-lookup"><span data-stu-id="902d2-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="902d2-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="902d2-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="902d2-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="902d2-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="902d2-158">Java</span><span class="sxs-lookup"><span data-stu-id="902d2-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-item-attachment-from-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="902d2-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="902d2-159">Response</span></span>
<span data-ttu-id="902d2-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="902d2-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
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

