---
title: tipo de recurso fileAttachment
description: 'Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento, mensagem ou postagem. O  **contentBytes** '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d71eb6e142097474ac6616456cf6e57ceb8cfb02
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484349"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="3facf-104">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="3facf-104">fileAttachment resource type</span></span>

<span data-ttu-id="3facf-p102">Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento, mensagem ou postagem. A propriedade **contentBytes** contém os conteúdos com codificação base64 do arquivo.</span><span class="sxs-lookup"><span data-stu-id="3facf-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="3facf-107">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="3facf-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="3facf-108">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="3facf-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="3facf-109">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3facf-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3facf-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="3facf-110">Methods</span></span>

| <span data-ttu-id="3facf-111">Método</span><span class="sxs-lookup"><span data-stu-id="3facf-111">Method</span></span>       | <span data-ttu-id="3facf-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3facf-112">Return Type</span></span>  |<span data-ttu-id="3facf-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3facf-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3facf-114">Get</span><span class="sxs-lookup"><span data-stu-id="3facf-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3facf-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="3facf-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="3facf-116">Leia as propriedades e os relacionamentos do objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="3facf-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="3facf-117">Delete</span><span class="sxs-lookup"><span data-stu-id="3facf-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="3facf-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3facf-118">None</span></span> |<span data-ttu-id="3facf-119">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="3facf-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3facf-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3facf-120">Properties</span></span>
| <span data-ttu-id="3facf-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3facf-121">Property</span></span>     | <span data-ttu-id="3facf-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3facf-122">Type</span></span>   |<span data-ttu-id="3facf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3facf-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3facf-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="3facf-124">contentBytes</span></span>|<span data-ttu-id="3facf-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="3facf-125">Edm.Binary</span></span>|<span data-ttu-id="3facf-126">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="3facf-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="3facf-127">contentId</span><span class="sxs-lookup"><span data-stu-id="3facf-127">contentId</span></span>|<span data-ttu-id="3facf-128">String</span><span class="sxs-lookup"><span data-stu-id="3facf-128">String</span></span>|<span data-ttu-id="3facf-129">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3facf-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="3facf-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="3facf-130">contentLocation</span></span>|<span data-ttu-id="3facf-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3facf-131">String</span></span>|<span data-ttu-id="3facf-132">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="3facf-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="3facf-133">contentType</span><span class="sxs-lookup"><span data-stu-id="3facf-133">contentType</span></span>|<span data-ttu-id="3facf-134">String</span><span class="sxs-lookup"><span data-stu-id="3facf-134">String</span></span>|<span data-ttu-id="3facf-135">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="3facf-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="3facf-136">id</span><span class="sxs-lookup"><span data-stu-id="3facf-136">id</span></span>|<span data-ttu-id="3facf-137">String</span><span class="sxs-lookup"><span data-stu-id="3facf-137">String</span></span>|<span data-ttu-id="3facf-138">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="3facf-138">The attachment ID.</span></span>|
|<span data-ttu-id="3facf-139">isInline</span><span class="sxs-lookup"><span data-stu-id="3facf-139">isInline</span></span>|<span data-ttu-id="3facf-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="3facf-140">Boolean</span></span>|<span data-ttu-id="3facf-141">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="3facf-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="3facf-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3facf-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3facf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3facf-143">DateTimeOffset</span></span>|<span data-ttu-id="3facf-144">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3facf-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="3facf-145">name</span><span class="sxs-lookup"><span data-stu-id="3facf-145">name</span></span>|<span data-ttu-id="3facf-146">String</span><span class="sxs-lookup"><span data-stu-id="3facf-146">String</span></span>|<span data-ttu-id="3facf-147">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="3facf-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="3facf-148">size</span><span class="sxs-lookup"><span data-stu-id="3facf-148">size</span></span>|<span data-ttu-id="3facf-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3facf-149">Int32</span></span>|<span data-ttu-id="3facf-150">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="3facf-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3facf-151">Relações</span><span class="sxs-lookup"><span data-stu-id="3facf-151">Relationships</span></span>
<span data-ttu-id="3facf-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3facf-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3facf-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3facf-153">JSON representation</span></span>

<span data-ttu-id="3facf-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3facf-154">Here is a JSON representation of the resource</span></span>

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
