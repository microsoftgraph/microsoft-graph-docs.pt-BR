---
title: tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit
description: Tipo de tempo de largura de banda e tipos de porcentagem
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 10b02e2dc25717d2363a2db2edbf57db858cb9db
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696234"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="f087a-103">tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="f087a-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

<span data-ttu-id="f087a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f087a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f087a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f087a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f087a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f087a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f087a-107">Tipo de tempo de largura de banda e tipos de porcentagem</span><span class="sxs-lookup"><span data-stu-id="f087a-107">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="f087a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f087a-108">Properties</span></span>
|<span data-ttu-id="f087a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f087a-109">Property</span></span>|<span data-ttu-id="f087a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f087a-110">Type</span></span>|<span data-ttu-id="f087a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f087a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f087a-112">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="f087a-112">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="f087a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f087a-113">Int32</span></span>|<span data-ttu-id="f087a-114">Especifica o início do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="f087a-114">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="f087a-115">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="f087a-115">Valid values 0 to 23</span></span>|
|<span data-ttu-id="f087a-116">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="f087a-116">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="f087a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f087a-117">Int32</span></span>|<span data-ttu-id="f087a-118">Especifica o fim do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="f087a-118">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="f087a-119">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="f087a-119">Valid values 0 to 23</span></span>|
|<span data-ttu-id="f087a-120">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="f087a-120">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="f087a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f087a-121">Int32</span></span>|<span data-ttu-id="f087a-122">Especifica a porcentagem de largura de banda a ser limite durante o horário comercial (0-100).</span><span class="sxs-lookup"><span data-stu-id="f087a-122">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="f087a-123">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="f087a-123">Valid values 0 to 100</span></span>|
|<span data-ttu-id="f087a-124">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="f087a-124">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="f087a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f087a-125">Int32</span></span>|<span data-ttu-id="f087a-126">Especifica a porcentagem de largura de banda para limitar o horário comercial de outsids (0-100).</span><span class="sxs-lookup"><span data-stu-id="f087a-126">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="f087a-127">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="f087a-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="f087a-128">Relações</span><span class="sxs-lookup"><span data-stu-id="f087a-128">Relationships</span></span>
<span data-ttu-id="f087a-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f087a-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f087a-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f087a-130">JSON Representation</span></span>
<span data-ttu-id="f087a-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f087a-131">Here is a JSON representation of the resource.</span></span>
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





