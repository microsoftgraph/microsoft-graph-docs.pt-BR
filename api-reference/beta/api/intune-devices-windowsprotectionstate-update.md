---
title: Atualizar Windowsprotectionstate foi
description: Atualiza as propriedades de um objeto Windowsprotectionstate foi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8aa21ece86f372274085bdad6d43df0a2893ba2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467638"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="ff100-103">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="ff100-103">Update windowsProtectionState</span></span>

<span data-ttu-id="ff100-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff100-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff100-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff100-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff100-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff100-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff100-107">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ff100-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff100-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff100-108">Prerequisites</span></span>
<span data-ttu-id="ff100-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff100-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff100-111">Permission type</span></span>|<span data-ttu-id="ff100-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff100-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff100-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff100-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff100-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff100-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ff100-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff100-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff100-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff100-116">Not supported.</span></span>|
|<span data-ttu-id="ff100-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff100-117">Application</span></span>|<span data-ttu-id="ff100-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff100-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff100-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff100-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="ff100-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff100-120">Request headers</span></span>
|<span data-ttu-id="ff100-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff100-121">Header</span></span>|<span data-ttu-id="ff100-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff100-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff100-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff100-123">Authorization</span></span>|<span data-ttu-id="ff100-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff100-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff100-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff100-125">Accept</span></span>|<span data-ttu-id="ff100-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff100-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff100-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff100-127">Request body</span></span>
<span data-ttu-id="ff100-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ff100-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="ff100-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="ff100-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="ff100-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff100-130">Property</span></span>|<span data-ttu-id="ff100-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff100-131">Type</span></span>|<span data-ttu-id="ff100-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff100-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff100-133">id</span><span class="sxs-lookup"><span data-stu-id="ff100-133">id</span></span>|<span data-ttu-id="ff100-134">String</span><span class="sxs-lookup"><span data-stu-id="ff100-134">String</span></span>|<span data-ttu-id="ff100-135">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff100-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="ff100-136">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ff100-136">This is device id of the device</span></span>|
|<span data-ttu-id="ff100-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ff100-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="ff100-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff100-138">Boolean</span></span>|<span data-ttu-id="ff100-139">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="ff100-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="ff100-140">DeviceState</span><span class="sxs-lookup"><span data-stu-id="ff100-140">deviceState</span></span>|[<span data-ttu-id="ff100-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="ff100-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="ff100-142">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="ff100-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="ff100-143">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="ff100-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="ff100-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ff100-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="ff100-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff100-145">Boolean</span></span>|<span data-ttu-id="ff100-146">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="ff100-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="ff100-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="ff100-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="ff100-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff100-148">Boolean</span></span>|<span data-ttu-id="ff100-149">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="ff100-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="ff100-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="ff100-150">quickScanOverdue</span></span>|<span data-ttu-id="ff100-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff100-151">Boolean</span></span>|<span data-ttu-id="ff100-152">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="ff100-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="ff100-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="ff100-153">fullScanOverdue</span></span>|<span data-ttu-id="ff100-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff100-154">Boolean</span></span>|<span data-ttu-id="ff100-155">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="ff100-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="ff100-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="ff100-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="ff100-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff100-157">Boolean</span></span>|<span data-ttu-id="ff100-158">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="ff100-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="ff100-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="ff100-159">rebootRequired</span></span>|<span data-ttu-id="ff100-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff100-160">Boolean</span></span>|<span data-ttu-id="ff100-161">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="ff100-161">Reboot required or not?</span></span>|
|<span data-ttu-id="ff100-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="ff100-162">fullScanRequired</span></span>|<span data-ttu-id="ff100-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff100-163">Boolean</span></span>|<span data-ttu-id="ff100-164">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="ff100-164">Full scan required or not?</span></span>|
|<span data-ttu-id="ff100-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="ff100-165">engineVersion</span></span>|<span data-ttu-id="ff100-166">String</span><span class="sxs-lookup"><span data-stu-id="ff100-166">String</span></span>|<span data-ttu-id="ff100-167">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="ff100-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="ff100-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="ff100-168">signatureVersion</span></span>|<span data-ttu-id="ff100-169">String</span><span class="sxs-lookup"><span data-stu-id="ff100-169">String</span></span>|<span data-ttu-id="ff100-170">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="ff100-170">Current malware definitions version</span></span>|
|<span data-ttu-id="ff100-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="ff100-171">antiMalwareVersion</span></span>|<span data-ttu-id="ff100-172">String</span><span class="sxs-lookup"><span data-stu-id="ff100-172">String</span></span>|<span data-ttu-id="ff100-173">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="ff100-173">Current anti malware version</span></span>|
|<span data-ttu-id="ff100-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="ff100-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="ff100-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff100-175">DateTimeOffset</span></span>|<span data-ttu-id="ff100-176">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="ff100-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="ff100-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="ff100-177">lastFullScanDateTime</span></span>|<span data-ttu-id="ff100-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff100-178">DateTimeOffset</span></span>|<span data-ttu-id="ff100-179">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="ff100-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="ff100-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="ff100-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="ff100-181">String</span><span class="sxs-lookup"><span data-stu-id="ff100-181">String</span></span>|<span data-ttu-id="ff100-182">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="ff100-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="ff100-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="ff100-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="ff100-184">String</span><span class="sxs-lookup"><span data-stu-id="ff100-184">String</span></span>|<span data-ttu-id="ff100-185">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="ff100-185">Last full scan signature version</span></span>|
|<span data-ttu-id="ff100-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff100-186">lastReportedDateTime</span></span>|<span data-ttu-id="ff100-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff100-187">DateTimeOffset</span></span>|<span data-ttu-id="ff100-188">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="ff100-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="ff100-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff100-189">Response</span></span>
<span data-ttu-id="ff100-190">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff100-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff100-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff100-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff100-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff100-192">Request</span></span>
<span data-ttu-id="ff100-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff100-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff100-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff100-194">Response</span></span>
<span data-ttu-id="ff100-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff100-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





