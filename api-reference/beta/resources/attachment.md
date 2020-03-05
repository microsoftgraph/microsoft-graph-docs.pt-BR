---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 7aebce941e9af369dc8e04c41f75142479f42d4c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508161"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="92ce1-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="92ce1-103">attachment resource type</span></span>

<span data-ttu-id="92ce1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92ce1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92ce1-105">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md)de usuário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) de grupo no formato de um anexo.</span><span class="sxs-lookup"><span data-stu-id="92ce1-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="92ce1-106">Os eventos em calendários de grupo não têm suporte para anexos.</span><span class="sxs-lookup"><span data-stu-id="92ce1-106">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="92ce1-107">As tarefas do Outlook não dão suporte a anexos de referência.</span><span class="sxs-lookup"><span data-stu-id="92ce1-107">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="92ce1-108">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="92ce1-108">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="92ce1-109">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="92ce1-109">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="92ce1-110">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="92ce1-110">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="92ce1-111">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="92ce1-111">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="92ce1-112">**Observação**: há um limite para o tamanho do arquivo ou anexo de item que pode ser adicionado abaixo de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="92ce1-112">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="92ce1-113">No entanto, se estiver anexando a uma mensagem um arquivo entre 3 MB e 150MB, você pode [criar uma sessão de carregamento](../api/attachment-createuploadsession.md) e carregar de forma iterativa os intervalos do arquivo para anexá-lo.</span><span class="sxs-lookup"><span data-stu-id="92ce1-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="92ce1-114">Consulte [anexar arquivos grandes às mensagens do Outlook](/graph/outlook-large-attachments) para obter um exemplo.</span><span class="sxs-lookup"><span data-stu-id="92ce1-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="92ce1-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="92ce1-115">Methods</span></span>

<span data-ttu-id="92ce1-116">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="92ce1-116">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="92ce1-117">Método</span><span class="sxs-lookup"><span data-stu-id="92ce1-117">Method</span></span>       | <span data-ttu-id="92ce1-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="92ce1-118">Return Type</span></span>  |<span data-ttu-id="92ce1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ce1-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92ce1-120">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="92ce1-120">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="92ce1-121">anexo</span><span class="sxs-lookup"><span data-stu-id="92ce1-121">attachment</span></span>](attachment.md) |<span data-ttu-id="92ce1-122">Leia as propriedades, relações ou conteúdo bruto de um anexo, anexados a um evento de usuário, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="92ce1-122">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="92ce1-123">Adicionar anexo a um evento do usuário</span><span class="sxs-lookup"><span data-stu-id="92ce1-123">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="92ce1-124">attachment</span><span class="sxs-lookup"><span data-stu-id="92ce1-124">attachment</span></span>](attachment.md) |<span data-ttu-id="92ce1-125">Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="92ce1-125">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="92ce1-126">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="92ce1-126">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="92ce1-127">attachment</span><span class="sxs-lookup"><span data-stu-id="92ce1-127">attachment</span></span>](attachment.md) |<span data-ttu-id="92ce1-128">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="92ce1-128">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="92ce1-129">Esta operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="92ce1-129">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="92ce1-130">Criar sessão para anexar arquivo grande</span><span class="sxs-lookup"><span data-stu-id="92ce1-130">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="92ce1-131">uploadSession</span><span class="sxs-lookup"><span data-stu-id="92ce1-131">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="92ce1-132">Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de um arquivo de forma iterativa, para anexar o arquivo à **mensagem**especificada.</span><span class="sxs-lookup"><span data-stu-id="92ce1-132">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="92ce1-133">O tamanho do arquivo deve estar entre 3 MB e 150MB.</span><span class="sxs-lookup"><span data-stu-id="92ce1-133">The file size must be between 3MB and 150MB.</span></span>|
|[<span data-ttu-id="92ce1-134">Adicionar anexo a uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="92ce1-134">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="92ce1-135">attachment</span><span class="sxs-lookup"><span data-stu-id="92ce1-135">attachment</span></span>](attachment.md) |<span data-ttu-id="92ce1-136">Adicionar um anexo de arquivo ou item a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="92ce1-136">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="92ce1-137">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="92ce1-137">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="92ce1-138">attachment</span><span class="sxs-lookup"><span data-stu-id="92ce1-138">attachment</span></span>](attachment.md) |<span data-ttu-id="92ce1-139">Adicionar um anexo de arquivo, item ou link a uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="92ce1-139">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="92ce1-140">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="92ce1-140">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="92ce1-141">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="92ce1-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="92ce1-142">Obtenha uma lista de anexos de um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="92ce1-142">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="92ce1-143">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="92ce1-143">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="92ce1-144">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="92ce1-144">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="92ce1-145">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="92ce1-145">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="92ce1-146">Listar anexos de uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="92ce1-146">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="92ce1-147">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="92ce1-147">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="92ce1-148">Obter uma lista de anexos para uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="92ce1-148">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="92ce1-149">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="92ce1-149">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="92ce1-150">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="92ce1-150">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="92ce1-151">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="92ce1-151">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="92ce1-152">Delete</span><span class="sxs-lookup"><span data-stu-id="92ce1-152">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="92ce1-153">None</span><span class="sxs-lookup"><span data-stu-id="92ce1-153">None</span></span> |<span data-ttu-id="92ce1-154">Excluir um anexo de um evento, de uma mensagem, de uma tarefa do Outlook ou de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="92ce1-154">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="92ce1-155">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92ce1-155">Properties</span></span>

