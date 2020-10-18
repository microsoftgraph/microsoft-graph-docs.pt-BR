---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: db7b744a15035ab00a878119e29021ab4b825490
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581908"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="11b3e-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="11b3e-103">attachment resource type</span></span>

<span data-ttu-id="11b3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11b3e-105">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md) de usuário, [mensagem](../resources/message.md) ou [postagem](../resources/post.md) na forma de anexo.</span><span class="sxs-lookup"><span data-stu-id="11b3e-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="11b3e-106">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="11b3e-106">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="11b3e-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="11b3e-107">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="11b3e-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="11b3e-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="11b3e-109">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="11b3e-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="11b3e-110">Os eventos em calendários de grupo não têm suporte para anexos.</span><span class="sxs-lookup"><span data-stu-id="11b3e-110">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="11b3e-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="11b3e-111">Methods</span></span>

<span data-ttu-id="11b3e-112">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="11b3e-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="11b3e-113">Método</span><span class="sxs-lookup"><span data-stu-id="11b3e-113">Method</span></span>       | <span data-ttu-id="11b3e-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="11b3e-114">Return Type</span></span>  |<span data-ttu-id="11b3e-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="11b3e-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11b3e-116">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="11b3e-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="11b3e-117">anexo</span><span class="sxs-lookup"><span data-stu-id="11b3e-117">attachment</span></span>](attachment.md) |<span data-ttu-id="11b3e-118">Leia as propriedades, relações ou conteúdo bruto de um anexo, anexado a um evento de usuário, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="11b3e-118">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, or post.</span></span>|
|[<span data-ttu-id="11b3e-119">Adicionar anexo a um evento do usuário</span><span class="sxs-lookup"><span data-stu-id="11b3e-119">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="11b3e-120">attachment</span><span class="sxs-lookup"><span data-stu-id="11b3e-120">attachment</span></span>](attachment.md) |<span data-ttu-id="11b3e-121">Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="11b3e-121">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="11b3e-122">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="11b3e-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="11b3e-123">attachment</span><span class="sxs-lookup"><span data-stu-id="11b3e-123">attachment</span></span>](attachment.md) |<span data-ttu-id="11b3e-124">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="11b3e-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="11b3e-125">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="11b3e-125">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="11b3e-126">attachment</span><span class="sxs-lookup"><span data-stu-id="11b3e-126">attachment</span></span>](attachment.md) |<span data-ttu-id="11b3e-127">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="11b3e-127">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="11b3e-128">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="11b3e-128">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="11b3e-129">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="11b3e-129">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="11b3e-130">Obtenha uma lista de anexos de um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="11b3e-130">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="11b3e-131">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="11b3e-131">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="11b3e-132">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="11b3e-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="11b3e-133">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="11b3e-133">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="11b3e-134">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="11b3e-134">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="11b3e-135">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="11b3e-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="11b3e-136">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="11b3e-136">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="11b3e-137">Delete</span><span class="sxs-lookup"><span data-stu-id="11b3e-137">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="11b3e-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11b3e-138">None</span></span> |<span data-ttu-id="11b3e-139">Exclua um anexo em um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="11b3e-139">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="11b3e-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11b3e-140">Properties</span></span>

<span data-ttu-id="11b3e-p101">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="11b3e-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="11b3e-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11b3e-143">Property</span></span>     | <span data-ttu-id="11b3e-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="11b3e-144">Type</span></span>   |<span data-ttu-id="11b3e-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="11b3e-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11b3e-146">contentType</span><span class="sxs-lookup"><span data-stu-id="11b3e-146">contentType</span></span>|<span data-ttu-id="11b3e-147">String</span><span class="sxs-lookup"><span data-stu-id="11b3e-147">String</span></span>|<span data-ttu-id="11b3e-148">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="11b3e-148">The MIME type.</span></span>|
|<span data-ttu-id="11b3e-149">id</span><span class="sxs-lookup"><span data-stu-id="11b3e-149">id</span></span>|<span data-ttu-id="11b3e-150">String</span><span class="sxs-lookup"><span data-stu-id="11b3e-150">String</span></span>| <span data-ttu-id="11b3e-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11b3e-151">Read-only.</span></span>|
|<span data-ttu-id="11b3e-152">isInline</span><span class="sxs-lookup"><span data-stu-id="11b3e-152">isInline</span></span>|<span data-ttu-id="11b3e-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="11b3e-153">Boolean</span></span>|<span data-ttu-id="11b3e-154">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="11b3e-154">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="11b3e-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11b3e-155">lastModifiedDateTime</span></span>|<span data-ttu-id="11b3e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b3e-156">DateTimeOffset</span></span>|<span data-ttu-id="11b3e-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="11b3e-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="11b3e-159">nome</span><span class="sxs-lookup"><span data-stu-id="11b3e-159">name</span></span>|<span data-ttu-id="11b3e-160">String</span><span class="sxs-lookup"><span data-stu-id="11b3e-160">String</span></span>|<span data-ttu-id="11b3e-161">Nome de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="11b3e-161">The attachment's file name.</span></span>|
|<span data-ttu-id="11b3e-162">size</span><span class="sxs-lookup"><span data-stu-id="11b3e-162">size</span></span>|<span data-ttu-id="11b3e-163">Int32</span><span class="sxs-lookup"><span data-stu-id="11b3e-163">Int32</span></span>|<span data-ttu-id="11b3e-164">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="11b3e-164">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11b3e-165">Relações</span><span class="sxs-lookup"><span data-stu-id="11b3e-165">Relationships</span></span>
<span data-ttu-id="11b3e-166">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11b3e-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11b3e-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11b3e-167">JSON representation</span></span>

<span data-ttu-id="11b3e-168">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="11b3e-168">Here is a JSON representation of the resource</span></span>

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

