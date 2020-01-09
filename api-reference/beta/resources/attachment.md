---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 0c0f257a9bdcf6c149b4f6374e2011cebb437603
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994961"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="6f4b5-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="6f4b5-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f4b5-104">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md)de usuário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) de grupo no formato de um anexo.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="6f4b5-105">Os eventos em calendários de grupo não têm suporte para anexos.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-105">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="6f4b5-106">As tarefas do Outlook não dão suporte a anexos de referência.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-106">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="6f4b5-107">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="6f4b5-107">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="6f4b5-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="6f4b5-108">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="6f4b5-109">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="6f4b5-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="6f4b5-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="6f4b5-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="6f4b5-111">**Observação**: há um limite para o tamanho do arquivo ou anexo de item que pode ser adicionado abaixo de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-111">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="6f4b5-112">No entanto, se estiver anexando a uma mensagem um arquivo entre 3 MB e 150MB, você pode [criar uma sessão de carregamento](../api/attachment-createuploadsession.md) e carregar de forma iterativa os intervalos do arquivo para anexá-lo.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-112">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="6f4b5-113">Consulte [anexar arquivos grandes às mensagens do Outlook](/graph/outlook-large-attachments) para obter um exemplo.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-113">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="6f4b5-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="6f4b5-114">Methods</span></span>

<span data-ttu-id="6f4b5-115">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="6f4b5-115">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="6f4b5-116">Método</span><span class="sxs-lookup"><span data-stu-id="6f4b5-116">Method</span></span>       | <span data-ttu-id="6f4b5-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6f4b5-117">Return Type</span></span>  |<span data-ttu-id="6f4b5-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f4b5-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6f4b5-119">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="6f4b5-119">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="6f4b5-120">anexo</span><span class="sxs-lookup"><span data-stu-id="6f4b5-120">attachment</span></span>](attachment.md) |<span data-ttu-id="6f4b5-121">Leia as propriedades, relações ou conteúdo bruto de um anexo, anexados a um evento de usuário, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-121">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="6f4b5-122">Adicionar anexo a um evento do usuário</span><span class="sxs-lookup"><span data-stu-id="6f4b5-122">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="6f4b5-123">attachment</span><span class="sxs-lookup"><span data-stu-id="6f4b5-123">attachment</span></span>](attachment.md) |<span data-ttu-id="6f4b5-124">Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-124">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="6f4b5-125">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="6f4b5-125">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="6f4b5-126">attachment</span><span class="sxs-lookup"><span data-stu-id="6f4b5-126">attachment</span></span>](attachment.md) |<span data-ttu-id="6f4b5-127">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-127">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="6f4b5-128">Esta operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-128">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="6f4b5-129">Criar sessão para anexar arquivo grande</span><span class="sxs-lookup"><span data-stu-id="6f4b5-129">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="6f4b5-130">uploadSession</span><span class="sxs-lookup"><span data-stu-id="6f4b5-130">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="6f4b5-131">Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de um arquivo de forma iterativa, para anexar o arquivo à **mensagem**especificada.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-131">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="6f4b5-132">O tamanho do arquivo deve estar entre 3 MB e 150MB.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-132">The file size must be between 3MB and 150MB.</span></span>|
|[<span data-ttu-id="6f4b5-133">Adicionar anexo a uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="6f4b5-133">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="6f4b5-134">attachment</span><span class="sxs-lookup"><span data-stu-id="6f4b5-134">attachment</span></span>](attachment.md) |<span data-ttu-id="6f4b5-135">Adicionar um anexo de arquivo ou item a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-135">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="6f4b5-136">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="6f4b5-136">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="6f4b5-137">attachment</span><span class="sxs-lookup"><span data-stu-id="6f4b5-137">attachment</span></span>](attachment.md) |<span data-ttu-id="6f4b5-138">Adicionar um anexo de arquivo, item ou link a uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-138">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="6f4b5-139">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="6f4b5-139">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="6f4b5-140">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="6f4b5-140">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="6f4b5-141">Obtenha uma lista de anexos de um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-141">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="6f4b5-142">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="6f4b5-142">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="6f4b5-143">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="6f4b5-143">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="6f4b5-144">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-144">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="6f4b5-145">Listar anexos de uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="6f4b5-145">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="6f4b5-146">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="6f4b5-146">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="6f4b5-147">Obter uma lista de anexos para uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-147">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="6f4b5-148">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="6f4b5-148">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="6f4b5-149">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="6f4b5-149">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="6f4b5-150">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-150">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="6f4b5-151">Delete</span><span class="sxs-lookup"><span data-stu-id="6f4b5-151">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="6f4b5-152">None</span><span class="sxs-lookup"><span data-stu-id="6f4b5-152">None</span></span> |<span data-ttu-id="6f4b5-153">Excluir um anexo de um evento, de uma mensagem, de uma tarefa do Outlook ou de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-153">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="6f4b5-154">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f4b5-154">Properties</span></span>

<span data-ttu-id="6f4b5-p104">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="6f4b5-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f4b5-157">Property</span></span>     | <span data-ttu-id="6f4b5-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f4b5-158">Type</span></span>   |<span data-ttu-id="6f4b5-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f4b5-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f4b5-160">contentType</span><span class="sxs-lookup"><span data-stu-id="6f4b5-160">contentType</span></span>|<span data-ttu-id="6f4b5-161">String</span><span class="sxs-lookup"><span data-stu-id="6f4b5-161">String</span></span>|<span data-ttu-id="6f4b5-162">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-162">The MIME type.</span></span>|
|<span data-ttu-id="6f4b5-163">id</span><span class="sxs-lookup"><span data-stu-id="6f4b5-163">id</span></span>|<span data-ttu-id="6f4b5-164">String</span><span class="sxs-lookup"><span data-stu-id="6f4b5-164">String</span></span>| <span data-ttu-id="6f4b5-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-165">Read-only.</span></span>|
|<span data-ttu-id="6f4b5-166">isInline</span><span class="sxs-lookup"><span data-stu-id="6f4b5-166">isInline</span></span>|<span data-ttu-id="6f4b5-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f4b5-167">Boolean</span></span>|<span data-ttu-id="6f4b5-168">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-168">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="6f4b5-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f4b5-169">lastModifiedDateTime</span></span>|<span data-ttu-id="6f4b5-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f4b5-170">DateTimeOffset</span></span>|<span data-ttu-id="6f4b5-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6f4b5-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6f4b5-173">nome</span><span class="sxs-lookup"><span data-stu-id="6f4b5-173">name</span></span>|<span data-ttu-id="6f4b5-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f4b5-174">String</span></span>|<span data-ttu-id="6f4b5-175">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-175">The display name of the attachment.</span></span> <span data-ttu-id="6f4b5-176">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-176">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="6f4b5-177">size</span><span class="sxs-lookup"><span data-stu-id="6f4b5-177">size</span></span>|<span data-ttu-id="6f4b5-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6f4b5-178">Int32</span></span>|<span data-ttu-id="6f4b5-179">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="6f4b5-179">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f4b5-180">Relações</span><span class="sxs-lookup"><span data-stu-id="6f4b5-180">Relationships</span></span>
<span data-ttu-id="6f4b5-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f4b5-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f4b5-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f4b5-182">JSON representation</span></span>

<span data-ttu-id="6f4b5-183">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6f4b5-183">Here is a JSON representation of the resource</span></span>

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
