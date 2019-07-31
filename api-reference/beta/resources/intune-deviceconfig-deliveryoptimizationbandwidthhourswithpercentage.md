---
title: tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage
description: Limite de largura de banda como uma porcentagem com horário comercial.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 022bada2d0dcfff6cf09ad5ae7719e3cd54107c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970791"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="57e13-103">tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage</span><span class="sxs-lookup"><span data-stu-id="57e13-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="57e13-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57e13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57e13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57e13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57e13-106">Limite de largura de banda como uma porcentagem com horário comercial.</span><span class="sxs-lookup"><span data-stu-id="57e13-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="57e13-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="57e13-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57e13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57e13-108">Properties</span></span>
|<span data-ttu-id="57e13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57e13-109">Property</span></span>|<span data-ttu-id="57e13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="57e13-110">Type</span></span>|<span data-ttu-id="57e13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="57e13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57e13-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="57e13-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="57e13-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="57e13-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="57e13-114">Porcentagem de tempo de download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="57e13-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="57e13-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="57e13-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="57e13-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="57e13-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="57e13-117">Porcentagem de tempo de download do primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="57e13-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57e13-118">Relações</span><span class="sxs-lookup"><span data-stu-id="57e13-118">Relationships</span></span>
<span data-ttu-id="57e13-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57e13-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57e13-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57e13-120">JSON Representation</span></span>
<span data-ttu-id="57e13-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57e13-121">Here is a JSON representation of the resource.</span></span>
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





