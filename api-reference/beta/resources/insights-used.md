---
title: tipo de recurso usedInsight
description: Uma percepção representando documentos usados por um usuário específico. O insights retorna os documentos mais relevantes que um usuário tenha exibido ou acessado.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7a334e701012b4794018c19d57f350e7f4fe1b07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495470"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="52c3e-104">tipo de recurso usedInsight</span><span class="sxs-lookup"><span data-stu-id="52c3e-104">usedInsight resource type</span></span>

<span data-ttu-id="52c3e-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52c3e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52c3e-106">Uma percepção representando documentos usados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="52c3e-106">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="52c3e-107">O insights retorna os documentos mais relevantes que um usuário tenha exibido ou acessado.</span><span class="sxs-lookup"><span data-stu-id="52c3e-107">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="52c3e-108">Isso inclui documentos em:</span><span class="sxs-lookup"><span data-stu-id="52c3e-108">This includes documents in:</span></span>

- <span data-ttu-id="52c3e-109">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="52c3e-109">OneDrive for Business</span></span>
- <span data-ttu-id="52c3e-110">SharePoint</span><span class="sxs-lookup"><span data-stu-id="52c3e-110">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="52c3e-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="52c3e-111">Methods</span></span>

| <span data-ttu-id="52c3e-112">Método</span><span class="sxs-lookup"><span data-stu-id="52c3e-112">Method</span></span>       | <span data-ttu-id="52c3e-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52c3e-113">Return Type</span></span>  |<span data-ttu-id="52c3e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="52c3e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52c3e-115">Listar usados</span><span class="sxs-lookup"><span data-stu-id="52c3e-115">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="52c3e-116">coleção [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="52c3e-116">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="52c3e-117">Obtenha uma lista de arquivos usados.</span><span class="sxs-lookup"><span data-stu-id="52c3e-117">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="52c3e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52c3e-118">Properties</span></span>

| <span data-ttu-id="52c3e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52c3e-119">Property</span></span>              | <span data-ttu-id="52c3e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="52c3e-120">Type</span></span>                      | <span data-ttu-id="52c3e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="52c3e-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="52c3e-122">id</span><span class="sxs-lookup"><span data-stu-id="52c3e-122">id</span></span>                    | <span data-ttu-id="52c3e-123">String</span><span class="sxs-lookup"><span data-stu-id="52c3e-123">String</span></span>                    | <span data-ttu-id="52c3e-124">Identificador exclusivo da relação.</span><span class="sxs-lookup"><span data-stu-id="52c3e-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="52c3e-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52c3e-125">Read only.</span></span>        |
| <span data-ttu-id="52c3e-126">lastUsed</span><span class="sxs-lookup"><span data-stu-id="52c3e-126">lastUsed</span></span>              | [<span data-ttu-id="52c3e-127">usageDetails</span><span class="sxs-lookup"><span data-stu-id="52c3e-127">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="52c3e-128">Informações sobre quando o item foi exibido e modificado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="52c3e-128">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="52c3e-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52c3e-129">Read only.</span></span>     |
| <span data-ttu-id="52c3e-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="52c3e-130">resourceVisualization</span></span> | [<span data-ttu-id="52c3e-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="52c3e-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="52c3e-132">Propriedades que você pode usar para visualizar o documento em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="52c3e-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="52c3e-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="52c3e-133">Read-only</span></span>      |
| <span data-ttu-id="52c3e-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="52c3e-134">resourceReference</span></span>     | [<span data-ttu-id="52c3e-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="52c3e-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="52c3e-136">Propriedades de referência do documento usado, como a URL e o tipo do documento.</span><span class="sxs-lookup"><span data-stu-id="52c3e-136">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="52c3e-137">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="52c3e-137">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="52c3e-138">Relações</span><span class="sxs-lookup"><span data-stu-id="52c3e-138">Relationships</span></span>

| <span data-ttu-id="52c3e-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52c3e-139">Property</span></span>      | <span data-ttu-id="52c3e-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="52c3e-140">Type</span></span>          | <span data-ttu-id="52c3e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="52c3e-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="52c3e-142">recurso</span><span class="sxs-lookup"><span data-stu-id="52c3e-142">resource</span></span>      | <span data-ttu-id="52c3e-143">coleção [Entity](entity.md)</span><span class="sxs-lookup"><span data-stu-id="52c3e-143">[entity](entity.md) collection</span></span>    | <span data-ttu-id="52c3e-144">Usado para navegar até o item que foi usado.</span><span class="sxs-lookup"><span data-stu-id="52c3e-144">Used for navigating to the item that was used.</span></span> <span data-ttu-id="52c3e-145">Para anexos de arquivo, o tipo é *Fileattachment*.</span><span class="sxs-lookup"><span data-stu-id="52c3e-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="52c3e-146">Para anexos vinculados, o tipo é *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="52c3e-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52c3e-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52c3e-147">JSON representation</span></span>
<span data-ttu-id="52c3e-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="52c3e-148">Here is a JSON representation of the resource</span></span>

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
