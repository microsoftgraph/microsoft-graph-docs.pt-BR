---
title: Adicionar anexo
description: Use esta API para adicionar um anexo a um evento. Desde lá
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 18c73e333c98c86c66b8ed8227aa9f98cfcfcbb8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042531"
---
# <a name="add-attachment"></a><span data-ttu-id="e2a13-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="e2a13-104">Add attachment</span></span>

<span data-ttu-id="e2a13-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2a13-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2a13-106">Use essa API para adicionar um [anexo](../resources/attachment.md) a um evento [existente.](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="e2a13-106">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="e2a13-107">Essa operação limita o tamanho do anexo que você pode adicionar a menos de 3 MB.</span><span class="sxs-lookup"><span data-stu-id="e2a13-107">This operation limits the size of the attachment you can add to under 3 MB.</span></span>

<span data-ttu-id="e2a13-108">Se um organizador adiciona um anexo a um [](event-update.md) evento de reunião, o organizador pode atualizar o evento posteriormente para enviar o anexo e atualizar o evento para cada participante também.</span><span class="sxs-lookup"><span data-stu-id="e2a13-108">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2a13-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2a13-109">Permissions</span></span>

<span data-ttu-id="e2a13-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2a13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2a13-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2a13-112">Permission type</span></span>      | <span data-ttu-id="e2a13-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2a13-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2a13-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2a13-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e2a13-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2a13-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e2a13-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2a13-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2a13-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2a13-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e2a13-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2a13-118">Application</span></span> | <span data-ttu-id="e2a13-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2a13-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2a13-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a13-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="e2a13-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a13-121">Request headers</span></span>

| <span data-ttu-id="e2a13-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e2a13-122">Name</span></span>       | <span data-ttu-id="e2a13-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2a13-123">Type</span></span> | <span data-ttu-id="e2a13-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2a13-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2a13-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2a13-125">Authorization</span></span>  | <span data-ttu-id="e2a13-126">string</span><span class="sxs-lookup"><span data-stu-id="e2a13-126">string</span></span>  | <span data-ttu-id="e2a13-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2a13-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2a13-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2a13-129">Content-Type</span></span> | <span data-ttu-id="e2a13-130">string</span><span class="sxs-lookup"><span data-stu-id="e2a13-130">string</span></span>  | <span data-ttu-id="e2a13-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2a13-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2a13-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a13-133">Request body</span></span>

<span data-ttu-id="e2a13-134">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2a13-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a13-135">Response</span></span>

<span data-ttu-id="e2a13-136">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a13-136">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="e2a13-137">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="e2a13-137">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="e2a13-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a13-138">Request</span></span>

<span data-ttu-id="e2a13-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2a13-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2a13-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a13-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e2a13-141">C#</span><span class="sxs-lookup"><span data-stu-id="e2a13-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2a13-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2a13-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2a13-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2a13-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2a13-144">Java</span><span class="sxs-lookup"><span data-stu-id="e2a13-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-event-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e2a13-145">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e2a13-145">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="e2a13-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a13-146">Response</span></span>

<span data-ttu-id="e2a13-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a13-147">Here is an example of the response.</span></span> <span data-ttu-id="e2a13-148">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2a13-148">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="e2a13-149">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="e2a13-149">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="e2a13-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a13-150">Request</span></span>

<span data-ttu-id="e2a13-151">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="e2a13-151">Here is an example which attaches an event with another event as an item attachment.</span></span>

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


### <a name="response"></a><span data-ttu-id="e2a13-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a13-152">Response</span></span>

<span data-ttu-id="e2a13-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a13-153">Here is an example of the response.</span></span> <span data-ttu-id="e2a13-154">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2a13-154">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="e2a13-155">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="e2a13-155">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="e2a13-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a13-156">Request</span></span>

<span data-ttu-id="e2a13-157">Aqui está um exemplo de uma solicitação que adiciona um anexo de referência a um evento existente.</span><span class="sxs-lookup"><span data-stu-id="e2a13-157">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="e2a13-158">O anexo aponta para uma pasta OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e2a13-158">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2a13-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a13-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e2a13-160">C#</span><span class="sxs-lookup"><span data-stu-id="e2a13-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2a13-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2a13-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2a13-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2a13-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2a13-163">Java</span><span class="sxs-lookup"><span data-stu-id="e2a13-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-from-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2a13-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a13-164">Response</span></span>

<span data-ttu-id="e2a13-165">Aqui está um exemplo de uma resposta completa.</span><span class="sxs-lookup"><span data-stu-id="e2a13-165">Here is an example of a full response.</span></span>
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


