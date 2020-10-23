---
title: Atualizar Windowsprotectionstate foi
description: Atualiza as propriedades de um objeto Windowsprotectionstate foi.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42e44f3d5fc96dd382435502c82b187f58207709
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724238"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="81d77-103">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="81d77-103">Update windowsProtectionState</span></span>

<span data-ttu-id="81d77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81d77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81d77-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81d77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81d77-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81d77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81d77-107">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="81d77-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81d77-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81d77-108">Prerequisites</span></span>
<span data-ttu-id="81d77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81d77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81d77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81d77-111">Permission type</span></span>|<span data-ttu-id="81d77-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81d77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81d77-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81d77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81d77-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81d77-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="81d77-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81d77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81d77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81d77-116">Not supported.</span></span>|
|<span data-ttu-id="81d77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81d77-117">Application</span></span>|<span data-ttu-id="81d77-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81d77-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81d77-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81d77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="81d77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81d77-120">Request headers</span></span>
|<span data-ttu-id="81d77-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81d77-121">Header</span></span>|<span data-ttu-id="81d77-122">Valor</span><span class="sxs-lookup"><span data-stu-id="81d77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81d77-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81d77-123">Authorization</span></span>|<span data-ttu-id="81d77-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81d77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81d77-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81d77-125">Accept</span></span>|<span data-ttu-id="81d77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81d77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81d77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81d77-127">Request body</span></span>
<span data-ttu-id="81d77-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="81d77-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="81d77-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="81d77-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="81d77-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81d77-130">Property</span></span>|<span data-ttu-id="81d77-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="81d77-131">Type</span></span>|<span data-ttu-id="81d77-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="81d77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81d77-133">id</span><span class="sxs-lookup"><span data-stu-id="81d77-133">id</span></span>|<span data-ttu-id="81d77-134">String</span><span class="sxs-lookup"><span data-stu-id="81d77-134">String</span></span>|<span data-ttu-id="81d77-135">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81d77-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="81d77-136">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81d77-136">This is device id of the device</span></span>|
|<span data-ttu-id="81d77-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="81d77-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="81d77-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d77-138">Boolean</span></span>|<span data-ttu-id="81d77-139">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="81d77-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="81d77-140">DeviceState</span><span class="sxs-lookup"><span data-stu-id="81d77-140">deviceState</span></span>|[<span data-ttu-id="81d77-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="81d77-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="81d77-142">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="81d77-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="81d77-143">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="81d77-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="81d77-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="81d77-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="81d77-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d77-145">Boolean</span></span>|<span data-ttu-id="81d77-146">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="81d77-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="81d77-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="81d77-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="81d77-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d77-148">Boolean</span></span>|<span data-ttu-id="81d77-149">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="81d77-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="81d77-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="81d77-150">quickScanOverdue</span></span>|<span data-ttu-id="81d77-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d77-151">Boolean</span></span>|<span data-ttu-id="81d77-152">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="81d77-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="81d77-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="81d77-153">fullScanOverdue</span></span>|<span data-ttu-id="81d77-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d77-154">Boolean</span></span>|<span data-ttu-id="81d77-155">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="81d77-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="81d77-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="81d77-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="81d77-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d77-157">Boolean</span></span>|<span data-ttu-id="81d77-158">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="81d77-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="81d77-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="81d77-159">rebootRequired</span></span>|<span data-ttu-id="81d77-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d77-160">Boolean</span></span>|<span data-ttu-id="81d77-161">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="81d77-161">Reboot required or not?</span></span>|
|<span data-ttu-id="81d77-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="81d77-162">fullScanRequired</span></span>|<span data-ttu-id="81d77-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="81d77-163">Boolean</span></span>|<span data-ttu-id="81d77-164">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="81d77-164">Full scan required or not?</span></span>|
|<span data-ttu-id="81d77-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="81d77-165">engineVersion</span></span>|<span data-ttu-id="81d77-166">String</span><span class="sxs-lookup"><span data-stu-id="81d77-166">String</span></span>|<span data-ttu-id="81d77-167">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="81d77-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="81d77-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="81d77-168">signatureVersion</span></span>|<span data-ttu-id="81d77-169">String</span><span class="sxs-lookup"><span data-stu-id="81d77-169">String</span></span>|<span data-ttu-id="81d77-170">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="81d77-170">Current malware definitions version</span></span>|
|<span data-ttu-id="81d77-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="81d77-171">antiMalwareVersion</span></span>|<span data-ttu-id="81d77-172">String</span><span class="sxs-lookup"><span data-stu-id="81d77-172">String</span></span>|<span data-ttu-id="81d77-173">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="81d77-173">Current anti malware version</span></span>|
|<span data-ttu-id="81d77-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="81d77-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="81d77-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d77-175">DateTimeOffset</span></span>|<span data-ttu-id="81d77-176">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="81d77-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="81d77-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="81d77-177">lastFullScanDateTime</span></span>|<span data-ttu-id="81d77-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d77-178">DateTimeOffset</span></span>|<span data-ttu-id="81d77-179">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="81d77-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="81d77-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="81d77-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="81d77-181">String</span><span class="sxs-lookup"><span data-stu-id="81d77-181">String</span></span>|<span data-ttu-id="81d77-182">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="81d77-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="81d77-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="81d77-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="81d77-184">String</span><span class="sxs-lookup"><span data-stu-id="81d77-184">String</span></span>|<span data-ttu-id="81d77-185">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="81d77-185">Last full scan signature version</span></span>|
|<span data-ttu-id="81d77-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="81d77-186">lastReportedDateTime</span></span>|<span data-ttu-id="81d77-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d77-187">DateTimeOffset</span></span>|<span data-ttu-id="81d77-188">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="81d77-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="81d77-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="81d77-189">Response</span></span>
<span data-ttu-id="81d77-190">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81d77-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81d77-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81d77-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="81d77-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81d77-192">Request</span></span>
<span data-ttu-id="81d77-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81d77-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
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

### <a name="response"></a><span data-ttu-id="81d77-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="81d77-194">Response</span></span>
<span data-ttu-id="81d77-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81d77-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





