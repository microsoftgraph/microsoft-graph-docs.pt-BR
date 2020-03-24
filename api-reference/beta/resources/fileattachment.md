---
title: tipo de recurso fileAttachment
description: Um arquivo (como um arquivo de texto ou documento do Word) anexado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: e14b98c5ee3302d5b19bc7ad92187112b6d8c80b
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926796"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="e50c1-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="e50c1-103">fileAttachment resource type</span></span>

<span data-ttu-id="e50c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e50c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e50c1-105">Um arquivo (como um arquivo de texto ou documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="e50c1-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="e50c1-106">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="e50c1-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="e50c1-107">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="e50c1-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="e50c1-108">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e50c1-108">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="e50c1-109">Certifique-se de codificar o conteúdo do arquivo na base64 antes de atribuí-lo ao **contentbytes necessárias**.</span><span class="sxs-lookup"><span data-stu-id="e50c1-109">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="e50c1-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="e50c1-110">Methods</span></span>

| <span data-ttu-id="e50c1-111">Método</span><span class="sxs-lookup"><span data-stu-id="e50c1-111">Method</span></span>       | <span data-ttu-id="e50c1-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e50c1-112">Return Type</span></span>  |<span data-ttu-id="e50c1-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e50c1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e50c1-114">Get</span><span class="sxs-lookup"><span data-stu-id="e50c1-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e50c1-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="e50c1-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="e50c1-116">Leia as propriedades, relações ou conteúdo bruto de um objeto fileattachment.</span><span class="sxs-lookup"><span data-stu-id="e50c1-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="e50c1-117">Delete</span><span class="sxs-lookup"><span data-stu-id="e50c1-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e50c1-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e50c1-118">None</span></span> |<span data-ttu-id="e50c1-119">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="e50c1-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e50c1-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e50c1-120">Properties</span></span>
| <span data-ttu-id="e50c1-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e50c1-121">Property</span></span>     | <span data-ttu-id="e50c1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e50c1-122">Type</span></span>   |<span data-ttu-id="e50c1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e50c1-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e50c1-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="e50c1-124">contentBytes</span></span>|<span data-ttu-id="e50c1-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="e50c1-125">Edm.Binary</span></span>|<span data-ttu-id="e50c1-126">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="e50c1-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="e50c1-127">contentId</span><span class="sxs-lookup"><span data-stu-id="e50c1-127">contentId</span></span>|<span data-ttu-id="e50c1-128">String</span><span class="sxs-lookup"><span data-stu-id="e50c1-128">String</span></span>|<span data-ttu-id="e50c1-129">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e50c1-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="e50c1-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="e50c1-130">contentLocation</span></span>|<span data-ttu-id="e50c1-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e50c1-131">String</span></span>|<span data-ttu-id="e50c1-132">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="e50c1-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="e50c1-133">contentType</span><span class="sxs-lookup"><span data-stu-id="e50c1-133">contentType</span></span>|<span data-ttu-id="e50c1-134">String</span><span class="sxs-lookup"><span data-stu-id="e50c1-134">String</span></span>|<span data-ttu-id="e50c1-135">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="e50c1-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="e50c1-136">id</span><span class="sxs-lookup"><span data-stu-id="e50c1-136">id</span></span>|<span data-ttu-id="e50c1-137">String</span><span class="sxs-lookup"><span data-stu-id="e50c1-137">String</span></span>|<span data-ttu-id="e50c1-138">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="e50c1-138">The attachment ID.</span></span>|
|<span data-ttu-id="e50c1-139">isInline</span><span class="sxs-lookup"><span data-stu-id="e50c1-139">isInline</span></span>|<span data-ttu-id="e50c1-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="e50c1-140">Boolean</span></span>|<span data-ttu-id="e50c1-141">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="e50c1-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="e50c1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e50c1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e50c1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e50c1-143">DateTimeOffset</span></span>|<span data-ttu-id="e50c1-144">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e50c1-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="e50c1-145">name</span><span class="sxs-lookup"><span data-stu-id="e50c1-145">name</span></span>|<span data-ttu-id="e50c1-146">String</span><span class="sxs-lookup"><span data-stu-id="e50c1-146">String</span></span>|<span data-ttu-id="e50c1-147">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="e50c1-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e50c1-148">size</span><span class="sxs-lookup"><span data-stu-id="e50c1-148">size</span></span>|<span data-ttu-id="e50c1-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e50c1-149">Int32</span></span>|<span data-ttu-id="e50c1-150">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="e50c1-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e50c1-151">Relações</span><span class="sxs-lookup"><span data-stu-id="e50c1-151">Relationships</span></span>
<span data-ttu-id="e50c1-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e50c1-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e50c1-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e50c1-153">JSON representation</span></span>

<span data-ttu-id="e50c1-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e50c1-154">Here is a JSON representation of the resource</span></span>

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
