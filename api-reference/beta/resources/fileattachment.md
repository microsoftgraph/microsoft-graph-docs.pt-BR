---
title: tipo de recurso fileAttachment
description: Um arquivo (como um arquivo de texto ou documento do Word) anexado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: ab81c67bbf0c4d7ab6699d17977c4d1a3907f94e
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484314"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="1b78e-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="1b78e-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b78e-104">Um arquivo (como um arquivo de texto ou documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="1b78e-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="1b78e-105">A propriedade **contentBytes** contém os conteúdos com codificação base64 do arquivo.</span><span class="sxs-lookup"><span data-stu-id="1b78e-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="1b78e-106">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="1b78e-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="1b78e-107">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="1b78e-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="1b78e-108">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="1b78e-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1b78e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b78e-109">Methods</span></span>

| <span data-ttu-id="1b78e-110">Método</span><span class="sxs-lookup"><span data-stu-id="1b78e-110">Method</span></span>       | <span data-ttu-id="1b78e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b78e-111">Return Type</span></span>  |<span data-ttu-id="1b78e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b78e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b78e-113">Get</span><span class="sxs-lookup"><span data-stu-id="1b78e-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="1b78e-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="1b78e-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="1b78e-115">Leia as propriedades e os relacionamentos do objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="1b78e-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="1b78e-116">Delete</span><span class="sxs-lookup"><span data-stu-id="1b78e-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="1b78e-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1b78e-117">None</span></span> |<span data-ttu-id="1b78e-118">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="1b78e-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b78e-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b78e-119">Properties</span></span>
| <span data-ttu-id="1b78e-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b78e-120">Property</span></span>     | <span data-ttu-id="1b78e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b78e-121">Type</span></span>   |<span data-ttu-id="1b78e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b78e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b78e-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="1b78e-123">contentBytes</span></span>|<span data-ttu-id="1b78e-124">EDM. Binary</span><span class="sxs-lookup"><span data-stu-id="1b78e-124">Edm.Binary</span></span>|<span data-ttu-id="1b78e-125">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="1b78e-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="1b78e-126">contentId</span><span class="sxs-lookup"><span data-stu-id="1b78e-126">contentId</span></span>|<span data-ttu-id="1b78e-127">String</span><span class="sxs-lookup"><span data-stu-id="1b78e-127">String</span></span>|<span data-ttu-id="1b78e-128">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b78e-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="1b78e-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="1b78e-129">contentLocation</span></span>|<span data-ttu-id="1b78e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b78e-130">String</span></span>|<span data-ttu-id="1b78e-131">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b78e-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="1b78e-132">contentType</span><span class="sxs-lookup"><span data-stu-id="1b78e-132">contentType</span></span>|<span data-ttu-id="1b78e-133">String</span><span class="sxs-lookup"><span data-stu-id="1b78e-133">String</span></span>|<span data-ttu-id="1b78e-134">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="1b78e-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="1b78e-135">id</span><span class="sxs-lookup"><span data-stu-id="1b78e-135">id</span></span>|<span data-ttu-id="1b78e-136">String</span><span class="sxs-lookup"><span data-stu-id="1b78e-136">String</span></span>|<span data-ttu-id="1b78e-137">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="1b78e-137">The attachment ID.</span></span>|
|<span data-ttu-id="1b78e-138">isInline</span><span class="sxs-lookup"><span data-stu-id="1b78e-138">isInline</span></span>|<span data-ttu-id="1b78e-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b78e-139">Boolean</span></span>|<span data-ttu-id="1b78e-140">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="1b78e-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="1b78e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b78e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1b78e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b78e-142">DateTimeOffset</span></span>|<span data-ttu-id="1b78e-143">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1b78e-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="1b78e-144">name</span><span class="sxs-lookup"><span data-stu-id="1b78e-144">name</span></span>|<span data-ttu-id="1b78e-145">String</span><span class="sxs-lookup"><span data-stu-id="1b78e-145">String</span></span>|<span data-ttu-id="1b78e-146">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="1b78e-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="1b78e-147">size</span><span class="sxs-lookup"><span data-stu-id="1b78e-147">size</span></span>|<span data-ttu-id="1b78e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1b78e-148">Int32</span></span>|<span data-ttu-id="1b78e-149">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="1b78e-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b78e-150">Relações</span><span class="sxs-lookup"><span data-stu-id="1b78e-150">Relationships</span></span>
<span data-ttu-id="1b78e-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b78e-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1b78e-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b78e-152">JSON representation</span></span>

<span data-ttu-id="1b78e-153">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1b78e-153">Here is a JSON representation of the resource</span></span>

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
