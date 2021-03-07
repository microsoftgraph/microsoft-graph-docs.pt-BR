---
title: Tipo de recurso printUsageByPrinter
description: Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 8c5a69d01f0b8da05a5f72f5c2c7d9bacf10ff1a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517012"
---
# <a name="printusagebyprinter-resource-type"></a><span data-ttu-id="85479-103">Tipo de recurso printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="85479-103">printUsageByPrinter resource type</span></span>

<span data-ttu-id="85479-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85479-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="85479-105">Descreve a atividade de impressão de uma impressora durante um período de tempo especificado (usageDate).</span><span class="sxs-lookup"><span data-stu-id="85479-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="85479-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="85479-106">Methods</span></span>
|<span data-ttu-id="85479-107">Método</span><span class="sxs-lookup"><span data-stu-id="85479-107">Method</span></span>|<span data-ttu-id="85479-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="85479-108">Return type</span></span>|<span data-ttu-id="85479-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="85479-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="85479-110">Lista (diariamente)</span><span class="sxs-lookup"><span data-stu-id="85479-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyprinter.md) | [<span data-ttu-id="85479-111">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="85479-111">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="85479-112">Obter uma lista de resumos de uso diário de impressão, agrupados por impressora.</span><span class="sxs-lookup"><span data-stu-id="85479-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="85479-113">Lista (mensal)</span><span class="sxs-lookup"><span data-stu-id="85479-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyprinter.md) | [<span data-ttu-id="85479-114">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="85479-114">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="85479-115">Obter uma lista de resumos de uso de impressão mensal, agrupados por impressora.</span><span class="sxs-lookup"><span data-stu-id="85479-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="85479-116">Get</span><span class="sxs-lookup"><span data-stu-id="85479-116">Get</span></span>](../api/printUsageByPrinter-get.md) | [<span data-ttu-id="85479-117">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="85479-117">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="85479-118">Leia as propriedades e as relações de um **objeto printUsageByPrinter.**</span><span class="sxs-lookup"><span data-stu-id="85479-118">Read the properties and relationships of a **printUsageByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="85479-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85479-119">Properties</span></span>
|<span data-ttu-id="85479-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85479-120">Property</span></span>|<span data-ttu-id="85479-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="85479-121">Type</span></span>|<span data-ttu-id="85479-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="85479-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85479-123">id</span><span class="sxs-lookup"><span data-stu-id="85479-123">id</span></span>|<span data-ttu-id="85479-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85479-124">String</span></span>|<span data-ttu-id="85479-125">A ID deste resumo de uso.</span><span class="sxs-lookup"><span data-stu-id="85479-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="85479-126">printerID</span><span class="sxs-lookup"><span data-stu-id="85479-126">printerID</span></span>|<span data-ttu-id="85479-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85479-127">String</span></span>|<span data-ttu-id="85479-128">A ID da impressora representada por essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="85479-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="85479-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="85479-129">usageDate</span></span>|<span data-ttu-id="85479-130">Data</span><span class="sxs-lookup"><span data-stu-id="85479-130">Date</span></span>|<span data-ttu-id="85479-131">A data associada a essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="85479-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="85479-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="85479-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="85479-133">Int64</span><span class="sxs-lookup"><span data-stu-id="85479-133">Int64</span></span>|<span data-ttu-id="85479-134">O número de trabalhos de impressão em preto e branco concluídos pela impressora na data associada.</span><span class="sxs-lookup"><span data-stu-id="85479-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="85479-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="85479-135">completedColorJobCount</span></span>|<span data-ttu-id="85479-136">Int64</span><span class="sxs-lookup"><span data-stu-id="85479-136">Int64</span></span>|<span data-ttu-id="85479-137">O número de trabalhos de impressão de cores concluídos pela impressora na data associada.</span><span class="sxs-lookup"><span data-stu-id="85479-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="85479-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="85479-138">incompleteJobCount</span></span>|<span data-ttu-id="85479-139">Int64</span><span class="sxs-lookup"><span data-stu-id="85479-139">Int64</span></span>|<span data-ttu-id="85479-140">O número de trabalhos de impressão que foram enraizadas para a impressora, mas não concluídos, na data associada.</span><span class="sxs-lookup"><span data-stu-id="85479-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85479-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85479-141">JSON representation</span></span>
<span data-ttu-id="85479-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85479-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByPrinter",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByPrinter",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "printerId": "String"
}
```

