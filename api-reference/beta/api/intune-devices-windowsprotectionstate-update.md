---
title: Atualizar Windowsprotectionstate foi
description: Atualiza as propriedades de um objeto Windowsprotectionstate foi.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f315188c9a2b666f72af7b6a214a6de6cd6e6e79
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378171"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="ef16b-103">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="ef16b-103">Update windowsProtectionState</span></span>

<span data-ttu-id="ef16b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef16b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef16b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef16b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef16b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef16b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef16b-107">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ef16b-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef16b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef16b-108">Prerequisites</span></span>
<span data-ttu-id="ef16b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef16b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef16b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef16b-111">Permission type</span></span>|<span data-ttu-id="ef16b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef16b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef16b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef16b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef16b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef16b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ef16b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef16b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef16b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef16b-116">Not supported.</span></span>|
|<span data-ttu-id="ef16b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef16b-117">Application</span></span>|<span data-ttu-id="ef16b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef16b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef16b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef16b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="ef16b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef16b-120">Request headers</span></span>
|<span data-ttu-id="ef16b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef16b-121">Header</span></span>|<span data-ttu-id="ef16b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef16b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef16b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef16b-123">Authorization</span></span>|<span data-ttu-id="ef16b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef16b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef16b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef16b-125">Accept</span></span>|<span data-ttu-id="ef16b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef16b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef16b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef16b-127">Request body</span></span>
<span data-ttu-id="ef16b-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ef16b-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="ef16b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="ef16b-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="ef16b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef16b-130">Property</span></span>|<span data-ttu-id="ef16b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef16b-131">Type</span></span>|<span data-ttu-id="ef16b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef16b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef16b-133">id</span><span class="sxs-lookup"><span data-stu-id="ef16b-133">id</span></span>|<span data-ttu-id="ef16b-134">String</span><span class="sxs-lookup"><span data-stu-id="ef16b-134">String</span></span>|<span data-ttu-id="ef16b-135">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef16b-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="ef16b-136">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ef16b-136">This is device id of the device</span></span>|
|<span data-ttu-id="ef16b-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ef16b-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="ef16b-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef16b-138">Boolean</span></span>|<span data-ttu-id="ef16b-139">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="ef16b-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="ef16b-140">DeviceState</span><span class="sxs-lookup"><span data-stu-id="ef16b-140">deviceState</span></span>|[<span data-ttu-id="ef16b-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="ef16b-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="ef16b-142">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="ef16b-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="ef16b-143">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="ef16b-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="ef16b-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ef16b-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="ef16b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef16b-145">Boolean</span></span>|<span data-ttu-id="ef16b-146">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="ef16b-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="ef16b-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="ef16b-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="ef16b-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef16b-148">Boolean</span></span>|<span data-ttu-id="ef16b-149">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="ef16b-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="ef16b-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="ef16b-150">quickScanOverdue</span></span>|<span data-ttu-id="ef16b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef16b-151">Boolean</span></span>|<span data-ttu-id="ef16b-152">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="ef16b-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="ef16b-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="ef16b-153">fullScanOverdue</span></span>|<span data-ttu-id="ef16b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef16b-154">Boolean</span></span>|<span data-ttu-id="ef16b-155">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="ef16b-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="ef16b-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="ef16b-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="ef16b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef16b-157">Boolean</span></span>|<span data-ttu-id="ef16b-158">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="ef16b-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="ef16b-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="ef16b-159">rebootRequired</span></span>|<span data-ttu-id="ef16b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef16b-160">Boolean</span></span>|<span data-ttu-id="ef16b-161">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="ef16b-161">Reboot required or not?</span></span>|
|<span data-ttu-id="ef16b-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="ef16b-162">fullScanRequired</span></span>|<span data-ttu-id="ef16b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef16b-163">Boolean</span></span>|<span data-ttu-id="ef16b-164">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="ef16b-164">Full scan required or not?</span></span>|
|<span data-ttu-id="ef16b-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="ef16b-165">engineVersion</span></span>|<span data-ttu-id="ef16b-166">String</span><span class="sxs-lookup"><span data-stu-id="ef16b-166">String</span></span>|<span data-ttu-id="ef16b-167">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="ef16b-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="ef16b-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="ef16b-168">signatureVersion</span></span>|<span data-ttu-id="ef16b-169">String</span><span class="sxs-lookup"><span data-stu-id="ef16b-169">String</span></span>|<span data-ttu-id="ef16b-170">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="ef16b-170">Current malware definitions version</span></span>|
|<span data-ttu-id="ef16b-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="ef16b-171">antiMalwareVersion</span></span>|<span data-ttu-id="ef16b-172">String</span><span class="sxs-lookup"><span data-stu-id="ef16b-172">String</span></span>|<span data-ttu-id="ef16b-173">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="ef16b-173">Current anti malware version</span></span>|
|<span data-ttu-id="ef16b-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="ef16b-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="ef16b-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef16b-175">DateTimeOffset</span></span>|<span data-ttu-id="ef16b-176">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="ef16b-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="ef16b-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="ef16b-177">lastFullScanDateTime</span></span>|<span data-ttu-id="ef16b-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef16b-178">DateTimeOffset</span></span>|<span data-ttu-id="ef16b-179">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="ef16b-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="ef16b-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="ef16b-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="ef16b-181">String</span><span class="sxs-lookup"><span data-stu-id="ef16b-181">String</span></span>|<span data-ttu-id="ef16b-182">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="ef16b-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="ef16b-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="ef16b-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="ef16b-184">String</span><span class="sxs-lookup"><span data-stu-id="ef16b-184">String</span></span>|<span data-ttu-id="ef16b-185">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="ef16b-185">Last full scan signature version</span></span>|
|<span data-ttu-id="ef16b-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef16b-186">lastReportedDateTime</span></span>|<span data-ttu-id="ef16b-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef16b-187">DateTimeOffset</span></span>|<span data-ttu-id="ef16b-188">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="ef16b-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="ef16b-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef16b-189">Response</span></span>
<span data-ttu-id="ef16b-190">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef16b-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef16b-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef16b-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef16b-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef16b-192">Request</span></span>
<span data-ttu-id="ef16b-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef16b-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 865

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="ef16b-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef16b-194">Response</span></span>
<span data-ttu-id="ef16b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef16b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```



