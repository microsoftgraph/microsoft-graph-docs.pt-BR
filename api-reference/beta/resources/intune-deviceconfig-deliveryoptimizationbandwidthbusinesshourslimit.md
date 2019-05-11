---
title: tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit
description: Tipo de tempo de largura de banda e tipos de porcentagem
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71dae93d44f7b7276bd268170a2c37b434b5bbb2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947264"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="c4afa-103">tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="c4afa-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

> <span data-ttu-id="c4afa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4afa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4afa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4afa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4afa-106">Tipo de tempo de largura de banda e tipos de porcentagem</span><span class="sxs-lookup"><span data-stu-id="c4afa-106">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="c4afa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4afa-107">Properties</span></span>
|<span data-ttu-id="c4afa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4afa-108">Property</span></span>|<span data-ttu-id="c4afa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4afa-109">Type</span></span>|<span data-ttu-id="c4afa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4afa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4afa-111">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="c4afa-111">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="c4afa-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c4afa-112">Int32</span></span>|<span data-ttu-id="c4afa-113">Especifica o início do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="c4afa-113">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="c4afa-114">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="c4afa-114">Valid values 0 to 23</span></span>|
|<span data-ttu-id="c4afa-115">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="c4afa-115">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="c4afa-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c4afa-116">Int32</span></span>|<span data-ttu-id="c4afa-117">Especifica o fim do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="c4afa-117">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="c4afa-118">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="c4afa-118">Valid values 0 to 23</span></span>|
|<span data-ttu-id="c4afa-119">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="c4afa-119">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="c4afa-120">Int32</span><span class="sxs-lookup"><span data-stu-id="c4afa-120">Int32</span></span>|<span data-ttu-id="c4afa-121">Especifica a porcentagem de largura de banda a ser limite durante o horário comercial (0-100).</span><span class="sxs-lookup"><span data-stu-id="c4afa-121">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="c4afa-122">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="c4afa-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="c4afa-123">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="c4afa-123">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="c4afa-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c4afa-124">Int32</span></span>|<span data-ttu-id="c4afa-125">Especifica a porcentagem de largura de banda para limitar o horário comercial de outsids (0-100).</span><span class="sxs-lookup"><span data-stu-id="c4afa-125">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="c4afa-126">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="c4afa-126">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4afa-127">Relações</span><span class="sxs-lookup"><span data-stu-id="c4afa-127">Relationships</span></span>
<span data-ttu-id="c4afa-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c4afa-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4afa-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4afa-129">JSON Representation</span></span>
<span data-ttu-id="c4afa-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4afa-130">Here is a JSON representation of the resource.</span></span>
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




