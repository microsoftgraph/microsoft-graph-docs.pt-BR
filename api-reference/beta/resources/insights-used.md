---
title: tipo de recurso usedInsight
description: Uma percepção representando documentos usados por um usuário específico. O insights retorna os documentos mais relevantes exibidos ou modificados por um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4c1d159ecb9750e7ad531f19f61d8ebbb462dbcc
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2020
ms.locfileid: "44226993"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="c5b27-104">tipo de recurso usedInsight</span><span class="sxs-lookup"><span data-stu-id="c5b27-104">usedInsight resource type</span></span>

<span data-ttu-id="c5b27-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5b27-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5b27-106">Uma percepção representando documentos usados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="c5b27-106">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="c5b27-107">O insights retorna os documentos mais relevantes exibidos ou modificados por um usuário.</span><span class="sxs-lookup"><span data-stu-id="c5b27-107">The insights returns the most relevant documents that a user viewed or modified.</span></span> <span data-ttu-id="c5b27-108">Isso inclui documentos em:</span><span class="sxs-lookup"><span data-stu-id="c5b27-108">This includes documents in:</span></span>

- <span data-ttu-id="c5b27-109">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="c5b27-109">OneDrive for Business</span></span>
- <span data-ttu-id="c5b27-110">SharePoint</span><span class="sxs-lookup"><span data-stu-id="c5b27-110">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="c5b27-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5b27-111">Methods</span></span>

| <span data-ttu-id="c5b27-112">Método</span><span class="sxs-lookup"><span data-stu-id="c5b27-112">Method</span></span>       | <span data-ttu-id="c5b27-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5b27-113">Return Type</span></span>  |<span data-ttu-id="c5b27-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5b27-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5b27-115">Listar usados</span><span class="sxs-lookup"><span data-stu-id="c5b27-115">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="c5b27-116">coleção [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="c5b27-116">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="c5b27-117">Obtenha uma lista de arquivos usados.</span><span class="sxs-lookup"><span data-stu-id="c5b27-117">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5b27-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5b27-118">Properties</span></span>

| <span data-ttu-id="c5b27-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5b27-119">Property</span></span>              | <span data-ttu-id="c5b27-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5b27-120">Type</span></span>                      | <span data-ttu-id="c5b27-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5b27-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="c5b27-122">id</span><span class="sxs-lookup"><span data-stu-id="c5b27-122">id</span></span>                    | <span data-ttu-id="c5b27-123">String</span><span class="sxs-lookup"><span data-stu-id="c5b27-123">String</span></span>                    | <span data-ttu-id="c5b27-124">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="c5b27-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="c5b27-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5b27-125">Read only.</span></span>        |
| <span data-ttu-id="c5b27-126">lastUsed</span><span class="sxs-lookup"><span data-stu-id="c5b27-126">lastUsed</span></span>              | [<span data-ttu-id="c5b27-127">usageDetails</span><span class="sxs-lookup"><span data-stu-id="c5b27-127">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="c5b27-128">Informações sobre quando o item foi visualizado ou modificado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="c5b27-128">Information about when the item was last viewed or modified by the user.</span></span> <span data-ttu-id="c5b27-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5b27-129">Read only.</span></span>      |
| <span data-ttu-id="c5b27-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="c5b27-130">resourceVisualization</span></span> | [<span data-ttu-id="c5b27-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="c5b27-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="c5b27-132">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="c5b27-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="c5b27-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c5b27-133">Read-only</span></span>      |
| <span data-ttu-id="c5b27-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="c5b27-134">resourceReference</span></span>     | [<span data-ttu-id="c5b27-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="c5b27-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="c5b27-136">Propriedades de referência do documento usado, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="c5b27-136">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="c5b27-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c5b27-137">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="c5b27-138">Relações</span><span class="sxs-lookup"><span data-stu-id="c5b27-138">Relationships</span></span>

| <span data-ttu-id="c5b27-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5b27-139">Property</span></span>      | <span data-ttu-id="c5b27-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5b27-140">Type</span></span>          | <span data-ttu-id="c5b27-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5b27-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="c5b27-142">recurso</span><span class="sxs-lookup"><span data-stu-id="c5b27-142">resource</span></span>      | <span data-ttu-id="c5b27-143">coleção [Entity](entity.md)</span><span class="sxs-lookup"><span data-stu-id="c5b27-143">[entity](entity.md) collection</span></span>    | <span data-ttu-id="c5b27-144">Usado para navegar até o item que foi usado.</span><span class="sxs-lookup"><span data-stu-id="c5b27-144">Used for navigating to the item that was used.</span></span> <span data-ttu-id="c5b27-145">Para anexos de arquivo, o tipo é *Fileattachment*.</span><span class="sxs-lookup"><span data-stu-id="c5b27-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="c5b27-146">Para anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="c5b27-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5b27-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5b27-147">JSON representation</span></span>
<span data-ttu-id="c5b27-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c5b27-148">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```
