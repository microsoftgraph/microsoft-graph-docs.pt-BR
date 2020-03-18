---
title: tipo de recurso Windowsprotectionstate foi
description: Entidade de status de proteção de dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d42efcc04a060d9585c8d02d17d72449ae0a9c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783596"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="59d9b-103">tipo de recurso Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="59d9b-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="59d9b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59d9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59d9b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59d9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59d9b-106">Entidade de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59d9b-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="59d9b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="59d9b-107">Methods</span></span>
|<span data-ttu-id="59d9b-108">Método</span><span class="sxs-lookup"><span data-stu-id="59d9b-108">Method</span></span>|<span data-ttu-id="59d9b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="59d9b-109">Return Type</span></span>|<span data-ttu-id="59d9b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d9b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59d9b-111">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="59d9b-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="59d9b-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="59d9b-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="59d9b-113">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="59d9b-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="59d9b-114">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="59d9b-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="59d9b-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="59d9b-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="59d9b-116">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="59d9b-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59d9b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59d9b-117">Properties</span></span>
|<span data-ttu-id="59d9b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59d9b-118">Property</span></span>|<span data-ttu-id="59d9b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="59d9b-119">Type</span></span>|<span data-ttu-id="59d9b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d9b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59d9b-121">id</span><span class="sxs-lookup"><span data-stu-id="59d9b-121">id</span></span>|<span data-ttu-id="59d9b-122">String</span><span class="sxs-lookup"><span data-stu-id="59d9b-122">String</span></span>|<span data-ttu-id="59d9b-123">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59d9b-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="59d9b-124">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="59d9b-124">This is device id of the device</span></span>|
|<span data-ttu-id="59d9b-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="59d9b-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="59d9b-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d9b-126">Boolean</span></span>|<span data-ttu-id="59d9b-127">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="59d9b-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="59d9b-128">DeviceState</span><span class="sxs-lookup"><span data-stu-id="59d9b-128">deviceState</span></span>|[<span data-ttu-id="59d9b-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="59d9b-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="59d9b-130">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="59d9b-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="59d9b-131">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="59d9b-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="59d9b-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="59d9b-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="59d9b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d9b-133">Boolean</span></span>|<span data-ttu-id="59d9b-134">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="59d9b-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="59d9b-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="59d9b-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="59d9b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d9b-136">Boolean</span></span>|<span data-ttu-id="59d9b-137">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="59d9b-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="59d9b-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="59d9b-138">quickScanOverdue</span></span>|<span data-ttu-id="59d9b-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d9b-139">Boolean</span></span>|<span data-ttu-id="59d9b-140">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="59d9b-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="59d9b-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="59d9b-141">fullScanOverdue</span></span>|<span data-ttu-id="59d9b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d9b-142">Boolean</span></span>|<span data-ttu-id="59d9b-143">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="59d9b-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="59d9b-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="59d9b-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="59d9b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d9b-145">Boolean</span></span>|<span data-ttu-id="59d9b-146">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="59d9b-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="59d9b-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="59d9b-147">rebootRequired</span></span>|<span data-ttu-id="59d9b-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d9b-148">Boolean</span></span>|<span data-ttu-id="59d9b-149">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="59d9b-149">Reboot required or not?</span></span>|
|<span data-ttu-id="59d9b-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="59d9b-150">fullScanRequired</span></span>|<span data-ttu-id="59d9b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d9b-151">Boolean</span></span>|<span data-ttu-id="59d9b-152">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="59d9b-152">Full scan required or not?</span></span>|
|<span data-ttu-id="59d9b-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="59d9b-153">engineVersion</span></span>|<span data-ttu-id="59d9b-154">String</span><span class="sxs-lookup"><span data-stu-id="59d9b-154">String</span></span>|<span data-ttu-id="59d9b-155">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="59d9b-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="59d9b-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="59d9b-156">signatureVersion</span></span>|<span data-ttu-id="59d9b-157">String</span><span class="sxs-lookup"><span data-stu-id="59d9b-157">String</span></span>|<span data-ttu-id="59d9b-158">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="59d9b-158">Current malware definitions version</span></span>|
|<span data-ttu-id="59d9b-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="59d9b-159">antiMalwareVersion</span></span>|<span data-ttu-id="59d9b-160">String</span><span class="sxs-lookup"><span data-stu-id="59d9b-160">String</span></span>|<span data-ttu-id="59d9b-161">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="59d9b-161">Current anti malware version</span></span>|
|<span data-ttu-id="59d9b-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="59d9b-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="59d9b-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59d9b-163">DateTimeOffset</span></span>|<span data-ttu-id="59d9b-164">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="59d9b-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="59d9b-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="59d9b-165">lastFullScanDateTime</span></span>|<span data-ttu-id="59d9b-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59d9b-166">DateTimeOffset</span></span>|<span data-ttu-id="59d9b-167">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="59d9b-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="59d9b-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="59d9b-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="59d9b-169">String</span><span class="sxs-lookup"><span data-stu-id="59d9b-169">String</span></span>|<span data-ttu-id="59d9b-170">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="59d9b-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="59d9b-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="59d9b-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="59d9b-172">String</span><span class="sxs-lookup"><span data-stu-id="59d9b-172">String</span></span>|<span data-ttu-id="59d9b-173">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="59d9b-173">Last full scan signature version</span></span>|
|<span data-ttu-id="59d9b-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="59d9b-174">lastReportedDateTime</span></span>|<span data-ttu-id="59d9b-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59d9b-175">DateTimeOffset</span></span>|<span data-ttu-id="59d9b-176">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="59d9b-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="59d9b-177">Relações</span><span class="sxs-lookup"><span data-stu-id="59d9b-177">Relationships</span></span>
|<span data-ttu-id="59d9b-178">Relação</span><span class="sxs-lookup"><span data-stu-id="59d9b-178">Relationship</span></span>|<span data-ttu-id="59d9b-179">Tipo</span><span class="sxs-lookup"><span data-stu-id="59d9b-179">Type</span></span>|<span data-ttu-id="59d9b-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d9b-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59d9b-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="59d9b-181">detectedMalwareState</span></span>|<span data-ttu-id="59d9b-182">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="59d9b-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="59d9b-183">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="59d9b-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59d9b-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59d9b-184">JSON Representation</span></span>
<span data-ttu-id="59d9b-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59d9b-185">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```