<span data-ttu-id="92ce1-p104">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="92ce1-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="92ce1-158">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92ce1-158">Property</span></span>     | <span data-ttu-id="92ce1-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="92ce1-159">Type</span></span>   |<span data-ttu-id="92ce1-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ce1-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92ce1-161">contentType</span><span class="sxs-lookup"><span data-stu-id="92ce1-161">contentType</span></span>|<span data-ttu-id="92ce1-162">String</span><span class="sxs-lookup"><span data-stu-id="92ce1-162">String</span></span>|<span data-ttu-id="92ce1-163">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="92ce1-163">The MIME type.</span></span>|
|<span data-ttu-id="92ce1-164">id</span><span class="sxs-lookup"><span data-stu-id="92ce1-164">id</span></span>|<span data-ttu-id="92ce1-165">String</span><span class="sxs-lookup"><span data-stu-id="92ce1-165">String</span></span>| <span data-ttu-id="92ce1-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92ce1-166">Read-only.</span></span>|
|<span data-ttu-id="92ce1-167">isInline</span><span class="sxs-lookup"><span data-stu-id="92ce1-167">isInline</span></span>|<span data-ttu-id="92ce1-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="92ce1-168">Boolean</span></span>|<span data-ttu-id="92ce1-169">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="92ce1-169">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="92ce1-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92ce1-170">lastModifiedDateTime</span></span>|<span data-ttu-id="92ce1-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92ce1-171">DateTimeOffset</span></span>|<span data-ttu-id="92ce1-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="92ce1-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="92ce1-174">nome</span><span class="sxs-lookup"><span data-stu-id="92ce1-174">name</span></span>|<span data-ttu-id="92ce1-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92ce1-175">String</span></span>|<span data-ttu-id="92ce1-176">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="92ce1-176">The display name of the attachment.</span></span> <span data-ttu-id="92ce1-177">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="92ce1-177">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="92ce1-178">size</span><span class="sxs-lookup"><span data-stu-id="92ce1-178">size</span></span>|<span data-ttu-id="92ce1-179">Int32</span><span class="sxs-lookup"><span data-stu-id="92ce1-179">Int32</span></span>|<span data-ttu-id="92ce1-180">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="92ce1-180">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92ce1-181">Relações</span><span class="sxs-lookup"><span data-stu-id="92ce1-181">Relationships</span></span>
<span data-ttu-id="92ce1-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92ce1-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92ce1-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92ce1-183">JSON representation</span></span>

<span data-ttu-id="92ce1-184">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="92ce1-184">Here is a JSON representation of the resource</span></span>

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
