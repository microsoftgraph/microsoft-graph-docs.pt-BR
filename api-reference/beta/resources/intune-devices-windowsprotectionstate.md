---
title: tipo de recurso de windowsProtectionState
description: Entidade de status de proteção do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f15044f597fb04e98571de7aec8796e9a9ddf74
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954523"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="5df95-103">tipo de recurso de windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5df95-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="5df95-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5df95-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5df95-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5df95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5df95-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5df95-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5df95-107">Entidade de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5df95-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="5df95-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5df95-108">Methods</span></span>
|<span data-ttu-id="5df95-109">Método</span><span class="sxs-lookup"><span data-stu-id="5df95-109">Method</span></span>|<span data-ttu-id="5df95-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5df95-110">Return Type</span></span>|<span data-ttu-id="5df95-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5df95-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5df95-112">Obter windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5df95-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="5df95-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5df95-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="5df95-114">Leia as propriedades e os relacionamentos do objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5df95-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="5df95-115">Atualizar windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5df95-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="5df95-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5df95-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="5df95-117">Atualize as propriedades de um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5df95-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5df95-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5df95-118">Properties</span></span>
|<span data-ttu-id="5df95-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5df95-119">Property</span></span>|<span data-ttu-id="5df95-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5df95-120">Type</span></span>|<span data-ttu-id="5df95-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5df95-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df95-122">id</span><span class="sxs-lookup"><span data-stu-id="5df95-122">id</span></span>|<span data-ttu-id="5df95-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5df95-123">String</span></span>|<span data-ttu-id="5df95-124">O identificador exclusivo para o objeto de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5df95-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="5df95-125">Este é o id do dispositivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5df95-125">This is device id of the device</span></span>|
|<span data-ttu-id="5df95-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5df95-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="5df95-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="5df95-127">Boolean</span></span>|<span data-ttu-id="5df95-128">Anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="5df95-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="5df95-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="5df95-129">deviceState</span></span>|[<span data-ttu-id="5df95-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="5df95-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="5df95-131">Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.).</span><span class="sxs-lookup"><span data-stu-id="5df95-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="5df95-132">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="5df95-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="5df95-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5df95-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="5df95-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="5df95-134">Boolean</span></span>|<span data-ttu-id="5df95-135">Proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="5df95-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="5df95-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="5df95-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="5df95-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="5df95-137">Boolean</span></span>|<span data-ttu-id="5df95-138">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="5df95-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="5df95-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="5df95-139">quickScanOverdue</span></span>|<span data-ttu-id="5df95-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="5df95-140">Boolean</span></span>|<span data-ttu-id="5df95-141">Verificação rápida vencidos ou não?</span><span class="sxs-lookup"><span data-stu-id="5df95-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="5df95-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="5df95-142">fullScanOverdue</span></span>|<span data-ttu-id="5df95-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="5df95-143">Boolean</span></span>|<span data-ttu-id="5df95-144">Completos exame vencido ou não?</span><span class="sxs-lookup"><span data-stu-id="5df95-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="5df95-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="5df95-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="5df95-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="5df95-146">Boolean</span></span>|<span data-ttu-id="5df95-147">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="5df95-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="5df95-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="5df95-148">rebootRequired</span></span>|<span data-ttu-id="5df95-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="5df95-149">Boolean</span></span>|<span data-ttu-id="5df95-150">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="5df95-150">Reboot required or not?</span></span>|
|<span data-ttu-id="5df95-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="5df95-151">fullScanRequired</span></span>|<span data-ttu-id="5df95-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="5df95-152">Boolean</span></span>|<span data-ttu-id="5df95-153">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="5df95-153">Full scan required or not?</span></span>|
|<span data-ttu-id="5df95-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="5df95-154">engineVersion</span></span>|<span data-ttu-id="5df95-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5df95-155">String</span></span>|<span data-ttu-id="5df95-156">Versão do mecanismo de proteção de ponto de extremidade atual</span><span class="sxs-lookup"><span data-stu-id="5df95-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="5df95-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="5df95-157">signatureVersion</span></span>|<span data-ttu-id="5df95-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5df95-158">String</span></span>|<span data-ttu-id="5df95-159">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="5df95-159">Current malware definitions version</span></span>|
|<span data-ttu-id="5df95-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="5df95-160">antiMalwareVersion</span></span>|<span data-ttu-id="5df95-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5df95-161">String</span></span>|<span data-ttu-id="5df95-162">Atual anti-malware versão</span><span class="sxs-lookup"><span data-stu-id="5df95-162">Current anti malware version</span></span>|
|<span data-ttu-id="5df95-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="5df95-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="5df95-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df95-164">DateTimeOffset</span></span>|<span data-ttu-id="5df95-165">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="5df95-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="5df95-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="5df95-166">lastFullScanDateTime</span></span>|<span data-ttu-id="5df95-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df95-167">DateTimeOffset</span></span>|<span data-ttu-id="5df95-168">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="5df95-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="5df95-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="5df95-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="5df95-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5df95-170">String</span></span>|<span data-ttu-id="5df95-171">Última versão de assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="5df95-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="5df95-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="5df95-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="5df95-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5df95-173">String</span></span>|<span data-ttu-id="5df95-174">Última versão de assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="5df95-174">Last full scan signature version</span></span>|
|<span data-ttu-id="5df95-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5df95-175">lastReportedDateTime</span></span>|<span data-ttu-id="5df95-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df95-176">DateTimeOffset</span></span>|<span data-ttu-id="5df95-177">Tempo de informado último status de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5df95-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="5df95-178">Relações</span><span class="sxs-lookup"><span data-stu-id="5df95-178">Relationships</span></span>
|<span data-ttu-id="5df95-179">Relação</span><span class="sxs-lookup"><span data-stu-id="5df95-179">Relationship</span></span>|<span data-ttu-id="5df95-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="5df95-180">Type</span></span>|<span data-ttu-id="5df95-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="5df95-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df95-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="5df95-182">detectedMalwareState</span></span>|<span data-ttu-id="5df95-183">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="5df95-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="5df95-184">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5df95-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5df95-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5df95-185">JSON Representation</span></span>
<span data-ttu-id="5df95-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5df95-186">Here is a JSON representation of the resource.</span></span>
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





