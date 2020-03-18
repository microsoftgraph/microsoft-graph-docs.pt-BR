---
title: tipo de recurso deliveryOptimizationBandwidthPercentage
description: Limites de largura de banda especificados como uma porcentagem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34e3a76bf7b7ef70f880d4de8c432f84d7eb3509
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794372"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="34594-103">tipo de recurso deliveryOptimizationBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="34594-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="34594-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34594-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34594-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34594-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34594-106">Limites de largura de banda especificados como uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="34594-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="34594-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="34594-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34594-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34594-108">Properties</span></span>
|<span data-ttu-id="34594-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34594-109">Property</span></span>|<span data-ttu-id="34594-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="34594-110">Type</span></span>|<span data-ttu-id="34594-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="34594-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34594-112">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="34594-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="34594-113">Int32</span><span class="sxs-lookup"><span data-stu-id="34594-113">Int32</span></span>|<span data-ttu-id="34594-114">Especifica a largura de banda de download máximo que a otimização de entrega usa em todas as atividades de download simultâneas como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="34594-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="34594-115">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="34594-115">Valid values 0 to 100</span></span>
<span data-ttu-id="34594-116">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="34594-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="34594-117">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="34594-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="34594-118">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="34594-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="34594-119">Int32</span><span class="sxs-lookup"><span data-stu-id="34594-119">Int32</span></span>|<span data-ttu-id="34594-120">Especifica a largura de banda máxima de download de primeiro plano que a otimização de entrega usa em todas as atividades de download simultâneos como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="34594-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="34594-121">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="34594-121">Valid values 0 to 100</span></span>
<span data-ttu-id="34594-122">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads de primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="34594-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="34594-123">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="34594-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="34594-124">Relações</span><span class="sxs-lookup"><span data-stu-id="34594-124">Relationships</span></span>
<span data-ttu-id="34594-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34594-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34594-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34594-126">JSON Representation</span></span>
<span data-ttu-id="34594-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34594-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```



