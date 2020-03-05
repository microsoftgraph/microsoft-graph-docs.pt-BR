---
title: tipo de recurso deliveryOptimizationBandwidthAbsolute
description: Limites de largura de banda em quilobytes por segundo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 536ba80fbc1ae0cee8bbef9933d6366a05284c33
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526821"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="b2df9-103">tipo de recurso deliveryOptimizationBandwidthAbsolute</span><span class="sxs-lookup"><span data-stu-id="b2df9-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

<span data-ttu-id="b2df9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b2df9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2df9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2df9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2df9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2df9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2df9-107">Limites de largura de banda em quilobytes por segundo.</span><span class="sxs-lookup"><span data-stu-id="b2df9-107">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="b2df9-108">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="b2df9-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2df9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2df9-109">Properties</span></span>
|<span data-ttu-id="b2df9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2df9-110">Property</span></span>|<span data-ttu-id="b2df9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2df9-111">Type</span></span>|<span data-ttu-id="b2df9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2df9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2df9-113">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="b2df9-113">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="b2df9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b2df9-114">Int64</span></span>|<span data-ttu-id="b2df9-115">Especifica a largura de banda máxima de download em quilobytes/segundo que o dispositivo pode usar em todas as atividades de download simultâneos usando a otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="b2df9-115">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="b2df9-116">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="b2df9-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="b2df9-117">O valor 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads.</span><span class="sxs-lookup"><span data-stu-id="b2df9-117">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="b2df9-118">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="b2df9-118">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="b2df9-119">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="b2df9-119">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="b2df9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="b2df9-120">Int64</span></span>|<span data-ttu-id="b2df9-121">Especifica a largura de banda de upload máxima em KiloBytes/segundo que um dispositivo usará em toda a atividade de upload simultâneo usando a otimização de entrega (0-4000000).</span><span class="sxs-lookup"><span data-stu-id="b2df9-121">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="b2df9-122">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="b2df9-122">Valid values 0 to 4000000</span></span>
<span data-ttu-id="b2df9-123">O valor padrão é 0, que permite uma largura de banda possivelmente ilimitada (otimizada para uso mínimo da largura de banda de upload).</span><span class="sxs-lookup"><span data-stu-id="b2df9-123">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="b2df9-124">Valores válidos de 0 a 4 milhões</span><span class="sxs-lookup"><span data-stu-id="b2df9-124">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2df9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="b2df9-125">Relationships</span></span>
<span data-ttu-id="b2df9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2df9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2df9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2df9-127">JSON Representation</span></span>
<span data-ttu-id="b2df9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2df9-128">Here is a JSON representation of the resource.</span></span>
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



