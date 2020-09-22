---
title: tipo de recurso deliveryOptimizationBandwidthAbsolute
description: Limites de largura de banda em quilobytes por segundo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8df502e294979ea81d26858f64cd386b83057f99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973796"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="3d095-103">tipo de recurso deliveryOptimizationBandwidthAbsolute</span><span class="sxs-lookup"><span data-stu-id="3d095-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

<span data-ttu-id="3d095-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d095-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d095-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d095-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d095-107">Limites de largura de banda em quilobytes por segundo.</span><span class="sxs-lookup"><span data-stu-id="3d095-107">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="3d095-108">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="3d095-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3d095-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d095-109">Properties</span></span>
|<span data-ttu-id="3d095-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d095-110">Property</span></span>|<span data-ttu-id="3d095-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d095-111">Type</span></span>|<span data-ttu-id="3d095-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d095-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d095-113">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="3d095-113">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="3d095-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3d095-114">Int64</span></span>|<span data-ttu-id="3d095-115">Especifica a largura de banda máxima de download em quilobytes/segundo que o dispositivo pode usar em todas as atividades de download simultâneos usando a otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="3d095-115">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="3d095-116">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="3d095-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="3d095-117">O valor 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads.</span><span class="sxs-lookup"><span data-stu-id="3d095-117">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="3d095-118">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="3d095-118">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="3d095-119">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="3d095-119">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="3d095-120">Int64</span><span class="sxs-lookup"><span data-stu-id="3d095-120">Int64</span></span>|<span data-ttu-id="3d095-121">Especifica a largura de banda de upload máxima em KiloBytes/segundo que um dispositivo usará em toda a atividade de upload simultâneo usando a otimização de entrega (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="3d095-121">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="3d095-122">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="3d095-122">Valid values 0 to 4000000</span></span>
<span data-ttu-id="3d095-123">O valor padrão é 0, que permite uma largura de banda possivelmente ilimitada (otimizada para uso mínimo da largura de banda de upload).</span><span class="sxs-lookup"><span data-stu-id="3d095-123">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="3d095-124">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="3d095-124">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d095-125">Relações</span><span class="sxs-lookup"><span data-stu-id="3d095-125">Relationships</span></span>
<span data-ttu-id="3d095-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d095-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d095-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d095-127">JSON Representation</span></span>
<span data-ttu-id="3d095-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d095-128">Here is a JSON representation of the resource.</span></span>
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






