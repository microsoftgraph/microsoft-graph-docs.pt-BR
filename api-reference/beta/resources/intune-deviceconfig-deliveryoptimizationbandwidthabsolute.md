---
title: tipo de recurso deliveryOptimizationBandwidthAbsolute
description: Limites de largura de banda em quilobytes por segundo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: addb48091e3682019a508b7f19832b5acccd6aa7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947285"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="8d760-103">tipo de recurso deliveryOptimizationBandwidthAbsolute</span><span class="sxs-lookup"><span data-stu-id="8d760-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

> <span data-ttu-id="8d760-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d760-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d760-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d760-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d760-106">Limites de largura de banda em quilobytes por segundo.</span><span class="sxs-lookup"><span data-stu-id="8d760-106">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="8d760-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="8d760-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d760-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d760-108">Properties</span></span>
|<span data-ttu-id="8d760-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d760-109">Property</span></span>|<span data-ttu-id="8d760-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d760-110">Type</span></span>|<span data-ttu-id="8d760-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d760-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d760-112">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="8d760-112">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="8d760-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8d760-113">Int64</span></span>|<span data-ttu-id="8d760-114">Especifica a largura de banda máxima de download em quilobytes/segundo que o dispositivo pode usar em todas as atividades de download simultâneos usando a otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="8d760-114">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="8d760-115">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="8d760-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="8d760-116">O valor 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads.</span><span class="sxs-lookup"><span data-stu-id="8d760-116">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="8d760-117">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="8d760-117">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="8d760-118">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="8d760-118">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="8d760-119">Int64</span><span class="sxs-lookup"><span data-stu-id="8d760-119">Int64</span></span>|<span data-ttu-id="8d760-120">Especifica a largura de banda de upload máxima em KiloBytes/segundo que um dispositivo usará em toda a atividade de upload simultâneo usando a otimização de entrega (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="8d760-120">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="8d760-121">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="8d760-121">Valid values 0 to 4000000</span></span>
<span data-ttu-id="8d760-122">O valor padrão é 0, que permite uma largura de banda possivelmente ilimitada (otimizada para uso mínimo da largura de banda de upload).</span><span class="sxs-lookup"><span data-stu-id="8d760-122">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="8d760-123">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="8d760-123">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d760-124">Relações</span><span class="sxs-lookup"><span data-stu-id="8d760-124">Relationships</span></span>
<span data-ttu-id="8d760-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d760-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d760-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d760-126">JSON Representation</span></span>
<span data-ttu-id="8d760-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d760-127">Here is a JSON representation of the resource.</span></span>
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




