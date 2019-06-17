---
title: tipo de recurso deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1c721039df8b4c656e84a91da76be60dcdd25cf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995221"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="8581c-103">tipo de recurso deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="8581c-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="8581c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8581c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8581c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8581c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8581c-106">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8581c-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="8581c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8581c-107">Properties</span></span>
|<span data-ttu-id="8581c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8581c-108">Property</span></span>|<span data-ttu-id="8581c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8581c-109">Type</span></span>|<span data-ttu-id="8581c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8581c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8581c-111">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="8581c-112">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-112">Int32</span></span>|<span data-ttu-id="8581c-113">Contagem total de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8581c-113">Total device count.</span></span>|
|<span data-ttu-id="8581c-114">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="8581c-115">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-115">Int32</span></span>|<span data-ttu-id="8581c-116">Dispositivo com contagem inativa de agente de ameaça</span><span class="sxs-lookup"><span data-stu-id="8581c-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="8581c-117">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="8581c-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-118">Int32</span></span>|<span data-ttu-id="8581c-119">Dispositivo com o estado do agente de ameaça como contagem desconhecida.</span><span class="sxs-lookup"><span data-stu-id="8581c-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="8581c-120">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="8581c-121">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-121">Int32</span></span>|<span data-ttu-id="8581c-122">Dispositivo com a contagem de assinatura antiga.</span><span class="sxs-lookup"><span data-stu-id="8581c-122">Device with old signature count.</span></span>|
|<span data-ttu-id="8581c-123">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-123">cleanDeviceCount</span></span>|<span data-ttu-id="8581c-124">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-124">Int32</span></span>|<span data-ttu-id="8581c-125">Limpar contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8581c-125">Clean device count.</span></span>|
|<span data-ttu-id="8581c-126">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="8581c-127">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-127">Int32</span></span>|<span data-ttu-id="8581c-128">Contagem de dispositivos de verificação completa pendente.</span><span class="sxs-lookup"><span data-stu-id="8581c-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="8581c-129">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="8581c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-130">Int32</span></span>|<span data-ttu-id="8581c-131">Contagem de dispositivos de reinicialização pendente.</span><span class="sxs-lookup"><span data-stu-id="8581c-131">Pending restart device count.</span></span>|
|<span data-ttu-id="8581c-132">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="8581c-133">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-133">Int32</span></span>|<span data-ttu-id="8581c-134">Contagem de dispositivos de etapas manuais pendentes.</span><span class="sxs-lookup"><span data-stu-id="8581c-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="8581c-135">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="8581c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-136">Int32</span></span>|<span data-ttu-id="8581c-137">Contagem de dispositivos de verificação offline pendente.</span><span class="sxs-lookup"><span data-stu-id="8581c-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="8581c-138">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8581c-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="8581c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8581c-139">Int32</span></span>|<span data-ttu-id="8581c-140">Contagem de dispositivos de falhas críticas.</span><span class="sxs-lookup"><span data-stu-id="8581c-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8581c-141">Relações</span><span class="sxs-lookup"><span data-stu-id="8581c-141">Relationships</span></span>
<span data-ttu-id="8581c-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8581c-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8581c-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8581c-143">JSON Representation</span></span>
<span data-ttu-id="8581c-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8581c-144">Here is a JSON representation of the resource.</span></span>
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





