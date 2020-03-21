---
title: tipo de recurso printUsageSummaryByPrinter
description: Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 86d7b4eb107ac6e2732e32bf55a65a7125edb529
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895494"
---
# <a name="printusagesummarybyprinter-resource-type"></a><span data-ttu-id="dae90-103">tipo de recurso printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="dae90-103">printUsageSummaryByPrinter resource type</span></span>

<span data-ttu-id="dae90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dae90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dae90-105">Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).</span><span class="sxs-lookup"><span data-stu-id="dae90-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="dae90-106">Methods</span><span class="sxs-lookup"><span data-stu-id="dae90-106">Methods</span></span>

| <span data-ttu-id="dae90-107">Método</span><span class="sxs-lookup"><span data-stu-id="dae90-107">Method</span></span>       | <span data-ttu-id="dae90-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dae90-108">Return Type</span></span> | <span data-ttu-id="dae90-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dae90-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dae90-110">Listar (diariamente)</span><span class="sxs-lookup"><span data-stu-id="dae90-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [<span data-ttu-id="dae90-111">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="dae90-111">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="dae90-112">Obtenha uma lista de resumos diários de uso de impressão, agrupadas por impressora.</span><span class="sxs-lookup"><span data-stu-id="dae90-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="dae90-113">Listar (mensal)</span><span class="sxs-lookup"><span data-stu-id="dae90-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [<span data-ttu-id="dae90-114">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="dae90-114">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="dae90-115">Obter uma lista de resumos de uso de impressão mensal, agrupados por impressora.</span><span class="sxs-lookup"><span data-stu-id="dae90-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="dae90-116">Get</span><span class="sxs-lookup"><span data-stu-id="dae90-116">Get</span></span>](../api/printusagesummarybyprinter-get.md) | [<span data-ttu-id="dae90-117">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="dae90-117">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="dae90-118">Leia as propriedades e os relacionamentos de um objeto **printUsageSummaryByPrinter** .</span><span class="sxs-lookup"><span data-stu-id="dae90-118">Read the properties and relationships of a **printUsageSummaryByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dae90-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dae90-119">Properties</span></span>
| <span data-ttu-id="dae90-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dae90-120">Property</span></span>     | <span data-ttu-id="dae90-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="dae90-121">Type</span></span>        | <span data-ttu-id="dae90-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dae90-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dae90-123">id</span><span class="sxs-lookup"><span data-stu-id="dae90-123">id</span></span>|<span data-ttu-id="dae90-124">String</span><span class="sxs-lookup"><span data-stu-id="dae90-124">String</span></span>|<span data-ttu-id="dae90-125">A ID deste Resumo de uso.</span><span class="sxs-lookup"><span data-stu-id="dae90-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="dae90-126">printerid</span><span class="sxs-lookup"><span data-stu-id="dae90-126">printerID</span></span>|<span data-ttu-id="dae90-127">String</span><span class="sxs-lookup"><span data-stu-id="dae90-127">String</span></span>|<span data-ttu-id="dae90-128">A ID da impressora representada por essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="dae90-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="dae90-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="dae90-129">usageDate</span></span>|<span data-ttu-id="dae90-130">Data</span><span class="sxs-lookup"><span data-stu-id="dae90-130">Date</span></span>|<span data-ttu-id="dae90-131">A data associada a essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="dae90-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="dae90-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="dae90-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="dae90-133">Int64</span><span class="sxs-lookup"><span data-stu-id="dae90-133">Int64</span></span>|<span data-ttu-id="dae90-134">O número de trabalhos de impressão em preto e branco concluídos pela impressora na data associada.</span><span class="sxs-lookup"><span data-stu-id="dae90-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="dae90-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="dae90-135">completedColorJobCount</span></span>|<span data-ttu-id="dae90-136">Int64</span><span class="sxs-lookup"><span data-stu-id="dae90-136">Int64</span></span>|<span data-ttu-id="dae90-137">O número de trabalhos de impressão de cores concluídos pela impressora na data associada.</span><span class="sxs-lookup"><span data-stu-id="dae90-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="dae90-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="dae90-138">incompleteJobCount</span></span>|<span data-ttu-id="dae90-139">Int64</span><span class="sxs-lookup"><span data-stu-id="dae90-139">Int64</span></span>|<span data-ttu-id="dae90-140">O número de trabalhos de impressão que foram enfileirados para a impressora, mas que não foram concluídos, na data associada.</span><span class="sxs-lookup"><span data-stu-id="dae90-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dae90-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dae90-141">JSON representation</span></span>

<span data-ttu-id="dae90-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dae90-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
}-->

```json
{
    "id": "String (identifier)",
    "printerId": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageSummaryByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->