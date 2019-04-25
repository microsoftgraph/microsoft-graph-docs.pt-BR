---
title: tipo de recurso Windowsprotectionstate foi
description: Entidade de status de proteção de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ecdc3ab743502ff4aef78fa8923248399ce16f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520078"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="74cf3-103">tipo de recurso Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="74cf3-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="74cf3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74cf3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74cf3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74cf3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74cf3-106">Entidade de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74cf3-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="74cf3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="74cf3-107">Methods</span></span>
|<span data-ttu-id="74cf3-108">Método</span><span class="sxs-lookup"><span data-stu-id="74cf3-108">Method</span></span>|<span data-ttu-id="74cf3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74cf3-109">Return Type</span></span>|<span data-ttu-id="74cf3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="74cf3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74cf3-111">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="74cf3-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="74cf3-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="74cf3-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="74cf3-113">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="74cf3-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="74cf3-114">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="74cf3-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="74cf3-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="74cf3-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="74cf3-116">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="74cf3-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74cf3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74cf3-117">Properties</span></span>
|<span data-ttu-id="74cf3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74cf3-118">Property</span></span>|<span data-ttu-id="74cf3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="74cf3-119">Type</span></span>|<span data-ttu-id="74cf3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="74cf3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74cf3-121">id</span><span class="sxs-lookup"><span data-stu-id="74cf3-121">id</span></span>|<span data-ttu-id="74cf3-122">String</span><span class="sxs-lookup"><span data-stu-id="74cf3-122">String</span></span>|<span data-ttu-id="74cf3-123">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74cf3-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="74cf3-124">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74cf3-124">This is device id of the device</span></span>|
|<span data-ttu-id="74cf3-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="74cf3-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="74cf3-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="74cf3-126">Boolean</span></span>|<span data-ttu-id="74cf3-127">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="74cf3-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="74cf3-128">DeviceState</span><span class="sxs-lookup"><span data-stu-id="74cf3-128">deviceState</span></span>|[<span data-ttu-id="74cf3-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="74cf3-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="74cf3-130">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="74cf3-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="74cf3-131">Os valores possíveis são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="74cf3-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="74cf3-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="74cf3-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="74cf3-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="74cf3-133">Boolean</span></span>|<span data-ttu-id="74cf3-134">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="74cf3-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="74cf3-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="74cf3-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="74cf3-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="74cf3-136">Boolean</span></span>|<span data-ttu-id="74cf3-137">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="74cf3-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="74cf3-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="74cf3-138">quickScanOverdue</span></span>|<span data-ttu-id="74cf3-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="74cf3-139">Boolean</span></span>|<span data-ttu-id="74cf3-140">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="74cf3-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="74cf3-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="74cf3-141">fullScanOverdue</span></span>|<span data-ttu-id="74cf3-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="74cf3-142">Boolean</span></span>|<span data-ttu-id="74cf3-143">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="74cf3-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="74cf3-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="74cf3-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="74cf3-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="74cf3-145">Boolean</span></span>|<span data-ttu-id="74cf3-146">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="74cf3-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="74cf3-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="74cf3-147">rebootRequired</span></span>|<span data-ttu-id="74cf3-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="74cf3-148">Boolean</span></span>|<span data-ttu-id="74cf3-149">ReInicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="74cf3-149">Reboot required or not?</span></span>|
|<span data-ttu-id="74cf3-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="74cf3-150">fullScanRequired</span></span>|<span data-ttu-id="74cf3-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="74cf3-151">Boolean</span></span>|<span data-ttu-id="74cf3-152">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="74cf3-152">Full scan required or not?</span></span>|
|<span data-ttu-id="74cf3-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="74cf3-153">engineVersion</span></span>|<span data-ttu-id="74cf3-154">String</span><span class="sxs-lookup"><span data-stu-id="74cf3-154">String</span></span>|<span data-ttu-id="74cf3-155">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="74cf3-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="74cf3-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="74cf3-156">signatureVersion</span></span>|<span data-ttu-id="74cf3-157">String</span><span class="sxs-lookup"><span data-stu-id="74cf3-157">String</span></span>|<span data-ttu-id="74cf3-158">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="74cf3-158">Current malware definitions version</span></span>|
|<span data-ttu-id="74cf3-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="74cf3-159">antiMalwareVersion</span></span>|<span data-ttu-id="74cf3-160">String</span><span class="sxs-lookup"><span data-stu-id="74cf3-160">String</span></span>|<span data-ttu-id="74cf3-161">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="74cf3-161">Current anti malware version</span></span>|
|<span data-ttu-id="74cf3-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="74cf3-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="74cf3-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74cf3-163">DateTimeOffset</span></span>|<span data-ttu-id="74cf3-164">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="74cf3-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="74cf3-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="74cf3-165">lastFullScanDateTime</span></span>|<span data-ttu-id="74cf3-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74cf3-166">DateTimeOffset</span></span>|<span data-ttu-id="74cf3-167">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="74cf3-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="74cf3-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="74cf3-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="74cf3-169">String</span><span class="sxs-lookup"><span data-stu-id="74cf3-169">String</span></span>|<span data-ttu-id="74cf3-170">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="74cf3-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="74cf3-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="74cf3-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="74cf3-172">String</span><span class="sxs-lookup"><span data-stu-id="74cf3-172">String</span></span>|<span data-ttu-id="74cf3-173">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="74cf3-173">Last full scan signature version</span></span>|
|<span data-ttu-id="74cf3-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="74cf3-174">lastReportedDateTime</span></span>|<span data-ttu-id="74cf3-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74cf3-175">DateTimeOffset</span></span>|<span data-ttu-id="74cf3-176">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="74cf3-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="74cf3-177">Relações</span><span class="sxs-lookup"><span data-stu-id="74cf3-177">Relationships</span></span>
|<span data-ttu-id="74cf3-178">Relação</span><span class="sxs-lookup"><span data-stu-id="74cf3-178">Relationship</span></span>|<span data-ttu-id="74cf3-179">Tipo</span><span class="sxs-lookup"><span data-stu-id="74cf3-179">Type</span></span>|<span data-ttu-id="74cf3-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="74cf3-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74cf3-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="74cf3-181">detectedMalwareState</span></span>|<span data-ttu-id="74cf3-182">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="74cf3-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="74cf3-183">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74cf3-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74cf3-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74cf3-184">JSON Representation</span></span>
<span data-ttu-id="74cf3-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74cf3-185">Here is a JSON representation of the resource.</span></span>
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





