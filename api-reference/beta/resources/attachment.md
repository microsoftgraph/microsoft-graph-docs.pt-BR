---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: a6810ff870124a793bee40ec9df66ae7cb5eabc8
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621656"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="e54f2-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="e54f2-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e54f2-104">Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md)de usuário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) de grupo no formato de um anexo.</span><span class="sxs-lookup"><span data-stu-id="e54f2-104">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="e54f2-105">Os eventos em calendários de grupo não têm suporte para anexos.</span><span class="sxs-lookup"><span data-stu-id="e54f2-105">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="e54f2-106">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="e54f2-106">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="e54f2-107">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="e54f2-107">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="e54f2-108">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="e54f2-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="e54f2-109">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="e54f2-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="e54f2-110">**Observação**: como há atualmente um limite de 4MB no tamanho total de cada solicitação REST, em geral, isso limita o tamanho do anexo de arquivo ou item que pode ser adicionado em 4 MB.</span><span class="sxs-lookup"><span data-stu-id="e54f2-110">**Note**: Since there is currently a limit of 4MB on the total size of each REST request, in general, this limits the size of the file or item attachment you can add to under 4MB.</span></span> 
>
> <span data-ttu-id="e54f2-111">No entanto, se estiver anexando a uma mensagem um arquivo entre 3 MB e 150MB, você pode [criar uma sessão de carregamento](../api/attachment-createuploadsession.md) e carregar de forma iterativa os intervalos do arquivo para anexá-lo.</span><span class="sxs-lookup"><span data-stu-id="e54f2-111">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="e54f2-112">Consulte [anexar arquivos grandes às mensagens do Outlook](/graph/outlook-large-attachments) para obter um exemplo.</span><span class="sxs-lookup"><span data-stu-id="e54f2-112">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="e54f2-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="e54f2-113">Methods</span></span>

<span data-ttu-id="e54f2-114">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="e54f2-114">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="e54f2-115">Método</span><span class="sxs-lookup"><span data-stu-id="e54f2-115">Method</span></span>       | <span data-ttu-id="e54f2-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e54f2-116">Return Type</span></span>  |<span data-ttu-id="e54f2-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e54f2-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e54f2-118">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="e54f2-118">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e54f2-119">anexo</span><span class="sxs-lookup"><span data-stu-id="e54f2-119">attachment</span></span>](attachment.md) |<span data-ttu-id="e54f2-120">Leia as propriedades, relações ou conteúdo bruto de um anexo, anexados a um evento de usuário, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="e54f2-120">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="e54f2-121">Adicionar anexo a um evento do usuário</span><span class="sxs-lookup"><span data-stu-id="e54f2-121">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="e54f2-122">attachment</span><span class="sxs-lookup"><span data-stu-id="e54f2-122">attachment</span></span>](attachment.md) |<span data-ttu-id="e54f2-123">Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="e54f2-123">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="e54f2-124">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="e54f2-124">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="e54f2-125">attachment</span><span class="sxs-lookup"><span data-stu-id="e54f2-125">attachment</span></span>](attachment.md) |<span data-ttu-id="e54f2-126">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="e54f2-126">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="e54f2-127">Ao anexar um arquivo, o tamanho do arquivo deve ser menor que 4 MB.</span><span class="sxs-lookup"><span data-stu-id="e54f2-127">If attaching a file, the file size must be less than 4MB.</span></span>|
|[<span data-ttu-id="e54f2-128">Criar sessão para anexar arquivo grande</span><span class="sxs-lookup"><span data-stu-id="e54f2-128">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="e54f2-129">uploadSession</span><span class="sxs-lookup"><span data-stu-id="e54f2-129">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="e54f2-130">Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de um arquivo de forma iterativa, para anexar o arquivo à **mensagem**especificada.</span><span class="sxs-lookup"><span data-stu-id="e54f2-130">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="e54f2-131">O tamanho do arquivo deve estar entre 3 MB e 150MB.</span><span class="sxs-lookup"><span data-stu-id="e54f2-131">The file size must be between 3MB and 150MB.</span></span>|
|[<span data-ttu-id="e54f2-132">Adicionar anexo a uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="e54f2-132">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="e54f2-133">attachment</span><span class="sxs-lookup"><span data-stu-id="e54f2-133">attachment</span></span>](attachment.md) |<span data-ttu-id="e54f2-134">Adicionar um anexo de arquivo, item ou link a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="e54f2-134">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="e54f2-135">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="e54f2-135">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="e54f2-136">attachment</span><span class="sxs-lookup"><span data-stu-id="e54f2-136">attachment</span></span>](attachment.md) |<span data-ttu-id="e54f2-137">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="e54f2-137">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="e54f2-138">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="e54f2-138">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="e54f2-139">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="e54f2-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e54f2-140">Obtenha uma lista de anexos de um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="e54f2-140">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="e54f2-141">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="e54f2-141">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="e54f2-142">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="e54f2-142">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e54f2-143">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="e54f2-143">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="e54f2-144">Listar anexos de uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="e54f2-144">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="e54f2-145">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="e54f2-145">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e54f2-146">Obter uma lista de anexos para uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="e54f2-146">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="e54f2-147">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="e54f2-147">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="e54f2-148">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="e54f2-148">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e54f2-149">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="e54f2-149">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="e54f2-150">Delete</span><span class="sxs-lookup"><span data-stu-id="e54f2-150">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e54f2-151">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e54f2-151">None</span></span> |<span data-ttu-id="e54f2-152">Excluir um anexo de um evento, de uma mensagem, de uma tarefa do Outlook ou de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="e54f2-152">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="e54f2-153">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e54f2-153">Properties</span></span>

