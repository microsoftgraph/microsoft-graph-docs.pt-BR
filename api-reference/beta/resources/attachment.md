---
title: tipo de recurso attachment
description: Você pode adicionar conteúdo relacionado a um evento,
ms.openlocfilehash: f0bb9ec37d2fe3d034dce9532ad316d371c4937e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040475"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="7eb7d-103">tipo de recurso attachment</span><span class="sxs-lookup"><span data-stu-id="7eb7d-103">attachment resource type</span></span>

> <span data-ttu-id="7eb7d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7eb7d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7eb7d-106">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md) na forma de um anexo.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-106">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="7eb7d-107">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="7eb7d-107">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="7eb7d-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="7eb7d-108">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="7eb7d-109">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="7eb7d-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="7eb7d-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="7eb7d-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="7eb7d-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="7eb7d-111">Methods</span></span>

<span data-ttu-id="7eb7d-112">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="7eb7d-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="7eb7d-113">Método</span><span class="sxs-lookup"><span data-stu-id="7eb7d-113">Method</span></span>       | <span data-ttu-id="7eb7d-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7eb7d-114">Return Type</span></span>  |<span data-ttu-id="7eb7d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb7d-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7eb7d-116">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="7eb7d-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="7eb7d-117">attachment</span><span class="sxs-lookup"><span data-stu-id="7eb7d-117">attachment</span></span>](attachment.md) |<span data-ttu-id="7eb7d-118">Leia as propriedades e relacionamentos de um anexo, anexados a um evento, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-118">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="7eb7d-119">Adicionar anexo a um event</span><span class="sxs-lookup"><span data-stu-id="7eb7d-119">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="7eb7d-120">attachment</span><span class="sxs-lookup"><span data-stu-id="7eb7d-120">attachment</span></span>](attachment.md) |<span data-ttu-id="7eb7d-121">Adicione um arquivo, item ou anexo de link a um evento.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-121">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="7eb7d-122">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="7eb7d-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="7eb7d-123">attachment</span><span class="sxs-lookup"><span data-stu-id="7eb7d-123">attachment</span></span>](attachment.md) |<span data-ttu-id="7eb7d-124">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="7eb7d-125">Adicionar anexos para uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="7eb7d-125">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="7eb7d-126">attachment</span><span class="sxs-lookup"><span data-stu-id="7eb7d-126">attachment</span></span>](attachment.md) |<span data-ttu-id="7eb7d-127">Adicione um arquivo, item ou anexo de link a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-127">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="7eb7d-128">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="7eb7d-128">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="7eb7d-129">attachment</span><span class="sxs-lookup"><span data-stu-id="7eb7d-129">attachment</span></span>](attachment.md) |<span data-ttu-id="7eb7d-130">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-130">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="7eb7d-131">Listar anexos de um evento</span><span class="sxs-lookup"><span data-stu-id="7eb7d-131">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="7eb7d-132">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7eb7d-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="7eb7d-133">Obtenha uma lista de anexos de um evento.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-133">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="7eb7d-134">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="7eb7d-134">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="7eb7d-135">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7eb7d-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="7eb7d-136">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-136">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="7eb7d-137">Listar anexos de uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="7eb7d-137">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="7eb7d-138">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7eb7d-138">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="7eb7d-139">Obtenha uma lista de anexos para uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-139">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="7eb7d-140">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="7eb7d-140">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="7eb7d-141">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7eb7d-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="7eb7d-142">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-142">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="7eb7d-143">Delete</span><span class="sxs-lookup"><span data-stu-id="7eb7d-143">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="7eb7d-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7eb7d-144">None</span></span> |<span data-ttu-id="7eb7d-145">Exclua um anexo em um evento, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-145">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="7eb7d-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7eb7d-146">Properties</span></span>

<span data-ttu-id="7eb7d-p102">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-p102">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="7eb7d-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7eb7d-149">Property</span></span>     | <span data-ttu-id="7eb7d-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eb7d-150">Type</span></span>   |<span data-ttu-id="7eb7d-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb7d-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7eb7d-152">contentType</span><span class="sxs-lookup"><span data-stu-id="7eb7d-152">contentType</span></span>|<span data-ttu-id="7eb7d-153">String</span><span class="sxs-lookup"><span data-stu-id="7eb7d-153">String</span></span>|<span data-ttu-id="7eb7d-154">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-154">The MIME type.</span></span>|
|<span data-ttu-id="7eb7d-155">id</span><span class="sxs-lookup"><span data-stu-id="7eb7d-155">id</span></span>|<span data-ttu-id="7eb7d-156">String</span><span class="sxs-lookup"><span data-stu-id="7eb7d-156">String</span></span>| <span data-ttu-id="7eb7d-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-157">Read-only.</span></span>|
|<span data-ttu-id="7eb7d-158">isInline</span><span class="sxs-lookup"><span data-stu-id="7eb7d-158">isInline</span></span>|<span data-ttu-id="7eb7d-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="7eb7d-159">Boolean</span></span>|<span data-ttu-id="7eb7d-160">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-160">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="7eb7d-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7eb7d-161">lastModifiedDateTime</span></span>|<span data-ttu-id="7eb7d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7eb7d-162">DateTimeOffset</span></span>|<span data-ttu-id="7eb7d-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7eb7d-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7eb7d-165">nome</span><span class="sxs-lookup"><span data-stu-id="7eb7d-165">name</span></span>|<span data-ttu-id="7eb7d-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7eb7d-166">String</span></span>|<span data-ttu-id="7eb7d-167">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-167">The display name of the attachment.</span></span> <span data-ttu-id="7eb7d-168">Isso não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-168">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="7eb7d-169">size</span><span class="sxs-lookup"><span data-stu-id="7eb7d-169">size</span></span>|<span data-ttu-id="7eb7d-170">Int32</span><span class="sxs-lookup"><span data-stu-id="7eb7d-170">Int32</span></span>|<span data-ttu-id="7eb7d-171">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-171">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7eb7d-172">Relações</span><span class="sxs-lookup"><span data-stu-id="7eb7d-172">Relationships</span></span>
<span data-ttu-id="7eb7d-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7eb7d-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7eb7d-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7eb7d-174">JSON representation</span></span>

<span data-ttu-id="7eb7d-175">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7eb7d-175">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
