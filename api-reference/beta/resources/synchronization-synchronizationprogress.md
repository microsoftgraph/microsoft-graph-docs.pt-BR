---
title: tipo de recurso synchronizationProgress
description: Representa o andamento de um synchronizationJob para a conclusão.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd1292d34abdc745075e030609d3f28a17b2431a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964638"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="a2f81-103">tipo de recurso synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="a2f81-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2f81-104">Representa o andamento de um [synchronizationJob](synchronization-synchronizationjob.md) para a conclusão.</span><span class="sxs-lookup"><span data-stu-id="a2f81-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="a2f81-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2f81-105">Properties</span></span>

| <span data-ttu-id="a2f81-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2f81-106">Property</span></span>                              | <span data-ttu-id="a2f81-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2f81-107">Type</span></span>      | <span data-ttu-id="a2f81-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2f81-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="a2f81-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="a2f81-109">completedUnits</span></span>|<span data-ttu-id="a2f81-110">Int32</span><span class="sxs-lookup"><span data-stu-id="a2f81-110">Int32</span></span>|<span data-ttu-id="a2f81-111">O numerador de uma taxa de progresso; o número de unidades de alterações já processadas.</span><span class="sxs-lookup"><span data-stu-id="a2f81-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="a2f81-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="a2f81-112">progressObservationDateTime</span></span>|<span data-ttu-id="a2f81-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2f81-113">DateTimeOffset</span></span>|<span data-ttu-id="a2f81-114">O tempo de uma observação de progresso como um deslocamento em minutos do UTC.</span><span class="sxs-lookup"><span data-stu-id="a2f81-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="a2f81-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="a2f81-115">totalUnits</span></span>|<span data-ttu-id="a2f81-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a2f81-116">Int32</span></span>|<span data-ttu-id="a2f81-117">O denominador de uma taxa de progresso; várias unidades de alterações a serem processadas para realizar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="a2f81-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="a2f81-118">unid</span><span class="sxs-lookup"><span data-stu-id="a2f81-118">units</span></span>|<span data-ttu-id="a2f81-119">String</span><span class="sxs-lookup"><span data-stu-id="a2f81-119">String</span></span>|<span data-ttu-id="a2f81-120">Uma descrição opcional das unidades.</span><span class="sxs-lookup"><span data-stu-id="a2f81-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="a2f81-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2f81-121">JSON representation</span></span>

<span data-ttu-id="a2f81-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2f81-122">The following is a JSON representation of the resource.</span></span>

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
