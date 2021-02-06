---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: d1296c40bfc434262f1911c6f9453725bc033999
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137617"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="7ac79-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="7ac79-103">attachment resource type</span></span>

<span data-ttu-id="7ac79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="7ac79-105">Você pode adicionar conteúdo relacionado a um evento de [usuário,](../resources/event.md) [mensagem,](../resources/message.md)tarefa do [Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) de grupo na forma de um anexo.</span><span class="sxs-lookup"><span data-stu-id="7ac79-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="7ac79-106">Os eventos em calendários de grupo não têm suporte para anexos.</span><span class="sxs-lookup"><span data-stu-id="7ac79-106">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="7ac79-107">As tarefas do Outlook não suportam anexos de referência.</span><span class="sxs-lookup"><span data-stu-id="7ac79-107">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="7ac79-108">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="7ac79-108">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="7ac79-109">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="7ac79-109">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="7ac79-110">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="7ac79-110">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="7ac79-111">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="7ac79-111">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="7ac79-112">**Observação:** há um limite para o tamanho do arquivo ou anexo de item que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="7ac79-112">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="7ac79-113">No entanto, se você estiver anexando a uma mensagem um arquivo entre 3 MB e 150 MB, poderá criar uma sessão de [upload](../api/attachment-createuploadsession.md) e carregar iterativamente intervalos do arquivo para anexá-lo.</span><span class="sxs-lookup"><span data-stu-id="7ac79-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="7ac79-114">Veja [anexar arquivos grandes a mensagens do Outlook](/graph/outlook-large-attachments) para ver um exemplo.</span><span class="sxs-lookup"><span data-stu-id="7ac79-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="7ac79-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ac79-115">Methods</span></span>

