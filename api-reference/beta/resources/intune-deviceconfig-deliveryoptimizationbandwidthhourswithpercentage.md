---
title: tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage
description: Limite de largura de banda como uma porcentagem com horário comercial.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69656b0336dc09b2aa0a2f97cfe781347f5adc88
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333405"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="b835c-103">tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage</span><span class="sxs-lookup"><span data-stu-id="b835c-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="b835c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b835c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b835c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b835c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b835c-106">Limite de largura de banda como uma porcentagem com horário comercial.</span><span class="sxs-lookup"><span data-stu-id="b835c-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="b835c-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="b835c-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b835c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b835c-108">Properties</span></span>
|<span data-ttu-id="b835c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b835c-109">Property</span></span>|<span data-ttu-id="b835c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b835c-110">Type</span></span>|<span data-ttu-id="b835c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b835c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b835c-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="b835c-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="b835c-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="b835c-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="b835c-114">Porcentagem de tempo de download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="b835c-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="b835c-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="b835c-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="b835c-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="b835c-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="b835c-117">Porcentagem de tempo de download do primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="b835c-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b835c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b835c-118">Relationships</span></span>
<span data-ttu-id="b835c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b835c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b835c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b835c-120">JSON Representation</span></span>
<span data-ttu-id="b835c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b835c-121">Here is a JSON representation of the resource.</span></span>
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



