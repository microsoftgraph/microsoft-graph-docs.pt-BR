---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 3faea96a9ef9c19c2d5471c1cc6f58ed84b9a2ef
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721625"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="b49f6-103">tipo de recurso anexo</span><span class="sxs-lookup"><span data-stu-id="b49f6-103">attachment resource type</span></span>

<span data-ttu-id="b49f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b49f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="b49f6-105">Você pode adicionar conteúdo relacionado a um evento [de](../resources/event.md)usuário, [mensagem,](../resources/message.md)tarefa do [Outlook](../resources/outlooktask.md)ou postagem de grupo na forma de um anexo. [](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="b49f6-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md) in the form of an attachment.</span></span> 

<span data-ttu-id="b49f6-106">Os eventos em calendários de grupo não têm suporte para anexos.</span><span class="sxs-lookup"><span data-stu-id="b49f6-106">Events in group calendars do not support attachments.</span></span>

<span data-ttu-id="b49f6-107">As tarefas do Outlook não suportam anexos de referência.</span><span class="sxs-lookup"><span data-stu-id="b49f6-107">Outlook tasks do not support reference attachments.</span></span>

<span data-ttu-id="b49f6-108">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="b49f6-108">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="b49f6-109">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="b49f6-109">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="b49f6-110">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="b49f6-110">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="b49f6-111">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))</span><span class="sxs-lookup"><span data-stu-id="b49f6-111">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

><span data-ttu-id="b49f6-112">**Observação**: há um limite para o tamanho do anexo de arquivo ou item que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="b49f6-112">**Note**: There is a limit to the size of the file or item attachment you can add to under 4 MB.</span></span> 
>
> <span data-ttu-id="b49f6-113">No entanto, se você estiver anexando a uma mensagem um arquivo que esteja entre 3MB e 150 MB, você pode criar uma sessão de [carregamento](../api/attachment-createuploadsession.md) e carregar iterativamente intervalos do arquivo para anexá-lo.</span><span class="sxs-lookup"><span data-stu-id="b49f6-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](../api/attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="b49f6-114">Consulte [anexar arquivos grandes a mensagens do Outlook](/graph/outlook-large-attachments) para um exemplo.</span><span class="sxs-lookup"><span data-stu-id="b49f6-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

## <a name="methods"></a><span data-ttu-id="b49f6-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="b49f6-115">Methods</span></span>

