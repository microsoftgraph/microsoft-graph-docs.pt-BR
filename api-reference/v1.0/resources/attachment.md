---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e82ce58786e23448458e9e1c60fad5d0c54b6388
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722430"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="2fd00-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="2fd00-103">attachment resource type</span></span>

<span data-ttu-id="2fd00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fd00-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2fd00-105">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md) de usuário, [mensagem](../resources/message.md) ou [postagem](../resources/post.md) na forma de anexo.</span><span class="sxs-lookup"><span data-stu-id="2fd00-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="2fd00-106">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="2fd00-106">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="2fd00-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="2fd00-107">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="2fd00-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="2fd00-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="2fd00-109">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="2fd00-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="2fd00-110">Os eventos em calendários de grupo não têm suporte para anexos.</span><span class="sxs-lookup"><span data-stu-id="2fd00-110">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="2fd00-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="2fd00-111">Methods</span></span>

<span data-ttu-id="2fd00-112">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="2fd00-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="2fd00-113">Método</span><span class="sxs-lookup"><span data-stu-id="2fd00-113">Method</span></span>       | <span data-ttu-id="2fd00-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2fd00-114">Return Type</span></span>  |<span data-ttu-id="2fd00-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd00-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2fd00-116">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="2fd00-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="2fd00-117">anexo</span><span class="sxs-lookup"><span data-stu-id="2fd00-117">attachment</span></span>](attachment.md) |<span data-ttu-id="2fd00-118">Leia as propriedades, relações ou conteúdo bruto de um anexo, anexado a um evento de usuário, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="2fd00-118">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, or post.</span></span>|
|[<span data-ttu-id="2fd00-119">Adicionar anexo a um evento do usuário</span><span class="sxs-lookup"><span data-stu-id="2fd00-119">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="2fd00-120">attachment</span><span class="sxs-lookup"><span data-stu-id="2fd00-120">attachment</span></span>](attachment.md) |<span data-ttu-id="2fd00-121">Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="2fd00-121">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="2fd00-122">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="2fd00-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="2fd00-123">attachment</span><span class="sxs-lookup"><span data-stu-id="2fd00-123">attachment</span></span>](attachment.md) |<span data-ttu-id="2fd00-124">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="2fd00-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="2fd00-125">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="2fd00-125">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="2fd00-126">attachment</span><span class="sxs-lookup"><span data-stu-id="2fd00-126">attachment</span></span>](attachment.md) |<span data-ttu-id="2fd00-127">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="2fd00-127">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="2fd00-128">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="2fd00-128">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="2fd00-129">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="2fd00-129">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2fd00-130">Obtenha uma lista de anexos de um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="2fd00-130">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="2fd00-131">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="2fd00-131">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="2fd00-132">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="2fd00-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2fd00-133">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="2fd00-133">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="2fd00-134">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="2fd00-134">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="2fd00-135">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="2fd00-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="2fd00-136">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="2fd00-136">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="2fd00-137">Delete</span><span class="sxs-lookup"><span data-stu-id="2fd00-137">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="2fd00-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fd00-138">None</span></span> |<span data-ttu-id="2fd00-139">Exclua um anexo em um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="2fd00-139">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="2fd00-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fd00-140">Properties</span></span>

<span data-ttu-id="2fd00-p101">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="2fd00-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="2fd00-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fd00-143">Property</span></span>     | <span data-ttu-id="2fd00-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fd00-144">Type</span></span>   |<span data-ttu-id="2fd00-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd00-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fd00-146">contentType</span><span class="sxs-lookup"><span data-stu-id="2fd00-146">contentType</span></span>|<span data-ttu-id="2fd00-147">String</span><span class="sxs-lookup"><span data-stu-id="2fd00-147">String</span></span>|<span data-ttu-id="2fd00-148">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="2fd00-148">The MIME type.</span></span>|
|<span data-ttu-id="2fd00-149">id</span><span class="sxs-lookup"><span data-stu-id="2fd00-149">id</span></span>|<span data-ttu-id="2fd00-150">String</span><span class="sxs-lookup"><span data-stu-id="2fd00-150">String</span></span>| <span data-ttu-id="2fd00-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2fd00-151">Read-only.</span></span>|
|<span data-ttu-id="2fd00-152">isInline</span><span class="sxs-lookup"><span data-stu-id="2fd00-152">isInline</span></span>|<span data-ttu-id="2fd00-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="2fd00-153">Boolean</span></span>|<span data-ttu-id="2fd00-154">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="2fd00-154">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="2fd00-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd00-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2fd00-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd00-156">DateTimeOffset</span></span>|<span data-ttu-id="2fd00-157">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2fd00-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2fd00-158">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2fd00-158">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2fd00-159">nome</span><span class="sxs-lookup"><span data-stu-id="2fd00-159">name</span></span>|<span data-ttu-id="2fd00-160">String</span><span class="sxs-lookup"><span data-stu-id="2fd00-160">String</span></span>|<span data-ttu-id="2fd00-161">Nome de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="2fd00-161">The attachment's file name.</span></span>|
|<span data-ttu-id="2fd00-162">size</span><span class="sxs-lookup"><span data-stu-id="2fd00-162">size</span></span>|<span data-ttu-id="2fd00-163">Int32</span><span class="sxs-lookup"><span data-stu-id="2fd00-163">Int32</span></span>|<span data-ttu-id="2fd00-164">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="2fd00-164">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fd00-165">Relações</span><span class="sxs-lookup"><span data-stu-id="2fd00-165">Relationships</span></span>
<span data-ttu-id="2fd00-166">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fd00-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fd00-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fd00-167">JSON representation</span></span>

<span data-ttu-id="2fd00-168">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2fd00-168">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

