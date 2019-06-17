---
title: tipo de recurso Windowsprotectionstate foi
description: Entidade de status de proteção de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd507daef4d9055dcabce1e90481e22a77ec8180
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983915"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="a9f43-103">tipo de recurso Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="a9f43-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="a9f43-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9f43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f43-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9f43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f43-106">Entidade de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9f43-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="a9f43-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a9f43-107">Methods</span></span>
|<span data-ttu-id="a9f43-108">Método</span><span class="sxs-lookup"><span data-stu-id="a9f43-108">Method</span></span>|<span data-ttu-id="a9f43-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a9f43-109">Return Type</span></span>|<span data-ttu-id="a9f43-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9f43-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a9f43-111">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="a9f43-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="a9f43-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a9f43-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="a9f43-113">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a9f43-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="a9f43-114">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="a9f43-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="a9f43-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a9f43-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="a9f43-116">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a9f43-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a9f43-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9f43-117">Properties</span></span>
|<span data-ttu-id="a9f43-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9f43-118">Property</span></span>|<span data-ttu-id="a9f43-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9f43-119">Type</span></span>|<span data-ttu-id="a9f43-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9f43-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f43-121">id</span><span class="sxs-lookup"><span data-stu-id="a9f43-121">id</span></span>|<span data-ttu-id="a9f43-122">String</span><span class="sxs-lookup"><span data-stu-id="a9f43-122">String</span></span>|<span data-ttu-id="a9f43-123">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9f43-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="a9f43-124">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a9f43-124">This is device id of the device</span></span>|
|<span data-ttu-id="a9f43-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a9f43-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="a9f43-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9f43-126">Boolean</span></span>|<span data-ttu-id="a9f43-127">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="a9f43-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="a9f43-128">DeviceState</span><span class="sxs-lookup"><span data-stu-id="a9f43-128">deviceState</span></span>|[<span data-ttu-id="a9f43-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="a9f43-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="a9f43-130">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="a9f43-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="a9f43-131">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="a9f43-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="a9f43-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a9f43-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="a9f43-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9f43-133">Boolean</span></span>|<span data-ttu-id="a9f43-134">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="a9f43-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="a9f43-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="a9f43-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="a9f43-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9f43-136">Boolean</span></span>|<span data-ttu-id="a9f43-137">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="a9f43-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="a9f43-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a9f43-138">quickScanOverdue</span></span>|<span data-ttu-id="a9f43-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9f43-139">Boolean</span></span>|<span data-ttu-id="a9f43-140">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="a9f43-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="a9f43-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a9f43-141">fullScanOverdue</span></span>|<span data-ttu-id="a9f43-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9f43-142">Boolean</span></span>|<span data-ttu-id="a9f43-143">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="a9f43-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="a9f43-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="a9f43-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="a9f43-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9f43-145">Boolean</span></span>|<span data-ttu-id="a9f43-146">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="a9f43-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="a9f43-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="a9f43-147">rebootRequired</span></span>|<span data-ttu-id="a9f43-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9f43-148">Boolean</span></span>|<span data-ttu-id="a9f43-149">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="a9f43-149">Reboot required or not?</span></span>|
|<span data-ttu-id="a9f43-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="a9f43-150">fullScanRequired</span></span>|<span data-ttu-id="a9f43-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9f43-151">Boolean</span></span>|<span data-ttu-id="a9f43-152">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="a9f43-152">Full scan required or not?</span></span>|
|<span data-ttu-id="a9f43-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="a9f43-153">engineVersion</span></span>|<span data-ttu-id="a9f43-154">String</span><span class="sxs-lookup"><span data-stu-id="a9f43-154">String</span></span>|<span data-ttu-id="a9f43-155">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="a9f43-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="a9f43-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="a9f43-156">signatureVersion</span></span>|<span data-ttu-id="a9f43-157">String</span><span class="sxs-lookup"><span data-stu-id="a9f43-157">String</span></span>|<span data-ttu-id="a9f43-158">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="a9f43-158">Current malware definitions version</span></span>|
|<span data-ttu-id="a9f43-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="a9f43-159">antiMalwareVersion</span></span>|<span data-ttu-id="a9f43-160">String</span><span class="sxs-lookup"><span data-stu-id="a9f43-160">String</span></span>|<span data-ttu-id="a9f43-161">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="a9f43-161">Current anti malware version</span></span>|
|<span data-ttu-id="a9f43-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f43-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="a9f43-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f43-163">DateTimeOffset</span></span>|<span data-ttu-id="a9f43-164">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a9f43-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="a9f43-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f43-165">lastFullScanDateTime</span></span>|<span data-ttu-id="a9f43-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f43-166">DateTimeOffset</span></span>|<span data-ttu-id="a9f43-167">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a9f43-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="a9f43-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a9f43-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="a9f43-169">String</span><span class="sxs-lookup"><span data-stu-id="a9f43-169">String</span></span>|<span data-ttu-id="a9f43-170">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a9f43-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="a9f43-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a9f43-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="a9f43-172">String</span><span class="sxs-lookup"><span data-stu-id="a9f43-172">String</span></span>|<span data-ttu-id="a9f43-173">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="a9f43-173">Last full scan signature version</span></span>|
|<span data-ttu-id="a9f43-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f43-174">lastReportedDateTime</span></span>|<span data-ttu-id="a9f43-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f43-175">DateTimeOffset</span></span>|<span data-ttu-id="a9f43-176">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="a9f43-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9f43-177">Relações</span><span class="sxs-lookup"><span data-stu-id="a9f43-177">Relationships</span></span>
|<span data-ttu-id="a9f43-178">Relação</span><span class="sxs-lookup"><span data-stu-id="a9f43-178">Relationship</span></span>|<span data-ttu-id="a9f43-179">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9f43-179">Type</span></span>|<span data-ttu-id="a9f43-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9f43-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f43-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="a9f43-181">detectedMalwareState</span></span>|<span data-ttu-id="a9f43-182">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="a9f43-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="a9f43-183">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a9f43-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9f43-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9f43-184">JSON Representation</span></span>
<span data-ttu-id="a9f43-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9f43-185">Here is a JSON representation of the resource.</span></span>
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