<span data-ttu-id="7ac79-116">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="7ac79-116">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="7ac79-117">Método</span><span class="sxs-lookup"><span data-stu-id="7ac79-117">Method</span></span>       | <span data-ttu-id="7ac79-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ac79-118">Return Type</span></span>  |<span data-ttu-id="7ac79-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac79-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ac79-120">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="7ac79-120">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="7ac79-121">attachment</span><span class="sxs-lookup"><span data-stu-id="7ac79-121">attachment</span></span>](attachment.md) |<span data-ttu-id="7ac79-122">Leia as propriedades, relações ou conteúdo bruto de um anexo, anexado a um evento de usuário, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="7ac79-122">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="7ac79-123">Adicionar anexo a um evento do usuário</span><span class="sxs-lookup"><span data-stu-id="7ac79-123">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="7ac79-124">attachment</span><span class="sxs-lookup"><span data-stu-id="7ac79-124">attachment</span></span>](attachment.md) |<span data-ttu-id="7ac79-125">Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="7ac79-125">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="7ac79-126">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="7ac79-126">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="7ac79-127">attachment</span><span class="sxs-lookup"><span data-stu-id="7ac79-127">attachment</span></span>](attachment.md) |<span data-ttu-id="7ac79-128">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="7ac79-128">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="7ac79-129">Essa operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="7ac79-129">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="7ac79-130">Criar sessão para anexar arquivo grande</span><span class="sxs-lookup"><span data-stu-id="7ac79-130">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="7ac79-131">uploadSession</span><span class="sxs-lookup"><span data-stu-id="7ac79-131">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="7ac79-132">Crie uma sessão de upload que permita que um aplicativo carregue iterativamente intervalos de um arquivo, para anexar o arquivo à mensagem **especificada.**</span><span class="sxs-lookup"><span data-stu-id="7ac79-132">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="7ac79-133">O tamanho do arquivo deve estar entre 3 MB e 150 MB.</span><span class="sxs-lookup"><span data-stu-id="7ac79-133">The file size must be between 3MB and 150MB.</span></span>|
|<span data-ttu-id="7ac79-134">[Adicionar anexo a uma tarefa do Outlook](../api/outlooktask-post-attachments.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="7ac79-134">[Add attachment to an Outlook task](../api/outlooktask-post-attachments.md) (deprecated)</span></span> | [<span data-ttu-id="7ac79-135">attachment</span><span class="sxs-lookup"><span data-stu-id="7ac79-135">attachment</span></span>](attachment.md) |<span data-ttu-id="7ac79-136">Adicionar um arquivo ou anexo de item a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7ac79-136">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="7ac79-137">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="7ac79-137">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="7ac79-138">attachment</span><span class="sxs-lookup"><span data-stu-id="7ac79-138">attachment</span></span>](attachment.md) |<span data-ttu-id="7ac79-139">Adicione um arquivo, item ou anexo de link a uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="7ac79-139">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="7ac79-140">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="7ac79-140">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="7ac79-141">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7ac79-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="7ac79-142">Obtenha uma lista de anexos de um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="7ac79-142">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="7ac79-143">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="7ac79-143">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="7ac79-144">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7ac79-144">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="7ac79-145">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="7ac79-145">Get a list of attachments for a message.</span></span> |
|<span data-ttu-id="7ac79-146">[Listar anexos de uma tarefa do Outlook](../api/outlooktask-list-attachments.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="7ac79-146">[List attachments of an Outlook task](../api/outlooktask-list-attachments.md) (deprecated)</span></span> | <span data-ttu-id="7ac79-147">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7ac79-147">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="7ac79-148">Obter uma lista de anexos de uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7ac79-148">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="7ac79-149">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="7ac79-149">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="7ac79-150">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="7ac79-150">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="7ac79-151">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="7ac79-151">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="7ac79-152">Delete</span><span class="sxs-lookup"><span data-stu-id="7ac79-152">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="7ac79-153">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7ac79-153">None</span></span> |<span data-ttu-id="7ac79-154">Excluir um anexo em um evento, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="7ac79-154">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ac79-155">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ac79-155">Properties</span></span>

<span data-ttu-id="7ac79-p104">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="7ac79-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="7ac79-158">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac79-158">Property</span></span>     | <span data-ttu-id="7ac79-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac79-159">Type</span></span>   |<span data-ttu-id="7ac79-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac79-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ac79-161">contentType</span><span class="sxs-lookup"><span data-stu-id="7ac79-161">contentType</span></span>|<span data-ttu-id="7ac79-162">String</span><span class="sxs-lookup"><span data-stu-id="7ac79-162">String</span></span>|<span data-ttu-id="7ac79-163">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="7ac79-163">The MIME type.</span></span>|
|<span data-ttu-id="7ac79-164">id</span><span class="sxs-lookup"><span data-stu-id="7ac79-164">id</span></span>|<span data-ttu-id="7ac79-165">String</span><span class="sxs-lookup"><span data-stu-id="7ac79-165">String</span></span>| <span data-ttu-id="7ac79-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ac79-166">Read-only.</span></span>|
|<span data-ttu-id="7ac79-167">isInline</span><span class="sxs-lookup"><span data-stu-id="7ac79-167">isInline</span></span>|<span data-ttu-id="7ac79-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ac79-168">Boolean</span></span>|<span data-ttu-id="7ac79-169">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="7ac79-169">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="7ac79-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac79-170">lastModifiedDateTime</span></span>|<span data-ttu-id="7ac79-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac79-171">DateTimeOffset</span></span>|<span data-ttu-id="7ac79-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7ac79-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7ac79-174">nome</span><span class="sxs-lookup"><span data-stu-id="7ac79-174">name</span></span>|<span data-ttu-id="7ac79-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac79-175">String</span></span>|<span data-ttu-id="7ac79-176">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="7ac79-176">The display name of the attachment.</span></span> <span data-ttu-id="7ac79-177">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="7ac79-177">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="7ac79-178">size</span><span class="sxs-lookup"><span data-stu-id="7ac79-178">size</span></span>|<span data-ttu-id="7ac79-179">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac79-179">Int32</span></span>|<span data-ttu-id="7ac79-180">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="7ac79-180">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ac79-181">Relações</span><span class="sxs-lookup"><span data-stu-id="7ac79-181">Relationships</span></span>
<span data-ttu-id="7ac79-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ac79-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ac79-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ac79-183">JSON representation</span></span>

<span data-ttu-id="7ac79-184">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7ac79-184">Here is a JSON representation of the resource</span></span>

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