<span data-ttu-id="b49f6-116">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="b49f6-116">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="b49f6-117">Método</span><span class="sxs-lookup"><span data-stu-id="b49f6-117">Method</span></span>       | <span data-ttu-id="b49f6-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b49f6-118">Return Type</span></span>  |<span data-ttu-id="b49f6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b49f6-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b49f6-120">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="b49f6-120">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="b49f6-121">attachment</span><span class="sxs-lookup"><span data-stu-id="b49f6-121">attachment</span></span>](attachment.md) |<span data-ttu-id="b49f6-122">Leia as propriedades, relações ou conteúdo bruto de um anexo, anexado a um evento de usuário, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="b49f6-122">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="b49f6-123">Adicionar anexo a um evento do usuário</span><span class="sxs-lookup"><span data-stu-id="b49f6-123">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="b49f6-124">attachment</span><span class="sxs-lookup"><span data-stu-id="b49f6-124">attachment</span></span>](attachment.md) |<span data-ttu-id="b49f6-125">Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="b49f6-125">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="b49f6-126">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="b49f6-126">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="b49f6-127">attachment</span><span class="sxs-lookup"><span data-stu-id="b49f6-127">attachment</span></span>](attachment.md) |<span data-ttu-id="b49f6-128">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b49f6-128">Add a file, item, or link attachment to a message.</span></span> <span data-ttu-id="b49f6-129">Essa operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="b49f6-129">This operation limits the size of the attachment you can add to under 4 MB.</span></span>|
|[<span data-ttu-id="b49f6-130">Criar sessão para anexar um arquivo grande</span><span class="sxs-lookup"><span data-stu-id="b49f6-130">Create session to attach large file</span></span>](../api/attachment-createuploadsession.md)| [<span data-ttu-id="b49f6-131">uploadSession</span><span class="sxs-lookup"><span data-stu-id="b49f6-131">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="b49f6-132">Crie uma sessão de carregamento que permita que um aplicativo carregue iterativamente intervalos de um arquivo, para anexar o arquivo à mensagem **especificada**.</span><span class="sxs-lookup"><span data-stu-id="b49f6-132">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified **message**.</span></span> <span data-ttu-id="b49f6-133">O tamanho do arquivo deve estar entre 3MB e 150 MB.</span><span class="sxs-lookup"><span data-stu-id="b49f6-133">The file size must be between 3MB and 150MB.</span></span>|
|<span data-ttu-id="b49f6-134">[Adicionar anexo a uma tarefa do Outlook](../api/outlooktask-post-attachments.md) (preterida)</span><span class="sxs-lookup"><span data-stu-id="b49f6-134">[Add attachment to an Outlook task](../api/outlooktask-post-attachments.md) (deprecated)</span></span> | [<span data-ttu-id="b49f6-135">attachment</span><span class="sxs-lookup"><span data-stu-id="b49f6-135">attachment</span></span>](attachment.md) |<span data-ttu-id="b49f6-136">Adicione um arquivo ou anexo de item a uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="b49f6-136">Add a file or item attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="b49f6-137">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="b49f6-137">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="b49f6-138">attachment</span><span class="sxs-lookup"><span data-stu-id="b49f6-138">attachment</span></span>](attachment.md) |<span data-ttu-id="b49f6-139">Adicione um arquivo, item ou anexo de link a uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="b49f6-139">Add a file, item, or link attachment to a group post.</span></span>|
|[<span data-ttu-id="b49f6-140">Listar anexos de um evento de usuário</span><span class="sxs-lookup"><span data-stu-id="b49f6-140">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="b49f6-141">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="b49f6-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="b49f6-142">Obtenha uma lista de anexos de um evento em um calendário de usuário.</span><span class="sxs-lookup"><span data-stu-id="b49f6-142">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="b49f6-143">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="b49f6-143">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="b49f6-144">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="b49f6-144">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="b49f6-145">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b49f6-145">Get a list of attachments for a message.</span></span> |
|<span data-ttu-id="b49f6-146">[Listar anexos de uma tarefa](../api/outlooktask-list-attachments.md) do Outlook (preterida)</span><span class="sxs-lookup"><span data-stu-id="b49f6-146">[List attachments of an Outlook task](../api/outlooktask-list-attachments.md) (deprecated)</span></span> | <span data-ttu-id="b49f6-147">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="b49f6-147">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="b49f6-148">Obter uma lista de anexos para uma tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="b49f6-148">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="b49f6-149">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="b49f6-149">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="b49f6-150">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="b49f6-150">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="b49f6-151">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="b49f6-151">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="b49f6-152">Delete</span><span class="sxs-lookup"><span data-stu-id="b49f6-152">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="b49f6-153">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="b49f6-153">None</span></span> |<span data-ttu-id="b49f6-154">Exclua um anexo em um evento, mensagem, tarefa do Outlook ou postagem.</span><span class="sxs-lookup"><span data-stu-id="b49f6-154">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="b49f6-155">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b49f6-155">Properties</span></span>

<span data-ttu-id="b49f6-p104">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="b49f6-p104">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="b49f6-158">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b49f6-158">Property</span></span>     | <span data-ttu-id="b49f6-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="b49f6-159">Type</span></span>   |<span data-ttu-id="b49f6-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="b49f6-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b49f6-161">contentType</span><span class="sxs-lookup"><span data-stu-id="b49f6-161">contentType</span></span>|<span data-ttu-id="b49f6-162">String</span><span class="sxs-lookup"><span data-stu-id="b49f6-162">String</span></span>|<span data-ttu-id="b49f6-163">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="b49f6-163">The MIME type.</span></span>|
|<span data-ttu-id="b49f6-164">id</span><span class="sxs-lookup"><span data-stu-id="b49f6-164">id</span></span>|<span data-ttu-id="b49f6-165">String</span><span class="sxs-lookup"><span data-stu-id="b49f6-165">String</span></span>| <span data-ttu-id="b49f6-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b49f6-166">Read-only.</span></span>|
|<span data-ttu-id="b49f6-167">isInline</span><span class="sxs-lookup"><span data-stu-id="b49f6-167">isInline</span></span>|<span data-ttu-id="b49f6-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="b49f6-168">Boolean</span></span>|<span data-ttu-id="b49f6-169">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="b49f6-169">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="b49f6-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b49f6-170">lastModifiedDateTime</span></span>|<span data-ttu-id="b49f6-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b49f6-171">DateTimeOffset</span></span>|<span data-ttu-id="b49f6-172">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b49f6-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b49f6-173">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b49f6-173">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b49f6-174">nome</span><span class="sxs-lookup"><span data-stu-id="b49f6-174">name</span></span>|<span data-ttu-id="b49f6-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b49f6-175">String</span></span>|<span data-ttu-id="b49f6-176">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="b49f6-176">The display name of the attachment.</span></span> <span data-ttu-id="b49f6-177">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="b49f6-177">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="b49f6-178">size</span><span class="sxs-lookup"><span data-stu-id="b49f6-178">size</span></span>|<span data-ttu-id="b49f6-179">Int32</span><span class="sxs-lookup"><span data-stu-id="b49f6-179">Int32</span></span>|<span data-ttu-id="b49f6-180">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="b49f6-180">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b49f6-181">Relações</span><span class="sxs-lookup"><span data-stu-id="b49f6-181">Relationships</span></span>
<span data-ttu-id="b49f6-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b49f6-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b49f6-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b49f6-183">JSON representation</span></span>

<span data-ttu-id="b49f6-184">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b49f6-184">Here is a JSON representation of the resource</span></span>

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


