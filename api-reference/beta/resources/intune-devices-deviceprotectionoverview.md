---
title: tipo de recurso deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5f6d4c325d11ee5f02277ad86f7bb038a2ac3b0f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123719"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="63264-103">tipo de recurso deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="63264-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="63264-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63264-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63264-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63264-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63264-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63264-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63264-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63264-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="63264-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63264-108">Properties</span></span>
|<span data-ttu-id="63264-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63264-109">Property</span></span>|<span data-ttu-id="63264-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="63264-110">Type</span></span>|<span data-ttu-id="63264-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="63264-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63264-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="63264-113">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-113">Int32</span></span>|<span data-ttu-id="63264-114">Contagem total de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="63264-114">Total device count.</span></span>|
|<span data-ttu-id="63264-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="63264-116">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-116">Int32</span></span>|<span data-ttu-id="63264-117">Dispositivo com contagem inativa de agente de ameaça</span><span class="sxs-lookup"><span data-stu-id="63264-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="63264-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="63264-119">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-119">Int32</span></span>|<span data-ttu-id="63264-120">Dispositivo com o estado do agente de ameaça como contagem desconhecida.</span><span class="sxs-lookup"><span data-stu-id="63264-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="63264-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="63264-122">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-122">Int32</span></span>|<span data-ttu-id="63264-123">Dispositivo com a contagem de assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="63264-123">Device with old signature count.</span></span>|
|<span data-ttu-id="63264-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-124">cleanDeviceCount</span></span>|<span data-ttu-id="63264-125">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-125">Int32</span></span>|<span data-ttu-id="63264-126">Limpar contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="63264-126">Clean device count.</span></span>|
|<span data-ttu-id="63264-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="63264-128">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-128">Int32</span></span>|<span data-ttu-id="63264-129">Contagem de dispositivos de verificação completa pendente.</span><span class="sxs-lookup"><span data-stu-id="63264-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="63264-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="63264-131">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-131">Int32</span></span>|<span data-ttu-id="63264-132">Contagem de dispositivos de reinicialização pendente.</span><span class="sxs-lookup"><span data-stu-id="63264-132">Pending restart device count.</span></span>|
|<span data-ttu-id="63264-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="63264-134">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-134">Int32</span></span>|<span data-ttu-id="63264-135">Contagem de dispositivos de etapas manuais pendentes.</span><span class="sxs-lookup"><span data-stu-id="63264-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="63264-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="63264-137">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-137">Int32</span></span>|<span data-ttu-id="63264-138">Contagem de dispositivos de verificação offline pendente.</span><span class="sxs-lookup"><span data-stu-id="63264-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="63264-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="63264-140">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-140">Int32</span></span>|<span data-ttu-id="63264-141">Contagem de dispositivos de falhas críticas.</span><span class="sxs-lookup"><span data-stu-id="63264-141">Critical failures device count.</span></span>|
|<span data-ttu-id="63264-142">pendingQuickScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63264-142">pendingQuickScanDeviceCount</span></span>|<span data-ttu-id="63264-143">Int32</span><span class="sxs-lookup"><span data-stu-id="63264-143">Int32</span></span>|<span data-ttu-id="63264-144">Contagem de dispositivos de verificação rápida pendente.</span><span class="sxs-lookup"><span data-stu-id="63264-144">Pending quick scan device count.</span></span> <span data-ttu-id="63264-145">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="63264-145">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="63264-146">Relações</span><span class="sxs-lookup"><span data-stu-id="63264-146">Relationships</span></span>
<span data-ttu-id="63264-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63264-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63264-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63264-148">JSON Representation</span></span>
<span data-ttu-id="63264-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63264-149">Here is a JSON representation of the resource.</span></span>
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
  "criticalFailuresDeviceCount": 1024,
  "pendingQuickScanDeviceCount": 1024
}
```



