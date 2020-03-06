---
title: Adicionar anexo
description: Use esta API para adicionar um anexo a um evento. Desde lá
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: af1226e5a8fbf9cd19c198a622e90f3a29873702
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517338"
---
# <a name="add-attachment"></a><span data-ttu-id="18f3e-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="18f3e-104">Add attachment</span></span>

<span data-ttu-id="18f3e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18f3e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18f3e-106">Use esta API para adicionar um [anexo](../resources/attachment.md) a um [evento](../resources/event.md)existente.</span><span class="sxs-lookup"><span data-stu-id="18f3e-106">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="18f3e-107">Esta operação limita o tamanho do anexo que você pode adicionar a menos de 3 MB.</span><span class="sxs-lookup"><span data-stu-id="18f3e-107">This operation limits the size of the attachment you can add to under 3 MB.</span></span>

<span data-ttu-id="18f3e-108">Se um organizador adicionar um anexo a um evento de reunião, o organizador poderá, subsequentemente, [Atualizar](event-update.md) o evento para enviar o anexo e também atualizar o evento para cada participante.</span><span class="sxs-lookup"><span data-stu-id="18f3e-108">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="18f3e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="18f3e-109">Permissions</span></span>
<span data-ttu-id="18f3e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18f3e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18f3e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18f3e-112">Permission type</span></span>      | <span data-ttu-id="18f3e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18f3e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18f3e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18f3e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="18f3e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18f3e-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="18f3e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18f3e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18f3e-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18f3e-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="18f3e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18f3e-118">Application</span></span> | <span data-ttu-id="18f3e-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18f3e-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18f3e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18f3e-120">HTTP request</span></span>
<span data-ttu-id="18f3e-121">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="18f3e-121">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="18f3e-122">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="18f3e-122">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="18f3e-123">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="18f3e-123">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="18f3e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18f3e-124">Request headers</span></span>
| <span data-ttu-id="18f3e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="18f3e-125">Name</span></span>       | <span data-ttu-id="18f3e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="18f3e-126">Type</span></span> | <span data-ttu-id="18f3e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="18f3e-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18f3e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="18f3e-128">Authorization</span></span>  | <span data-ttu-id="18f3e-129">string</span><span class="sxs-lookup"><span data-stu-id="18f3e-129">string</span></span>  | <span data-ttu-id="18f3e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18f3e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18f3e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18f3e-132">Content-Type</span></span> | <span data-ttu-id="18f3e-133">string</span><span class="sxs-lookup"><span data-stu-id="18f3e-133">string</span></span>  | <span data-ttu-id="18f3e-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18f3e-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18f3e-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18f3e-136">Request body</span></span>
<span data-ttu-id="18f3e-137">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="18f3e-137">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="18f3e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="18f3e-138">Response</span></span>

<span data-ttu-id="18f3e-139">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18f3e-139">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="18f3e-140">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="18f3e-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="18f3e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18f3e-141">Request</span></span>
<span data-ttu-id="18f3e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18f3e-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18f3e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="18f3e-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="18f3e-144">C#</span><span class="sxs-lookup"><span data-stu-id="18f3e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18f3e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18f3e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18f3e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18f3e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18f3e-147">Java</span><span class="sxs-lookup"><span data-stu-id="18f3e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-event-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="18f3e-148">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="18f3e-148">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="18f3e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="18f3e-149">Response</span></span>
<span data-ttu-id="18f3e-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18f3e-150">Here is an example of the response.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="18f3e-151">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="18f3e-151">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="18f3e-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18f3e-152">Request</span></span>

<span data-ttu-id="18f3e-153">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="18f3e-153">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "ignored",
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


##### <a name="response"></a><span data-ttu-id="18f3e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="18f3e-154">Response</span></span>
<span data-ttu-id="18f3e-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18f3e-155">Here is an example of the response.</span></span>
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
