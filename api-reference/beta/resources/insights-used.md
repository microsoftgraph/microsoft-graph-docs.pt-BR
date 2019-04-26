---
title: tipo de recurso usedInsight
description: Uma percepção representando documentos usados por um usuário específico. O insights retorna os documentos mais relevantes que um usuário tenha exibido ou acessado.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 407822dc4ff3f0536b0cbff3bf2894ad96d5d878
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333549"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="63956-104">tipo de recurso usedInsight</span><span class="sxs-lookup"><span data-stu-id="63956-104">usedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63956-105">Uma percepção representando documentos usados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="63956-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="63956-106">O insights retorna os documentos mais relevantes que um usuário tenha exibido ou acessado.</span><span class="sxs-lookup"><span data-stu-id="63956-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="63956-107">Isso inclui documentos em:</span><span class="sxs-lookup"><span data-stu-id="63956-107">This includes documents in:</span></span>

- <span data-ttu-id="63956-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="63956-108">OneDrive for Business</span></span>
- <span data-ttu-id="63956-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="63956-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="63956-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="63956-110">Methods</span></span>

| <span data-ttu-id="63956-111">Método</span><span class="sxs-lookup"><span data-stu-id="63956-111">Method</span></span>       | <span data-ttu-id="63956-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="63956-112">Return Type</span></span>  |<span data-ttu-id="63956-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="63956-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="63956-114">Listar usados</span><span class="sxs-lookup"><span data-stu-id="63956-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="63956-115">coleção [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="63956-115">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="63956-116">Obtenha uma lista de arquivos usados.</span><span class="sxs-lookup"><span data-stu-id="63956-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="63956-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63956-117">Properties</span></span>

| <span data-ttu-id="63956-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63956-118">Property</span></span>              | <span data-ttu-id="63956-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="63956-119">Type</span></span>                      | <span data-ttu-id="63956-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63956-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="63956-121">id</span><span class="sxs-lookup"><span data-stu-id="63956-121">id</span></span>                    | <span data-ttu-id="63956-122">String</span><span class="sxs-lookup"><span data-stu-id="63956-122">String</span></span>                    | <span data-ttu-id="63956-123">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="63956-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="63956-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63956-124">Read only.</span></span>        |
| <span data-ttu-id="63956-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="63956-125">lastUsed</span></span>              | [<span data-ttu-id="63956-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="63956-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="63956-127">Informações sobre quando o item foi exibido e modificado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="63956-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="63956-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63956-128">Read only.</span></span>     |
| <span data-ttu-id="63956-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="63956-129">resourceVisualization</span></span> | [<span data-ttu-id="63956-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="63956-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="63956-131">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="63956-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="63956-132">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="63956-132">Read-only</span></span>      |
| <span data-ttu-id="63956-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="63956-133">resourceReference</span></span>     | [<span data-ttu-id="63956-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="63956-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="63956-135">Propriedades de referência do documento usado, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="63956-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="63956-136">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="63956-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="63956-137">Relações</span><span class="sxs-lookup"><span data-stu-id="63956-137">Relationships</span></span>

| <span data-ttu-id="63956-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63956-138">Property</span></span>      | <span data-ttu-id="63956-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="63956-139">Type</span></span>          | <span data-ttu-id="63956-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="63956-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="63956-141">recurso</span><span class="sxs-lookup"><span data-stu-id="63956-141">resource</span></span>      | <span data-ttu-id="63956-142">coleção [Entity](entity.md)</span><span class="sxs-lookup"><span data-stu-id="63956-142">[entity](entity.md) collection</span></span>    | <span data-ttu-id="63956-143">Usado para navegar até o item que foi usado.</span><span class="sxs-lookup"><span data-stu-id="63956-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="63956-144">Para anexos de arquivo, o tipo \*\* é fileattachment.</span><span class="sxs-lookup"><span data-stu-id="63956-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="63956-145">Para anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="63956-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="63956-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63956-146">JSON representation</span></span>
<span data-ttu-id="63956-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="63956-147">Here is a JSON representation of the resource</span></span>

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
