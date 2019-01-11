---
title: Atualizar windowsProtectionState
description: Atualize as propriedades de um objeto windowsProtectionState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 97a11b8a3a26bea6f59cf0791bc8f5356f6fdb85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886867"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="5aaa3-103">Atualizar windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5aaa3-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="5aaa3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5aaa3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5aaa3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5aaa3-107">Atualize as propriedades de um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5aaa3-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5aaa3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5aaa3-108">Prerequisites</span></span>
<span data-ttu-id="5aaa3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aaa3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5aaa3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5aaa3-111">Permission type</span></span>|<span data-ttu-id="5aaa3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5aaa3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5aaa3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5aaa3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5aaa3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5aaa3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5aaa3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5aaa3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5aaa3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-116">Not supported.</span></span>|
|<span data-ttu-id="5aaa3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5aaa3-117">Application</span></span>|<span data-ttu-id="5aaa3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5aaa3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aaa3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="5aaa3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aaa3-120">Request headers</span></span>
|<span data-ttu-id="5aaa3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5aaa3-121">Header</span></span>|<span data-ttu-id="5aaa3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5aaa3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5aaa3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5aaa3-123">Authorization</span></span>|<span data-ttu-id="5aaa3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5aaa3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5aaa3-125">Accept</span></span>|<span data-ttu-id="5aaa3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5aaa3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5aaa3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5aaa3-127">Request body</span></span>
<span data-ttu-id="5aaa3-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5aaa3-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="5aaa3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="5aaa3-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="5aaa3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5aaa3-130">Property</span></span>|<span data-ttu-id="5aaa3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5aaa3-131">Type</span></span>|<span data-ttu-id="5aaa3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aaa3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5aaa3-133">id</span><span class="sxs-lookup"><span data-stu-id="5aaa3-133">id</span></span>|<span data-ttu-id="5aaa3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5aaa3-134">String</span></span>|<span data-ttu-id="5aaa3-135">O identificador exclusivo para o objeto de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="5aaa3-136">Este é o id do dispositivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5aaa3-136">This is device id of the device</span></span>|
|<span data-ttu-id="5aaa3-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5aaa3-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="5aaa3-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aaa3-138">Boolean</span></span>|<span data-ttu-id="5aaa3-139">Anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="5aaa3-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="5aaa3-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="5aaa3-140">deviceState</span></span>|[<span data-ttu-id="5aaa3-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="5aaa3-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="5aaa3-142">Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.).</span><span class="sxs-lookup"><span data-stu-id="5aaa3-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="5aaa3-143">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="5aaa3-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5aaa3-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="5aaa3-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aaa3-145">Boolean</span></span>|<span data-ttu-id="5aaa3-146">Proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="5aaa3-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="5aaa3-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="5aaa3-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="5aaa3-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aaa3-148">Boolean</span></span>|<span data-ttu-id="5aaa3-149">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="5aaa3-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="5aaa3-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="5aaa3-150">quickScanOverdue</span></span>|<span data-ttu-id="5aaa3-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aaa3-151">Boolean</span></span>|<span data-ttu-id="5aaa3-152">Verificação rápida vencidos ou não?</span><span class="sxs-lookup"><span data-stu-id="5aaa3-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="5aaa3-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="5aaa3-153">fullScanOverdue</span></span>|<span data-ttu-id="5aaa3-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aaa3-154">Boolean</span></span>|<span data-ttu-id="5aaa3-155">Completos exame vencido ou não?</span><span class="sxs-lookup"><span data-stu-id="5aaa3-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="5aaa3-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="5aaa3-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="5aaa3-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aaa3-157">Boolean</span></span>|<span data-ttu-id="5aaa3-158">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="5aaa3-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="5aaa3-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="5aaa3-159">rebootRequired</span></span>|<span data-ttu-id="5aaa3-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aaa3-160">Boolean</span></span>|<span data-ttu-id="5aaa3-161">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="5aaa3-161">Reboot required or not?</span></span>|
|<span data-ttu-id="5aaa3-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="5aaa3-162">fullScanRequired</span></span>|<span data-ttu-id="5aaa3-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="5aaa3-163">Boolean</span></span>|<span data-ttu-id="5aaa3-164">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="5aaa3-164">Full scan required or not?</span></span>|
|<span data-ttu-id="5aaa3-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="5aaa3-165">engineVersion</span></span>|<span data-ttu-id="5aaa3-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5aaa3-166">String</span></span>|<span data-ttu-id="5aaa3-167">Versão do mecanismo de proteção de ponto de extremidade atual</span><span class="sxs-lookup"><span data-stu-id="5aaa3-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="5aaa3-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="5aaa3-168">signatureVersion</span></span>|<span data-ttu-id="5aaa3-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5aaa3-169">String</span></span>|<span data-ttu-id="5aaa3-170">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="5aaa3-170">Current malware definitions version</span></span>|
|<span data-ttu-id="5aaa3-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="5aaa3-171">antiMalwareVersion</span></span>|<span data-ttu-id="5aaa3-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5aaa3-172">String</span></span>|<span data-ttu-id="5aaa3-173">Atual anti-malware versão</span><span class="sxs-lookup"><span data-stu-id="5aaa3-173">Current anti malware version</span></span>|
|<span data-ttu-id="5aaa3-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="5aaa3-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="5aaa3-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aaa3-175">DateTimeOffset</span></span>|<span data-ttu-id="5aaa3-176">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="5aaa3-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="5aaa3-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="5aaa3-177">lastFullScanDateTime</span></span>|<span data-ttu-id="5aaa3-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aaa3-178">DateTimeOffset</span></span>|<span data-ttu-id="5aaa3-179">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="5aaa3-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="5aaa3-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="5aaa3-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="5aaa3-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5aaa3-181">String</span></span>|<span data-ttu-id="5aaa3-182">Última versão de assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="5aaa3-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="5aaa3-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="5aaa3-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="5aaa3-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5aaa3-184">String</span></span>|<span data-ttu-id="5aaa3-185">Última versão de assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="5aaa3-185">Last full scan signature version</span></span>|
|<span data-ttu-id="5aaa3-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5aaa3-186">lastReportedDateTime</span></span>|<span data-ttu-id="5aaa3-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5aaa3-187">DateTimeOffset</span></span>|<span data-ttu-id="5aaa3-188">Tempo de informado último status de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5aaa3-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="5aaa3-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aaa3-189">Response</span></span>
<span data-ttu-id="5aaa3-190">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aaa3-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aaa3-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="5aaa3-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aaa3-192">Request</span></span>
<span data-ttu-id="5aaa3-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 804

{
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

### <a name="response"></a><span data-ttu-id="5aaa3-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aaa3-194">Response</span></span>
<span data-ttu-id="5aaa3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5aaa3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





