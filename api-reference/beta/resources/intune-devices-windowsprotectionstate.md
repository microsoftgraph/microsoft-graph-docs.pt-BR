---
title: tipo de recurso de windowsProtectionState
description: Entidade de status de proteção do dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef6c86983475abc687055ac2322ba02fae27ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423584"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="6fbed-103">tipo de recurso de windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="6fbed-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="6fbed-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6fbed-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6fbed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6fbed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fbed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6fbed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fbed-107">Entidade de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6fbed-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="6fbed-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6fbed-108">Methods</span></span>
|<span data-ttu-id="6fbed-109">Método</span><span class="sxs-lookup"><span data-stu-id="6fbed-109">Method</span></span>|<span data-ttu-id="6fbed-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6fbed-110">Return Type</span></span>|<span data-ttu-id="6fbed-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fbed-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fbed-112">Obter windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="6fbed-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="6fbed-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="6fbed-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="6fbed-114">Leia as propriedades e os relacionamentos do objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6fbed-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="6fbed-115">Atualizar windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="6fbed-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="6fbed-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="6fbed-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="6fbed-117">Atualize as propriedades de um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6fbed-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6fbed-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fbed-118">Properties</span></span>
|<span data-ttu-id="6fbed-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fbed-119">Property</span></span>|<span data-ttu-id="6fbed-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fbed-120">Type</span></span>|<span data-ttu-id="6fbed-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fbed-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fbed-122">id</span><span class="sxs-lookup"><span data-stu-id="6fbed-122">id</span></span>|<span data-ttu-id="6fbed-123">String</span><span class="sxs-lookup"><span data-stu-id="6fbed-123">String</span></span>|<span data-ttu-id="6fbed-124">O identificador exclusivo para o objeto de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6fbed-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="6fbed-125">Este é o id do dispositivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fbed-125">This is device id of the device</span></span>|
|<span data-ttu-id="6fbed-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6fbed-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="6fbed-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fbed-127">Boolean</span></span>|<span data-ttu-id="6fbed-128">Anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="6fbed-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="6fbed-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="6fbed-129">deviceState</span></span>|[<span data-ttu-id="6fbed-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="6fbed-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="6fbed-131">Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.).</span><span class="sxs-lookup"><span data-stu-id="6fbed-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="6fbed-132">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="6fbed-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="6fbed-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6fbed-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="6fbed-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fbed-134">Boolean</span></span>|<span data-ttu-id="6fbed-135">Proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="6fbed-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="6fbed-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="6fbed-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="6fbed-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fbed-137">Boolean</span></span>|<span data-ttu-id="6fbed-138">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="6fbed-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="6fbed-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="6fbed-139">quickScanOverdue</span></span>|<span data-ttu-id="6fbed-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fbed-140">Boolean</span></span>|<span data-ttu-id="6fbed-141">Verificação rápida vencidos ou não?</span><span class="sxs-lookup"><span data-stu-id="6fbed-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="6fbed-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="6fbed-142">fullScanOverdue</span></span>|<span data-ttu-id="6fbed-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fbed-143">Boolean</span></span>|<span data-ttu-id="6fbed-144">Completos exame vencido ou não?</span><span class="sxs-lookup"><span data-stu-id="6fbed-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="6fbed-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="6fbed-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="6fbed-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fbed-146">Boolean</span></span>|<span data-ttu-id="6fbed-147">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="6fbed-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="6fbed-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="6fbed-148">rebootRequired</span></span>|<span data-ttu-id="6fbed-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fbed-149">Boolean</span></span>|<span data-ttu-id="6fbed-150">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="6fbed-150">Reboot required or not?</span></span>|
|<span data-ttu-id="6fbed-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="6fbed-151">fullScanRequired</span></span>|<span data-ttu-id="6fbed-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fbed-152">Boolean</span></span>|<span data-ttu-id="6fbed-153">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="6fbed-153">Full scan required or not?</span></span>|
|<span data-ttu-id="6fbed-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="6fbed-154">engineVersion</span></span>|<span data-ttu-id="6fbed-155">String</span><span class="sxs-lookup"><span data-stu-id="6fbed-155">String</span></span>|<span data-ttu-id="6fbed-156">Versão do mecanismo de proteção de ponto de extremidade atual</span><span class="sxs-lookup"><span data-stu-id="6fbed-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="6fbed-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="6fbed-157">signatureVersion</span></span>|<span data-ttu-id="6fbed-158">String</span><span class="sxs-lookup"><span data-stu-id="6fbed-158">String</span></span>|<span data-ttu-id="6fbed-159">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="6fbed-159">Current malware definitions version</span></span>|
|<span data-ttu-id="6fbed-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="6fbed-160">antiMalwareVersion</span></span>|<span data-ttu-id="6fbed-161">String</span><span class="sxs-lookup"><span data-stu-id="6fbed-161">String</span></span>|<span data-ttu-id="6fbed-162">Atual anti-malware versão</span><span class="sxs-lookup"><span data-stu-id="6fbed-162">Current anti malware version</span></span>|
|<span data-ttu-id="6fbed-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="6fbed-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="6fbed-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fbed-164">DateTimeOffset</span></span>|<span data-ttu-id="6fbed-165">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="6fbed-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="6fbed-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="6fbed-166">lastFullScanDateTime</span></span>|<span data-ttu-id="6fbed-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fbed-167">DateTimeOffset</span></span>|<span data-ttu-id="6fbed-168">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="6fbed-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="6fbed-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="6fbed-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="6fbed-170">String</span><span class="sxs-lookup"><span data-stu-id="6fbed-170">String</span></span>|<span data-ttu-id="6fbed-171">Última versão de assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="6fbed-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="6fbed-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="6fbed-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="6fbed-173">String</span><span class="sxs-lookup"><span data-stu-id="6fbed-173">String</span></span>|<span data-ttu-id="6fbed-174">Última versão de assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="6fbed-174">Last full scan signature version</span></span>|
|<span data-ttu-id="6fbed-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fbed-175">lastReportedDateTime</span></span>|<span data-ttu-id="6fbed-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fbed-176">DateTimeOffset</span></span>|<span data-ttu-id="6fbed-177">Tempo de informado último status de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fbed-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fbed-178">Relações</span><span class="sxs-lookup"><span data-stu-id="6fbed-178">Relationships</span></span>
|<span data-ttu-id="6fbed-179">Relação</span><span class="sxs-lookup"><span data-stu-id="6fbed-179">Relationship</span></span>|<span data-ttu-id="6fbed-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fbed-180">Type</span></span>|<span data-ttu-id="6fbed-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fbed-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fbed-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="6fbed-182">detectedMalwareState</span></span>|<span data-ttu-id="6fbed-183">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="6fbed-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="6fbed-184">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6fbed-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fbed-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fbed-185">JSON Representation</span></span>
<span data-ttu-id="6fbed-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fbed-186">Here is a JSON representation of the resource.</span></span>
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




