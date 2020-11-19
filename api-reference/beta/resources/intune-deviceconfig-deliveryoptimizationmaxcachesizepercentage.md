---
title: tipo de recurso deliveryOptimizationMaxCacheSizePercentage
description: Tipos de percentual máximo de otimização de entrega.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53a32220a72b994bbbff4c39a16923fb27049051
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288723"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="b898f-103">tipo de recurso deliveryOptimizationMaxCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="b898f-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

<span data-ttu-id="b898f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b898f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b898f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b898f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b898f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b898f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b898f-107">Tipos de percentual máximo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="b898f-107">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="b898f-108">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="b898f-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b898f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b898f-109">Properties</span></span>
|<span data-ttu-id="b898f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b898f-110">Property</span></span>|<span data-ttu-id="b898f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b898f-111">Type</span></span>|<span data-ttu-id="b898f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b898f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b898f-113">maximumCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="b898f-113">maximumCacheSizePercentage</span></span>|<span data-ttu-id="b898f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b898f-114">Int32</span></span>|<span data-ttu-id="b898f-115">Especifica o tamanho máximo de cache que a otimização de entrega pode utilizar, como um percentual do tamanho do disco (1-100).</span><span class="sxs-lookup"><span data-stu-id="b898f-115">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="b898f-116">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="b898f-116">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="b898f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b898f-117">Relationships</span></span>
<span data-ttu-id="b898f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b898f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b898f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b898f-119">JSON Representation</span></span>
<span data-ttu-id="b898f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b898f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```




