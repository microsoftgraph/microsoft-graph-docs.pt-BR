---
title: tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage
description: Limite de largura de banda como uma porcentagem com horário comercial.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85008f7aee3c2f06536ef838df04e56ede36ed46
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420578"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="3a6ac-103">tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage</span><span class="sxs-lookup"><span data-stu-id="3a6ac-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

<span data-ttu-id="3a6ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a6ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a6ac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a6ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a6ac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a6ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a6ac-107">Limite de largura de banda como uma porcentagem com horário comercial.</span><span class="sxs-lookup"><span data-stu-id="3a6ac-107">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="3a6ac-108">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="3a6ac-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a6ac-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a6ac-109">Properties</span></span>
|<span data-ttu-id="3a6ac-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a6ac-110">Property</span></span>|<span data-ttu-id="3a6ac-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a6ac-111">Type</span></span>|<span data-ttu-id="3a6ac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a6ac-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a6ac-113">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="3a6ac-113">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="3a6ac-114">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="3a6ac-114">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="3a6ac-115">Porcentagem de tempo de download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="3a6ac-115">Background download percentage hours.</span></span>|
|<span data-ttu-id="3a6ac-116">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="3a6ac-116">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="3a6ac-117">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="3a6ac-117">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="3a6ac-118">Porcentagem de tempo de download do primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="3a6ac-118">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a6ac-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3a6ac-119">Relationships</span></span>
<span data-ttu-id="3a6ac-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a6ac-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a6ac-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a6ac-121">JSON Representation</span></span>
<span data-ttu-id="3a6ac-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a6ac-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  }
}
```



