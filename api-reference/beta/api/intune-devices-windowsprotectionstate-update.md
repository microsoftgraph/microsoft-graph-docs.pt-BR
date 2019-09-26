---
title: Atualizar Windowsprotectionstate foi
description: Atualiza as propriedades de um objeto Windowsprotectionstate foi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 74824bbc5c066d0e3df398786e5163642b64707a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187979"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="70cf4-103">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="70cf4-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="70cf4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70cf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70cf4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70cf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70cf4-106">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="70cf4-106">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70cf4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70cf4-107">Prerequisites</span></span>
<span data-ttu-id="70cf4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70cf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70cf4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70cf4-110">Permission type</span></span>|<span data-ttu-id="70cf4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70cf4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70cf4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70cf4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70cf4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70cf4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="70cf4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70cf4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70cf4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70cf4-115">Not supported.</span></span>|
|<span data-ttu-id="70cf4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70cf4-116">Application</span></span>|<span data-ttu-id="70cf4-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70cf4-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70cf4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70cf4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="70cf4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70cf4-119">Request headers</span></span>
|<span data-ttu-id="70cf4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70cf4-120">Header</span></span>|<span data-ttu-id="70cf4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="70cf4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70cf4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="70cf4-122">Authorization</span></span>|<span data-ttu-id="70cf4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70cf4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70cf4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70cf4-124">Accept</span></span>|<span data-ttu-id="70cf4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70cf4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70cf4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70cf4-126">Request body</span></span>
<span data-ttu-id="70cf4-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="70cf4-127">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="70cf4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="70cf4-128">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="70cf4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70cf4-129">Property</span></span>|<span data-ttu-id="70cf4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="70cf4-130">Type</span></span>|<span data-ttu-id="70cf4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="70cf4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70cf4-132">id</span><span class="sxs-lookup"><span data-stu-id="70cf4-132">id</span></span>|<span data-ttu-id="70cf4-133">String</span><span class="sxs-lookup"><span data-stu-id="70cf4-133">String</span></span>|<span data-ttu-id="70cf4-134">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="70cf4-134">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="70cf4-135">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="70cf4-135">This is device id of the device</span></span>|
|<span data-ttu-id="70cf4-136">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="70cf4-136">malwareProtectionEnabled</span></span>|<span data-ttu-id="70cf4-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="70cf4-137">Boolean</span></span>|<span data-ttu-id="70cf4-138">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="70cf4-138">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="70cf4-139">DeviceState</span><span class="sxs-lookup"><span data-stu-id="70cf4-139">deviceState</span></span>|[<span data-ttu-id="70cf4-140">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="70cf4-140">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="70cf4-141">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="70cf4-141">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="70cf4-142">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="70cf4-142">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="70cf4-143">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="70cf4-143">realTimeProtectionEnabled</span></span>|<span data-ttu-id="70cf4-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="70cf4-144">Boolean</span></span>|<span data-ttu-id="70cf4-145">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="70cf4-145">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="70cf4-146">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="70cf4-146">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="70cf4-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="70cf4-147">Boolean</span></span>|<span data-ttu-id="70cf4-148">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="70cf4-148">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="70cf4-149">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="70cf4-149">quickScanOverdue</span></span>|<span data-ttu-id="70cf4-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="70cf4-150">Boolean</span></span>|<span data-ttu-id="70cf4-151">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="70cf4-151">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="70cf4-152">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="70cf4-152">fullScanOverdue</span></span>|<span data-ttu-id="70cf4-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="70cf4-153">Boolean</span></span>|<span data-ttu-id="70cf4-154">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="70cf4-154">Full scan overdue or not?</span></span>|
|<span data-ttu-id="70cf4-155">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="70cf4-155">signatureUpdateOverdue</span></span>|<span data-ttu-id="70cf4-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="70cf4-156">Boolean</span></span>|<span data-ttu-id="70cf4-157">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="70cf4-157">Signature out of date or not?</span></span>|
|<span data-ttu-id="70cf4-158">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="70cf4-158">rebootRequired</span></span>|<span data-ttu-id="70cf4-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="70cf4-159">Boolean</span></span>|<span data-ttu-id="70cf4-160">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="70cf4-160">Reboot required or not?</span></span>|
|<span data-ttu-id="70cf4-161">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="70cf4-161">fullScanRequired</span></span>|<span data-ttu-id="70cf4-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="70cf4-162">Boolean</span></span>|<span data-ttu-id="70cf4-163">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="70cf4-163">Full scan required or not?</span></span>|
|<span data-ttu-id="70cf4-164">engineVersion</span><span class="sxs-lookup"><span data-stu-id="70cf4-164">engineVersion</span></span>|<span data-ttu-id="70cf4-165">String</span><span class="sxs-lookup"><span data-stu-id="70cf4-165">String</span></span>|<span data-ttu-id="70cf4-166">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="70cf4-166">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="70cf4-167">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="70cf4-167">signatureVersion</span></span>|<span data-ttu-id="70cf4-168">String</span><span class="sxs-lookup"><span data-stu-id="70cf4-168">String</span></span>|<span data-ttu-id="70cf4-169">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="70cf4-169">Current malware definitions version</span></span>|
|<span data-ttu-id="70cf4-170">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="70cf4-170">antiMalwareVersion</span></span>|<span data-ttu-id="70cf4-171">String</span><span class="sxs-lookup"><span data-stu-id="70cf4-171">String</span></span>|<span data-ttu-id="70cf4-172">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="70cf4-172">Current anti malware version</span></span>|
|<span data-ttu-id="70cf4-173">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="70cf4-173">lastQuickScanDateTime</span></span>|<span data-ttu-id="70cf4-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cf4-174">DateTimeOffset</span></span>|<span data-ttu-id="70cf4-175">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="70cf4-175">Last quick scan datetime</span></span>|
|<span data-ttu-id="70cf4-176">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="70cf4-176">lastFullScanDateTime</span></span>|<span data-ttu-id="70cf4-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cf4-177">DateTimeOffset</span></span>|<span data-ttu-id="70cf4-178">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="70cf4-178">Last quick scan datetime</span></span>|
|<span data-ttu-id="70cf4-179">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="70cf4-179">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="70cf4-180">String</span><span class="sxs-lookup"><span data-stu-id="70cf4-180">String</span></span>|<span data-ttu-id="70cf4-181">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="70cf4-181">Last quick scan signature version</span></span>|
|<span data-ttu-id="70cf4-182">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="70cf4-182">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="70cf4-183">String</span><span class="sxs-lookup"><span data-stu-id="70cf4-183">String</span></span>|<span data-ttu-id="70cf4-184">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="70cf4-184">Last full scan signature version</span></span>|
|<span data-ttu-id="70cf4-185">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="70cf4-185">lastReportedDateTime</span></span>|<span data-ttu-id="70cf4-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70cf4-186">DateTimeOffset</span></span>|<span data-ttu-id="70cf4-187">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="70cf4-187">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="70cf4-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="70cf4-188">Response</span></span>
<span data-ttu-id="70cf4-189">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70cf4-189">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70cf4-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70cf4-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="70cf4-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70cf4-191">Request</span></span>
<span data-ttu-id="70cf4-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70cf4-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70cf4-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="70cf4-193">Response</span></span>
<span data-ttu-id="70cf4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70cf4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




