---
title: tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute
description: Tipo absoluto de tamanho máximo de cache da otimização de entrega.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d6713eb502405a19925c5033a21b9b82361edb5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692566"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="d403d-103">tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute</span><span class="sxs-lookup"><span data-stu-id="d403d-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

<span data-ttu-id="d403d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d403d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d403d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d403d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d403d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d403d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d403d-107">Tipo absoluto de tamanho máximo de cache da otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="d403d-107">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="d403d-108">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="d403d-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d403d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d403d-109">Properties</span></span>
|<span data-ttu-id="d403d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d403d-110">Property</span></span>|<span data-ttu-id="d403d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d403d-111">Type</span></span>|<span data-ttu-id="d403d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d403d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d403d-113">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="d403d-113">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="d403d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d403d-114">Int64</span></span>|<span data-ttu-id="d403d-115">Especifica o tamanho máximo em GB de cache de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="d403d-115">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="d403d-116">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="d403d-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="d403d-117">O valor 0 (zero) significa cache "ilimitado".</span><span class="sxs-lookup"><span data-stu-id="d403d-117">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="d403d-118">A otimização de entrega limpará o cache quando o dispositivo estiver com pouco espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="d403d-118">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="d403d-119">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="d403d-119">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="d403d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d403d-120">Relationships</span></span>
<span data-ttu-id="d403d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d403d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d403d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d403d-122">JSON Representation</span></span>
<span data-ttu-id="d403d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d403d-123">Here is a JSON representation of the resource.</span></span>
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





