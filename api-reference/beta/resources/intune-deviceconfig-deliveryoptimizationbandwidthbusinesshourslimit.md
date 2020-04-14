---
title: tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit
description: Tipo de tempo de largura de banda e tipos de porcentagem
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4044b62a42c37abf030ff0a5d206093d4a2b8c80
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420585"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="f8639-103">tipo de recurso deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="f8639-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

<span data-ttu-id="f8639-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8639-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8639-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8639-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8639-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8639-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8639-107">Tipo de tempo de largura de banda e tipos de porcentagem</span><span class="sxs-lookup"><span data-stu-id="f8639-107">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="f8639-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8639-108">Properties</span></span>
|<span data-ttu-id="f8639-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8639-109">Property</span></span>|<span data-ttu-id="f8639-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8639-110">Type</span></span>|<span data-ttu-id="f8639-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8639-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8639-112">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="f8639-112">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="f8639-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f8639-113">Int32</span></span>|<span data-ttu-id="f8639-114">Especifica o início do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="f8639-114">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="f8639-115">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="f8639-115">Valid values 0 to 23</span></span>|
|<span data-ttu-id="f8639-116">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="f8639-116">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="f8639-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f8639-117">Int32</span></span>|<span data-ttu-id="f8639-118">Especifica o fim do horário comercial usando um relógio de 24 horas (0-23).</span><span class="sxs-lookup"><span data-stu-id="f8639-118">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="f8639-119">Valores válidos de 0 a 23</span><span class="sxs-lookup"><span data-stu-id="f8639-119">Valid values 0 to 23</span></span>|
|<span data-ttu-id="f8639-120">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="f8639-120">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="f8639-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f8639-121">Int32</span></span>|<span data-ttu-id="f8639-122">Especifica a porcentagem de largura de banda a ser limite durante o horário comercial (0-100).</span><span class="sxs-lookup"><span data-stu-id="f8639-122">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="f8639-123">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="f8639-123">Valid values 0 to 100</span></span>|
|<span data-ttu-id="f8639-124">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="f8639-124">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="f8639-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f8639-125">Int32</span></span>|<span data-ttu-id="f8639-126">Especifica a porcentagem de largura de banda para limitar o horário comercial de outsids (0-100).</span><span class="sxs-lookup"><span data-stu-id="f8639-126">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="f8639-127">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="f8639-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8639-128">Relações</span><span class="sxs-lookup"><span data-stu-id="f8639-128">Relationships</span></span>
<span data-ttu-id="f8639-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8639-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8639-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8639-130">JSON Representation</span></span>
<span data-ttu-id="f8639-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8639-131">Here is a JSON representation of the resource.</span></span>
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



