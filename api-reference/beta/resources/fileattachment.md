---
title: tipo de recurso fileAttachment
description: Um arquivo (como um arquivo de texto ou documento do Word) anexado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 7161d8bf17aa573cad61123200785ff254c24feb
ms.sourcegitcommit: 36066afdced00f32838a03747d3e7760fc43683a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36453152"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="9b814-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="9b814-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b814-104">Um arquivo (como um arquivo de texto ou documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="9b814-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="9b814-105">A propriedade **contentBytes** contém os conteúdos com codificação base64 do arquivo.</span><span class="sxs-lookup"><span data-stu-id="9b814-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="9b814-106">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="9b814-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="9b814-107">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="9b814-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="9b814-108">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9b814-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9b814-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="9b814-109">Methods</span></span>

| <span data-ttu-id="9b814-110">Método</span><span class="sxs-lookup"><span data-stu-id="9b814-110">Method</span></span>       | <span data-ttu-id="9b814-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9b814-111">Return Type</span></span>  |<span data-ttu-id="9b814-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b814-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b814-113">Get</span><span class="sxs-lookup"><span data-stu-id="9b814-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="9b814-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="9b814-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="9b814-115">Leia as propriedades e os relacionamentos do objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="9b814-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="9b814-116">Delete</span><span class="sxs-lookup"><span data-stu-id="9b814-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="9b814-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9b814-117">None</span></span> |<span data-ttu-id="9b814-118">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="9b814-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b814-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b814-119">Properties</span></span>
| <span data-ttu-id="9b814-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b814-120">Property</span></span>     | <span data-ttu-id="9b814-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b814-121">Type</span></span>   |<span data-ttu-id="9b814-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b814-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b814-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="9b814-123">contentBytes</span></span>|<span data-ttu-id="9b814-124">EDM. Binary</span><span class="sxs-lookup"><span data-stu-id="9b814-124">Edm.Binary</span></span>|<span data-ttu-id="9b814-125">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="9b814-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="9b814-126">contentId</span><span class="sxs-lookup"><span data-stu-id="9b814-126">contentId</span></span>|<span data-ttu-id="9b814-127">String</span><span class="sxs-lookup"><span data-stu-id="9b814-127">String</span></span>|<span data-ttu-id="9b814-128">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b814-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="9b814-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="9b814-129">contentLocation</span></span>|<span data-ttu-id="9b814-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b814-130">String</span></span>|<span data-ttu-id="9b814-131">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b814-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="9b814-132">contentType</span><span class="sxs-lookup"><span data-stu-id="9b814-132">contentType</span></span>|<span data-ttu-id="9b814-133">String</span><span class="sxs-lookup"><span data-stu-id="9b814-133">String</span></span>|<span data-ttu-id="9b814-134">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="9b814-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="9b814-135">id</span><span class="sxs-lookup"><span data-stu-id="9b814-135">id</span></span>|<span data-ttu-id="9b814-136">String</span><span class="sxs-lookup"><span data-stu-id="9b814-136">String</span></span>|<span data-ttu-id="9b814-137">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="9b814-137">The attachment ID.</span></span>|
|<span data-ttu-id="9b814-138">isInline</span><span class="sxs-lookup"><span data-stu-id="9b814-138">isInline</span></span>|<span data-ttu-id="9b814-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b814-139">Boolean</span></span>|<span data-ttu-id="9b814-140">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="9b814-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="9b814-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b814-141">lastModifiedDateTime</span></span>|<span data-ttu-id="9b814-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b814-142">DateTimeOffset</span></span>|<span data-ttu-id="9b814-143">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9b814-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="9b814-144">name</span><span class="sxs-lookup"><span data-stu-id="9b814-144">name</span></span>|<span data-ttu-id="9b814-145">String</span><span class="sxs-lookup"><span data-stu-id="9b814-145">String</span></span>|<span data-ttu-id="9b814-146">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="9b814-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="9b814-147">size</span><span class="sxs-lookup"><span data-stu-id="9b814-147">size</span></span>|<span data-ttu-id="9b814-148">Int32</span><span class="sxs-lookup"><span data-stu-id="9b814-148">Int32</span></span>|<span data-ttu-id="9b814-149">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="9b814-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b814-150">Relações</span><span class="sxs-lookup"><span data-stu-id="9b814-150">Relationships</span></span>
<span data-ttu-id="9b814-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b814-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9b814-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b814-152">JSON representation</span></span>

<span data-ttu-id="9b814-153">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9b814-153">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
