---
title: tipo de recurso Windowsprotectionstate foi
description: Entidade de status de proteção de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 00a04fe2f20270cdd0892829406fdccb240989ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080457"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="e0add-103">tipo de recurso Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="e0add-103">windowsProtectionState resource type</span></span>

<span data-ttu-id="e0add-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0add-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0add-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0add-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0add-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0add-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0add-107">Entidade de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0add-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="e0add-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e0add-108">Methods</span></span>
|<span data-ttu-id="e0add-109">Método</span><span class="sxs-lookup"><span data-stu-id="e0add-109">Method</span></span>|<span data-ttu-id="e0add-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e0add-110">Return Type</span></span>|<span data-ttu-id="e0add-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0add-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0add-112">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="e0add-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="e0add-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e0add-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="e0add-114">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="e0add-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="e0add-115">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="e0add-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="e0add-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="e0add-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="e0add-117">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="e0add-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0add-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0add-118">Properties</span></span>
|<span data-ttu-id="e0add-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0add-119">Property</span></span>|<span data-ttu-id="e0add-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0add-120">Type</span></span>|<span data-ttu-id="e0add-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0add-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0add-122">id</span><span class="sxs-lookup"><span data-stu-id="e0add-122">id</span></span>|<span data-ttu-id="e0add-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0add-123">String</span></span>|<span data-ttu-id="e0add-124">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0add-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="e0add-125">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e0add-125">This is device id of the device</span></span>|
|<span data-ttu-id="e0add-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e0add-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="e0add-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0add-127">Boolean</span></span>|<span data-ttu-id="e0add-128">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="e0add-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="e0add-129">DeviceState</span><span class="sxs-lookup"><span data-stu-id="e0add-129">deviceState</span></span>|[<span data-ttu-id="e0add-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="e0add-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="e0add-131">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="e0add-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="e0add-132">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="e0add-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="e0add-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e0add-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="e0add-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0add-134">Boolean</span></span>|<span data-ttu-id="e0add-135">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="e0add-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="e0add-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="e0add-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="e0add-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0add-137">Boolean</span></span>|<span data-ttu-id="e0add-138">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="e0add-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="e0add-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="e0add-139">quickScanOverdue</span></span>|<span data-ttu-id="e0add-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0add-140">Boolean</span></span>|<span data-ttu-id="e0add-141">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="e0add-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="e0add-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="e0add-142">fullScanOverdue</span></span>|<span data-ttu-id="e0add-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0add-143">Boolean</span></span>|<span data-ttu-id="e0add-144">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="e0add-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="e0add-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="e0add-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="e0add-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0add-146">Boolean</span></span>|<span data-ttu-id="e0add-147">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="e0add-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="e0add-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="e0add-148">rebootRequired</span></span>|<span data-ttu-id="e0add-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0add-149">Boolean</span></span>|<span data-ttu-id="e0add-150">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="e0add-150">Reboot required or not?</span></span>|
|<span data-ttu-id="e0add-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="e0add-151">fullScanRequired</span></span>|<span data-ttu-id="e0add-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0add-152">Boolean</span></span>|<span data-ttu-id="e0add-153">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="e0add-153">Full scan required or not?</span></span>|
|<span data-ttu-id="e0add-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="e0add-154">engineVersion</span></span>|<span data-ttu-id="e0add-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0add-155">String</span></span>|<span data-ttu-id="e0add-156">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="e0add-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="e0add-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="e0add-157">signatureVersion</span></span>|<span data-ttu-id="e0add-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0add-158">String</span></span>|<span data-ttu-id="e0add-159">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="e0add-159">Current malware definitions version</span></span>|
|<span data-ttu-id="e0add-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="e0add-160">antiMalwareVersion</span></span>|<span data-ttu-id="e0add-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0add-161">String</span></span>|<span data-ttu-id="e0add-162">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="e0add-162">Current anti malware version</span></span>|
|<span data-ttu-id="e0add-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="e0add-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="e0add-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0add-164">DateTimeOffset</span></span>|<span data-ttu-id="e0add-165">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="e0add-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="e0add-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="e0add-166">lastFullScanDateTime</span></span>|<span data-ttu-id="e0add-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0add-167">DateTimeOffset</span></span>|<span data-ttu-id="e0add-168">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="e0add-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="e0add-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="e0add-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="e0add-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0add-170">String</span></span>|<span data-ttu-id="e0add-171">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="e0add-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="e0add-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="e0add-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="e0add-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0add-173">String</span></span>|<span data-ttu-id="e0add-174">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="e0add-174">Last full scan signature version</span></span>|
|<span data-ttu-id="e0add-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0add-175">lastReportedDateTime</span></span>|<span data-ttu-id="e0add-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0add-176">DateTimeOffset</span></span>|<span data-ttu-id="e0add-177">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="e0add-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0add-178">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="e0add-178">Relationships</span></span>
|<span data-ttu-id="e0add-179">Relação</span><span class="sxs-lookup"><span data-stu-id="e0add-179">Relationship</span></span>|<span data-ttu-id="e0add-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0add-180">Type</span></span>|<span data-ttu-id="e0add-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0add-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0add-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="e0add-182">detectedMalwareState</span></span>|<span data-ttu-id="e0add-183">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="e0add-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="e0add-184">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e0add-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0add-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0add-185">JSON Representation</span></span>
<span data-ttu-id="e0add-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0add-186">Here is a JSON representation of the resource.</span></span>
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






