---
title: Atualizar windowsProtectionState
description: Atualize as propriedades de um objeto windowsProtectionState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ce3c4fcd46e2d627f94e1728d38e9a8f0f91ad30
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939872"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="87a5f-103">Atualizar windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="87a5f-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="87a5f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="87a5f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87a5f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87a5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87a5f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="87a5f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87a5f-107">Atualize as propriedades de um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="87a5f-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87a5f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87a5f-108">Prerequisites</span></span>
<span data-ttu-id="87a5f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87a5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87a5f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87a5f-111">Permission type</span></span>|<span data-ttu-id="87a5f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87a5f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87a5f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87a5f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87a5f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a5f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="87a5f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87a5f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87a5f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87a5f-116">Not supported.</span></span>|
|<span data-ttu-id="87a5f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87a5f-117">Application</span></span>|<span data-ttu-id="87a5f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87a5f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87a5f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87a5f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="87a5f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87a5f-120">Request headers</span></span>
|<span data-ttu-id="87a5f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87a5f-121">Header</span></span>|<span data-ttu-id="87a5f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="87a5f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87a5f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87a5f-123">Authorization</span></span>|<span data-ttu-id="87a5f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a5f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87a5f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87a5f-125">Accept</span></span>|<span data-ttu-id="87a5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87a5f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87a5f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87a5f-127">Request body</span></span>
<span data-ttu-id="87a5f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="87a5f-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="87a5f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="87a5f-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="87a5f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87a5f-130">Property</span></span>|<span data-ttu-id="87a5f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="87a5f-131">Type</span></span>|<span data-ttu-id="87a5f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a5f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87a5f-133">id</span><span class="sxs-lookup"><span data-stu-id="87a5f-133">id</span></span>|<span data-ttu-id="87a5f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87a5f-134">String</span></span>|<span data-ttu-id="87a5f-135">O identificador exclusivo para o objeto de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87a5f-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="87a5f-136">Este é o id do dispositivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="87a5f-136">This is device id of the device</span></span>|
|<span data-ttu-id="87a5f-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="87a5f-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="87a5f-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="87a5f-138">Boolean</span></span>|<span data-ttu-id="87a5f-139">Anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="87a5f-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="87a5f-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="87a5f-140">deviceState</span></span>|[<span data-ttu-id="87a5f-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="87a5f-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="87a5f-142">Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.).</span><span class="sxs-lookup"><span data-stu-id="87a5f-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="87a5f-143">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="87a5f-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="87a5f-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="87a5f-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="87a5f-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="87a5f-145">Boolean</span></span>|<span data-ttu-id="87a5f-146">Proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="87a5f-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="87a5f-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="87a5f-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="87a5f-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="87a5f-148">Boolean</span></span>|<span data-ttu-id="87a5f-149">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="87a5f-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="87a5f-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="87a5f-150">quickScanOverdue</span></span>|<span data-ttu-id="87a5f-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="87a5f-151">Boolean</span></span>|<span data-ttu-id="87a5f-152">Verificação rápida vencidos ou não?</span><span class="sxs-lookup"><span data-stu-id="87a5f-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="87a5f-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="87a5f-153">fullScanOverdue</span></span>|<span data-ttu-id="87a5f-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="87a5f-154">Boolean</span></span>|<span data-ttu-id="87a5f-155">Completos exame vencido ou não?</span><span class="sxs-lookup"><span data-stu-id="87a5f-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="87a5f-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="87a5f-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="87a5f-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="87a5f-157">Boolean</span></span>|<span data-ttu-id="87a5f-158">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="87a5f-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="87a5f-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="87a5f-159">rebootRequired</span></span>|<span data-ttu-id="87a5f-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="87a5f-160">Boolean</span></span>|<span data-ttu-id="87a5f-161">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="87a5f-161">Reboot required or not?</span></span>|
|<span data-ttu-id="87a5f-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="87a5f-162">fullScanRequired</span></span>|<span data-ttu-id="87a5f-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="87a5f-163">Boolean</span></span>|<span data-ttu-id="87a5f-164">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="87a5f-164">Full scan required or not?</span></span>|
|<span data-ttu-id="87a5f-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="87a5f-165">engineVersion</span></span>|<span data-ttu-id="87a5f-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87a5f-166">String</span></span>|<span data-ttu-id="87a5f-167">Versão do mecanismo de proteção de ponto de extremidade atual</span><span class="sxs-lookup"><span data-stu-id="87a5f-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="87a5f-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="87a5f-168">signatureVersion</span></span>|<span data-ttu-id="87a5f-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87a5f-169">String</span></span>|<span data-ttu-id="87a5f-170">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="87a5f-170">Current malware definitions version</span></span>|
|<span data-ttu-id="87a5f-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="87a5f-171">antiMalwareVersion</span></span>|<span data-ttu-id="87a5f-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87a5f-172">String</span></span>|<span data-ttu-id="87a5f-173">Atual anti-malware versão</span><span class="sxs-lookup"><span data-stu-id="87a5f-173">Current anti malware version</span></span>|
|<span data-ttu-id="87a5f-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="87a5f-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="87a5f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87a5f-175">DateTimeOffset</span></span>|<span data-ttu-id="87a5f-176">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="87a5f-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="87a5f-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="87a5f-177">lastFullScanDateTime</span></span>|<span data-ttu-id="87a5f-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87a5f-178">DateTimeOffset</span></span>|<span data-ttu-id="87a5f-179">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="87a5f-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="87a5f-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="87a5f-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="87a5f-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87a5f-181">String</span></span>|<span data-ttu-id="87a5f-182">Última versão de assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="87a5f-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="87a5f-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="87a5f-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="87a5f-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87a5f-184">String</span></span>|<span data-ttu-id="87a5f-185">Última versão de assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="87a5f-185">Last full scan signature version</span></span>|
|<span data-ttu-id="87a5f-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="87a5f-186">lastReportedDateTime</span></span>|<span data-ttu-id="87a5f-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87a5f-187">DateTimeOffset</span></span>|<span data-ttu-id="87a5f-188">Tempo de informado último status de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="87a5f-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="87a5f-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a5f-189">Response</span></span>
<span data-ttu-id="87a5f-190">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87a5f-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87a5f-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87a5f-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="87a5f-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87a5f-192">Request</span></span>
<span data-ttu-id="87a5f-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87a5f-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="87a5f-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a5f-194">Response</span></span>
<span data-ttu-id="87a5f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87a5f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





