---
title: tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage
description: Limite de largura de banda como uma porcentagem com horário comercial.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7fb685f87e602eb6312d3e80e441b2c064ec327b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696227"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="2c8a6-103">tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage</span><span class="sxs-lookup"><span data-stu-id="2c8a6-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

<span data-ttu-id="2c8a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c8a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c8a6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c8a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c8a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c8a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c8a6-107">Limite de largura de banda como uma porcentagem com horário comercial.</span><span class="sxs-lookup"><span data-stu-id="2c8a6-107">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="2c8a6-108">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="2c8a6-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c8a6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c8a6-109">Properties</span></span>
|<span data-ttu-id="2c8a6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c8a6-110">Property</span></span>|<span data-ttu-id="2c8a6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c8a6-111">Type</span></span>|<span data-ttu-id="2c8a6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8a6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c8a6-113">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="2c8a6-113">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="2c8a6-114">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="2c8a6-114">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="2c8a6-115">Porcentagem de tempo de download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="2c8a6-115">Background download percentage hours.</span></span>|
|<span data-ttu-id="2c8a6-116">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="2c8a6-116">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="2c8a6-117">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="2c8a6-117">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="2c8a6-118">Porcentagem de tempo de download do primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="2c8a6-118">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c8a6-119">Relações</span><span class="sxs-lookup"><span data-stu-id="2c8a6-119">Relationships</span></span>
<span data-ttu-id="2c8a6-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c8a6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c8a6-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c8a6-121">JSON Representation</span></span>
<span data-ttu-id="2c8a6-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c8a6-122">Here is a JSON representation of the resource.</span></span>
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





