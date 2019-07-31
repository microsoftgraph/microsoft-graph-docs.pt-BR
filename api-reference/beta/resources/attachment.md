---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6ee3ba645f71b100b78b01fa1821bf91ca21cb26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013259"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="48309-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="48309-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48309-104">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) no formato de um anexo.</span><span class="sxs-lookup"><span data-stu-id="48309-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="48309-105">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="48309-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="48309-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="48309-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="48309-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="48309-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="48309-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="48309-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="48309-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="48309-109">Methods</span></span>

<span data-ttu-id="48309-110">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="48309-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="48309-111">Método</span><span class="sxs-lookup"><span data-stu-id="48309-111">Method</span></span>       | <span data-ttu-id="48309-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48309-112">Return Type</span></span>  |<span data-ttu-id="48309-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="48309-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48309-114">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="48309-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="48309-115">attachment</span><span class="sxs-lookup"><span data-stu-id="48309-115">attachment</span></span>](attachment.md) |<span data-ttu-id="48309-116">Leia as propriedades e as relações de um anexo, anexados a um evento, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="48309-116">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="48309-117">Adicionar anexo a um event</span><span class="sxs-lookup"><span data-stu-id="48309-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="48309-118">attachment</span><span class="sxs-lookup"><span data-stu-id="48309-118">attachment</span></span>](attachment.md) |<span data-ttu-id="48309-119">Adicione um arquivo, item ou anexo de link a um evento.</span><span class="sxs-lookup"><span data-stu-id="48309-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="48309-120">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="48309-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="48309-121">attachment</span><span class="sxs-lookup"><span data-stu-id="48309-121">attachment</span></span>](attachment.md) |<span data-ttu-id="48309-122">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="48309-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="48309-123">Adicionar anexo a uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="48309-123">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="48309-124">attachment</span><span class="sxs-lookup"><span data-stu-id="48309-124">attachment</span></span>](attachment.md) |<span data-ttu-id="48309-125">Adicionar um anexo de arquivo, item ou link a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="48309-125">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="48309-126">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="48309-126">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="48309-127">attachment</span><span class="sxs-lookup"><span data-stu-id="48309-127">attachment</span></span>](attachment.md) |<span data-ttu-id="48309-128">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="48309-128">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="48309-129">Listar anexos de um evento</span><span class="sxs-lookup"><span data-stu-id="48309-129">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="48309-130">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="48309-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="48309-131">Obtenha uma lista de anexos de um evento.</span><span class="sxs-lookup"><span data-stu-id="48309-131">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="48309-132">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="48309-132">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="48309-133">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="48309-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="48309-134">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="48309-134">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="48309-135">Listar anexos de uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="48309-135">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="48309-136">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="48309-136">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="48309-137">Obter uma lista de anexos para uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="48309-137">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="48309-138">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="48309-138">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="48309-139">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="48309-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="48309-140">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="48309-140">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="48309-141">Delete</span><span class="sxs-lookup"><span data-stu-id="48309-141">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="48309-142">None</span><span class="sxs-lookup"><span data-stu-id="48309-142">None</span></span> |<span data-ttu-id="48309-143">Excluir um anexo de um evento, de uma mensagem, de uma tarefa do Outlook ou de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="48309-143">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="48309-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48309-144">Properties</span></span>

<span data-ttu-id="48309-p101">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="48309-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="48309-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48309-147">Property</span></span>     | <span data-ttu-id="48309-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="48309-148">Type</span></span>   |<span data-ttu-id="48309-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="48309-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48309-150">contentType</span><span class="sxs-lookup"><span data-stu-id="48309-150">contentType</span></span>|<span data-ttu-id="48309-151">String</span><span class="sxs-lookup"><span data-stu-id="48309-151">String</span></span>|<span data-ttu-id="48309-152">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="48309-152">The MIME type.</span></span>|
|<span data-ttu-id="48309-153">id</span><span class="sxs-lookup"><span data-stu-id="48309-153">id</span></span>|<span data-ttu-id="48309-154">String</span><span class="sxs-lookup"><span data-stu-id="48309-154">String</span></span>| <span data-ttu-id="48309-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48309-155">Read-only.</span></span>|
|<span data-ttu-id="48309-156">isInline</span><span class="sxs-lookup"><span data-stu-id="48309-156">isInline</span></span>|<span data-ttu-id="48309-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="48309-157">Boolean</span></span>|<span data-ttu-id="48309-158">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="48309-158">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="48309-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48309-159">lastModifiedDateTime</span></span>|<span data-ttu-id="48309-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48309-160">DateTimeOffset</span></span>|<span data-ttu-id="48309-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="48309-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="48309-163">nome</span><span class="sxs-lookup"><span data-stu-id="48309-163">name</span></span>|<span data-ttu-id="48309-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48309-164">String</span></span>|<span data-ttu-id="48309-165">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="48309-165">The display name of the attachment.</span></span> <span data-ttu-id="48309-166">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="48309-166">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="48309-167">size</span><span class="sxs-lookup"><span data-stu-id="48309-167">size</span></span>|<span data-ttu-id="48309-168">Int32</span><span class="sxs-lookup"><span data-stu-id="48309-168">Int32</span></span>|<span data-ttu-id="48309-169">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="48309-169">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48309-170">Relações</span><span class="sxs-lookup"><span data-stu-id="48309-170">Relationships</span></span>
<span data-ttu-id="48309-171">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48309-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48309-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48309-172">JSON representation</span></span>

<span data-ttu-id="48309-173">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="48309-173">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
