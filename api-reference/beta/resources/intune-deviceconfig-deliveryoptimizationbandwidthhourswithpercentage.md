---
title: tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage
description: Limite de largura de banda como uma porcentagem com horário comercial.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1ad2bbfef3a055a4d5449f7f165bd4bf2f9a07a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979694"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="cfe08-103">tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage</span><span class="sxs-lookup"><span data-stu-id="cfe08-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="cfe08-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfe08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfe08-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfe08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfe08-106">Limite de largura de banda como uma porcentagem com horário comercial.</span><span class="sxs-lookup"><span data-stu-id="cfe08-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="cfe08-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="cfe08-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cfe08-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfe08-108">Properties</span></span>
|<span data-ttu-id="cfe08-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfe08-109">Property</span></span>|<span data-ttu-id="cfe08-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfe08-110">Type</span></span>|<span data-ttu-id="cfe08-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfe08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe08-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="cfe08-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="cfe08-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="cfe08-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="cfe08-114">Porcentagem de tempo de download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="cfe08-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="cfe08-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="cfe08-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="cfe08-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="cfe08-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="cfe08-117">Porcentagem de tempo de download do primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="cfe08-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfe08-118">Relações</span><span class="sxs-lookup"><span data-stu-id="cfe08-118">Relationships</span></span>
<span data-ttu-id="cfe08-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cfe08-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfe08-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfe08-120">JSON Representation</span></span>
<span data-ttu-id="cfe08-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfe08-121">Here is a JSON representation of the resource.</span></span>
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





