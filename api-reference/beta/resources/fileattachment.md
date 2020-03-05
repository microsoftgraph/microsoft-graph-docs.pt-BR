---
title: tipo de recurso fileAttachment
description: Um arquivo (como um arquivo de texto ou documento do Word) anexado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: c77f5294a191b827673e52ee60c132713b16e490
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498298"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="55a23-103">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="55a23-103">fileAttachment resource type</span></span>

<span data-ttu-id="55a23-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="55a23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55a23-105">Um arquivo (como um arquivo de texto ou documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="55a23-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="55a23-106">A propriedade **contentBytes** contém os conteúdos com codificação base64 do arquivo.</span><span class="sxs-lookup"><span data-stu-id="55a23-106">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="55a23-107">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="55a23-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="55a23-108">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="55a23-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="55a23-109">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="55a23-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="55a23-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="55a23-110">Methods</span></span>

| <span data-ttu-id="55a23-111">Método</span><span class="sxs-lookup"><span data-stu-id="55a23-111">Method</span></span>       | <span data-ttu-id="55a23-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="55a23-112">Return Type</span></span>  |<span data-ttu-id="55a23-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="55a23-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55a23-114">Get</span><span class="sxs-lookup"><span data-stu-id="55a23-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="55a23-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="55a23-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="55a23-116">Leia as propriedades, relações ou conteúdo bruto de um objeto fileattachment.</span><span class="sxs-lookup"><span data-stu-id="55a23-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="55a23-117">Delete</span><span class="sxs-lookup"><span data-stu-id="55a23-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="55a23-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="55a23-118">None</span></span> |<span data-ttu-id="55a23-119">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="55a23-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="55a23-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55a23-120">Properties</span></span>
| <span data-ttu-id="55a23-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55a23-121">Property</span></span>     | <span data-ttu-id="55a23-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="55a23-122">Type</span></span>   |<span data-ttu-id="55a23-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="55a23-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55a23-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="55a23-124">contentBytes</span></span>|<span data-ttu-id="55a23-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="55a23-125">Edm.Binary</span></span>|<span data-ttu-id="55a23-126">O conteúdo do arquivo codificado pela base64.</span><span class="sxs-lookup"><span data-stu-id="55a23-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="55a23-127">contentId</span><span class="sxs-lookup"><span data-stu-id="55a23-127">contentId</span></span>|<span data-ttu-id="55a23-128">String</span><span class="sxs-lookup"><span data-stu-id="55a23-128">String</span></span>|<span data-ttu-id="55a23-129">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="55a23-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="55a23-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="55a23-130">contentLocation</span></span>|<span data-ttu-id="55a23-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55a23-131">String</span></span>|<span data-ttu-id="55a23-132">Não use essa propriedade que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="55a23-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="55a23-133">contentType</span><span class="sxs-lookup"><span data-stu-id="55a23-133">contentType</span></span>|<span data-ttu-id="55a23-134">String</span><span class="sxs-lookup"><span data-stu-id="55a23-134">String</span></span>|<span data-ttu-id="55a23-135">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="55a23-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="55a23-136">id</span><span class="sxs-lookup"><span data-stu-id="55a23-136">id</span></span>|<span data-ttu-id="55a23-137">String</span><span class="sxs-lookup"><span data-stu-id="55a23-137">String</span></span>|<span data-ttu-id="55a23-138">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="55a23-138">The attachment ID.</span></span>|
|<span data-ttu-id="55a23-139">isInline</span><span class="sxs-lookup"><span data-stu-id="55a23-139">isInline</span></span>|<span data-ttu-id="55a23-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="55a23-140">Boolean</span></span>|<span data-ttu-id="55a23-141">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="55a23-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="55a23-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55a23-142">lastModifiedDateTime</span></span>|<span data-ttu-id="55a23-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55a23-143">DateTimeOffset</span></span>|<span data-ttu-id="55a23-144">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="55a23-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="55a23-145">name</span><span class="sxs-lookup"><span data-stu-id="55a23-145">name</span></span>|<span data-ttu-id="55a23-146">String</span><span class="sxs-lookup"><span data-stu-id="55a23-146">String</span></span>|<span data-ttu-id="55a23-147">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="55a23-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="55a23-148">size</span><span class="sxs-lookup"><span data-stu-id="55a23-148">size</span></span>|<span data-ttu-id="55a23-149">Int32</span><span class="sxs-lookup"><span data-stu-id="55a23-149">Int32</span></span>|<span data-ttu-id="55a23-150">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="55a23-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55a23-151">Relações</span><span class="sxs-lookup"><span data-stu-id="55a23-151">Relationships</span></span>
<span data-ttu-id="55a23-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55a23-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="55a23-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55a23-153">JSON representation</span></span>

<span data-ttu-id="55a23-154">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="55a23-154">Here is a JSON representation of the resource</span></span>

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
