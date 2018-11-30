---
title: Adicionar anexo
description: Use essa API para adicionar um anexo a um evento. Desde daí
ms.openlocfilehash: 6a5d07c8cbbeab6895a38d915c2fcdfa9e2e5c50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035325"
---
# <a name="add-attachment"></a><span data-ttu-id="445b3-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="445b3-104">Add attachment</span></span>

> <span data-ttu-id="445b3-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="445b3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="445b3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="445b3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="445b3-p103">Use esta API para adicionar um [anexo](../resources/attachment.md) a um evento. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="445b3-p103">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="445b3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="445b3-109">Permissions</span></span>
<span data-ttu-id="445b3-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="445b3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="445b3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="445b3-112">Permission type</span></span>      | <span data-ttu-id="445b3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="445b3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="445b3-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="445b3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="445b3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="445b3-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="445b3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="445b3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="445b3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="445b3-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="445b3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="445b3-118">Application</span></span> | <span data-ttu-id="445b3-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="445b3-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="445b3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="445b3-120">HTTP request</span></span>
<span data-ttu-id="445b3-121">Anexos em um [evento](../resources/event.md) do usuário padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="445b3-121">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="445b3-122">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="445b3-122">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="445b3-123">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="445b3-123">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="445b3-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="445b3-124">Request headers</span></span>
| <span data-ttu-id="445b3-125">Nome</span><span class="sxs-lookup"><span data-stu-id="445b3-125">Name</span></span>       | <span data-ttu-id="445b3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="445b3-126">Type</span></span> | <span data-ttu-id="445b3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="445b3-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="445b3-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="445b3-128">Authorization</span></span>  | <span data-ttu-id="445b3-129">string</span><span class="sxs-lookup"><span data-stu-id="445b3-129">string</span></span>  | <span data-ttu-id="445b3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="445b3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="445b3-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="445b3-132">Content-Type</span></span> | <span data-ttu-id="445b3-133">string</span><span class="sxs-lookup"><span data-stu-id="445b3-133">string</span></span>  | <span data-ttu-id="445b3-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="445b3-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="445b3-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="445b3-136">Request body</span></span>
<span data-ttu-id="445b3-137">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="445b3-137">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="445b3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="445b3-138">Response</span></span>

<span data-ttu-id="445b3-139">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="445b3-139">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="445b3-140">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="445b3-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="445b3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="445b3-141">Request</span></span>
<span data-ttu-id="445b3-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="445b3-142">Here is an example of the request.</span></span>
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

<span data-ttu-id="445b3-143">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="445b3-143">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="445b3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="445b3-144">Response</span></span>
<span data-ttu-id="445b3-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="445b3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="445b3-148">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="445b3-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="445b3-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="445b3-149">Request</span></span>

<span data-ttu-id="445b3-150">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="445b3-150">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

##### <a name="response"></a><span data-ttu-id="445b3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="445b3-151">Response</span></span>
<span data-ttu-id="445b3-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="445b3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="445b3-155">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="445b3-155">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="445b3-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="445b3-156">Request</span></span>
<span data-ttu-id="445b3-157">Aqui está um exemplo de uma solicitação que adiciona um anexo de referência para um evento existente.</span><span class="sxs-lookup"><span data-stu-id="445b3-157">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="445b3-158">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="445b3-158">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
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

##### <a name="response"></a><span data-ttu-id="445b3-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="445b3-159">Response</span></span>
<span data-ttu-id="445b3-160">Aqui está um exemplo de uma resposta completa.</span><span class="sxs-lookup"><span data-stu-id="445b3-160">Here is an example of a full response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
