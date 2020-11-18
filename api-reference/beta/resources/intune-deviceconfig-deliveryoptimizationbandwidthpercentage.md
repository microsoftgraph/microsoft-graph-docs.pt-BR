---
title: tipo de recurso deliveryOptimizationBandwidthPercentage
description: Limites de largura de banda especificados como uma porcentagem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 85dc858431b15a142a42afc74b1b7c1ba76a4667
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199606"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="7ccb5-103">tipo de recurso deliveryOptimizationBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="7ccb5-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

<span data-ttu-id="7ccb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ccb5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ccb5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ccb5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ccb5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ccb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ccb5-107">Limites de largura de banda especificados como uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="7ccb5-107">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="7ccb5-108">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="7ccb5-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7ccb5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ccb5-109">Properties</span></span>
|<span data-ttu-id="7ccb5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ccb5-110">Property</span></span>|<span data-ttu-id="7ccb5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ccb5-111">Type</span></span>|<span data-ttu-id="7ccb5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ccb5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ccb5-113">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="7ccb5-113">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="7ccb5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7ccb5-114">Int32</span></span>|<span data-ttu-id="7ccb5-115">Especifica a largura de banda de download máximo que a otimização de entrega usa em todas as atividades de download simultâneas como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="7ccb5-115">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="7ccb5-116">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="7ccb5-116">Valid values 0 to 100</span></span>
<span data-ttu-id="7ccb5-117">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="7ccb5-117">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="7ccb5-118">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="7ccb5-118">Valid values 0 to 100</span></span>|
|<span data-ttu-id="7ccb5-119">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="7ccb5-119">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="7ccb5-120">Int32</span><span class="sxs-lookup"><span data-stu-id="7ccb5-120">Int32</span></span>|<span data-ttu-id="7ccb5-121">Especifica a largura de banda máxima de download de primeiro plano que a otimização de entrega usa em todas as atividades de download simultâneos como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="7ccb5-121">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="7ccb5-122">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="7ccb5-122">Valid values 0 to 100</span></span>
<span data-ttu-id="7ccb5-123">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads de primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="7ccb5-123">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="7ccb5-124">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="7ccb5-124">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ccb5-125">Relações</span><span class="sxs-lookup"><span data-stu-id="7ccb5-125">Relationships</span></span>
<span data-ttu-id="7ccb5-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ccb5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ccb5-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ccb5-127">JSON Representation</span></span>
<span data-ttu-id="7ccb5-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ccb5-128">Here is a JSON representation of the resource.</span></span>
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




