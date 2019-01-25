---
title: tipo de recurso fileAttachment
description: Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um evento,
localization_priority: Normal
ms.openlocfilehash: 7032bcd234d07f0f3fdce0787968d72530a0a442
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510761"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="a59fb-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="a59fb-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a59fb-104">Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="a59fb-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="a59fb-105">A propriedade **contentBytes** contém o conteúdo do arquivo codificado na base64.</span><span class="sxs-lookup"><span data-stu-id="a59fb-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="a59fb-106">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="a59fb-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="a59fb-107">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="a59fb-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="a59fb-108">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="a59fb-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a59fb-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a59fb-109">Methods</span></span>

| <span data-ttu-id="a59fb-110">Método</span><span class="sxs-lookup"><span data-stu-id="a59fb-110">Method</span></span>       | <span data-ttu-id="a59fb-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a59fb-111">Return Type</span></span>  |<span data-ttu-id="a59fb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a59fb-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a59fb-113">Get</span><span class="sxs-lookup"><span data-stu-id="a59fb-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="a59fb-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="a59fb-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="a59fb-115">Leia as propriedades e os relacionamentos do objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="a59fb-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="a59fb-116">Delete</span><span class="sxs-lookup"><span data-stu-id="a59fb-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="a59fb-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a59fb-117">None</span></span> |<span data-ttu-id="a59fb-118">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="a59fb-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a59fb-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a59fb-119">Properties</span></span>
| <span data-ttu-id="a59fb-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a59fb-120">Property</span></span>     | <span data-ttu-id="a59fb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a59fb-121">Type</span></span>   |<span data-ttu-id="a59fb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a59fb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a59fb-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="a59fb-123">contentBytes</span></span>|<span data-ttu-id="a59fb-124">Binária</span><span class="sxs-lookup"><span data-stu-id="a59fb-124">Binary</span></span>|<span data-ttu-id="a59fb-125">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="a59fb-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="a59fb-126">contentId</span><span class="sxs-lookup"><span data-stu-id="a59fb-126">contentId</span></span>|<span data-ttu-id="a59fb-127">String</span><span class="sxs-lookup"><span data-stu-id="a59fb-127">String</span></span>|<span data-ttu-id="a59fb-128">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a59fb-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="a59fb-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="a59fb-129">contentLocation</span></span>|<span data-ttu-id="a59fb-130">String</span><span class="sxs-lookup"><span data-stu-id="a59fb-130">String</span></span>|<span data-ttu-id="a59fb-131">O URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="a59fb-131">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="a59fb-132">contentType</span><span class="sxs-lookup"><span data-stu-id="a59fb-132">contentType</span></span>|<span data-ttu-id="a59fb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59fb-133">String</span></span>|<span data-ttu-id="a59fb-134">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="a59fb-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="a59fb-135">id</span><span class="sxs-lookup"><span data-stu-id="a59fb-135">id</span></span>|<span data-ttu-id="a59fb-136">String</span><span class="sxs-lookup"><span data-stu-id="a59fb-136">String</span></span>|<span data-ttu-id="a59fb-137">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="a59fb-137">The attachment ID.</span></span>|
|<span data-ttu-id="a59fb-138">isInline</span><span class="sxs-lookup"><span data-stu-id="a59fb-138">isInline</span></span>|<span data-ttu-id="a59fb-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="a59fb-139">Boolean</span></span>|<span data-ttu-id="a59fb-140">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="a59fb-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="a59fb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a59fb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="a59fb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59fb-142">DateTimeOffset</span></span>|<span data-ttu-id="a59fb-143">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a59fb-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="a59fb-144">name</span><span class="sxs-lookup"><span data-stu-id="a59fb-144">name</span></span>|<span data-ttu-id="a59fb-145">String</span><span class="sxs-lookup"><span data-stu-id="a59fb-145">String</span></span>|<span data-ttu-id="a59fb-146">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="a59fb-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="a59fb-147">size</span><span class="sxs-lookup"><span data-stu-id="a59fb-147">size</span></span>|<span data-ttu-id="a59fb-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a59fb-148">Int32</span></span>|<span data-ttu-id="a59fb-149">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="a59fb-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a59fb-150">Relações</span><span class="sxs-lookup"><span data-stu-id="a59fb-150">Relationships</span></span>
<span data-ttu-id="a59fb-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a59fb-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a59fb-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a59fb-152">JSON representation</span></span>

<span data-ttu-id="a59fb-153">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a59fb-153">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/fileattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