<span data-ttu-id="e54f2-p104">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="e54f2-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="e54f2-156">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e54f2-156">Property</span></span>     | <span data-ttu-id="e54f2-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="e54f2-157">Type</span></span>   |<span data-ttu-id="e54f2-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="e54f2-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e54f2-159">contentType</span><span class="sxs-lookup"><span data-stu-id="e54f2-159">contentType</span></span>|<span data-ttu-id="e54f2-160">String</span><span class="sxs-lookup"><span data-stu-id="e54f2-160">String</span></span>|<span data-ttu-id="e54f2-161">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="e54f2-161">The MIME type.</span></span>|
|<span data-ttu-id="e54f2-162">id</span><span class="sxs-lookup"><span data-stu-id="e54f2-162">id</span></span>|<span data-ttu-id="e54f2-163">String</span><span class="sxs-lookup"><span data-stu-id="e54f2-163">String</span></span>| <span data-ttu-id="e54f2-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e54f2-164">Read-only.</span></span>|
|<span data-ttu-id="e54f2-165">isInline</span><span class="sxs-lookup"><span data-stu-id="e54f2-165">isInline</span></span>|<span data-ttu-id="e54f2-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="e54f2-166">Boolean</span></span>|<span data-ttu-id="e54f2-167">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="e54f2-167">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="e54f2-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e54f2-168">lastModifiedDateTime</span></span>|<span data-ttu-id="e54f2-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e54f2-169">DateTimeOffset</span></span>|<span data-ttu-id="e54f2-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e54f2-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e54f2-172">nome</span><span class="sxs-lookup"><span data-stu-id="e54f2-172">name</span></span>|<span data-ttu-id="e54f2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e54f2-173">String</span></span>|<span data-ttu-id="e54f2-174">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="e54f2-174">The display name of the attachment.</span></span> <span data-ttu-id="e54f2-175">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e54f2-175">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e54f2-176">size</span><span class="sxs-lookup"><span data-stu-id="e54f2-176">size</span></span>|<span data-ttu-id="e54f2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e54f2-177">Int32</span></span>|<span data-ttu-id="e54f2-178">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="e54f2-178">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e54f2-179">Relações</span><span class="sxs-lookup"><span data-stu-id="e54f2-179">Relationships</span></span>
<span data-ttu-id="e54f2-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e54f2-180">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e54f2-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e54f2-181">JSON representation</span></span>

<span data-ttu-id="e54f2-182">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e54f2-182">Here is a JSON representation of the resource</span></span>

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
