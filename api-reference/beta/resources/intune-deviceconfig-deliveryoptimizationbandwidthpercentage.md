---
title: tipo de recurso deliveryOptimizationBandwidthPercentage
description: Limites de largura de banda especificados como uma porcentagem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba89d0101a603634399641ef1f9ccff28c02c42f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970777"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="72cfd-103">tipo de recurso deliveryOptimizationBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="72cfd-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="72cfd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72cfd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72cfd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72cfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72cfd-106">Limites de largura de banda especificados como uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="72cfd-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="72cfd-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="72cfd-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="72cfd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72cfd-108">Properties</span></span>
|<span data-ttu-id="72cfd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72cfd-109">Property</span></span>|<span data-ttu-id="72cfd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="72cfd-110">Type</span></span>|<span data-ttu-id="72cfd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="72cfd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72cfd-112">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="72cfd-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="72cfd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="72cfd-113">Int32</span></span>|<span data-ttu-id="72cfd-114">Especifica a largura de banda de download máximo que a otimização de entrega usa em todas as atividades de download simultâneas como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="72cfd-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="72cfd-115">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="72cfd-115">Valid values 0 to 100</span></span>
<span data-ttu-id="72cfd-116">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="72cfd-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="72cfd-117">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="72cfd-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="72cfd-118">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="72cfd-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="72cfd-119">Int32</span><span class="sxs-lookup"><span data-stu-id="72cfd-119">Int32</span></span>|<span data-ttu-id="72cfd-120">Especifica a largura de banda máxima de download de primeiro plano que a otimização de entrega usa em todas as atividades de download simultâneos como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="72cfd-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="72cfd-121">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="72cfd-121">Valid values 0 to 100</span></span>
<span data-ttu-id="72cfd-122">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads de primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="72cfd-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="72cfd-123">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="72cfd-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="72cfd-124">Relações</span><span class="sxs-lookup"><span data-stu-id="72cfd-124">Relationships</span></span>
<span data-ttu-id="72cfd-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72cfd-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72cfd-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72cfd-126">JSON Representation</span></span>
<span data-ttu-id="72cfd-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72cfd-127">Here is a JSON representation of the resource.</span></span>
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





