---
title: tipo de recurso de synchronizationProgress
description: Representa o progresso de um synchronizationJob rumo à conclusão.
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640067"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="b1600-103">tipo de recurso de synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="b1600-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1600-104">Representa o progresso de um [synchronizationJob](synchronization-synchronizationjob.md) rumo à conclusão.</span><span class="sxs-lookup"><span data-stu-id="b1600-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="b1600-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1600-105">Properties</span></span>

| <span data-ttu-id="b1600-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1600-106">Property</span></span>                              | <span data-ttu-id="b1600-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1600-107">Type</span></span>      | <span data-ttu-id="b1600-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1600-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="b1600-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="b1600-109">completedUnits</span></span>|<span data-ttu-id="b1600-110">Int32</span><span class="sxs-lookup"><span data-stu-id="b1600-110">Int32</span></span>|<span data-ttu-id="b1600-111">O numerador de uma proporção de progresso; o número de unidades de alterações já processadas.</span><span class="sxs-lookup"><span data-stu-id="b1600-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="b1600-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="b1600-112">progressObservationDateTime</span></span>|<span data-ttu-id="b1600-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1600-113">DateTimeOffset</span></span>|<span data-ttu-id="b1600-114">A hora de uma observação de progresso como um deslocamento em minutos de UTC.</span><span class="sxs-lookup"><span data-stu-id="b1600-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="b1600-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="b1600-115">totalUnits</span></span>|<span data-ttu-id="b1600-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b1600-116">Int32</span></span>|<span data-ttu-id="b1600-117">Denominador de uma proporção de progresso; um número de unidades de alterações a serem processados para realizar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="b1600-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="b1600-118">unidades</span><span class="sxs-lookup"><span data-stu-id="b1600-118">units</span></span>|<span data-ttu-id="b1600-119">String</span><span class="sxs-lookup"><span data-stu-id="b1600-119">String</span></span>|<span data-ttu-id="b1600-120">Uma descrição opcional das unidades.</span><span class="sxs-lookup"><span data-stu-id="b1600-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="b1600-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1600-121">JSON representation</span></span>

<span data-ttu-id="b1600-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1600-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
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
