---
title: tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute
description: Tipo absoluto de tamanho máximo de cache da otimização de entrega.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 096dbdd27d31e51849b8e8f53967e08a8029f756
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333280"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="3a44b-103">tipo de recurso deliveryOptimizationMaxCacheSizeAbsolute</span><span class="sxs-lookup"><span data-stu-id="3a44b-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

> <span data-ttu-id="3a44b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a44b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a44b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a44b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a44b-106">Tipo absoluto de tamanho máximo de cache da otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="3a44b-106">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="3a44b-107">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="3a44b-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a44b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a44b-108">Properties</span></span>
|<span data-ttu-id="3a44b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a44b-109">Property</span></span>|<span data-ttu-id="3a44b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a44b-110">Type</span></span>|<span data-ttu-id="3a44b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a44b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a44b-112">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="3a44b-112">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="3a44b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="3a44b-113">Int64</span></span>|<span data-ttu-id="3a44b-114">Especifica o tamanho máximo em GB de cache de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="3a44b-114">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="3a44b-115">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="3a44b-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="3a44b-116">O valor 0 (zero) significa cache "ilimitado".</span><span class="sxs-lookup"><span data-stu-id="3a44b-116">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="3a44b-117">A otimização de entrega limpará o cache quando o dispositivo estiver com pouco espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="3a44b-117">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="3a44b-118">Valores válidos de 0 a 4294967295</span><span class="sxs-lookup"><span data-stu-id="3a44b-118">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a44b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3a44b-119">Relationships</span></span>
<span data-ttu-id="3a44b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a44b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a44b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a44b-121">JSON Representation</span></span>
<span data-ttu-id="3a44b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a44b-122">Here is a JSON representation of the resource.</span></span>
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



