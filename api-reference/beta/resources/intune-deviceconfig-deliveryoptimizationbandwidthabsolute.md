---
title: tipo de recurso deliveryOptimizationBandwidthAbsolute
description: Limites de largura de banda em quilobytes por segundo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 759d124570a2ebf00ad9df6e030cce69f866ed44
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216224"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="102d5-103">tipo de recurso deliveryOptimizationBandwidthAbsolute</span><span class="sxs-lookup"><span data-stu-id="102d5-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

<span data-ttu-id="102d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="102d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="102d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="102d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="102d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="102d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="102d5-107">Limites de largura de banda em quilobytes por segundo.</span><span class="sxs-lookup"><span data-stu-id="102d5-107">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="102d5-108">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="102d5-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="102d5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="102d5-109">Properties</span></span>
|<span data-ttu-id="102d5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="102d5-110">Property</span></span>|<span data-ttu-id="102d5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="102d5-111">Type</span></span>|<span data-ttu-id="102d5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="102d5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="102d5-113">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="102d5-113">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="102d5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="102d5-114">Int64</span></span>|<span data-ttu-id="102d5-115">Especifica a largura de banda máxima de download em quilobytes/segundo que o dispositivo pode usar em todas as atividades de download simultâneos usando a otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="102d5-115">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="102d5-116">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="102d5-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="102d5-117">O valor 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads.</span><span class="sxs-lookup"><span data-stu-id="102d5-117">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="102d5-118">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="102d5-118">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="102d5-119">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="102d5-119">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="102d5-120">Int64</span><span class="sxs-lookup"><span data-stu-id="102d5-120">Int64</span></span>|<span data-ttu-id="102d5-121">Especifica a largura de banda de upload máxima em KiloBytes/segundo que um dispositivo usará em toda a atividade de upload simultâneo usando a otimização de entrega (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="102d5-121">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="102d5-122">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="102d5-122">Valid values 0 to 4000000</span></span>
<span data-ttu-id="102d5-123">O valor padrão é 0, que permite uma largura de banda possivelmente ilimitada (otimizada para uso mínimo da largura de banda de upload).</span><span class="sxs-lookup"><span data-stu-id="102d5-123">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="102d5-124">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="102d5-124">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="102d5-125">Relações</span><span class="sxs-lookup"><span data-stu-id="102d5-125">Relationships</span></span>
<span data-ttu-id="102d5-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="102d5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="102d5-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="102d5-127">JSON Representation</span></span>
<span data-ttu-id="102d5-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="102d5-128">Here is a JSON representation of the resource.</span></span>
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




