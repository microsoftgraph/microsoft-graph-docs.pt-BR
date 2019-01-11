---
title: tipo de recurso attachment
description: Você pode adicionar conteúdo relacionado a um evento,
localization_priority: Priority
ms.openlocfilehash: 284895871a0c6a80140ff248045b89d2de104c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892327"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="ad78c-103">tipo de recurso attachment</span><span class="sxs-lookup"><span data-stu-id="ad78c-103">attachment resource type</span></span>

<span data-ttu-id="ad78c-104">Você pode adicionar conteúdo relacionado a um [event](../resources/event.md), [message](../resources/message.md) u [post](../resources/post.md) na forma de anexo</span><span class="sxs-lookup"><span data-stu-id="ad78c-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="ad78c-105">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="ad78c-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="ad78c-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="ad78c-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="ad78c-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="ad78c-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="ad78c-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="ad78c-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="ad78c-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="ad78c-109">Methods</span></span>

<span data-ttu-id="ad78c-110">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="ad78c-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="ad78c-111">Método</span><span class="sxs-lookup"><span data-stu-id="ad78c-111">Method</span></span>       | <span data-ttu-id="ad78c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ad78c-112">Return Type</span></span>  |<span data-ttu-id="ad78c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad78c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad78c-114">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="ad78c-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ad78c-115">attachment</span><span class="sxs-lookup"><span data-stu-id="ad78c-115">attachment</span></span>](attachment.md) |<span data-ttu-id="ad78c-116">Leia as propriedades e as relações de um anexo, anexados a um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="ad78c-116">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="ad78c-117">Adicionar anexo a um event</span><span class="sxs-lookup"><span data-stu-id="ad78c-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="ad78c-118">attachment</span><span class="sxs-lookup"><span data-stu-id="ad78c-118">attachment</span></span>](attachment.md) |<span data-ttu-id="ad78c-119">Adicione um arquivo, item ou anexo de link a um evento.</span><span class="sxs-lookup"><span data-stu-id="ad78c-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="ad78c-120">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="ad78c-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="ad78c-121">attachment</span><span class="sxs-lookup"><span data-stu-id="ad78c-121">attachment</span></span>](attachment.md) |<span data-ttu-id="ad78c-122">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ad78c-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="ad78c-123">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="ad78c-123">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="ad78c-124">attachment</span><span class="sxs-lookup"><span data-stu-id="ad78c-124">attachment</span></span>](attachment.md) |<span data-ttu-id="ad78c-125">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="ad78c-125">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="ad78c-126">Listar anexos de um evento</span><span class="sxs-lookup"><span data-stu-id="ad78c-126">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="ad78c-127">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="ad78c-127">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="ad78c-128">Obtenha uma lista de anexos de um evento.</span><span class="sxs-lookup"><span data-stu-id="ad78c-128">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="ad78c-129">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="ad78c-129">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="ad78c-130">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="ad78c-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="ad78c-131">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="ad78c-131">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="ad78c-132">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="ad78c-132">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="ad78c-133">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="ad78c-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="ad78c-134">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="ad78c-134">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="ad78c-135">Delete</span><span class="sxs-lookup"><span data-stu-id="ad78c-135">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="ad78c-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad78c-136">None</span></span> |<span data-ttu-id="ad78c-137">Exclua um anexo em um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="ad78c-137">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="ad78c-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad78c-138">Properties</span></span>

<span data-ttu-id="ad78c-p101">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="ad78c-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="ad78c-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad78c-141">Property</span></span>     | <span data-ttu-id="ad78c-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad78c-142">Type</span></span>   |<span data-ttu-id="ad78c-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad78c-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad78c-144">contentType</span><span class="sxs-lookup"><span data-stu-id="ad78c-144">contentType</span></span>|<span data-ttu-id="ad78c-145">String</span><span class="sxs-lookup"><span data-stu-id="ad78c-145">String</span></span>|<span data-ttu-id="ad78c-146">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="ad78c-146">The MIME type.</span></span>|
|<span data-ttu-id="ad78c-147">id</span><span class="sxs-lookup"><span data-stu-id="ad78c-147">id</span></span>|<span data-ttu-id="ad78c-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad78c-148">String</span></span>| <span data-ttu-id="ad78c-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad78c-149">Read-only.</span></span>|
|<span data-ttu-id="ad78c-150">isInline</span><span class="sxs-lookup"><span data-stu-id="ad78c-150">isInline</span></span>|<span data-ttu-id="ad78c-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="ad78c-151">Boolean</span></span>|<span data-ttu-id="ad78c-152">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="ad78c-152">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="ad78c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad78c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ad78c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad78c-154">DateTimeOffset</span></span>|<span data-ttu-id="ad78c-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ad78c-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ad78c-157">nome</span><span class="sxs-lookup"><span data-stu-id="ad78c-157">name</span></span>|<span data-ttu-id="ad78c-158">String</span><span class="sxs-lookup"><span data-stu-id="ad78c-158">String</span></span>|<span data-ttu-id="ad78c-159">Nome de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="ad78c-159">The attachment's file name.</span></span>|
|<span data-ttu-id="ad78c-160">size</span><span class="sxs-lookup"><span data-stu-id="ad78c-160">size</span></span>|<span data-ttu-id="ad78c-161">Int32</span><span class="sxs-lookup"><span data-stu-id="ad78c-161">Int32</span></span>|<span data-ttu-id="ad78c-162">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="ad78c-162">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad78c-163">Relações</span><span class="sxs-lookup"><span data-stu-id="ad78c-163">Relationships</span></span>
<span data-ttu-id="ad78c-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad78c-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad78c-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad78c-165">JSON representation</span></span>

<span data-ttu-id="ad78c-166">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ad78c-166">Here is a JSON representation of the resource</span></span>

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
