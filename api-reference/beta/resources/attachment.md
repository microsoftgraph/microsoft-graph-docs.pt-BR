---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: da7e66d1edbda224fe547b7e7afc8fd88dc5e5aa
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622632"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="86237-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="86237-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86237-104">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md)de usuário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) de grupo no formato de um anexo.</span><span class="sxs-lookup"><span data-stu-id="86237-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="86237-105">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="86237-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="86237-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="86237-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="86237-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="86237-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="86237-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="86237-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="86237-109">Eventos em calendários de grupo não dão suporte a anexos.</span><span class="sxs-lookup"><span data-stu-id="86237-109">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="86237-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="86237-110">Methods</span></span>

<span data-ttu-id="86237-111">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="86237-111">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="86237-112">Método</span><span class="sxs-lookup"><span data-stu-id="86237-112">Method</span></span>       | <span data-ttu-id="86237-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86237-113">Return Type</span></span>  |<span data-ttu-id="86237-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="86237-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86237-115">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="86237-115">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="86237-116">attachment</span><span class="sxs-lookup"><span data-stu-id="86237-116">attachment</span></span>](attachment.md) |<span data-ttu-id="86237-117">Leia as propriedades e as relações de um anexo, anexados a um evento de usuário, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="86237-117">Read the properties and relationships of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="86237-118">Adicionar anexo a um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="86237-118">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="86237-119">attachment</span><span class="sxs-lookup"><span data-stu-id="86237-119">attachment</span></span>](attachment.md) |<span data-ttu-id="86237-120">Adicionar um anexo de arquivo, item ou link a um evento em um calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="86237-120">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="86237-121">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="86237-121">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="86237-122">attachment</span><span class="sxs-lookup"><span data-stu-id="86237-122">attachment</span></span>](attachment.md) |<span data-ttu-id="86237-123">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="86237-123">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="86237-124">Adicionar anexo a uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="86237-124">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="86237-125">attachment</span><span class="sxs-lookup"><span data-stu-id="86237-125">attachment</span></span>](attachment.md) |<span data-ttu-id="86237-126">Adicionar um anexo de arquivo, item ou link a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="86237-126">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="86237-127">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="86237-127">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="86237-128">attachment</span><span class="sxs-lookup"><span data-stu-id="86237-128">attachment</span></span>](attachment.md) |<span data-ttu-id="86237-129">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="86237-129">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="86237-130">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="86237-130">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="86237-131">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="86237-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="86237-132">Obter uma lista de anexos para um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="86237-132">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="86237-133">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="86237-133">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="86237-134">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="86237-134">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="86237-135">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="86237-135">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="86237-136">Listar anexos de uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="86237-136">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="86237-137">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="86237-137">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="86237-138">Obter uma lista de anexos para uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="86237-138">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="86237-139">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="86237-139">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="86237-140">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="86237-140">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="86237-141">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="86237-141">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="86237-142">Delete</span><span class="sxs-lookup"><span data-stu-id="86237-142">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="86237-143">None</span><span class="sxs-lookup"><span data-stu-id="86237-143">None</span></span> |<span data-ttu-id="86237-144">Excluir um anexo de um evento, de uma mensagem, de uma tarefa do Outlook ou de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="86237-144">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="86237-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86237-145">Properties</span></span>

<span data-ttu-id="86237-p101">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="86237-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="86237-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86237-148">Property</span></span>     | <span data-ttu-id="86237-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="86237-149">Type</span></span>   |<span data-ttu-id="86237-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="86237-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86237-151">contentType</span><span class="sxs-lookup"><span data-stu-id="86237-151">contentType</span></span>|<span data-ttu-id="86237-152">String</span><span class="sxs-lookup"><span data-stu-id="86237-152">String</span></span>|<span data-ttu-id="86237-153">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="86237-153">The MIME type.</span></span>|
|<span data-ttu-id="86237-154">id</span><span class="sxs-lookup"><span data-stu-id="86237-154">id</span></span>|<span data-ttu-id="86237-155">String</span><span class="sxs-lookup"><span data-stu-id="86237-155">String</span></span>| <span data-ttu-id="86237-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86237-156">Read-only.</span></span>|
|<span data-ttu-id="86237-157">isInline</span><span class="sxs-lookup"><span data-stu-id="86237-157">isInline</span></span>|<span data-ttu-id="86237-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="86237-158">Boolean</span></span>|<span data-ttu-id="86237-159">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="86237-159">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="86237-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86237-160">lastModifiedDateTime</span></span>|<span data-ttu-id="86237-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86237-161">DateTimeOffset</span></span>|<span data-ttu-id="86237-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="86237-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="86237-164">nome</span><span class="sxs-lookup"><span data-stu-id="86237-164">name</span></span>|<span data-ttu-id="86237-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86237-165">String</span></span>|<span data-ttu-id="86237-166">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="86237-166">The display name of the attachment.</span></span> <span data-ttu-id="86237-167">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="86237-167">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="86237-168">size</span><span class="sxs-lookup"><span data-stu-id="86237-168">size</span></span>|<span data-ttu-id="86237-169">Int32</span><span class="sxs-lookup"><span data-stu-id="86237-169">Int32</span></span>|<span data-ttu-id="86237-170">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="86237-170">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86237-171">Relações</span><span class="sxs-lookup"><span data-stu-id="86237-171">Relationships</span></span>
<span data-ttu-id="86237-172">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86237-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86237-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86237-173">JSON representation</span></span>

<span data-ttu-id="86237-174">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="86237-174">Here is a JSON representation of the resource</span></span>

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
