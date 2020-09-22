---
title: tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute
description: Tipo absoluto de tamanho máximo de cache da otimização de entrega.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 73e0f65711afc22a585cc2ecc9e27cf452e7be32
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085140"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="93f2e-103">tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute</span><span class="sxs-lookup"><span data-stu-id="93f2e-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

<span data-ttu-id="93f2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93f2e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93f2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93f2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93f2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93f2e-107">Tipo absoluto de tamanho máximo de cache da otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="93f2e-107">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="93f2e-108">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="93f2e-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="93f2e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93f2e-109">Properties</span></span>
|<span data-ttu-id="93f2e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93f2e-110">Property</span></span>|<span data-ttu-id="93f2e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="93f2e-111">Type</span></span>|<span data-ttu-id="93f2e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="93f2e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f2e-113">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="93f2e-113">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="93f2e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="93f2e-114">Int64</span></span>|<span data-ttu-id="93f2e-115">Especifica o tamanho máximo em GB de cache de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="93f2e-115">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="93f2e-116">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="93f2e-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="93f2e-117">O valor 0 (zero) significa cache "ilimitado".</span><span class="sxs-lookup"><span data-stu-id="93f2e-117">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="93f2e-118">A otimização de entrega limpará o cache quando o dispositivo estiver com pouco espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="93f2e-118">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="93f2e-119">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="93f2e-119">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="93f2e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="93f2e-120">Relationships</span></span>
<span data-ttu-id="93f2e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93f2e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93f2e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93f2e-122">JSON Representation</span></span>
<span data-ttu-id="93f2e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93f2e-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```






