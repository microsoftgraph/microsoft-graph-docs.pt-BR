---
title: tipo de recurso deliveryOptimizationMaxCacheSizePercentage
description: Tipos de percentual máximo de otimização de entrega.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f5ef7bef4f86f78207df37dcb684b714c93b8d5d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526747"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="0ad46-103">tipo de recurso deliveryOptimizationMaxCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="0ad46-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

<span data-ttu-id="0ad46-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ad46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ad46-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ad46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ad46-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ad46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ad46-107">Tipos de percentual máximo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="0ad46-107">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="0ad46-108">Herda de [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="0ad46-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ad46-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ad46-109">Properties</span></span>
|<span data-ttu-id="0ad46-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ad46-110">Property</span></span>|<span data-ttu-id="0ad46-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ad46-111">Type</span></span>|<span data-ttu-id="0ad46-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ad46-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ad46-113">maximumCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="0ad46-113">maximumCacheSizePercentage</span></span>|<span data-ttu-id="0ad46-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0ad46-114">Int32</span></span>|<span data-ttu-id="0ad46-115">Especifica o tamanho máximo de cache que a otimização de entrega pode utilizar, como um percentual do tamanho do disco (1-100).</span><span class="sxs-lookup"><span data-stu-id="0ad46-115">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="0ad46-116">Valores válidos de 1 a 100</span><span class="sxs-lookup"><span data-stu-id="0ad46-116">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ad46-117">Relações</span><span class="sxs-lookup"><span data-stu-id="0ad46-117">Relationships</span></span>
<span data-ttu-id="0ad46-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ad46-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ad46-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ad46-119">JSON Representation</span></span>
<span data-ttu-id="0ad46-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ad46-120">Here is a JSON representation of the resource.</span></span>
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



