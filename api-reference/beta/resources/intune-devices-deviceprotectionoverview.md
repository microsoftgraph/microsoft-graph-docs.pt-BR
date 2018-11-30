---
title: tipo de recurso de deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
ms.openlocfilehash: 81252fdf60c1de129a615b075968e0e6f1eca943
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038480"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="ed924-103">tipo de recurso de deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="ed924-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="ed924-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed924-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed924-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed924-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed924-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed924-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed924-107">Informações de hardware de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed924-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="ed924-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed924-108">Properties</span></span>
|<span data-ttu-id="ed924-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed924-109">Property</span></span>|<span data-ttu-id="ed924-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed924-110">Type</span></span>|<span data-ttu-id="ed924-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed924-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed924-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="ed924-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-113">Int32</span></span>|<span data-ttu-id="ed924-114">Contagem total de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed924-114">Total device count.</span></span>|
|<span data-ttu-id="ed924-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="ed924-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-116">Int32</span></span>|<span data-ttu-id="ed924-117">Dispositivo com contagem de agente de ameaça inativa</span><span class="sxs-lookup"><span data-stu-id="ed924-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="ed924-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="ed924-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-119">Int32</span></span>|<span data-ttu-id="ed924-120">Dispositivo com o estado de agente de ameaça como contagem desconhecido.</span><span class="sxs-lookup"><span data-stu-id="ed924-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="ed924-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="ed924-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-122">Int32</span></span>|<span data-ttu-id="ed924-123">Dispositivo com a contagem de assinatura antigo.</span><span class="sxs-lookup"><span data-stu-id="ed924-123">Device with old signature count.</span></span>|
|<span data-ttu-id="ed924-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-124">cleanDeviceCount</span></span>|<span data-ttu-id="ed924-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-125">Int32</span></span>|<span data-ttu-id="ed924-126">Limpar a contagem do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed924-126">Clean device count.</span></span>|
|<span data-ttu-id="ed924-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="ed924-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-128">Int32</span></span>|<span data-ttu-id="ed924-129">Contagem de dispositivo pendentes verificação completa.</span><span class="sxs-lookup"><span data-stu-id="ed924-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="ed924-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="ed924-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-131">Int32</span></span>|<span data-ttu-id="ed924-132">Contagem de reinicialização pendente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed924-132">Pending restart device count.</span></span>|
|<span data-ttu-id="ed924-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="ed924-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-134">Int32</span></span>|<span data-ttu-id="ed924-135">Contagem de dispositivo pendentes etapas manuais.</span><span class="sxs-lookup"><span data-stu-id="ed924-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="ed924-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="ed924-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-137">Int32</span></span>|<span data-ttu-id="ed924-138">Contagem de dispositivo pendentes verificação offline.</span><span class="sxs-lookup"><span data-stu-id="ed924-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="ed924-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed924-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="ed924-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ed924-140">Int32</span></span>|<span data-ttu-id="ed924-141">Contagem de falhas críticas do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed924-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed924-142">Relações</span><span class="sxs-lookup"><span data-stu-id="ed924-142">Relationships</span></span>
<span data-ttu-id="ed924-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed924-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed924-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed924-144">JSON Representation</span></span>
<span data-ttu-id="ed924-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed924-145">Here is a JSON representation of the resource.</span></span>
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





