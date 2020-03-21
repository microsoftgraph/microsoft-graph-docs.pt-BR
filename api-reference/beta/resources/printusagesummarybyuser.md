---
title: tipo de recurso printUsageSummaryByUser
description: Descreve a atividade de impressão para um usuário durante um período de tempo especificado (usageDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 30769d9bd7ee76494b1582a3d7afc8a7f75bb07a
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895471"
---
# <a name="printusagesummarybyuser-resource-type"></a><span data-ttu-id="c5053-103">tipo de recurso printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="c5053-103">printUsageSummaryByUser resource type</span></span>

<span data-ttu-id="c5053-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5053-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5053-105">Descreve a atividade de impressão para um usuário durante um período de tempo especificado (usageDate).</span><span class="sxs-lookup"><span data-stu-id="c5053-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="c5053-106">Methods</span><span class="sxs-lookup"><span data-stu-id="c5053-106">Methods</span></span>

| <span data-ttu-id="c5053-107">Método</span><span class="sxs-lookup"><span data-stu-id="c5053-107">Method</span></span>       | <span data-ttu-id="c5053-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5053-108">Return Type</span></span> | <span data-ttu-id="c5053-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5053-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c5053-110">Listar (diariamente)</span><span class="sxs-lookup"><span data-stu-id="c5053-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [<span data-ttu-id="c5053-111">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="c5053-111">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="c5053-112">Obtenha uma lista de resumos diários de uso de impressão, agrupados por usuário.</span><span class="sxs-lookup"><span data-stu-id="c5053-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="c5053-113">Listar (mensal)</span><span class="sxs-lookup"><span data-stu-id="c5053-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [<span data-ttu-id="c5053-114">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="c5053-114">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="c5053-115">Obter uma lista de resumos de uso de impressão mensal, agrupados por usuário.</span><span class="sxs-lookup"><span data-stu-id="c5053-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="c5053-116">Get</span><span class="sxs-lookup"><span data-stu-id="c5053-116">Get</span></span>](../api/printusagesummarybyuser-get.md) | [<span data-ttu-id="c5053-117">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="c5053-117">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="c5053-118">Ler propriedades e relações de um objeto printUsageSummaryByUser.</span><span class="sxs-lookup"><span data-stu-id="c5053-118">Read properties and relationships of a printUsageSummaryByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c5053-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5053-119">Properties</span></span>
| <span data-ttu-id="c5053-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5053-120">Property</span></span>     | <span data-ttu-id="c5053-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5053-121">Type</span></span>        | <span data-ttu-id="c5053-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5053-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c5053-123">id</span><span class="sxs-lookup"><span data-stu-id="c5053-123">id</span></span>|<span data-ttu-id="c5053-124">String</span><span class="sxs-lookup"><span data-stu-id="c5053-124">String</span></span>|<span data-ttu-id="c5053-125">A ID deste Resumo de uso.</span><span class="sxs-lookup"><span data-stu-id="c5053-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="c5053-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c5053-126">userPrincipalName</span></span>|<span data-ttu-id="c5053-127">String</span><span class="sxs-lookup"><span data-stu-id="c5053-127">String</span></span>|<span data-ttu-id="c5053-128">O UPN do usuário representado por essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="c5053-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="c5053-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="c5053-129">usageDate</span></span>|<span data-ttu-id="c5053-130">Data</span><span class="sxs-lookup"><span data-stu-id="c5053-130">Date</span></span>|<span data-ttu-id="c5053-131">A data associada a essas estatísticas.</span><span class="sxs-lookup"><span data-stu-id="c5053-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="c5053-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="c5053-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="c5053-133">Int64</span><span class="sxs-lookup"><span data-stu-id="c5053-133">Int64</span></span>|<span data-ttu-id="c5053-134">O número de trabalhos de impressão em preto e branco concluídos em nome do usuário na data associada.</span><span class="sxs-lookup"><span data-stu-id="c5053-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="c5053-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="c5053-135">completedColorJobCount</span></span>|<span data-ttu-id="c5053-136">Int64</span><span class="sxs-lookup"><span data-stu-id="c5053-136">Int64</span></span>|<span data-ttu-id="c5053-137">O número de trabalhos de impressão em cores concluídos em nome do usuário na data associada.</span><span class="sxs-lookup"><span data-stu-id="c5053-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="c5053-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="c5053-138">incompleteJobCount</span></span>|<span data-ttu-id="c5053-139">Int64</span><span class="sxs-lookup"><span data-stu-id="c5053-139">Int64</span></span>|<span data-ttu-id="c5053-140">O número de trabalhos de impressão que foram enfileirados em nome do usuário, mas não concluídos, na data associada.</span><span class="sxs-lookup"><span data-stu-id="c5053-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5053-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5053-141">JSON representation</span></span>

<span data-ttu-id="c5053-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5053-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
}-->

```json
{
    "id": "String (identifier)",
    "userPrincipalName": "String (identifier)",
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
  "description": "printUsageSummaryByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->