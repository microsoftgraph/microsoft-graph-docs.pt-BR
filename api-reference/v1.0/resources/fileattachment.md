---
title: tipo de recurso fileAttachment
description: 'Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um evento, a mensagem ou postagem. O **contentBytes** '
localization_priority: Priority
ms.openlocfilehash: 81de7a12ca371158d7f6369861a8a197fd544821
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870053"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="3ee4c-104">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="3ee4c-104">fileAttachment resource type</span></span>

<span data-ttu-id="3ee4c-p102">Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento, mensagem ou postagem. A propriedade **contentBytes** contém os conteúdos com codificação base64 do arquivo.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="3ee4c-107">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="3ee4c-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="3ee4c-108">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="3ee4c-109">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3ee4c-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3ee4c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="3ee4c-110">Methods</span></span>

| <span data-ttu-id="3ee4c-111">Método</span><span class="sxs-lookup"><span data-stu-id="3ee4c-111">Method</span></span>       | <span data-ttu-id="3ee4c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3ee4c-112">Return Type</span></span>  |<span data-ttu-id="3ee4c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ee4c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ee4c-114">Get</span><span class="sxs-lookup"><span data-stu-id="3ee4c-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3ee4c-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="3ee4c-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="3ee4c-116">Leia as propriedades e os relacionamentos do objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="3ee4c-117">Delete</span><span class="sxs-lookup"><span data-stu-id="3ee4c-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="3ee4c-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3ee4c-118">None</span></span> |<span data-ttu-id="3ee4c-119">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ee4c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ee4c-120">Properties</span></span>
| <span data-ttu-id="3ee4c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ee4c-121">Property</span></span>     | <span data-ttu-id="3ee4c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ee4c-122">Type</span></span>   |<span data-ttu-id="3ee4c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ee4c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ee4c-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="3ee4c-124">contentBytes</span></span>|<span data-ttu-id="3ee4c-125">Binária</span><span class="sxs-lookup"><span data-stu-id="3ee4c-125">Binary</span></span>|<span data-ttu-id="3ee4c-126">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="3ee4c-127">contentId</span><span class="sxs-lookup"><span data-stu-id="3ee4c-127">contentId</span></span>|<span data-ttu-id="3ee4c-128">String</span><span class="sxs-lookup"><span data-stu-id="3ee4c-128">String</span></span>|<span data-ttu-id="3ee4c-129">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="3ee4c-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="3ee4c-130">contentLocation</span></span>|<span data-ttu-id="3ee4c-131">String</span><span class="sxs-lookup"><span data-stu-id="3ee4c-131">String</span></span>|<span data-ttu-id="3ee4c-132">O URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-132">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="3ee4c-133">contentType</span><span class="sxs-lookup"><span data-stu-id="3ee4c-133">contentType</span></span>|<span data-ttu-id="3ee4c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ee4c-134">String</span></span>|<span data-ttu-id="3ee4c-135">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="3ee4c-136">id</span><span class="sxs-lookup"><span data-stu-id="3ee4c-136">id</span></span>|<span data-ttu-id="3ee4c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ee4c-137">String</span></span>|<span data-ttu-id="3ee4c-138">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-138">The attachment ID.</span></span>|
|<span data-ttu-id="3ee4c-139">isInline</span><span class="sxs-lookup"><span data-stu-id="3ee4c-139">isInline</span></span>|<span data-ttu-id="3ee4c-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ee4c-140">Boolean</span></span>|<span data-ttu-id="3ee4c-141">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="3ee4c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ee4c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3ee4c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ee4c-143">DateTimeOffset</span></span>|<span data-ttu-id="3ee4c-144">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="3ee4c-145">name</span><span class="sxs-lookup"><span data-stu-id="3ee4c-145">name</span></span>|<span data-ttu-id="3ee4c-146">String</span><span class="sxs-lookup"><span data-stu-id="3ee4c-146">String</span></span>|<span data-ttu-id="3ee4c-147">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="3ee4c-148">size</span><span class="sxs-lookup"><span data-stu-id="3ee4c-148">size</span></span>|<span data-ttu-id="3ee4c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3ee4c-149">Int32</span></span>|<span data-ttu-id="3ee4c-150">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="3ee4c-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ee4c-151">Relações</span><span class="sxs-lookup"><span data-stu-id="3ee4c-151">Relationships</span></span>
<span data-ttu-id="3ee4c-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ee4c-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3ee4c-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ee4c-153">JSON representation</span></span>

<span data-ttu-id="3ee4c-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3ee4c-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
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
