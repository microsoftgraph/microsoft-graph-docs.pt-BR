---
title: tipo de recurso fileAttachment
description: 'Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento, mensagem ou postagem. O  **contentBytes** '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ad8c1a9ffd4a4b5cc68554505464173a40aafd29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531430"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="889d3-104">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="889d3-104">fileAttachment resource type</span></span>

<span data-ttu-id="889d3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="889d3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="889d3-p102">Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md) ou [postagem](../resources/post.md). A propriedade **contentBytes** possui os conteúdos codificados base64 do arquivo.</span><span class="sxs-lookup"><span data-stu-id="889d3-p102">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md). The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="889d3-108">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="889d3-108">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="889d3-109">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="889d3-109">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="889d3-110">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="889d3-110">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="889d3-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="889d3-111">Methods</span></span>

| <span data-ttu-id="889d3-112">Método</span><span class="sxs-lookup"><span data-stu-id="889d3-112">Method</span></span>       | <span data-ttu-id="889d3-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="889d3-113">Return Type</span></span>  |<span data-ttu-id="889d3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="889d3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="889d3-115">Get</span><span class="sxs-lookup"><span data-stu-id="889d3-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="889d3-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="889d3-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="889d3-117">Leia as propriedades, relações ou conteúdo bruto de um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="889d3-117">Read properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="889d3-118">Delete</span><span class="sxs-lookup"><span data-stu-id="889d3-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="889d3-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="889d3-119">None</span></span> |<span data-ttu-id="889d3-120">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="889d3-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="889d3-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="889d3-121">Properties</span></span>
| <span data-ttu-id="889d3-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="889d3-122">Property</span></span>     | <span data-ttu-id="889d3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="889d3-123">Type</span></span>   |<span data-ttu-id="889d3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="889d3-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="889d3-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="889d3-125">contentBytes</span></span>|<span data-ttu-id="889d3-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="889d3-126">Edm.Binary</span></span>|<span data-ttu-id="889d3-127">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="889d3-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="889d3-128">contentId</span><span class="sxs-lookup"><span data-stu-id="889d3-128">contentId</span></span>|<span data-ttu-id="889d3-129">String</span><span class="sxs-lookup"><span data-stu-id="889d3-129">String</span></span>|<span data-ttu-id="889d3-130">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="889d3-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="889d3-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="889d3-131">contentLocation</span></span>|<span data-ttu-id="889d3-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="889d3-132">String</span></span>|<span data-ttu-id="889d3-133">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="889d3-133">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="889d3-134">contentType</span><span class="sxs-lookup"><span data-stu-id="889d3-134">contentType</span></span>|<span data-ttu-id="889d3-135">String</span><span class="sxs-lookup"><span data-stu-id="889d3-135">String</span></span>|<span data-ttu-id="889d3-136">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="889d3-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="889d3-137">id</span><span class="sxs-lookup"><span data-stu-id="889d3-137">id</span></span>|<span data-ttu-id="889d3-138">String</span><span class="sxs-lookup"><span data-stu-id="889d3-138">String</span></span>|<span data-ttu-id="889d3-139">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="889d3-139">The attachment ID.</span></span>|
|<span data-ttu-id="889d3-140">isInline</span><span class="sxs-lookup"><span data-stu-id="889d3-140">isInline</span></span>|<span data-ttu-id="889d3-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="889d3-141">Boolean</span></span>|<span data-ttu-id="889d3-142">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="889d3-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="889d3-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="889d3-143">lastModifiedDateTime</span></span>|<span data-ttu-id="889d3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="889d3-144">DateTimeOffset</span></span>|<span data-ttu-id="889d3-145">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="889d3-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="889d3-146">name</span><span class="sxs-lookup"><span data-stu-id="889d3-146">name</span></span>|<span data-ttu-id="889d3-147">String</span><span class="sxs-lookup"><span data-stu-id="889d3-147">String</span></span>|<span data-ttu-id="889d3-148">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="889d3-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="889d3-149">size</span><span class="sxs-lookup"><span data-stu-id="889d3-149">size</span></span>|<span data-ttu-id="889d3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="889d3-150">Int32</span></span>|<span data-ttu-id="889d3-151">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="889d3-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="889d3-152">Relações</span><span class="sxs-lookup"><span data-stu-id="889d3-152">Relationships</span></span>
<span data-ttu-id="889d3-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="889d3-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="889d3-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="889d3-154">JSON representation</span></span>

<span data-ttu-id="889d3-155">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="889d3-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "string (binary)",
  "contentId": "string",
  "contentLocation": "string",
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
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
