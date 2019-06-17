---
title: tipo de recurso deliveryOptimizationBandwidthPercentage
description: Limites de largura de banda especificados como uma porcentagem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 482dd1ee20e28a3ae9f5982d144d19a9143123af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979673"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="358c5-103">tipo de recurso deliveryOptimizationBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="358c5-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="358c5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="358c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="358c5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="358c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="358c5-106">Limites de largura de banda especificados como uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="358c5-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="358c5-107">Herda de [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="358c5-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="358c5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="358c5-108">Properties</span></span>
|<span data-ttu-id="358c5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="358c5-109">Property</span></span>|<span data-ttu-id="358c5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="358c5-110">Type</span></span>|<span data-ttu-id="358c5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="358c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="358c5-112">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="358c5-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="358c5-113">Int32</span><span class="sxs-lookup"><span data-stu-id="358c5-113">Int32</span></span>|<span data-ttu-id="358c5-114">Especifica a largura de banda de download máximo que a otimização de entrega usa em todas as atividades de download simultâneas como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="358c5-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="358c5-115">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="358c5-115">Valid values 0 to 100</span></span>
<span data-ttu-id="358c5-116">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="358c5-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="358c5-117">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="358c5-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="358c5-118">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="358c5-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="358c5-119">Int32</span><span class="sxs-lookup"><span data-stu-id="358c5-119">Int32</span></span>|<span data-ttu-id="358c5-120">Especifica a largura de banda máxima de download de primeiro plano que a otimização de entrega usa em todas as atividades de download simultâneos como uma porcentagem de largura de banda de download disponível (0-100).</span><span class="sxs-lookup"><span data-stu-id="358c5-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="358c5-121">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="358c5-121">Valid values 0 to 100</span></span>
<span data-ttu-id="358c5-122">O valor padrão 0 (zero) significa que a otimização de entrega é ajustada dinamicamente para usar a largura de banda disponível para downloads de primeiro plano.</span><span class="sxs-lookup"><span data-stu-id="358c5-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="358c5-123">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="358c5-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="358c5-124">Relações</span><span class="sxs-lookup"><span data-stu-id="358c5-124">Relationships</span></span>
<span data-ttu-id="358c5-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="358c5-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="358c5-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="358c5-126">JSON Representation</span></span>
<span data-ttu-id="358c5-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="358c5-127">Here is a JSON representation of the resource.</span></span>
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





