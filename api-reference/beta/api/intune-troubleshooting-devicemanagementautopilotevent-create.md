---
title: Criar deviceManagementAutopilotEvent
description: Criar um novo objeto deviceManagementAutopilotEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e33ab0fc0b48284457785702d3591f462039505c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800260"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="13bf5-103">Criar deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="13bf5-103">Create deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="13bf5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13bf5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13bf5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13bf5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13bf5-106">Criar um novo objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="13bf5-106">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13bf5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13bf5-107">Prerequisites</span></span>
<span data-ttu-id="13bf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13bf5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13bf5-110">Permission type</span></span>|<span data-ttu-id="13bf5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13bf5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13bf5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13bf5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13bf5-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bf5-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13bf5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13bf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13bf5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13bf5-115">Not supported.</span></span>|
|<span data-ttu-id="13bf5-116">Application</span><span class="sxs-lookup"><span data-stu-id="13bf5-116">Application</span></span>|<span data-ttu-id="13bf5-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13bf5-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13bf5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13bf5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="13bf5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13bf5-119">Request headers</span></span>
|<span data-ttu-id="13bf5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13bf5-120">Header</span></span>|<span data-ttu-id="13bf5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="13bf5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13bf5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13bf5-122">Authorization</span></span>|<span data-ttu-id="13bf5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13bf5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13bf5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13bf5-124">Accept</span></span>|<span data-ttu-id="13bf5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13bf5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13bf5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13bf5-126">Request body</span></span>
<span data-ttu-id="13bf5-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="13bf5-127">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="13bf5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="13bf5-128">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="13bf5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13bf5-129">Property</span></span>|<span data-ttu-id="13bf5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="13bf5-130">Type</span></span>|<span data-ttu-id="13bf5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="13bf5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13bf5-132">id</span><span class="sxs-lookup"><span data-stu-id="13bf5-132">id</span></span>|<span data-ttu-id="13bf5-133">String</span><span class="sxs-lookup"><span data-stu-id="13bf5-133">String</span></span>|<span data-ttu-id="13bf5-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="13bf5-134">UUID for the object</span></span>|
|<span data-ttu-id="13bf5-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="13bf5-135">deviceId</span></span>|<span data-ttu-id="13bf5-136">String</span><span class="sxs-lookup"><span data-stu-id="13bf5-136">String</span></span>|<span data-ttu-id="13bf5-137">ID de dispositivo associada ao objeto</span><span class="sxs-lookup"><span data-stu-id="13bf5-137">Device id associated with the object</span></span>|
|<span data-ttu-id="13bf5-138">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="13bf5-138">eventDateTime</span></span>|<span data-ttu-id="13bf5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bf5-139">DateTimeOffset</span></span>|<span data-ttu-id="13bf5-140">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="13bf5-140">Time when the event occurred .</span></span>|
|<span data-ttu-id="13bf5-141">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="13bf5-141">deviceRegisteredDateTime</span></span>|<span data-ttu-id="13bf5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bf5-142">DateTimeOffset</span></span>|<span data-ttu-id="13bf5-143">Data de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bf5-143">Device registration date.</span></span>|
|<span data-ttu-id="13bf5-144">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="13bf5-144">enrollmentStartDateTime</span></span>|<span data-ttu-id="13bf5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bf5-145">DateTimeOffset</span></span>|<span data-ttu-id="13bf5-146">Data de início do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bf5-146">Device enrollment start date.</span></span>|
|<span data-ttu-id="13bf5-147">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="13bf5-147">enrollmentType</span></span>|[<span data-ttu-id="13bf5-148">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="13bf5-148">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="13bf5-149">Tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="13bf5-149">Enrollment type.</span></span> <span data-ttu-id="13bf5-150">Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="13bf5-150">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="13bf5-151">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="13bf5-151">deviceSerialNumber</span></span>|<span data-ttu-id="13bf5-152">String</span><span class="sxs-lookup"><span data-stu-id="13bf5-152">String</span></span>|<span data-ttu-id="13bf5-153">Número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bf5-153">Device serial number.</span></span>|
|<span data-ttu-id="13bf5-154">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="13bf5-154">managedDeviceName</span></span>|<span data-ttu-id="13bf5-155">String</span><span class="sxs-lookup"><span data-stu-id="13bf5-155">String</span></span>|<span data-ttu-id="13bf5-156">Nome do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="13bf5-156">Managed device name.</span></span>|
|<span data-ttu-id="13bf5-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13bf5-157">userPrincipalName</span></span>|<span data-ttu-id="13bf5-158">String</span><span class="sxs-lookup"><span data-stu-id="13bf5-158">String</span></span>|<span data-ttu-id="13bf5-159">Nome principal do usuário usado para registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bf5-159">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="13bf5-160">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="13bf5-160">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="13bf5-161">String</span><span class="sxs-lookup"><span data-stu-id="13bf5-161">String</span></span>|<span data-ttu-id="13bf5-162">Nome do perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="13bf5-162">Autopilot profile name.</span></span>|
|<span data-ttu-id="13bf5-163">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="13bf5-163">enrollmentState</span></span>|[<span data-ttu-id="13bf5-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="13bf5-164">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="13bf5-165">Estado de registro como cadastrado, falhou.</span><span class="sxs-lookup"><span data-stu-id="13bf5-165">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="13bf5-166">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="13bf5-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="13bf5-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="13bf5-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="13bf5-168">String</span><span class="sxs-lookup"><span data-stu-id="13bf5-168">String</span></span>|<span data-ttu-id="13bf5-169">Nome do perfil da página de status do registro</span><span class="sxs-lookup"><span data-stu-id="13bf5-169">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="13bf5-170">DeploymentState</span><span class="sxs-lookup"><span data-stu-id="13bf5-170">deploymentState</span></span>|[<span data-ttu-id="13bf5-171">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="13bf5-171">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="13bf5-172">Estado de implantação como êxito, falha, InProgress, SuccessWithTimeout.</span><span class="sxs-lookup"><span data-stu-id="13bf5-172">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="13bf5-173">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="13bf5-173">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="13bf5-174">osVersion</span><span class="sxs-lookup"><span data-stu-id="13bf5-174">osVersion</span></span>|<span data-ttu-id="13bf5-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13bf5-175">String</span></span>|<span data-ttu-id="13bf5-176">Versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bf5-176">Device operating system version.</span></span>|
|<span data-ttu-id="13bf5-177">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="13bf5-177">deploymentDuration</span></span>|<span data-ttu-id="13bf5-178">Duração</span><span class="sxs-lookup"><span data-stu-id="13bf5-178">Duration</span></span>|<span data-ttu-id="13bf5-179">Duração da implantação do piloto automático, incluindo registro.</span><span class="sxs-lookup"><span data-stu-id="13bf5-179">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="13bf5-180">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="13bf5-180">deploymentTotalDuration</span></span>|<span data-ttu-id="13bf5-181">Duração</span><span class="sxs-lookup"><span data-stu-id="13bf5-181">Duration</span></span>|<span data-ttu-id="13bf5-182">Duração total da implantação na tela de registro na área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="13bf5-182">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="13bf5-183">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="13bf5-183">devicePreparationDuration</span></span>|<span data-ttu-id="13bf5-184">Duração</span><span class="sxs-lookup"><span data-stu-id="13bf5-184">Duration</span></span>|<span data-ttu-id="13bf5-185">Tempo gasto no registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bf5-185">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="13bf5-186">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="13bf5-186">deviceSetupDuration</span></span>|<span data-ttu-id="13bf5-187">Duração</span><span class="sxs-lookup"><span data-stu-id="13bf5-187">Duration</span></span>|<span data-ttu-id="13bf5-188">Tempo gasto em ESP de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="13bf5-188">Time spent in device ESP.</span></span>|
|<span data-ttu-id="13bf5-189">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="13bf5-189">accountSetupDuration</span></span>|<span data-ttu-id="13bf5-190">Duração</span><span class="sxs-lookup"><span data-stu-id="13bf5-190">Duration</span></span>|<span data-ttu-id="13bf5-191">Tempo gasto na ESP do usuário.</span><span class="sxs-lookup"><span data-stu-id="13bf5-191">Time spent in user ESP.</span></span>|
|<span data-ttu-id="13bf5-192">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="13bf5-192">deploymentStartDateTime</span></span>|<span data-ttu-id="13bf5-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bf5-193">DateTimeOffset</span></span>|<span data-ttu-id="13bf5-194">Hora de início da implantação.</span><span class="sxs-lookup"><span data-stu-id="13bf5-194">Deployment start time.</span></span>|
|<span data-ttu-id="13bf5-195">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="13bf5-195">deploymentEndDateTime</span></span>|<span data-ttu-id="13bf5-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13bf5-196">DateTimeOffset</span></span>|<span data-ttu-id="13bf5-197">Hora de término da implantação.</span><span class="sxs-lookup"><span data-stu-id="13bf5-197">Deployment end time.</span></span>|
|<span data-ttu-id="13bf5-198">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="13bf5-198">targetedAppCount</span></span>|<span data-ttu-id="13bf5-199">Int32</span><span class="sxs-lookup"><span data-stu-id="13bf5-199">Int32</span></span>|<span data-ttu-id="13bf5-200">Contagem de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="13bf5-200">Count of applications targeted.</span></span>|
|<span data-ttu-id="13bf5-201">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="13bf5-201">targetedPolicyCount</span></span>|<span data-ttu-id="13bf5-202">Int32</span><span class="sxs-lookup"><span data-stu-id="13bf5-202">Int32</span></span>|<span data-ttu-id="13bf5-203">Contagem de políticas direcionadas.</span><span class="sxs-lookup"><span data-stu-id="13bf5-203">Count of policies targeted.</span></span>|
|<span data-ttu-id="13bf5-204">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="13bf5-204">enrollmentFailureDetails</span></span>|<span data-ttu-id="13bf5-205">String</span><span class="sxs-lookup"><span data-stu-id="13bf5-205">String</span></span>|<span data-ttu-id="13bf5-206">Detalhes da falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="13bf5-206">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="13bf5-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="13bf5-207">Response</span></span>
<span data-ttu-id="13bf5-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13bf5-208">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13bf5-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13bf5-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="13bf5-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13bf5-210">Request</span></span>
<span data-ttu-id="13bf5-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13bf5-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1357

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

### <a name="response"></a><span data-ttu-id="13bf5-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="13bf5-212">Response</span></span>
<span data-ttu-id="13bf5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13bf5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1406

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
  "deviceId": "Device Id value",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```




