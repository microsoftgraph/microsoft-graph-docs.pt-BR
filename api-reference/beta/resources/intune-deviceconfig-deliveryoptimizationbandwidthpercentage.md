---
title: tipo de recurso deliveryOptimizationBandwidthPercentage
description: Limites de largura de banda especificados como uma porcentagem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fb30ca54911723c619c8199ca32a9542772a6da
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177858"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="eb059-103">tipo de recurso deliveryOptimizationBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="eb059-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="eb059-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb059-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb059-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb059-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb059-106">Limites de largura de banda especificados como uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="eb059-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="eb059-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="eb059-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb059-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb059-108">Properties</span></span>
|<span data-ttu-id="eb059-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb059-109">Property</span></span>|<span data-ttu-id="eb059-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb059-110">Type</span></span>|<span data-ttu-id="eb059-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb059-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb059-112">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="eb059-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="eb059-113">Int32</span><span class="sxs-lookup"><span data-stu-id="eb059-113">Int32</span></span>|<span data-ttu-id="eb059-114">Especifica a largura de banda de download máximo que a otimização de entrega usa em todas as atividades de download simultâneas como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="eb059-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="eb059-115">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="eb059-115">Valid values 0 to 100</span></span>
<span data-ttu-id="eb059-116">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="eb059-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="eb059-117">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="eb059-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="eb059-118">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="eb059-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="eb059-119">Int32</span><span class="sxs-lookup"><span data-stu-id="eb059-119">Int32</span></span>|<span data-ttu-id="eb059-120">Especifica a largura de banda máxima de download de primeiro plano que a otimização de entrega usa em todas as atividades de download simultâneos como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="eb059-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="eb059-121">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="eb059-121">Valid values 0 to 100</span></span>
<span data-ttu-id="eb059-122">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads de primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="eb059-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="eb059-123">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="eb059-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb059-124">Relações</span><span class="sxs-lookup"><span data-stu-id="eb059-124">Relationships</span></span>
<span data-ttu-id="eb059-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb059-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb059-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb059-126">JSON Representation</span></span>
<span data-ttu-id="eb059-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb059-127">Here is a JSON representation of the resource.</span></span>
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




