---
title: tipo de recurso synchronizationProgress
description: Representa o andamento de um synchronizationJob para a conclusão.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5040cb32b664497f2cbed9dc9ca77ce2a2a54ee7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023825"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="b0ae6-103">tipo de recurso synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="b0ae6-103">synchronizationProgress resource type</span></span>

<span data-ttu-id="b0ae6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0ae6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ae6-105">Representa o andamento de um [synchronizationJob](synchronization-synchronizationjob.md) para a conclusão.</span><span class="sxs-lookup"><span data-stu-id="b0ae6-105">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="b0ae6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0ae6-106">Properties</span></span>

| <span data-ttu-id="b0ae6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0ae6-107">Property</span></span>                              | <span data-ttu-id="b0ae6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0ae6-108">Type</span></span>      | <span data-ttu-id="b0ae6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ae6-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="b0ae6-110">completedUnits</span><span class="sxs-lookup"><span data-stu-id="b0ae6-110">completedUnits</span></span>|<span data-ttu-id="b0ae6-111">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ae6-111">Int32</span></span>|<span data-ttu-id="b0ae6-112">O numerador de uma taxa de progresso; o número de unidades de alterações já processadas.</span><span class="sxs-lookup"><span data-stu-id="b0ae6-112">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="b0ae6-113">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="b0ae6-113">progressObservationDateTime</span></span>|<span data-ttu-id="b0ae6-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0ae6-114">DateTimeOffset</span></span>|<span data-ttu-id="b0ae6-115">O tempo de uma observação de progresso como um deslocamento em minutos do UTC.</span><span class="sxs-lookup"><span data-stu-id="b0ae6-115">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="b0ae6-116">totalUnits</span><span class="sxs-lookup"><span data-stu-id="b0ae6-116">totalUnits</span></span>|<span data-ttu-id="b0ae6-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b0ae6-117">Int32</span></span>|<span data-ttu-id="b0ae6-118">O denominador de uma taxa de progresso; várias unidades de alterações a serem processadas para realizar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="b0ae6-118">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="b0ae6-119">unid</span><span class="sxs-lookup"><span data-stu-id="b0ae6-119">units</span></span>|<span data-ttu-id="b0ae6-120">String</span><span class="sxs-lookup"><span data-stu-id="b0ae6-120">String</span></span>|<span data-ttu-id="b0ae6-121">Uma descrição opcional das unidades.</span><span class="sxs-lookup"><span data-stu-id="b0ae6-121">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="b0ae6-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0ae6-122">JSON representation</span></span>

<span data-ttu-id="b0ae6-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0ae6-123">The following is a JSON representation of the resource.</span></span>

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


