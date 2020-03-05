---
title: tipo de recurso synchronizationProgress
description: Representa o andamento de um synchronizationJob para a conclusão.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4fb5fb9482a9b8523f1967928a4243a5b104f6a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520055"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="9a70a-103">tipo de recurso synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="9a70a-103">synchronizationProgress resource type</span></span>

<span data-ttu-id="9a70a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9a70a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a70a-105">Representa o andamento de um [synchronizationJob](synchronization-synchronizationjob.md) para a conclusão.</span><span class="sxs-lookup"><span data-stu-id="9a70a-105">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="9a70a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a70a-106">Properties</span></span>

| <span data-ttu-id="9a70a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a70a-107">Property</span></span>                              | <span data-ttu-id="9a70a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a70a-108">Type</span></span>      | <span data-ttu-id="9a70a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a70a-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="9a70a-110">completedUnits</span><span class="sxs-lookup"><span data-stu-id="9a70a-110">completedUnits</span></span>|<span data-ttu-id="9a70a-111">Int32</span><span class="sxs-lookup"><span data-stu-id="9a70a-111">Int32</span></span>|<span data-ttu-id="9a70a-112">O numerador de uma taxa de progresso; o número de unidades de alterações já processadas.</span><span class="sxs-lookup"><span data-stu-id="9a70a-112">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="9a70a-113">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="9a70a-113">progressObservationDateTime</span></span>|<span data-ttu-id="9a70a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a70a-114">DateTimeOffset</span></span>|<span data-ttu-id="9a70a-115">O tempo de uma observação de progresso como um deslocamento em minutos do UTC.</span><span class="sxs-lookup"><span data-stu-id="9a70a-115">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="9a70a-116">totalUnits</span><span class="sxs-lookup"><span data-stu-id="9a70a-116">totalUnits</span></span>|<span data-ttu-id="9a70a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="9a70a-117">Int32</span></span>|<span data-ttu-id="9a70a-118">O denominador de uma taxa de progresso; várias unidades de alterações a serem processadas para realizar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="9a70a-118">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="9a70a-119">unid</span><span class="sxs-lookup"><span data-stu-id="9a70a-119">units</span></span>|<span data-ttu-id="9a70a-120">String</span><span class="sxs-lookup"><span data-stu-id="9a70a-120">String</span></span>|<span data-ttu-id="9a70a-121">Uma descrição opcional das unidades.</span><span class="sxs-lookup"><span data-stu-id="9a70a-121">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="9a70a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a70a-122">JSON representation</span></span>

<span data-ttu-id="9a70a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a70a-123">The following is a JSON representation of the resource.</span></span>

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
