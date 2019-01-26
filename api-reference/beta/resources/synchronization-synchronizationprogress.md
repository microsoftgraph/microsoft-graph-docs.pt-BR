---
title: tipo de recurso de synchronizationProgress
description: Representa o progresso de um synchronizationJob rumo à conclusão.
localization_priority: Normal
ms.openlocfilehash: 39351f07720d44679675396f9e995f5e78e25fcc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572742"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="38774-103">tipo de recurso de synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="38774-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38774-104">Representa o progresso de um [synchronizationJob](synchronization-synchronizationjob.md) rumo à conclusão.</span><span class="sxs-lookup"><span data-stu-id="38774-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="38774-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38774-105">Properties</span></span>

| <span data-ttu-id="38774-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38774-106">Property</span></span>                              | <span data-ttu-id="38774-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="38774-107">Type</span></span>      | <span data-ttu-id="38774-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="38774-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="38774-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="38774-109">completedUnits</span></span>|<span data-ttu-id="38774-110">Int32</span><span class="sxs-lookup"><span data-stu-id="38774-110">Int32</span></span>|<span data-ttu-id="38774-111">O numerador de uma proporção de progresso; o número de unidades de alterações já processadas.</span><span class="sxs-lookup"><span data-stu-id="38774-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="38774-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="38774-112">progressObservationDateTime</span></span>|<span data-ttu-id="38774-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38774-113">DateTimeOffset</span></span>|<span data-ttu-id="38774-114">A hora de uma observação de progresso como um deslocamento em minutos de UTC.</span><span class="sxs-lookup"><span data-stu-id="38774-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="38774-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="38774-115">totalUnits</span></span>|<span data-ttu-id="38774-116">Int32</span><span class="sxs-lookup"><span data-stu-id="38774-116">Int32</span></span>|<span data-ttu-id="38774-117">Denominador de uma proporção de progresso; um número de unidades de alterações a serem processados para realizar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="38774-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="38774-118">unidades</span><span class="sxs-lookup"><span data-stu-id="38774-118">units</span></span>|<span data-ttu-id="38774-119">String</span><span class="sxs-lookup"><span data-stu-id="38774-119">String</span></span>|<span data-ttu-id="38774-120">Uma descrição opcional das unidades.</span><span class="sxs-lookup"><span data-stu-id="38774-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="38774-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38774-121">JSON representation</span></span>

<span data-ttu-id="38774-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38774-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
