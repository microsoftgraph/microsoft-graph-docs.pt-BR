---
title: Adicionar anexo
description: Use esta API para adicionar um anexo a um evento. Como não há
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cd295ba9b80bbbfcbdf4c6f7bebe95e8b0e4bfcb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584310"
---
# <a name="add-attachment"></a><span data-ttu-id="0539c-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="0539c-104">Add attachment</span></span>

<span data-ttu-id="0539c-p102">Use esta API para adicionar um [anexo](../resources/attachment.md) a um evento. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="0539c-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="0539c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0539c-107">Permissions</span></span>
<span data-ttu-id="0539c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0539c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0539c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0539c-110">Permission type</span></span>      | <span data-ttu-id="0539c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0539c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0539c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0539c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0539c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0539c-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0539c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0539c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0539c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0539c-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0539c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0539c-116">Application</span></span> | <span data-ttu-id="0539c-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0539c-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0539c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0539c-118">HTTP request</span></span>
<span data-ttu-id="0539c-119">Anexos de um [evento](../resources/event.md) no [calendário](../resources/calendar.md)padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="0539c-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="0539c-120">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="0539c-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="0539c-121">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="0539c-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="0539c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0539c-122">Request headers</span></span>
| <span data-ttu-id="0539c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0539c-123">Name</span></span>       | <span data-ttu-id="0539c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0539c-124">Type</span></span> | <span data-ttu-id="0539c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0539c-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0539c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0539c-126">Authorization</span></span>  | <span data-ttu-id="0539c-127">string</span><span class="sxs-lookup"><span data-stu-id="0539c-127">string</span></span>  | <span data-ttu-id="0539c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0539c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0539c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0539c-130">Content-Type</span></span> | <span data-ttu-id="0539c-131">string</span><span class="sxs-lookup"><span data-stu-id="0539c-131">string</span></span>  | <span data-ttu-id="0539c-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0539c-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0539c-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0539c-134">Request body</span></span>
<span data-ttu-id="0539c-135">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="0539c-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0539c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0539c-136">Response</span></span>

<span data-ttu-id="0539c-137">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0539c-137">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="0539c-138">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="0539c-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0539c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0539c-139">Request</span></span>
<span data-ttu-id="0539c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0539c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_file_attachment_from_event"
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

<span data-ttu-id="0539c-141">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="0539c-141">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0539c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0539c-142">Response</span></span>
<span data-ttu-id="0539c-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0539c-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
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
    "contentBytes":"base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="0539c-144">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="0539c-144">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0539c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0539c-145">Request</span></span>

<span data-ttu-id="0539c-146">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="0539c-146">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
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

##### <a name="response"></a><span data-ttu-id="0539c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0539c-147">Response</span></span>
<span data-ttu-id="0539c-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0539c-148">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
