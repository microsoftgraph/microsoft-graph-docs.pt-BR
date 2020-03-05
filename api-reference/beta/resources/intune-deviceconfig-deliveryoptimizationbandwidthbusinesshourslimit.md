---
title: tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit
description: Tipo de tempo de largura de banda e tipos de porcentagem
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1284062e20df896dd30a99bec5506ad101c742ca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526808"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="3799c-103">tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="3799c-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

<span data-ttu-id="3799c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3799c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3799c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3799c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3799c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3799c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3799c-107">Tipo de tempo de largura de banda e tipos de porcentagem</span><span class="sxs-lookup"><span data-stu-id="3799c-107">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="3799c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3799c-108">Properties</span></span>
|<span data-ttu-id="3799c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3799c-109">Property</span></span>|<span data-ttu-id="3799c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3799c-110">Type</span></span>|<span data-ttu-id="3799c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3799c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3799c-112">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="3799c-112">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="3799c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3799c-113">Int32</span></span>|<span data-ttu-id="3799c-114">Especifica o início do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="3799c-114">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="3799c-115">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="3799c-115">Valid values 0 to 23</span></span>|
|<span data-ttu-id="3799c-116">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="3799c-116">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="3799c-117">Int32</span><span class="sxs-lookup"><span data-stu-id="3799c-117">Int32</span></span>|<span data-ttu-id="3799c-118">Especifica o fim do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="3799c-118">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="3799c-119">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="3799c-119">Valid values 0 to 23</span></span>|
|<span data-ttu-id="3799c-120">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="3799c-120">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="3799c-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3799c-121">Int32</span></span>|<span data-ttu-id="3799c-122">Especifica a porcentagem de largura de banda a ser limite durante o horário comercial (0-100).</span><span class="sxs-lookup"><span data-stu-id="3799c-122">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="3799c-123">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="3799c-123">Valid values 0 to 100</span></span>|
|<span data-ttu-id="3799c-124">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="3799c-124">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="3799c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3799c-125">Int32</span></span>|<span data-ttu-id="3799c-126">Especifica a porcentagem de largura de banda para limitar o horário comercial de outsids (0-100).</span><span class="sxs-lookup"><span data-stu-id="3799c-126">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="3799c-127">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="3799c-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="3799c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="3799c-128">Relationships</span></span>
<span data-ttu-id="3799c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3799c-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3799c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3799c-130">JSON Representation</span></span>
<span data-ttu-id="3799c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3799c-131">Here is a JSON representation of the resource.</span></span>
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



