---
title: tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute
description: Tipo absoluto de tamanho máximo de cache da otimização de entrega.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a15b1bfea6da2af43c360ff143d8bb55bc44f6b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420454"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="dd923-103">tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute</span><span class="sxs-lookup"><span data-stu-id="dd923-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

<span data-ttu-id="dd923-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd923-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd923-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd923-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd923-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd923-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd923-107">Tipo absoluto de tamanho máximo de cache da otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="dd923-107">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="dd923-108">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="dd923-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dd923-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd923-109">Properties</span></span>
|<span data-ttu-id="dd923-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd923-110">Property</span></span>|<span data-ttu-id="dd923-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd923-111">Type</span></span>|<span data-ttu-id="dd923-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd923-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd923-113">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="dd923-113">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="dd923-114">Int64</span><span class="sxs-lookup"><span data-stu-id="dd923-114">Int64</span></span>|<span data-ttu-id="dd923-115">Especifica o tamanho máximo em GB de cache de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="dd923-115">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="dd923-116">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="dd923-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="dd923-117">O valor 0 (zero) significa cache "ilimitado".</span><span class="sxs-lookup"><span data-stu-id="dd923-117">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="dd923-118">A otimização de entrega limpará o cache quando o dispositivo estiver com pouco espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="dd923-118">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="dd923-119">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="dd923-119">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd923-120">Relações</span><span class="sxs-lookup"><span data-stu-id="dd923-120">Relationships</span></span>
<span data-ttu-id="dd923-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd923-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd923-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd923-122">JSON Representation</span></span>
<span data-ttu-id="dd923-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd923-123">Here is a JSON representation of the resource.</span></span>
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



