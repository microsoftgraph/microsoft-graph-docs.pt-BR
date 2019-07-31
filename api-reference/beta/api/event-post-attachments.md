---
title: Adicionar anexo
description: Use esta API para adicionar um anexo a um evento. Desde lá
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e21cf245c0e370c4db7d8d52b39ef3db8cd111c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954477"
---
# <a name="add-attachment"></a><span data-ttu-id="008f6-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="008f6-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="008f6-p102">Use esta API para adicionar um [anexo](../resources/attachment.md) a um evento. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="008f6-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="008f6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="008f6-107">Permissions</span></span>

<span data-ttu-id="008f6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="008f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="008f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="008f6-110">Permission type</span></span>      | <span data-ttu-id="008f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="008f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="008f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="008f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="008f6-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="008f6-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="008f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="008f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="008f6-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="008f6-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="008f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="008f6-116">Application</span></span> | <span data-ttu-id="008f6-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="008f6-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="008f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="008f6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="008f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="008f6-119">Request headers</span></span>

| <span data-ttu-id="008f6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="008f6-120">Name</span></span>       | <span data-ttu-id="008f6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="008f6-121">Type</span></span> | <span data-ttu-id="008f6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="008f6-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="008f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="008f6-123">Authorization</span></span>  | <span data-ttu-id="008f6-124">string</span><span class="sxs-lookup"><span data-stu-id="008f6-124">string</span></span>  | <span data-ttu-id="008f6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="008f6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="008f6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="008f6-127">Content-Type</span></span> | <span data-ttu-id="008f6-128">string</span><span class="sxs-lookup"><span data-stu-id="008f6-128">string</span></span>  | <span data-ttu-id="008f6-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="008f6-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="008f6-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="008f6-131">Request body</span></span>

<span data-ttu-id="008f6-132">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="008f6-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="008f6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="008f6-133">Response</span></span>

<span data-ttu-id="008f6-134">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="008f6-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="008f6-135">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="008f6-135">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="008f6-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="008f6-136">Request</span></span>

<span data-ttu-id="008f6-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="008f6-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="008f6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="008f6-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="008f6-139">C#</span><span class="sxs-lookup"><span data-stu-id="008f6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="008f6-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="008f6-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="008f6-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="008f6-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="008f6-142">Java</span><span class="sxs-lookup"><span data-stu-id="008f6-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="008f6-143">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="008f6-143">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="008f6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="008f6-144">Response</span></span>

<span data-ttu-id="008f6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="008f6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="008f6-148">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="008f6-148">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="008f6-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="008f6-149">Request</span></span>

<span data-ttu-id="008f6-150">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="008f6-150">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- { "blockType": "ignored" } -->

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


### <a name="response"></a><span data-ttu-id="008f6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="008f6-151">Response</span></span>

<span data-ttu-id="008f6-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="008f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="008f6-155">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="008f6-155">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="008f6-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="008f6-156">Request</span></span>

<span data-ttu-id="008f6-157">Veja um exemplo de uma solicitação que adiciona um anexo de referência a um evento existente.</span><span class="sxs-lookup"><span data-stu-id="008f6-157">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="008f6-158">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="008f6-158">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="008f6-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="008f6-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="008f6-160">C#</span><span class="sxs-lookup"><span data-stu-id="008f6-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="008f6-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="008f6-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="008f6-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="008f6-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="008f6-163">Java</span><span class="sxs-lookup"><span data-stu-id="008f6-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-from-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="008f6-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="008f6-164">Response</span></span>

<span data-ttu-id="008f6-165">Veja um exemplo de resposta completa.</span><span class="sxs-lookup"><span data-stu-id="008f6-165">Here is an example of a full response.</span></span>
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
    "Error: create_file_attachment_from_event/contentBytes:\r\n      Expected type Binary but actual was String. Property: contentBytes, actual value: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk='"
  ]
}
-->
