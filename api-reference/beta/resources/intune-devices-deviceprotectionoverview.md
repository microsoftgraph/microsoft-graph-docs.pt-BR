---
title: tipo de recurso deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d6cd5cc1eef939476a6fa3b5c46a7cfa315607b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154086"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="27939-103">tipo de recurso deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="27939-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="27939-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27939-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27939-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27939-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27939-106">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27939-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="27939-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27939-107">Properties</span></span>
|<span data-ttu-id="27939-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27939-108">Property</span></span>|<span data-ttu-id="27939-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="27939-109">Type</span></span>|<span data-ttu-id="27939-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="27939-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27939-111">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="27939-112">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-112">Int32</span></span>|<span data-ttu-id="27939-113">Contagem total de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="27939-113">Total device count.</span></span>|
|<span data-ttu-id="27939-114">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="27939-115">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-115">Int32</span></span>|<span data-ttu-id="27939-116">Dispositivo com contagem inativa de agente de ameaça</span><span class="sxs-lookup"><span data-stu-id="27939-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="27939-117">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="27939-118">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-118">Int32</span></span>|<span data-ttu-id="27939-119">Dispositivo com o estado do agente de ameaça como contagem desconhecida.</span><span class="sxs-lookup"><span data-stu-id="27939-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="27939-120">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="27939-121">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-121">Int32</span></span>|<span data-ttu-id="27939-122">Dispositivo com a contagem de assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="27939-122">Device with old signature count.</span></span>|
|<span data-ttu-id="27939-123">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-123">cleanDeviceCount</span></span>|<span data-ttu-id="27939-124">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-124">Int32</span></span>|<span data-ttu-id="27939-125">Limpar contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="27939-125">Clean device count.</span></span>|
|<span data-ttu-id="27939-126">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="27939-127">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-127">Int32</span></span>|<span data-ttu-id="27939-128">Contagem de dispositivos de verificação completa pendente.</span><span class="sxs-lookup"><span data-stu-id="27939-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="27939-129">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="27939-130">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-130">Int32</span></span>|<span data-ttu-id="27939-131">Contagem de dispositivos de reinicialização pendente.</span><span class="sxs-lookup"><span data-stu-id="27939-131">Pending restart device count.</span></span>|
|<span data-ttu-id="27939-132">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="27939-133">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-133">Int32</span></span>|<span data-ttu-id="27939-134">Contagem de dispositivos de etapas manuais pendentes.</span><span class="sxs-lookup"><span data-stu-id="27939-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="27939-135">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="27939-136">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-136">Int32</span></span>|<span data-ttu-id="27939-137">Contagem de dispositivos de verificação offline pendente.</span><span class="sxs-lookup"><span data-stu-id="27939-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="27939-138">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27939-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="27939-139">Int32</span><span class="sxs-lookup"><span data-stu-id="27939-139">Int32</span></span>|<span data-ttu-id="27939-140">Contagem de dispositivos de falhas críticas.</span><span class="sxs-lookup"><span data-stu-id="27939-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27939-141">Relações</span><span class="sxs-lookup"><span data-stu-id="27939-141">Relationships</span></span>
<span data-ttu-id="27939-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27939-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27939-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27939-143">JSON Representation</span></span>
<span data-ttu-id="27939-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27939-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```




