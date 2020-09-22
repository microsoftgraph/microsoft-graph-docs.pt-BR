---
title: tipo de recurso fileAttachment
description: Um arquivo (como um arquivo de texto ou documento do Word) anexado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: a850e05622b22bf05dfec1011cd4371cbc9e7cc4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058456"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="f0eda-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="f0eda-103">fileAttachment resource type</span></span>

<span data-ttu-id="f0eda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0eda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="f0eda-105">Um arquivo (como um arquivo de texto ou documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0eda-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="f0eda-106">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="f0eda-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="f0eda-107">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="f0eda-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="f0eda-108">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f0eda-108">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f0eda-109">Certifique-se de codificar o conteúdo do arquivo em Base64 antes de atribuí-lo a **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="f0eda-109">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="f0eda-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="f0eda-110">Methods</span></span>

| <span data-ttu-id="f0eda-111">Método</span><span class="sxs-lookup"><span data-stu-id="f0eda-111">Method</span></span>       | <span data-ttu-id="f0eda-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f0eda-112">Return Type</span></span>  |<span data-ttu-id="f0eda-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0eda-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0eda-114">Get</span><span class="sxs-lookup"><span data-stu-id="f0eda-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="f0eda-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="f0eda-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="f0eda-116">Leia as propriedades, relações ou conteúdo bruto de um objeto fileattachment.</span><span class="sxs-lookup"><span data-stu-id="f0eda-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="f0eda-117">Delete</span><span class="sxs-lookup"><span data-stu-id="f0eda-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="f0eda-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f0eda-118">None</span></span> |<span data-ttu-id="f0eda-119">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="f0eda-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f0eda-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0eda-120">Properties</span></span>
| <span data-ttu-id="f0eda-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0eda-121">Property</span></span>     | <span data-ttu-id="f0eda-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0eda-122">Type</span></span>   |<span data-ttu-id="f0eda-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0eda-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0eda-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="f0eda-124">contentBytes</span></span>|<span data-ttu-id="f0eda-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="f0eda-125">Edm.Binary</span></span>|<span data-ttu-id="f0eda-126">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="f0eda-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="f0eda-127">contentId</span><span class="sxs-lookup"><span data-stu-id="f0eda-127">contentId</span></span>|<span data-ttu-id="f0eda-128">String</span><span class="sxs-lookup"><span data-stu-id="f0eda-128">String</span></span>|<span data-ttu-id="f0eda-129">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0eda-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="f0eda-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="f0eda-130">contentLocation</span></span>|<span data-ttu-id="f0eda-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0eda-131">String</span></span>|<span data-ttu-id="f0eda-132">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0eda-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="f0eda-133">contentType</span><span class="sxs-lookup"><span data-stu-id="f0eda-133">contentType</span></span>|<span data-ttu-id="f0eda-134">String</span><span class="sxs-lookup"><span data-stu-id="f0eda-134">String</span></span>|<span data-ttu-id="f0eda-135">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="f0eda-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="f0eda-136">id</span><span class="sxs-lookup"><span data-stu-id="f0eda-136">id</span></span>|<span data-ttu-id="f0eda-137">String</span><span class="sxs-lookup"><span data-stu-id="f0eda-137">String</span></span>|<span data-ttu-id="f0eda-138">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="f0eda-138">The attachment ID.</span></span>|
|<span data-ttu-id="f0eda-139">isInline</span><span class="sxs-lookup"><span data-stu-id="f0eda-139">isInline</span></span>|<span data-ttu-id="f0eda-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0eda-140">Boolean</span></span>|<span data-ttu-id="f0eda-141">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="f0eda-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="f0eda-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0eda-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f0eda-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0eda-143">DateTimeOffset</span></span>|<span data-ttu-id="f0eda-144">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f0eda-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="f0eda-145">name</span><span class="sxs-lookup"><span data-stu-id="f0eda-145">name</span></span>|<span data-ttu-id="f0eda-146">String</span><span class="sxs-lookup"><span data-stu-id="f0eda-146">String</span></span>|<span data-ttu-id="f0eda-147">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="f0eda-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="f0eda-148">size</span><span class="sxs-lookup"><span data-stu-id="f0eda-148">size</span></span>|<span data-ttu-id="f0eda-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f0eda-149">Int32</span></span>|<span data-ttu-id="f0eda-150">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="f0eda-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0eda-151">Relações</span><span class="sxs-lookup"><span data-stu-id="f0eda-151">Relationships</span></span>
<span data-ttu-id="f0eda-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0eda-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f0eda-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0eda-153">JSON representation</span></span>

<span data-ttu-id="f0eda-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f0eda-154">Here is a JSON representation of the resource</span></span>

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


