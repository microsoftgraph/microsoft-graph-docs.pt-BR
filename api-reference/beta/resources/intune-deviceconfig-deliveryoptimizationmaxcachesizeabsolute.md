---
title: tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute
description: Tipo absoluto de tamanho máximo de cache da otimização de entrega.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dfb158b30c8c2d75a58ddcbab190eaa37e9153bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294715"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="616cb-103">tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute</span><span class="sxs-lookup"><span data-stu-id="616cb-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

<span data-ttu-id="616cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="616cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="616cb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="616cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="616cb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="616cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="616cb-107">Tipo absoluto de tamanho máximo de cache da otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="616cb-107">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="616cb-108">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="616cb-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="616cb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="616cb-109">Properties</span></span>
|<span data-ttu-id="616cb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="616cb-110">Property</span></span>|<span data-ttu-id="616cb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="616cb-111">Type</span></span>|<span data-ttu-id="616cb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="616cb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="616cb-113">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="616cb-113">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="616cb-114">Int64</span><span class="sxs-lookup"><span data-stu-id="616cb-114">Int64</span></span>|<span data-ttu-id="616cb-115">Especifica o tamanho máximo em GB de cache de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="616cb-115">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="616cb-116">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="616cb-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="616cb-117">O valor 0 (zero) significa cache "ilimitado".</span><span class="sxs-lookup"><span data-stu-id="616cb-117">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="616cb-118">A otimização de entrega limpará o cache quando o dispositivo estiver com pouco espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="616cb-118">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="616cb-119">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="616cb-119">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="616cb-120">Relações</span><span class="sxs-lookup"><span data-stu-id="616cb-120">Relationships</span></span>
<span data-ttu-id="616cb-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="616cb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="616cb-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="616cb-122">JSON Representation</span></span>
<span data-ttu-id="616cb-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="616cb-123">Here is a JSON representation of the resource.</span></span>
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




