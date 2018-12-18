---
title: tipo de recurso de windowsProtectionState
description: Entidade de status de proteção do dispositivo.
author: tfitzmac
ms.openlocfilehash: 636b969ddafde5976939df764ae1180e19a181c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328074"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="a3282-103">tipo de recurso de windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a3282-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="a3282-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a3282-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3282-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a3282-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3282-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a3282-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3282-107">Entidade de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a3282-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="a3282-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a3282-108">Methods</span></span>
|<span data-ttu-id="a3282-109">Método</span><span class="sxs-lookup"><span data-stu-id="a3282-109">Method</span></span>|<span data-ttu-id="a3282-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a3282-110">Return Type</span></span>|<span data-ttu-id="a3282-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3282-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3282-112">Obter windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a3282-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="a3282-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a3282-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="a3282-114">Leia as propriedades e os relacionamentos do objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a3282-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="a3282-115">Atualizar windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a3282-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="a3282-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a3282-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="a3282-117">Atualize as propriedades de um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a3282-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3282-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3282-118">Properties</span></span>
|<span data-ttu-id="a3282-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3282-119">Property</span></span>|<span data-ttu-id="a3282-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3282-120">Type</span></span>|<span data-ttu-id="a3282-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3282-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3282-122">id</span><span class="sxs-lookup"><span data-stu-id="a3282-122">id</span></span>|<span data-ttu-id="a3282-123">String</span><span class="sxs-lookup"><span data-stu-id="a3282-123">String</span></span>|<span data-ttu-id="a3282-124">O identificador exclusivo para o objeto de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a3282-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="a3282-125">Este é o id do dispositivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a3282-125">This is device id of the device</span></span>|
|<span data-ttu-id="a3282-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a3282-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="a3282-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3282-127">Boolean</span></span>|<span data-ttu-id="a3282-128">Anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="a3282-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="a3282-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="a3282-129">deviceState</span></span>|[<span data-ttu-id="a3282-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="a3282-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="a3282-131">Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.).</span><span class="sxs-lookup"><span data-stu-id="a3282-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="a3282-132">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="a3282-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="a3282-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a3282-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="a3282-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3282-134">Boolean</span></span>|<span data-ttu-id="a3282-135">Proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="a3282-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="a3282-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="a3282-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="a3282-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3282-137">Boolean</span></span>|<span data-ttu-id="a3282-138">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="a3282-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="a3282-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a3282-139">quickScanOverdue</span></span>|<span data-ttu-id="a3282-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3282-140">Boolean</span></span>|<span data-ttu-id="a3282-141">Verificação rápida vencidos ou não?</span><span class="sxs-lookup"><span data-stu-id="a3282-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="a3282-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a3282-142">fullScanOverdue</span></span>|<span data-ttu-id="a3282-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3282-143">Boolean</span></span>|<span data-ttu-id="a3282-144">Completos exame vencido ou não?</span><span class="sxs-lookup"><span data-stu-id="a3282-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="a3282-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="a3282-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="a3282-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3282-146">Boolean</span></span>|<span data-ttu-id="a3282-147">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="a3282-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="a3282-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="a3282-148">rebootRequired</span></span>|<span data-ttu-id="a3282-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3282-149">Boolean</span></span>|<span data-ttu-id="a3282-150">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="a3282-150">Reboot required or not?</span></span>|
|<span data-ttu-id="a3282-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="a3282-151">fullScanRequired</span></span>|<span data-ttu-id="a3282-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3282-152">Boolean</span></span>|<span data-ttu-id="a3282-153">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="a3282-153">Full scan required or not?</span></span>|
|<span data-ttu-id="a3282-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="a3282-154">engineVersion</span></span>|<span data-ttu-id="a3282-155">String</span><span class="sxs-lookup"><span data-stu-id="a3282-155">String</span></span>|<span data-ttu-id="a3282-156">Versão do mecanismo de proteção de ponto de extremidade atual</span><span class="sxs-lookup"><span data-stu-id="a3282-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="a3282-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="a3282-157">signatureVersion</span></span>|<span data-ttu-id="a3282-158">String</span><span class="sxs-lookup"><span data-stu-id="a3282-158">String</span></span>|<span data-ttu-id="a3282-159">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="a3282-159">Current malware definitions version</span></span>|
|<span data-ttu-id="a3282-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="a3282-160">antiMalwareVersion</span></span>|<span data-ttu-id="a3282-161">String</span><span class="sxs-lookup"><span data-stu-id="a3282-161">String</span></span>|<span data-ttu-id="a3282-162">Atual anti-malware versão</span><span class="sxs-lookup"><span data-stu-id="a3282-162">Current anti malware version</span></span>|
|<span data-ttu-id="a3282-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a3282-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="a3282-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3282-164">DateTimeOffset</span></span>|<span data-ttu-id="a3282-165">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a3282-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="a3282-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a3282-166">lastFullScanDateTime</span></span>|<span data-ttu-id="a3282-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3282-167">DateTimeOffset</span></span>|<span data-ttu-id="a3282-168">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a3282-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="a3282-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a3282-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="a3282-170">String</span><span class="sxs-lookup"><span data-stu-id="a3282-170">String</span></span>|<span data-ttu-id="a3282-171">Última versão de assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a3282-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="a3282-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a3282-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="a3282-173">String</span><span class="sxs-lookup"><span data-stu-id="a3282-173">String</span></span>|<span data-ttu-id="a3282-174">Última versão de assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="a3282-174">Last full scan signature version</span></span>|
|<span data-ttu-id="a3282-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3282-175">lastReportedDateTime</span></span>|<span data-ttu-id="a3282-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3282-176">DateTimeOffset</span></span>|<span data-ttu-id="a3282-177">Tempo de informado último status de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a3282-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3282-178">Relações</span><span class="sxs-lookup"><span data-stu-id="a3282-178">Relationships</span></span>
|<span data-ttu-id="a3282-179">Relação</span><span class="sxs-lookup"><span data-stu-id="a3282-179">Relationship</span></span>|<span data-ttu-id="a3282-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3282-180">Type</span></span>|<span data-ttu-id="a3282-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3282-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3282-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="a3282-182">detectedMalwareState</span></span>|<span data-ttu-id="a3282-183">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="a3282-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="a3282-184">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a3282-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3282-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3282-185">JSON Representation</span></span>
<span data-ttu-id="a3282-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3282-186">Here is a JSON representation of the resource.</span></span>
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





