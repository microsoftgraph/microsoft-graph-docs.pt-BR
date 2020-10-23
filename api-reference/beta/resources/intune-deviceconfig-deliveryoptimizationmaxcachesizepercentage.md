---
title: tipo de recurso deliveryOptimizationMaxCacheSizePercentage
description: Tipos de percentual máximo de otimização de entrega.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02b522ccfac58a6c4ff9f9780512e83abf2cdec8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692545"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="3383d-103">tipo de recurso deliveryOptimizationMaxCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="3383d-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

<span data-ttu-id="3383d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3383d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3383d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3383d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3383d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3383d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3383d-107">Tipos de percentual máximo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="3383d-107">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="3383d-108">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="3383d-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3383d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3383d-109">Properties</span></span>
|<span data-ttu-id="3383d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3383d-110">Property</span></span>|<span data-ttu-id="3383d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3383d-111">Type</span></span>|<span data-ttu-id="3383d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3383d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3383d-113">maximumCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="3383d-113">maximumCacheSizePercentage</span></span>|<span data-ttu-id="3383d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3383d-114">Int32</span></span>|<span data-ttu-id="3383d-115">Especifica o tamanho máximo de cache que a otimização de entrega pode utilizar, como um percentual do tamanho do disco (1-100).</span><span class="sxs-lookup"><span data-stu-id="3383d-115">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="3383d-116">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="3383d-116">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="3383d-117">Relações</span><span class="sxs-lookup"><span data-stu-id="3383d-117">Relationships</span></span>
<span data-ttu-id="3383d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3383d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3383d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3383d-119">JSON Representation</span></span>
<span data-ttu-id="3383d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3383d-120">Here is a JSON representation of the resource.</span></span>
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





