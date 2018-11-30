---
title: tipo de recurso de synchronizationProgress
description: Representa o progresso de um synchronizationJob rumo à conclusão.
ms.openlocfilehash: 412b7754dac97a36efe082026ab360569c0fe789
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040761"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="f0f59-103">tipo de recurso de synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="f0f59-103">synchronizationProgress resource type</span></span>

> <span data-ttu-id="f0f59-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f0f59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0f59-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f0f59-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0f59-106">Representa o progresso de um [synchronizationJob](synchronization-synchronizationjob.md) rumo à conclusão.</span><span class="sxs-lookup"><span data-stu-id="f0f59-106">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="f0f59-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0f59-107">Properties</span></span>

| <span data-ttu-id="f0f59-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0f59-108">Property</span></span>                              | <span data-ttu-id="f0f59-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0f59-109">Type</span></span>      | <span data-ttu-id="f0f59-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0f59-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="f0f59-111">completedUnits</span><span class="sxs-lookup"><span data-stu-id="f0f59-111">completedUnits</span></span>|<span data-ttu-id="f0f59-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f59-112">Int32</span></span>|<span data-ttu-id="f0f59-113">O numerador de uma proporção de progresso; o número de unidades de alterações já processadas.</span><span class="sxs-lookup"><span data-stu-id="f0f59-113">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="f0f59-114">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="f0f59-114">progressObservationDateTime</span></span>|<span data-ttu-id="f0f59-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0f59-115">DateTimeOffset</span></span>|<span data-ttu-id="f0f59-116">A hora de uma observação de progresso como um deslocamento em minutos de UTC.</span><span class="sxs-lookup"><span data-stu-id="f0f59-116">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="f0f59-117">totalUnits</span><span class="sxs-lookup"><span data-stu-id="f0f59-117">totalUnits</span></span>|<span data-ttu-id="f0f59-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f59-118">Int32</span></span>|<span data-ttu-id="f0f59-119">Denominador de uma proporção de progresso; um número de unidades de alterações a serem processados para realizar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="f0f59-119">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="f0f59-120">unidades</span><span class="sxs-lookup"><span data-stu-id="f0f59-120">units</span></span>|<span data-ttu-id="f0f59-121">String</span><span class="sxs-lookup"><span data-stu-id="f0f59-121">String</span></span>|<span data-ttu-id="f0f59-122">Uma descrição opcional das unidades.</span><span class="sxs-lookup"><span data-stu-id="f0f59-122">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="f0f59-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0f59-123">JSON representation</span></span>

<span data-ttu-id="f0f59-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0f59-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
