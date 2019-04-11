---
title: tipo de recurso Windowsprotectionstate foi
description: Entidade de status de proteção de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ecdc3ab743502ff4aef78fa8923248399ce16f4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803098"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="b1945-103">tipo de recurso Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="b1945-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="b1945-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1945-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1945-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1945-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1945-106">Entidade de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1945-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="b1945-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b1945-107">Methods</span></span>
|<span data-ttu-id="b1945-108">Método</span><span class="sxs-lookup"><span data-stu-id="b1945-108">Method</span></span>|<span data-ttu-id="b1945-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b1945-109">Return Type</span></span>|<span data-ttu-id="b1945-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1945-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b1945-111">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="b1945-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="b1945-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="b1945-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="b1945-113">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="b1945-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="b1945-114">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="b1945-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="b1945-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="b1945-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="b1945-116">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="b1945-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1945-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1945-117">Properties</span></span>
|<span data-ttu-id="b1945-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1945-118">Property</span></span>|<span data-ttu-id="b1945-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1945-119">Type</span></span>|<span data-ttu-id="b1945-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1945-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1945-121">id</span><span class="sxs-lookup"><span data-stu-id="b1945-121">id</span></span>|<span data-ttu-id="b1945-122">String</span><span class="sxs-lookup"><span data-stu-id="b1945-122">String</span></span>|<span data-ttu-id="b1945-123">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1945-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="b1945-124">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b1945-124">This is device id of the device</span></span>|
|<span data-ttu-id="b1945-125">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b1945-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="b1945-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1945-126">Boolean</span></span>|<span data-ttu-id="b1945-127">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="b1945-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="b1945-128">DeviceState</span><span class="sxs-lookup"><span data-stu-id="b1945-128">deviceState</span></span>|[<span data-ttu-id="b1945-129">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="b1945-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="b1945-130">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="b1945-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="b1945-131">Os valores possíveis são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="b1945-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="b1945-132">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b1945-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="b1945-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1945-133">Boolean</span></span>|<span data-ttu-id="b1945-134">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="b1945-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="b1945-135">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="b1945-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="b1945-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1945-136">Boolean</span></span>|<span data-ttu-id="b1945-137">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="b1945-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="b1945-138">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="b1945-138">quickScanOverdue</span></span>|<span data-ttu-id="b1945-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1945-139">Boolean</span></span>|<span data-ttu-id="b1945-140">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="b1945-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="b1945-141">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="b1945-141">fullScanOverdue</span></span>|<span data-ttu-id="b1945-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1945-142">Boolean</span></span>|<span data-ttu-id="b1945-143">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="b1945-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="b1945-144">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="b1945-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="b1945-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1945-145">Boolean</span></span>|<span data-ttu-id="b1945-146">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="b1945-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="b1945-147">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="b1945-147">rebootRequired</span></span>|<span data-ttu-id="b1945-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1945-148">Boolean</span></span>|<span data-ttu-id="b1945-149">ReInicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="b1945-149">Reboot required or not?</span></span>|
|<span data-ttu-id="b1945-150">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="b1945-150">fullScanRequired</span></span>|<span data-ttu-id="b1945-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1945-151">Boolean</span></span>|<span data-ttu-id="b1945-152">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="b1945-152">Full scan required or not?</span></span>|
|<span data-ttu-id="b1945-153">engineVersion</span><span class="sxs-lookup"><span data-stu-id="b1945-153">engineVersion</span></span>|<span data-ttu-id="b1945-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1945-154">String</span></span>|<span data-ttu-id="b1945-155">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="b1945-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="b1945-156">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="b1945-156">signatureVersion</span></span>|<span data-ttu-id="b1945-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1945-157">String</span></span>|<span data-ttu-id="b1945-158">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="b1945-158">Current malware definitions version</span></span>|
|<span data-ttu-id="b1945-159">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="b1945-159">antiMalwareVersion</span></span>|<span data-ttu-id="b1945-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1945-160">String</span></span>|<span data-ttu-id="b1945-161">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="b1945-161">Current anti malware version</span></span>|
|<span data-ttu-id="b1945-162">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="b1945-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="b1945-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1945-163">DateTimeOffset</span></span>|<span data-ttu-id="b1945-164">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="b1945-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="b1945-165">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="b1945-165">lastFullScanDateTime</span></span>|<span data-ttu-id="b1945-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1945-166">DateTimeOffset</span></span>|<span data-ttu-id="b1945-167">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="b1945-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="b1945-168">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="b1945-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="b1945-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1945-169">String</span></span>|<span data-ttu-id="b1945-170">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="b1945-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="b1945-171">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="b1945-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="b1945-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1945-172">String</span></span>|<span data-ttu-id="b1945-173">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="b1945-173">Last full scan signature version</span></span>|
|<span data-ttu-id="b1945-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1945-174">lastReportedDateTime</span></span>|<span data-ttu-id="b1945-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1945-175">DateTimeOffset</span></span>|<span data-ttu-id="b1945-176">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="b1945-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1945-177">Relações</span><span class="sxs-lookup"><span data-stu-id="b1945-177">Relationships</span></span>
|<span data-ttu-id="b1945-178">Relação</span><span class="sxs-lookup"><span data-stu-id="b1945-178">Relationship</span></span>|<span data-ttu-id="b1945-179">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1945-179">Type</span></span>|<span data-ttu-id="b1945-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1945-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1945-181">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="b1945-181">detectedMalwareState</span></span>|<span data-ttu-id="b1945-182">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="b1945-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="b1945-183">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b1945-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1945-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1945-184">JSON Representation</span></span>
<span data-ttu-id="b1945-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1945-185">Here is a JSON representation of the resource.</span></span>
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





