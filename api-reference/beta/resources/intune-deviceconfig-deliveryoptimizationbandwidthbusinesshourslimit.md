---
title: tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit
description: Tipo de tempo de largura de banda e tipos de porcentagem
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83e0402e7b63925e8c02c87a5c1abd9b08c9c8c6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794386"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="18f0c-103">tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="18f0c-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

> <span data-ttu-id="18f0c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18f0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18f0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18f0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18f0c-106">Tipo de tempo de largura de banda e tipos de porcentagem</span><span class="sxs-lookup"><span data-stu-id="18f0c-106">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="18f0c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18f0c-107">Properties</span></span>
|<span data-ttu-id="18f0c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18f0c-108">Property</span></span>|<span data-ttu-id="18f0c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="18f0c-109">Type</span></span>|<span data-ttu-id="18f0c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18f0c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18f0c-111">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="18f0c-111">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="18f0c-112">Int32</span><span class="sxs-lookup"><span data-stu-id="18f0c-112">Int32</span></span>|<span data-ttu-id="18f0c-113">Especifica o início do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="18f0c-113">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="18f0c-114">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="18f0c-114">Valid values 0 to 23</span></span>|
|<span data-ttu-id="18f0c-115">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="18f0c-115">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="18f0c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="18f0c-116">Int32</span></span>|<span data-ttu-id="18f0c-117">Especifica o fim do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="18f0c-117">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="18f0c-118">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="18f0c-118">Valid values 0 to 23</span></span>|
|<span data-ttu-id="18f0c-119">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="18f0c-119">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="18f0c-120">Int32</span><span class="sxs-lookup"><span data-stu-id="18f0c-120">Int32</span></span>|<span data-ttu-id="18f0c-121">Especifica a porcentagem de largura de banda a ser limite durante o horário comercial (0-100).</span><span class="sxs-lookup"><span data-stu-id="18f0c-121">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="18f0c-122">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="18f0c-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="18f0c-123">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="18f0c-123">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="18f0c-124">Int32</span><span class="sxs-lookup"><span data-stu-id="18f0c-124">Int32</span></span>|<span data-ttu-id="18f0c-125">Especifica a porcentagem de largura de banda para limitar o horário comercial de outsids (0-100).</span><span class="sxs-lookup"><span data-stu-id="18f0c-125">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="18f0c-126">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="18f0c-126">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="18f0c-127">Relações</span><span class="sxs-lookup"><span data-stu-id="18f0c-127">Relationships</span></span>
<span data-ttu-id="18f0c-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18f0c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18f0c-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18f0c-129">JSON Representation</span></span>
<span data-ttu-id="18f0c-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18f0c-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```



