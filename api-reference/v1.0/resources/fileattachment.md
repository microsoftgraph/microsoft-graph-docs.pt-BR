---
title: tipo de recurso fileAttachment
description: 'Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento, mensagem ou postagem. O  **contentBytes** '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: be0f4a15b42b869ae4f8c11f4e384220063dbe97
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926761"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="91f3b-104">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="91f3b-104">fileAttachment resource type</span></span>

<span data-ttu-id="91f3b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91f3b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91f3b-106">Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md) ou [postagem](../resources/post.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="91f3b-106">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="91f3b-107">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="91f3b-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="91f3b-108">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="91f3b-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="91f3b-109">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="91f3b-109">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="91f3b-110">Certifique-se de codificar o conteúdo do arquivo em Base64 antes de atribuí-lo a **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="91f3b-110">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="91f3b-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="91f3b-111">Methods</span></span>

| <span data-ttu-id="91f3b-112">Método</span><span class="sxs-lookup"><span data-stu-id="91f3b-112">Method</span></span>       | <span data-ttu-id="91f3b-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="91f3b-113">Return Type</span></span>  |<span data-ttu-id="91f3b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="91f3b-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91f3b-115">Get</span><span class="sxs-lookup"><span data-stu-id="91f3b-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="91f3b-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="91f3b-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="91f3b-117">Leia as propriedades, relações ou conteúdo bruto de um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="91f3b-117">Read properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="91f3b-118">Delete</span><span class="sxs-lookup"><span data-stu-id="91f3b-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="91f3b-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="91f3b-119">None</span></span> |<span data-ttu-id="91f3b-120">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="91f3b-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="91f3b-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91f3b-121">Properties</span></span>
| <span data-ttu-id="91f3b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91f3b-122">Property</span></span>     | <span data-ttu-id="91f3b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="91f3b-123">Type</span></span>   |<span data-ttu-id="91f3b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="91f3b-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91f3b-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="91f3b-125">contentBytes</span></span>|<span data-ttu-id="91f3b-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="91f3b-126">Edm.Binary</span></span>|<span data-ttu-id="91f3b-127">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="91f3b-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="91f3b-128">contentId</span><span class="sxs-lookup"><span data-stu-id="91f3b-128">contentId</span></span>|<span data-ttu-id="91f3b-129">String</span><span class="sxs-lookup"><span data-stu-id="91f3b-129">String</span></span>|<span data-ttu-id="91f3b-130">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="91f3b-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="91f3b-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="91f3b-131">contentLocation</span></span>|<span data-ttu-id="91f3b-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f3b-132">String</span></span>|<span data-ttu-id="91f3b-133">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="91f3b-133">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="91f3b-134">contentType</span><span class="sxs-lookup"><span data-stu-id="91f3b-134">contentType</span></span>|<span data-ttu-id="91f3b-135">String</span><span class="sxs-lookup"><span data-stu-id="91f3b-135">String</span></span>|<span data-ttu-id="91f3b-136">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="91f3b-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="91f3b-137">id</span><span class="sxs-lookup"><span data-stu-id="91f3b-137">id</span></span>|<span data-ttu-id="91f3b-138">String</span><span class="sxs-lookup"><span data-stu-id="91f3b-138">String</span></span>|<span data-ttu-id="91f3b-139">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="91f3b-139">The attachment ID.</span></span>|
|<span data-ttu-id="91f3b-140">isInline</span><span class="sxs-lookup"><span data-stu-id="91f3b-140">isInline</span></span>|<span data-ttu-id="91f3b-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f3b-141">Boolean</span></span>|<span data-ttu-id="91f3b-142">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="91f3b-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="91f3b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91f3b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="91f3b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f3b-144">DateTimeOffset</span></span>|<span data-ttu-id="91f3b-145">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="91f3b-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="91f3b-146">name</span><span class="sxs-lookup"><span data-stu-id="91f3b-146">name</span></span>|<span data-ttu-id="91f3b-147">String</span><span class="sxs-lookup"><span data-stu-id="91f3b-147">String</span></span>|<span data-ttu-id="91f3b-148">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="91f3b-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="91f3b-149">size</span><span class="sxs-lookup"><span data-stu-id="91f3b-149">size</span></span>|<span data-ttu-id="91f3b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="91f3b-150">Int32</span></span>|<span data-ttu-id="91f3b-151">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="91f3b-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91f3b-152">Relações</span><span class="sxs-lookup"><span data-stu-id="91f3b-152">Relationships</span></span>
<span data-ttu-id="91f3b-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91f3b-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="91f3b-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91f3b-154">JSON representation</span></span>

<span data-ttu-id="91f3b-155">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="91f3b-155">Here is a JSON representation of the resource</span></span>

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
