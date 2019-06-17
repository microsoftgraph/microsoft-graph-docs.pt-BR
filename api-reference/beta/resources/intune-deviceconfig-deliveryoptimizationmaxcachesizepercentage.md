---
title: tipo de recurso deliveryOptimizationMaxCacheSizePercentage
description: Tipos de percentual máximo de otimização de entrega.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f80634e421b7106bee5f9a1b369e22c3b4e6155
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979575"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="dab76-103">tipo de recurso deliveryOptimizationMaxCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="dab76-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

> <span data-ttu-id="dab76-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dab76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dab76-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dab76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dab76-106">Tipos de percentual máximo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="dab76-106">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="dab76-107">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="dab76-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dab76-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dab76-108">Properties</span></span>
|<span data-ttu-id="dab76-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dab76-109">Property</span></span>|<span data-ttu-id="dab76-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dab76-110">Type</span></span>|<span data-ttu-id="dab76-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dab76-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dab76-112">maximumCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="dab76-112">maximumCacheSizePercentage</span></span>|<span data-ttu-id="dab76-113">Int32</span><span class="sxs-lookup"><span data-stu-id="dab76-113">Int32</span></span>|<span data-ttu-id="dab76-114">Especifica o tamanho máximo de cache que a otimização de entrega pode utilizar, como um percentual do tamanho do disco (1-100).</span><span class="sxs-lookup"><span data-stu-id="dab76-114">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="dab76-115">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="dab76-115">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="dab76-116">Relações</span><span class="sxs-lookup"><span data-stu-id="dab76-116">Relationships</span></span>
<span data-ttu-id="dab76-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dab76-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dab76-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dab76-118">JSON Representation</span></span>
<span data-ttu-id="dab76-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dab76-119">Here is a JSON representation of the resource.</span></span>
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





