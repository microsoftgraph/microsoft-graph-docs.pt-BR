---
title: tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage
description: Limite de largura de banda como uma porcentagem com horário comercial.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecb024d15ee5d4e748d57e1b895c9418feadd52a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562724"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="55ca9-103">tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage</span><span class="sxs-lookup"><span data-stu-id="55ca9-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="55ca9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55ca9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55ca9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55ca9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55ca9-106">Limite de largura de banda como uma porcentagem com horário comercial.</span><span class="sxs-lookup"><span data-stu-id="55ca9-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="55ca9-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="55ca9-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="55ca9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55ca9-108">Properties</span></span>
|<span data-ttu-id="55ca9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55ca9-109">Property</span></span>|<span data-ttu-id="55ca9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="55ca9-110">Type</span></span>|<span data-ttu-id="55ca9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="55ca9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55ca9-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="55ca9-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="55ca9-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="55ca9-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="55ca9-114">Porcentagem de tempo de download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="55ca9-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="55ca9-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="55ca9-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="55ca9-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="55ca9-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="55ca9-117">Porcentagem de tempo de download do primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="55ca9-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55ca9-118">Relações</span><span class="sxs-lookup"><span data-stu-id="55ca9-118">Relationships</span></span>
<span data-ttu-id="55ca9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55ca9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55ca9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55ca9-120">JSON Representation</span></span>
<span data-ttu-id="55ca9-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55ca9-121">Here is a JSON representation of the resource.</span></span>
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





