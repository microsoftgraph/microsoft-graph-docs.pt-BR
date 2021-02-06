---
title: Tipo de recurso synchronizationProgress
description: Representa o progresso de um synchronizationJob em direção à conclusão.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: f6f8f7cc5d0419a6f0e9203513db5b1452db1797
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131639"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="33363-103">Tipo de recurso synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="33363-103">synchronizationProgress resource type</span></span>

<span data-ttu-id="33363-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33363-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33363-105">Representa o progresso de [um synchronizationJob em](synchronization-synchronizationjob.md) direção à conclusão.</span><span class="sxs-lookup"><span data-stu-id="33363-105">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="33363-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33363-106">Properties</span></span>

| <span data-ttu-id="33363-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33363-107">Property</span></span>                              | <span data-ttu-id="33363-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="33363-108">Type</span></span>      | <span data-ttu-id="33363-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="33363-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="33363-110">completedUnits</span><span class="sxs-lookup"><span data-stu-id="33363-110">completedUnits</span></span>|<span data-ttu-id="33363-111">Int32</span><span class="sxs-lookup"><span data-stu-id="33363-111">Int32</span></span>|<span data-ttu-id="33363-112">O numerador de uma taxa de progresso; o número de unidades de alterações já processadas.</span><span class="sxs-lookup"><span data-stu-id="33363-112">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="33363-113">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="33363-113">progressObservationDateTime</span></span>|<span data-ttu-id="33363-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33363-114">DateTimeOffset</span></span>|<span data-ttu-id="33363-115">O tempo de uma observação de progresso como um deslocamento em minutos de UTC.</span><span class="sxs-lookup"><span data-stu-id="33363-115">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="33363-116">totalUnits</span><span class="sxs-lookup"><span data-stu-id="33363-116">totalUnits</span></span>|<span data-ttu-id="33363-117">Int32</span><span class="sxs-lookup"><span data-stu-id="33363-117">Int32</span></span>|<span data-ttu-id="33363-118">O denominador de uma taxa de progresso; várias unidades de alterações a serem processadas para realizar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="33363-118">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="33363-119">unidades</span><span class="sxs-lookup"><span data-stu-id="33363-119">units</span></span>|<span data-ttu-id="33363-120">String</span><span class="sxs-lookup"><span data-stu-id="33363-120">String</span></span>|<span data-ttu-id="33363-121">Uma descrição opcional das unidades.</span><span class="sxs-lookup"><span data-stu-id="33363-121">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="33363-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33363-122">JSON representation</span></span>

<span data-ttu-id="33363-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33363-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


