---
title: tipo de recurso de deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418985"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="ff39a-103">tipo de recurso de deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="ff39a-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="ff39a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ff39a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff39a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ff39a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff39a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ff39a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff39a-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff39a-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="ff39a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff39a-108">Properties</span></span>
|<span data-ttu-id="ff39a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff39a-109">Property</span></span>|<span data-ttu-id="ff39a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff39a-110">Type</span></span>|<span data-ttu-id="ff39a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff39a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff39a-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="ff39a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-113">Int32</span></span>|<span data-ttu-id="ff39a-114">Contagem total de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff39a-114">Total device count.</span></span>|
|<span data-ttu-id="ff39a-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="ff39a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-116">Int32</span></span>|<span data-ttu-id="ff39a-117">Dispositivo com contagem de agente de ameaça inativa</span><span class="sxs-lookup"><span data-stu-id="ff39a-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="ff39a-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="ff39a-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-119">Int32</span></span>|<span data-ttu-id="ff39a-120">Dispositivo com o estado de agente de ameaça como contagem desconhecido.</span><span class="sxs-lookup"><span data-stu-id="ff39a-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="ff39a-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="ff39a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-122">Int32</span></span>|<span data-ttu-id="ff39a-123">Dispositivo com a contagem de assinatura antigo.</span><span class="sxs-lookup"><span data-stu-id="ff39a-123">Device with old signature count.</span></span>|
|<span data-ttu-id="ff39a-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-124">cleanDeviceCount</span></span>|<span data-ttu-id="ff39a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-125">Int32</span></span>|<span data-ttu-id="ff39a-126">Limpar a contagem do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff39a-126">Clean device count.</span></span>|
|<span data-ttu-id="ff39a-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="ff39a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-128">Int32</span></span>|<span data-ttu-id="ff39a-129">Contagem de dispositivo pendentes verificação completa.</span><span class="sxs-lookup"><span data-stu-id="ff39a-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="ff39a-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="ff39a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-131">Int32</span></span>|<span data-ttu-id="ff39a-132">Contagem de reinicialização pendente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff39a-132">Pending restart device count.</span></span>|
|<span data-ttu-id="ff39a-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="ff39a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-134">Int32</span></span>|<span data-ttu-id="ff39a-135">Contagem de dispositivo pendentes etapas manuais.</span><span class="sxs-lookup"><span data-stu-id="ff39a-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="ff39a-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="ff39a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-137">Int32</span></span>|<span data-ttu-id="ff39a-138">Contagem de dispositivo pendentes verificação offline.</span><span class="sxs-lookup"><span data-stu-id="ff39a-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="ff39a-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff39a-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="ff39a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ff39a-140">Int32</span></span>|<span data-ttu-id="ff39a-141">Contagem de falhas críticas do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff39a-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff39a-142">Relações</span><span class="sxs-lookup"><span data-stu-id="ff39a-142">Relationships</span></span>
<span data-ttu-id="ff39a-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff39a-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff39a-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff39a-144">JSON Representation</span></span>
<span data-ttu-id="ff39a-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff39a-145">Here is a JSON representation of the resource.</span></span>
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




