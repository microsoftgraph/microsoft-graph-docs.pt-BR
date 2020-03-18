---
title: tipo de recurso deliveryOptimizationBandwidthAbsolute
description: Limites de largura de banda em quilobytes por segundo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8313f742c407eb6ca7b4dffeaf6dba86a631843
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794393"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="27446-103">tipo de recurso deliveryOptimizationBandwidthAbsolute</span><span class="sxs-lookup"><span data-stu-id="27446-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

> <span data-ttu-id="27446-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27446-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27446-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27446-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27446-106">Limites de largura de banda em quilobytes por segundo.</span><span class="sxs-lookup"><span data-stu-id="27446-106">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="27446-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="27446-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27446-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27446-108">Properties</span></span>
|<span data-ttu-id="27446-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27446-109">Property</span></span>|<span data-ttu-id="27446-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="27446-110">Type</span></span>|<span data-ttu-id="27446-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="27446-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27446-112">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="27446-112">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="27446-113">Int64</span><span class="sxs-lookup"><span data-stu-id="27446-113">Int64</span></span>|<span data-ttu-id="27446-114">Especifica a largura de banda máxima de download em quilobytes/segundo que o dispositivo pode usar em todas as atividades de download simultâneos usando a otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="27446-114">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="27446-115">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="27446-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="27446-116">O valor 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads.</span><span class="sxs-lookup"><span data-stu-id="27446-116">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="27446-117">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="27446-117">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="27446-118">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="27446-118">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="27446-119">Int64</span><span class="sxs-lookup"><span data-stu-id="27446-119">Int64</span></span>|<span data-ttu-id="27446-120">Especifica a largura de banda de upload máxima em KiloBytes/segundo que um dispositivo usará em toda a atividade de upload simultâneo usando a otimização de entrega (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="27446-120">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="27446-121">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="27446-121">Valid values 0 to 4000000</span></span>
<span data-ttu-id="27446-122">O valor padrão é 0, que permite uma largura de banda possivelmente ilimitada (otimizada para uso mínimo da largura de banda de upload).</span><span class="sxs-lookup"><span data-stu-id="27446-122">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="27446-123">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="27446-123">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="27446-124">Relações</span><span class="sxs-lookup"><span data-stu-id="27446-124">Relationships</span></span>
<span data-ttu-id="27446-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27446-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27446-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27446-126">JSON Representation</span></span>
<span data-ttu-id="27446-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27446-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```



