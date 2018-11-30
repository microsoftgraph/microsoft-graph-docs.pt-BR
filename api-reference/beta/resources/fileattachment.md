---
title: tipo de recurso fileAttachment
description: Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um evento,
ms.openlocfilehash: 2a43ebbc78d831e907bfd19d647e4b7e398abe90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037337"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="cb00c-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="cb00c-103">fileAttachment resource type</span></span>

> <span data-ttu-id="cb00c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb00c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb00c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb00c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb00c-106">Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="cb00c-106">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="cb00c-107">A propriedade **contentBytes** contém o conteúdo do arquivo codificado na base64.</span><span class="sxs-lookup"><span data-stu-id="cb00c-107">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="cb00c-108">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="cb00c-108">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="cb00c-109">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="cb00c-109">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="cb00c-110">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="cb00c-110">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cb00c-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="cb00c-111">Methods</span></span>

| <span data-ttu-id="cb00c-112">Método</span><span class="sxs-lookup"><span data-stu-id="cb00c-112">Method</span></span>       | <span data-ttu-id="cb00c-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cb00c-113">Return Type</span></span>  |<span data-ttu-id="cb00c-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb00c-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cb00c-115">Get</span><span class="sxs-lookup"><span data-stu-id="cb00c-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="cb00c-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="cb00c-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="cb00c-117">Leia as propriedades e os relacionamentos do objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="cb00c-117">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="cb00c-118">Delete</span><span class="sxs-lookup"><span data-stu-id="cb00c-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="cb00c-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cb00c-119">None</span></span> |<span data-ttu-id="cb00c-120">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="cb00c-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb00c-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb00c-121">Properties</span></span>
| <span data-ttu-id="cb00c-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb00c-122">Property</span></span>     | <span data-ttu-id="cb00c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb00c-123">Type</span></span>   |<span data-ttu-id="cb00c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb00c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb00c-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="cb00c-125">contentBytes</span></span>|<span data-ttu-id="cb00c-126">Binária</span><span class="sxs-lookup"><span data-stu-id="cb00c-126">Binary</span></span>|<span data-ttu-id="cb00c-127">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="cb00c-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="cb00c-128">contentId</span><span class="sxs-lookup"><span data-stu-id="cb00c-128">contentId</span></span>|<span data-ttu-id="cb00c-129">String</span><span class="sxs-lookup"><span data-stu-id="cb00c-129">String</span></span>|<span data-ttu-id="cb00c-130">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb00c-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="cb00c-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="cb00c-131">contentLocation</span></span>|<span data-ttu-id="cb00c-132">String</span><span class="sxs-lookup"><span data-stu-id="cb00c-132">String</span></span>|<span data-ttu-id="cb00c-133">O URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="cb00c-133">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="cb00c-134">contentType</span><span class="sxs-lookup"><span data-stu-id="cb00c-134">contentType</span></span>|<span data-ttu-id="cb00c-135">String</span><span class="sxs-lookup"><span data-stu-id="cb00c-135">String</span></span>|<span data-ttu-id="cb00c-136">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="cb00c-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="cb00c-137">id</span><span class="sxs-lookup"><span data-stu-id="cb00c-137">id</span></span>|<span data-ttu-id="cb00c-138">String</span><span class="sxs-lookup"><span data-stu-id="cb00c-138">String</span></span>|<span data-ttu-id="cb00c-139">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="cb00c-139">The attachment ID.</span></span>|
|<span data-ttu-id="cb00c-140">isInline</span><span class="sxs-lookup"><span data-stu-id="cb00c-140">isInline</span></span>|<span data-ttu-id="cb00c-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="cb00c-141">Boolean</span></span>|<span data-ttu-id="cb00c-142">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="cb00c-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="cb00c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb00c-143">lastModifiedDateTime</span></span>|<span data-ttu-id="cb00c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb00c-144">DateTimeOffset</span></span>|<span data-ttu-id="cb00c-145">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cb00c-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="cb00c-146">name</span><span class="sxs-lookup"><span data-stu-id="cb00c-146">name</span></span>|<span data-ttu-id="cb00c-147">String</span><span class="sxs-lookup"><span data-stu-id="cb00c-147">String</span></span>|<span data-ttu-id="cb00c-148">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="cb00c-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="cb00c-149">size</span><span class="sxs-lookup"><span data-stu-id="cb00c-149">size</span></span>|<span data-ttu-id="cb00c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="cb00c-150">Int32</span></span>|<span data-ttu-id="cb00c-151">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="cb00c-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb00c-152">Relações</span><span class="sxs-lookup"><span data-stu-id="cb00c-152">Relationships</span></span>
<span data-ttu-id="cb00c-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb00c-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cb00c-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb00c-154">JSON representation</span></span>

<span data-ttu-id="cb00c-155">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cb00c-155">Here is a JSON representation of the resource</span></span>

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
