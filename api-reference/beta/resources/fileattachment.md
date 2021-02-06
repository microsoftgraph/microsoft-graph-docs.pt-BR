---
title: tipo de recurso fileAttachment
description: Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 1ef32e91897ac322b84922012df47c168094f57d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135643"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="f5a9d-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="f5a9d-103">fileAttachment resource type</span></span>

<span data-ttu-id="f5a9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5a9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="f5a9d-105">Um arquivo (como um arquivo de texto ou documento do Word) anexado a um evento de usuário [,](../resources/event.md) [mensagem](../resources/message.md), tarefa do [Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="f5a9d-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="f5a9d-106">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="f5a9d-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="f5a9d-107">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="f5a9d-108">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f5a9d-108">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f5a9d-109">Certifique-se de codificar o conteúdo do arquivo em Base64 antes de atribuí-lo a **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-109">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="f5a9d-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="f5a9d-110">Methods</span></span>

| <span data-ttu-id="f5a9d-111">Método</span><span class="sxs-lookup"><span data-stu-id="f5a9d-111">Method</span></span>       | <span data-ttu-id="f5a9d-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f5a9d-112">Return Type</span></span>  |<span data-ttu-id="f5a9d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5a9d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5a9d-114">Get</span><span class="sxs-lookup"><span data-stu-id="f5a9d-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="f5a9d-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="f5a9d-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="f5a9d-116">Leia as propriedades, relações ou conteúdo bruto de um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="f5a9d-117">Delete</span><span class="sxs-lookup"><span data-stu-id="f5a9d-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="f5a9d-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f5a9d-118">None</span></span> |<span data-ttu-id="f5a9d-119">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f5a9d-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5a9d-120">Properties</span></span>
| <span data-ttu-id="f5a9d-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5a9d-121">Property</span></span>     | <span data-ttu-id="f5a9d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5a9d-122">Type</span></span>   |<span data-ttu-id="f5a9d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5a9d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5a9d-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="f5a9d-124">contentBytes</span></span>|<span data-ttu-id="f5a9d-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="f5a9d-125">Edm.Binary</span></span>|<span data-ttu-id="f5a9d-126">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="f5a9d-127">contentId</span><span class="sxs-lookup"><span data-stu-id="f5a9d-127">contentId</span></span>|<span data-ttu-id="f5a9d-128">String</span><span class="sxs-lookup"><span data-stu-id="f5a9d-128">String</span></span>|<span data-ttu-id="f5a9d-129">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="f5a9d-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="f5a9d-130">contentLocation</span></span>|<span data-ttu-id="f5a9d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5a9d-131">String</span></span>|<span data-ttu-id="f5a9d-132">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="f5a9d-133">contentType</span><span class="sxs-lookup"><span data-stu-id="f5a9d-133">contentType</span></span>|<span data-ttu-id="f5a9d-134">String</span><span class="sxs-lookup"><span data-stu-id="f5a9d-134">String</span></span>|<span data-ttu-id="f5a9d-135">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="f5a9d-136">id</span><span class="sxs-lookup"><span data-stu-id="f5a9d-136">id</span></span>|<span data-ttu-id="f5a9d-137">String</span><span class="sxs-lookup"><span data-stu-id="f5a9d-137">String</span></span>|<span data-ttu-id="f5a9d-138">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-138">The attachment ID.</span></span>|
|<span data-ttu-id="f5a9d-139">isInline</span><span class="sxs-lookup"><span data-stu-id="f5a9d-139">isInline</span></span>|<span data-ttu-id="f5a9d-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5a9d-140">Boolean</span></span>|<span data-ttu-id="f5a9d-141">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="f5a9d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5a9d-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f5a9d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5a9d-143">DateTimeOffset</span></span>|<span data-ttu-id="f5a9d-144">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="f5a9d-145">name</span><span class="sxs-lookup"><span data-stu-id="f5a9d-145">name</span></span>|<span data-ttu-id="f5a9d-146">String</span><span class="sxs-lookup"><span data-stu-id="f5a9d-146">String</span></span>|<span data-ttu-id="f5a9d-147">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="f5a9d-148">size</span><span class="sxs-lookup"><span data-stu-id="f5a9d-148">size</span></span>|<span data-ttu-id="f5a9d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f5a9d-149">Int32</span></span>|<span data-ttu-id="f5a9d-150">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="f5a9d-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5a9d-151">Relações</span><span class="sxs-lookup"><span data-stu-id="f5a9d-151">Relationships</span></span>
<span data-ttu-id="f5a9d-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5a9d-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f5a9d-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5a9d-153">JSON representation</span></span>

<span data-ttu-id="f5a9d-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f5a9d-154">Here is a JSON representation of the resource</span></span>

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


