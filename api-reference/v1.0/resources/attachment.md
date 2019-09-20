---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c7bf5eef63921f1cc3fab985f4832177767fe1fc
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036071"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="3349b-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="3349b-103">attachment resource type</span></span>

<span data-ttu-id="3349b-104">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md) de usuário, [mensagem](../resources/message.md) ou [postagem](../resources/post.md) na forma de anexo.</span><span class="sxs-lookup"><span data-stu-id="3349b-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="3349b-105">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="3349b-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="3349b-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="3349b-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="3349b-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="3349b-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="3349b-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="3349b-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="3349b-109">Os eventos em calendários de grupo não têm suporte para anexos.</span><span class="sxs-lookup"><span data-stu-id="3349b-109">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="3349b-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="3349b-110">Methods</span></span>

<span data-ttu-id="3349b-111">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="3349b-111">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="3349b-112">Método</span><span class="sxs-lookup"><span data-stu-id="3349b-112">Method</span></span>       | <span data-ttu-id="3349b-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3349b-113">Return Type</span></span>  |<span data-ttu-id="3349b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="3349b-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3349b-115">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="3349b-115">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3349b-116">anexo</span><span class="sxs-lookup"><span data-stu-id="3349b-116">attachment</span></span>](attachment.md) |<span data-ttu-id="3349b-117">Leia as propriedades, relações ou conteúdo bruto de um anexo, anexado a um evento de usuário, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="3349b-117">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="3349b-118">Adicionar anexo a um evento do usuário</span><span class="sxs-lookup"><span data-stu-id="3349b-118">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="3349b-119">attachment</span><span class="sxs-lookup"><span data-stu-id="3349b-119">attachment</span></span>](attachment.md) |<span data-ttu-id="3349b-120">Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="3349b-120">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="3349b-121">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="3349b-121">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="3349b-122">attachment</span><span class="sxs-lookup"><span data-stu-id="3349b-122">attachment</span></span>](attachment.md) |<span data-ttu-id="3349b-123">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="3349b-123">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="3349b-124">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="3349b-124">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="3349b-125">attachment</span><span class="sxs-lookup"><span data-stu-id="3349b-125">attachment</span></span>](attachment.md) |<span data-ttu-id="3349b-126">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="3349b-126">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="3349b-127">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="3349b-127">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="3349b-128">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="3349b-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3349b-129">Obtenha uma lista de anexos de um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="3349b-129">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="3349b-130">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="3349b-130">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="3349b-131">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="3349b-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3349b-132">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="3349b-132">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="3349b-133">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="3349b-133">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="3349b-134">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="3349b-134">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="3349b-135">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="3349b-135">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="3349b-136">Delete</span><span class="sxs-lookup"><span data-stu-id="3349b-136">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="3349b-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3349b-137">None</span></span> |<span data-ttu-id="3349b-138">Exclua um anexo em um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="3349b-138">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="3349b-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3349b-139">Properties</span></span>

<span data-ttu-id="3349b-p101">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="3349b-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="3349b-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3349b-142">Property</span></span>     | <span data-ttu-id="3349b-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="3349b-143">Type</span></span>   |<span data-ttu-id="3349b-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="3349b-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3349b-145">contentType</span><span class="sxs-lookup"><span data-stu-id="3349b-145">contentType</span></span>|<span data-ttu-id="3349b-146">String</span><span class="sxs-lookup"><span data-stu-id="3349b-146">String</span></span>|<span data-ttu-id="3349b-147">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="3349b-147">The MIME type.</span></span>|
|<span data-ttu-id="3349b-148">id</span><span class="sxs-lookup"><span data-stu-id="3349b-148">id</span></span>|<span data-ttu-id="3349b-149">String</span><span class="sxs-lookup"><span data-stu-id="3349b-149">String</span></span>| <span data-ttu-id="3349b-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3349b-150">Read-only.</span></span>|
|<span data-ttu-id="3349b-151">isInline</span><span class="sxs-lookup"><span data-stu-id="3349b-151">isInline</span></span>|<span data-ttu-id="3349b-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="3349b-152">Boolean</span></span>|<span data-ttu-id="3349b-153">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="3349b-153">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="3349b-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3349b-154">lastModifiedDateTime</span></span>|<span data-ttu-id="3349b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3349b-155">DateTimeOffset</span></span>|<span data-ttu-id="3349b-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3349b-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3349b-158">nome</span><span class="sxs-lookup"><span data-stu-id="3349b-158">name</span></span>|<span data-ttu-id="3349b-159">String</span><span class="sxs-lookup"><span data-stu-id="3349b-159">String</span></span>|<span data-ttu-id="3349b-160">Nome de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="3349b-160">The attachment's file name.</span></span>|
|<span data-ttu-id="3349b-161">size</span><span class="sxs-lookup"><span data-stu-id="3349b-161">size</span></span>|<span data-ttu-id="3349b-162">Int32</span><span class="sxs-lookup"><span data-stu-id="3349b-162">Int32</span></span>|<span data-ttu-id="3349b-163">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="3349b-163">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3349b-164">Relações</span><span class="sxs-lookup"><span data-stu-id="3349b-164">Relationships</span></span>
<span data-ttu-id="3349b-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3349b-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3349b-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3349b-166">JSON representation</span></span>

<span data-ttu-id="3349b-167">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3349b-167">Here is a JSON representation of the resource</span></span>

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
