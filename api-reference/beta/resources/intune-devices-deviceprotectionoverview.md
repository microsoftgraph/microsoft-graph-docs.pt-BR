---
title: tipo de recurso deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e9bdadb7cef003a8d22653660d516afe8357d59
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784137"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="44cf4-103">tipo de recurso deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="44cf4-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="44cf4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44cf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44cf4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44cf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44cf4-106">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44cf4-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="44cf4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44cf4-107">Properties</span></span>
|<span data-ttu-id="44cf4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44cf4-108">Property</span></span>|<span data-ttu-id="44cf4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="44cf4-109">Type</span></span>|<span data-ttu-id="44cf4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="44cf4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44cf4-111">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="44cf4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-112">Int32</span></span>|<span data-ttu-id="44cf4-113">Contagem total de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="44cf4-113">Total device count.</span></span>|
|<span data-ttu-id="44cf4-114">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="44cf4-115">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-115">Int32</span></span>|<span data-ttu-id="44cf4-116">Dispositivo com contagem inativa de agente de ameaça</span><span class="sxs-lookup"><span data-stu-id="44cf4-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="44cf4-117">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="44cf4-118">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-118">Int32</span></span>|<span data-ttu-id="44cf4-119">Dispositivo com o estado do agente de ameaça como contagem desconhecida.</span><span class="sxs-lookup"><span data-stu-id="44cf4-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="44cf4-120">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="44cf4-121">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-121">Int32</span></span>|<span data-ttu-id="44cf4-122">Dispositivo com a contagem de assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="44cf4-122">Device with old signature count.</span></span>|
|<span data-ttu-id="44cf4-123">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-123">cleanDeviceCount</span></span>|<span data-ttu-id="44cf4-124">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-124">Int32</span></span>|<span data-ttu-id="44cf4-125">Limpar contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="44cf4-125">Clean device count.</span></span>|
|<span data-ttu-id="44cf4-126">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="44cf4-127">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-127">Int32</span></span>|<span data-ttu-id="44cf4-128">Contagem de dispositivos de verificação completa pendente.</span><span class="sxs-lookup"><span data-stu-id="44cf4-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="44cf4-129">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="44cf4-130">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-130">Int32</span></span>|<span data-ttu-id="44cf4-131">Contagem de dispositivos de reinicialização pendente.</span><span class="sxs-lookup"><span data-stu-id="44cf4-131">Pending restart device count.</span></span>|
|<span data-ttu-id="44cf4-132">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="44cf4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-133">Int32</span></span>|<span data-ttu-id="44cf4-134">Contagem de dispositivos de etapas manuais pendentes.</span><span class="sxs-lookup"><span data-stu-id="44cf4-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="44cf4-135">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="44cf4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-136">Int32</span></span>|<span data-ttu-id="44cf4-137">Contagem de dispositivos de verificação offline pendente.</span><span class="sxs-lookup"><span data-stu-id="44cf4-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="44cf4-138">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44cf4-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="44cf4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="44cf4-139">Int32</span></span>|<span data-ttu-id="44cf4-140">Contagem de dispositivos de falhas críticas.</span><span class="sxs-lookup"><span data-stu-id="44cf4-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44cf4-141">Relações</span><span class="sxs-lookup"><span data-stu-id="44cf4-141">Relationships</span></span>
<span data-ttu-id="44cf4-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44cf4-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44cf4-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44cf4-143">JSON Representation</span></span>
<span data-ttu-id="44cf4-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44cf4-144">Here is a JSON representation of the resource.</span></span>
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



