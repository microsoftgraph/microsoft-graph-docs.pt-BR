---
title: Adicionar anexo
description: Use essa API para adicionar um anexo a um evento. Desde daí
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5364da921cd05699ffcd13754e3ac296653dd0d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926453"
---
# <a name="add-attachment"></a><span data-ttu-id="ab585-104">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="ab585-104">Add attachment</span></span>

> <span data-ttu-id="ab585-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab585-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab585-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab585-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab585-p103">Use esta API para adicionar um [anexo](../resources/attachment.md) a um evento. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="ab585-p103">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab585-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab585-109">Permissions</span></span>

<span data-ttu-id="ab585-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab585-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab585-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab585-112">Permission type</span></span>      | <span data-ttu-id="ab585-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab585-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab585-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab585-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ab585-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab585-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ab585-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab585-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab585-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab585-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ab585-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab585-118">Application</span></span> | <span data-ttu-id="ab585-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab585-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab585-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab585-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="ab585-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab585-121">Request headers</span></span>

| <span data-ttu-id="ab585-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ab585-122">Name</span></span>       | <span data-ttu-id="ab585-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab585-123">Type</span></span> | <span data-ttu-id="ab585-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab585-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ab585-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab585-125">Authorization</span></span>  | <span data-ttu-id="ab585-126">string</span><span class="sxs-lookup"><span data-stu-id="ab585-126">string</span></span>  | <span data-ttu-id="ab585-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab585-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab585-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab585-129">Content-Type</span></span> | <span data-ttu-id="ab585-130">string</span><span class="sxs-lookup"><span data-stu-id="ab585-130">string</span></span>  | <span data-ttu-id="ab585-p106">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab585-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab585-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab585-133">Request body</span></span>

<span data-ttu-id="ab585-134">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ab585-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ab585-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab585-135">Response</span></span>

<span data-ttu-id="ab585-136">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab585-136">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="ab585-137">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="ab585-137">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="ab585-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab585-138">Request</span></span>

<span data-ttu-id="ab585-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab585-139">Here is an example of the request.</span></span>
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

<span data-ttu-id="ab585-140">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ab585-140">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="ab585-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab585-141">Response</span></span>

<span data-ttu-id="ab585-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab585-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="ab585-145">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="ab585-145">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="ab585-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab585-146">Request</span></span>

<span data-ttu-id="ab585-147">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="ab585-147">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

### <a name="response"></a><span data-ttu-id="ab585-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab585-148">Response</span></span>

<span data-ttu-id="ab585-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab585-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="ab585-152">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="ab585-152">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="ab585-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab585-153">Request</span></span>

<span data-ttu-id="ab585-154">Aqui está um exemplo de uma solicitação que adiciona um anexo de referência para um evento existente.</span><span class="sxs-lookup"><span data-stu-id="ab585-154">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="ab585-155">O anexo aponta para uma pasta no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ab585-155">The attachment points to a folder on OneDrive.</span></span>
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

### <a name="response"></a><span data-ttu-id="ab585-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab585-156">Response</span></span>

<span data-ttu-id="ab585-157">Aqui está um exemplo de uma resposta completa.</span><span class="sxs-lookup"><span data-stu-id="ab585-157">Here is an example of a full response.</span></span>
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
