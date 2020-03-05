---
title: tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage
description: Limite de largura de banda como uma porcentagem com horário comercial.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd7035bbd57e8deb5e80fdc4cfa770c559e30ef0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526807"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="494e4-103">tipo de recurso deliveryOptimizationBandwidthHoursWithPercentage</span><span class="sxs-lookup"><span data-stu-id="494e4-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

<span data-ttu-id="494e4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="494e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="494e4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="494e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="494e4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="494e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="494e4-107">Limite de largura de banda como uma porcentagem com horário comercial.</span><span class="sxs-lookup"><span data-stu-id="494e4-107">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="494e4-108">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="494e4-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="494e4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="494e4-109">Properties</span></span>
|<span data-ttu-id="494e4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="494e4-110">Property</span></span>|<span data-ttu-id="494e4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="494e4-111">Type</span></span>|<span data-ttu-id="494e4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="494e4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="494e4-113">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="494e4-113">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="494e4-114">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="494e4-114">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="494e4-115">Porcentagem de tempo de download em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="494e4-115">Background download percentage hours.</span></span>|
|<span data-ttu-id="494e4-116">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="494e4-116">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="494e4-117">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="494e4-117">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="494e4-118">Porcentagem de tempo de download do primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="494e4-118">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="494e4-119">Relações</span><span class="sxs-lookup"><span data-stu-id="494e4-119">Relationships</span></span>
<span data-ttu-id="494e4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="494e4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="494e4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="494e4-121">JSON Representation</span></span>
<span data-ttu-id="494e4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="494e4-122">Here is a JSON representation of the resource.</span></span>
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



