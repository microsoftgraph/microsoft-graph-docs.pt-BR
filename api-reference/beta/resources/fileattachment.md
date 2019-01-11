---
title: tipo de recurso fileAttachment
description: Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um evento,
localization_priority: Normal
ms.openlocfilehash: 7f7270bd5392e2d880daeb45491f4c65e9fca198
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869276"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="e33e2-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="e33e2-103">fileAttachment resource type</span></span>

> <span data-ttu-id="e33e2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e33e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e33e2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e33e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e33e2-106">Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="e33e2-106">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="e33e2-107">A propriedade **contentBytes** contém o conteúdo do arquivo codificado na base64.</span><span class="sxs-lookup"><span data-stu-id="e33e2-107">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="e33e2-108">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="e33e2-108">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="e33e2-109">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="e33e2-109">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="e33e2-110">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e33e2-110">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e33e2-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="e33e2-111">Methods</span></span>

| <span data-ttu-id="e33e2-112">Método</span><span class="sxs-lookup"><span data-stu-id="e33e2-112">Method</span></span>       | <span data-ttu-id="e33e2-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e33e2-113">Return Type</span></span>  |<span data-ttu-id="e33e2-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e33e2-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e33e2-115">Get</span><span class="sxs-lookup"><span data-stu-id="e33e2-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e33e2-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="e33e2-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="e33e2-117">Leia as propriedades e os relacionamentos do objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="e33e2-117">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="e33e2-118">Delete</span><span class="sxs-lookup"><span data-stu-id="e33e2-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e33e2-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e33e2-119">None</span></span> |<span data-ttu-id="e33e2-120">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="e33e2-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e33e2-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e33e2-121">Properties</span></span>
| <span data-ttu-id="e33e2-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e33e2-122">Property</span></span>     | <span data-ttu-id="e33e2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e33e2-123">Type</span></span>   |<span data-ttu-id="e33e2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e33e2-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e33e2-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="e33e2-125">contentBytes</span></span>|<span data-ttu-id="e33e2-126">Binária</span><span class="sxs-lookup"><span data-stu-id="e33e2-126">Binary</span></span>|<span data-ttu-id="e33e2-127">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="e33e2-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="e33e2-128">contentId</span><span class="sxs-lookup"><span data-stu-id="e33e2-128">contentId</span></span>|<span data-ttu-id="e33e2-129">String</span><span class="sxs-lookup"><span data-stu-id="e33e2-129">String</span></span>|<span data-ttu-id="e33e2-130">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e33e2-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="e33e2-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="e33e2-131">contentLocation</span></span>|<span data-ttu-id="e33e2-132">String</span><span class="sxs-lookup"><span data-stu-id="e33e2-132">String</span></span>|<span data-ttu-id="e33e2-133">O URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="e33e2-133">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="e33e2-134">contentType</span><span class="sxs-lookup"><span data-stu-id="e33e2-134">contentType</span></span>|<span data-ttu-id="e33e2-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e33e2-135">String</span></span>|<span data-ttu-id="e33e2-136">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="e33e2-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="e33e2-137">id</span><span class="sxs-lookup"><span data-stu-id="e33e2-137">id</span></span>|<span data-ttu-id="e33e2-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e33e2-138">String</span></span>|<span data-ttu-id="e33e2-139">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="e33e2-139">The attachment ID.</span></span>|
|<span data-ttu-id="e33e2-140">isInline</span><span class="sxs-lookup"><span data-stu-id="e33e2-140">isInline</span></span>|<span data-ttu-id="e33e2-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="e33e2-141">Boolean</span></span>|<span data-ttu-id="e33e2-142">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="e33e2-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="e33e2-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e33e2-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e33e2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33e2-144">DateTimeOffset</span></span>|<span data-ttu-id="e33e2-145">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e33e2-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="e33e2-146">name</span><span class="sxs-lookup"><span data-stu-id="e33e2-146">name</span></span>|<span data-ttu-id="e33e2-147">String</span><span class="sxs-lookup"><span data-stu-id="e33e2-147">String</span></span>|<span data-ttu-id="e33e2-148">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="e33e2-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e33e2-149">size</span><span class="sxs-lookup"><span data-stu-id="e33e2-149">size</span></span>|<span data-ttu-id="e33e2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e33e2-150">Int32</span></span>|<span data-ttu-id="e33e2-151">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="e33e2-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e33e2-152">Relações</span><span class="sxs-lookup"><span data-stu-id="e33e2-152">Relationships</span></span>
<span data-ttu-id="e33e2-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e33e2-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e33e2-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e33e2-154">JSON representation</span></span>

<span data-ttu-id="e33e2-155">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e33e2-155">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
