---
title: tipo de recurso fileAttachment
description: 'Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento, mensagem ou postagem. O  **contentBytes** '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4975e9b46a4b55429906fbcd9b7b23f8774a47e9
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036197"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="528b9-104">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="528b9-104">fileAttachment resource type</span></span>

<span data-ttu-id="528b9-p102">Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md) ou [postagem](../resources/post.md). A propriedade **contentBytes** possui os conteúdos codificados base64 do arquivo.</span><span class="sxs-lookup"><span data-stu-id="528b9-p102">A file (such as a text file or Word document) attached to an event, message or post. The  contentBytes property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="528b9-107">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="528b9-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="528b9-108">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="528b9-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="528b9-109">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="528b9-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="528b9-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="528b9-110">Methods</span></span>

| <span data-ttu-id="528b9-111">Método</span><span class="sxs-lookup"><span data-stu-id="528b9-111">Method</span></span>       | <span data-ttu-id="528b9-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="528b9-112">Return Type</span></span>  |<span data-ttu-id="528b9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="528b9-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="528b9-114">Get</span><span class="sxs-lookup"><span data-stu-id="528b9-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="528b9-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="528b9-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="528b9-116">Leia as propriedades, relações ou conteúdo bruto de um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="528b9-116">Read properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="528b9-117">Delete</span><span class="sxs-lookup"><span data-stu-id="528b9-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="528b9-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="528b9-118">None</span></span> |<span data-ttu-id="528b9-119">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="528b9-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="528b9-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="528b9-120">Properties</span></span>
| <span data-ttu-id="528b9-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="528b9-121">Property</span></span>     | <span data-ttu-id="528b9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="528b9-122">Type</span></span>   |<span data-ttu-id="528b9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="528b9-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="528b9-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="528b9-124">contentBytes</span></span>|<span data-ttu-id="528b9-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="528b9-125">Edm.Binary</span></span>|<span data-ttu-id="528b9-126">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="528b9-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="528b9-127">contentId</span><span class="sxs-lookup"><span data-stu-id="528b9-127">contentId</span></span>|<span data-ttu-id="528b9-128">String</span><span class="sxs-lookup"><span data-stu-id="528b9-128">String</span></span>|<span data-ttu-id="528b9-129">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="528b9-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="528b9-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="528b9-130">contentLocation</span></span>|<span data-ttu-id="528b9-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="528b9-131">String</span></span>|<span data-ttu-id="528b9-132">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="528b9-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="528b9-133">contentType</span><span class="sxs-lookup"><span data-stu-id="528b9-133">contentType</span></span>|<span data-ttu-id="528b9-134">String</span><span class="sxs-lookup"><span data-stu-id="528b9-134">String</span></span>|<span data-ttu-id="528b9-135">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="528b9-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="528b9-136">id</span><span class="sxs-lookup"><span data-stu-id="528b9-136">id</span></span>|<span data-ttu-id="528b9-137">String</span><span class="sxs-lookup"><span data-stu-id="528b9-137">String</span></span>|<span data-ttu-id="528b9-138">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="528b9-138">The attachment ID.</span></span>|
|<span data-ttu-id="528b9-139">isInline</span><span class="sxs-lookup"><span data-stu-id="528b9-139">isInline</span></span>|<span data-ttu-id="528b9-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="528b9-140">Boolean</span></span>|<span data-ttu-id="528b9-141">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="528b9-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="528b9-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="528b9-142">lastModifiedDateTime</span></span>|<span data-ttu-id="528b9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="528b9-143">DateTimeOffset</span></span>|<span data-ttu-id="528b9-144">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="528b9-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="528b9-145">name</span><span class="sxs-lookup"><span data-stu-id="528b9-145">name</span></span>|<span data-ttu-id="528b9-146">String</span><span class="sxs-lookup"><span data-stu-id="528b9-146">String</span></span>|<span data-ttu-id="528b9-147">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="528b9-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="528b9-148">size</span><span class="sxs-lookup"><span data-stu-id="528b9-148">size</span></span>|<span data-ttu-id="528b9-149">Int32</span><span class="sxs-lookup"><span data-stu-id="528b9-149">Int32</span></span>|<span data-ttu-id="528b9-150">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="528b9-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="528b9-151">Relações</span><span class="sxs-lookup"><span data-stu-id="528b9-151">Relationships</span></span>
<span data-ttu-id="528b9-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="528b9-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="528b9-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="528b9-153">JSON representation</span></span>

<span data-ttu-id="528b9-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="528b9-154">Here is a JSON representation of the resource</span></span>

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
