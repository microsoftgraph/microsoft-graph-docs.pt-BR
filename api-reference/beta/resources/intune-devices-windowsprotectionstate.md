---
title: tipo de recurso Windowsprotectionstate foi
description: Entidade de status de proteção de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63ac9a9e5f6dd153238ea2666cf0bffd88ebf9da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731033"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="3f751-103">tipo de recurso Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="3f751-103">windowsProtectionState resource type</span></span>

<span data-ttu-id="3f751-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f751-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f751-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f751-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f751-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f751-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f751-107">Entidade de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f751-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="3f751-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3f751-108">Methods</span></span>
|<span data-ttu-id="3f751-109">Método</span><span class="sxs-lookup"><span data-stu-id="3f751-109">Method</span></span>|<span data-ttu-id="3f751-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3f751-110">Return Type</span></span>|<span data-ttu-id="3f751-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f751-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f751-112">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="3f751-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="3f751-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="3f751-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="3f751-114">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="3f751-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="3f751-115">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="3f751-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="3f751-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="3f751-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="3f751-117">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="3f751-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f751-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f751-118">Properties</span></span>
|<span data-ttu-id="3f751-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f751-119">Property</span></span>|<span data-ttu-id="3f751-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f751-120">Type</span></span>|<span data-ttu-id="3f751-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f751-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f751-122">id</span><span class="sxs-lookup"><span data-stu-id="3f751-122">id</span></span>|<span data-ttu-id="3f751-123">String</span><span class="sxs-lookup"><span data-stu-id="3f751-123">String</span></span>|<span data-ttu-id="3f751-124">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f751-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="3f751-125">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3f751-125">This is device id of the device</span></span>|
|<span data-ttu-id="3f751-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3f751-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="3f751-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f751-127">Boolean</span></span>|<span data-ttu-id="3f751-128">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="3f751-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="3f751-129">DeviceState</span><span class="sxs-lookup"><span data-stu-id="3f751-129">deviceState</span></span>|[<span data-ttu-id="3f751-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="3f751-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="3f751-131">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="3f751-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="3f751-132">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="3f751-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="3f751-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3f751-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="3f751-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f751-134">Boolean</span></span>|<span data-ttu-id="3f751-135">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="3f751-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="3f751-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="3f751-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="3f751-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f751-137">Boolean</span></span>|<span data-ttu-id="3f751-138">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="3f751-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="3f751-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="3f751-139">quickScanOverdue</span></span>|<span data-ttu-id="3f751-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f751-140">Boolean</span></span>|<span data-ttu-id="3f751-141">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="3f751-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="3f751-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="3f751-142">fullScanOverdue</span></span>|<span data-ttu-id="3f751-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f751-143">Boolean</span></span>|<span data-ttu-id="3f751-144">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="3f751-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="3f751-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="3f751-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="3f751-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f751-146">Boolean</span></span>|<span data-ttu-id="3f751-147">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="3f751-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="3f751-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="3f751-148">rebootRequired</span></span>|<span data-ttu-id="3f751-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f751-149">Boolean</span></span>|<span data-ttu-id="3f751-150">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="3f751-150">Reboot required or not?</span></span>|
|<span data-ttu-id="3f751-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="3f751-151">fullScanRequired</span></span>|<span data-ttu-id="3f751-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f751-152">Boolean</span></span>|<span data-ttu-id="3f751-153">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="3f751-153">Full scan required or not?</span></span>|
|<span data-ttu-id="3f751-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="3f751-154">engineVersion</span></span>|<span data-ttu-id="3f751-155">String</span><span class="sxs-lookup"><span data-stu-id="3f751-155">String</span></span>|<span data-ttu-id="3f751-156">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="3f751-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="3f751-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="3f751-157">signatureVersion</span></span>|<span data-ttu-id="3f751-158">String</span><span class="sxs-lookup"><span data-stu-id="3f751-158">String</span></span>|<span data-ttu-id="3f751-159">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="3f751-159">Current malware definitions version</span></span>|
|<span data-ttu-id="3f751-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="3f751-160">antiMalwareVersion</span></span>|<span data-ttu-id="3f751-161">String</span><span class="sxs-lookup"><span data-stu-id="3f751-161">String</span></span>|<span data-ttu-id="3f751-162">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="3f751-162">Current anti malware version</span></span>|
|<span data-ttu-id="3f751-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3f751-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="3f751-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f751-164">DateTimeOffset</span></span>|<span data-ttu-id="3f751-165">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3f751-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="3f751-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3f751-166">lastFullScanDateTime</span></span>|<span data-ttu-id="3f751-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f751-167">DateTimeOffset</span></span>|<span data-ttu-id="3f751-168">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3f751-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="3f751-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="3f751-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="3f751-170">String</span><span class="sxs-lookup"><span data-stu-id="3f751-170">String</span></span>|<span data-ttu-id="3f751-171">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3f751-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="3f751-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="3f751-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="3f751-173">String</span><span class="sxs-lookup"><span data-stu-id="3f751-173">String</span></span>|<span data-ttu-id="3f751-174">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="3f751-174">Last full scan signature version</span></span>|
|<span data-ttu-id="3f751-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f751-175">lastReportedDateTime</span></span>|<span data-ttu-id="3f751-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f751-176">DateTimeOffset</span></span>|<span data-ttu-id="3f751-177">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="3f751-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f751-178">Relações</span><span class="sxs-lookup"><span data-stu-id="3f751-178">Relationships</span></span>
|<span data-ttu-id="3f751-179">Relação</span><span class="sxs-lookup"><span data-stu-id="3f751-179">Relationship</span></span>|<span data-ttu-id="3f751-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f751-180">Type</span></span>|<span data-ttu-id="3f751-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f751-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f751-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="3f751-182">detectedMalwareState</span></span>|<span data-ttu-id="3f751-183">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="3f751-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="3f751-184">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3f751-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f751-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f751-185">JSON Representation</span></span>
<span data-ttu-id="3f751-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f751-186">Here is a JSON representation of the resource.</span></span>
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





