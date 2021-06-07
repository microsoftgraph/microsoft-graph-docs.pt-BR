---
title: Tipo de recurso printUsageByPrinter
description: Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2826e73ef68d9ee2162c6a2de0bbaba351fd87bd
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781230"
---
# <a name="printusagebyprinter-resource-type"></a><span data-ttu-id="2d771-103">Tipo de recurso printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="2d771-103">printUsageByPrinter resource type</span></span>

<span data-ttu-id="2d771-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d771-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d771-105">Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).</span><span class="sxs-lookup"><span data-stu-id="2d771-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="2d771-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2d771-106">Methods</span></span>

| <span data-ttu-id="2d771-107">Método</span><span class="sxs-lookup"><span data-stu-id="2d771-107">Method</span></span>       | <span data-ttu-id="2d771-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2d771-108">Return Type</span></span> | <span data-ttu-id="2d771-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d771-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2d771-110">Lista (diariamente)</span><span class="sxs-lookup"><span data-stu-id="2d771-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyprinter.md) | [<span data-ttu-id="2d771-111">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="2d771-111">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="2d771-112">Obter uma lista de resumos de uso diário de impressão, agrupados por impressora.</span><span class="sxs-lookup"><span data-stu-id="2d771-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="2d771-113">Lista (mensal)</span><span class="sxs-lookup"><span data-stu-id="2d771-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyprinter.md) | [<span data-ttu-id="2d771-114">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="2d771-114">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="2d771-115">Obter uma lista de resumos de uso de impressão mensal, agrupados por impressora.</span><span class="sxs-lookup"><span data-stu-id="2d771-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="2d771-116">Get</span><span class="sxs-lookup"><span data-stu-id="2d771-116">Get</span></span>](../api/printUsageByPrinter-get.md) | [<span data-ttu-id="2d771-117">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="2d771-117">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="2d771-118">Leia as propriedades e as relações de um **objeto printUsageByPrinter.**</span><span class="sxs-lookup"><span data-stu-id="2d771-118">Read the properties and relationships of a **printUsageByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2d771-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d771-119">Properties</span></span>
| <span data-ttu-id="2d771-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d771-120">Property</span></span>     | <span data-ttu-id="2d771-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d771-121">Type</span></span>        | <span data-ttu-id="2d771-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d771-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d771-123">id</span><span class="sxs-lookup"><span data-stu-id="2d771-123">id</span></span>|<span data-ttu-id="2d771-124">String</span><span class="sxs-lookup"><span data-stu-id="2d771-124">String</span></span>|<span data-ttu-id="2d771-125">A ID deste resumo de uso.</span><span class="sxs-lookup"><span data-stu-id="2d771-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="2d771-126">printerID</span><span class="sxs-lookup"><span data-stu-id="2d771-126">printerID</span></span>|<span data-ttu-id="2d771-127">String</span><span class="sxs-lookup"><span data-stu-id="2d771-127">String</span></span>|<span data-ttu-id="2d771-128">A ID da impressora representada por essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="2d771-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="2d771-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="2d771-129">usageDate</span></span>|<span data-ttu-id="2d771-130">Data</span><span class="sxs-lookup"><span data-stu-id="2d771-130">Date</span></span>|<span data-ttu-id="2d771-131">A data associada a essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="2d771-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="2d771-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="2d771-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="2d771-133">Int64</span><span class="sxs-lookup"><span data-stu-id="2d771-133">Int64</span></span>|<span data-ttu-id="2d771-134">O número de trabalhos de impressão em preto e branco concluídos pela impressora na data associada.</span><span class="sxs-lookup"><span data-stu-id="2d771-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="2d771-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="2d771-135">completedColorJobCount</span></span>|<span data-ttu-id="2d771-136">Int64</span><span class="sxs-lookup"><span data-stu-id="2d771-136">Int64</span></span>|<span data-ttu-id="2d771-137">O número de trabalhos de impressão de cores concluídos pela impressora na data associada.</span><span class="sxs-lookup"><span data-stu-id="2d771-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="2d771-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="2d771-138">incompleteJobCount</span></span>|<span data-ttu-id="2d771-139">Int64</span><span class="sxs-lookup"><span data-stu-id="2d771-139">Int64</span></span>|<span data-ttu-id="2d771-140">O número de trabalhos de impressão que foram enraizadas para a impressora, mas não concluídos, na data associada.</span><span class="sxs-lookup"><span data-stu-id="2d771-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d771-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d771-141">JSON representation</span></span>

<span data-ttu-id="2d771-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d771-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageByPrinter"
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
  "description": "printUsageByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

