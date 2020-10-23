---
title: Criar deviceManagementAutopilotEvent
description: Criar um novo objeto deviceManagementAutopilotEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f19348e301873b98b8ddf7491160323e5b009f1b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701673"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="bb022-103">Criar deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="bb022-103">Create deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="bb022-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb022-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb022-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb022-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb022-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb022-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb022-107">Criar um novo objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="bb022-107">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb022-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb022-108">Prerequisites</span></span>
<span data-ttu-id="bb022-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb022-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb022-111">Permission type</span></span>|<span data-ttu-id="bb022-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb022-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb022-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb022-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb022-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb022-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb022-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb022-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb022-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb022-116">Not supported.</span></span>|
|<span data-ttu-id="bb022-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb022-117">Application</span></span>|<span data-ttu-id="bb022-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb022-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb022-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb022-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="bb022-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb022-120">Request headers</span></span>
|<span data-ttu-id="bb022-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb022-121">Header</span></span>|<span data-ttu-id="bb022-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bb022-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb022-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb022-123">Authorization</span></span>|<span data-ttu-id="bb022-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb022-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb022-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb022-125">Accept</span></span>|<span data-ttu-id="bb022-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb022-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb022-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb022-127">Request body</span></span>
<span data-ttu-id="bb022-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="bb022-128">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="bb022-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="bb022-129">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="bb022-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb022-130">Property</span></span>|<span data-ttu-id="bb022-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb022-131">Type</span></span>|<span data-ttu-id="bb022-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb022-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb022-133">id</span><span class="sxs-lookup"><span data-stu-id="bb022-133">id</span></span>|<span data-ttu-id="bb022-134">String</span><span class="sxs-lookup"><span data-stu-id="bb022-134">String</span></span>|<span data-ttu-id="bb022-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="bb022-135">UUID for the object</span></span>|
|<span data-ttu-id="bb022-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="bb022-136">deviceId</span></span>|<span data-ttu-id="bb022-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb022-137">String</span></span>|<span data-ttu-id="bb022-138">ID de dispositivo associada ao objeto</span><span class="sxs-lookup"><span data-stu-id="bb022-138">Device id associated with the object</span></span>|
|<span data-ttu-id="bb022-139">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="bb022-139">eventDateTime</span></span>|<span data-ttu-id="bb022-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb022-140">DateTimeOffset</span></span>|<span data-ttu-id="bb022-141">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="bb022-141">Time when the event occurred .</span></span>|
|<span data-ttu-id="bb022-142">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="bb022-142">deviceRegisteredDateTime</span></span>|<span data-ttu-id="bb022-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb022-143">DateTimeOffset</span></span>|<span data-ttu-id="bb022-144">Data de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb022-144">Device registration date.</span></span>|
|<span data-ttu-id="bb022-145">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="bb022-145">enrollmentStartDateTime</span></span>|<span data-ttu-id="bb022-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb022-146">DateTimeOffset</span></span>|<span data-ttu-id="bb022-147">Data de início do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb022-147">Device enrollment start date.</span></span>|
|<span data-ttu-id="bb022-148">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="bb022-148">enrollmentType</span></span>|[<span data-ttu-id="bb022-149">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="bb022-149">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="bb022-150">Tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="bb022-150">Enrollment type.</span></span> <span data-ttu-id="bb022-151">Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="bb022-151">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="bb022-152">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="bb022-152">deviceSerialNumber</span></span>|<span data-ttu-id="bb022-153">String</span><span class="sxs-lookup"><span data-stu-id="bb022-153">String</span></span>|<span data-ttu-id="bb022-154">Número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb022-154">Device serial number.</span></span>|
|<span data-ttu-id="bb022-155">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="bb022-155">managedDeviceName</span></span>|<span data-ttu-id="bb022-156">String</span><span class="sxs-lookup"><span data-stu-id="bb022-156">String</span></span>|<span data-ttu-id="bb022-157">Nome do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="bb022-157">Managed device name.</span></span>|
|<span data-ttu-id="bb022-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb022-158">userPrincipalName</span></span>|<span data-ttu-id="bb022-159">String</span><span class="sxs-lookup"><span data-stu-id="bb022-159">String</span></span>|<span data-ttu-id="bb022-160">Nome principal do usuário usado para registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb022-160">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="bb022-161">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb022-161">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="bb022-162">String</span><span class="sxs-lookup"><span data-stu-id="bb022-162">String</span></span>|<span data-ttu-id="bb022-163">Nome do perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="bb022-163">Autopilot profile name.</span></span>|
|<span data-ttu-id="bb022-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="bb022-164">enrollmentState</span></span>|[<span data-ttu-id="bb022-165">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="bb022-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="bb022-166">Estado de registro como cadastrado, falhou.</span><span class="sxs-lookup"><span data-stu-id="bb022-166">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="bb022-167">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="bb022-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="bb022-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb022-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="bb022-169">String</span><span class="sxs-lookup"><span data-stu-id="bb022-169">String</span></span>|<span data-ttu-id="bb022-170">Nome do perfil da página de status do registro</span><span class="sxs-lookup"><span data-stu-id="bb022-170">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="bb022-171">DeploymentState</span><span class="sxs-lookup"><span data-stu-id="bb022-171">deploymentState</span></span>|[<span data-ttu-id="bb022-172">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="bb022-172">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="bb022-173">Estado de implantação como êxito, falha, InProgress, SuccessWithTimeout.</span><span class="sxs-lookup"><span data-stu-id="bb022-173">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="bb022-174">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="bb022-174">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="bb022-175">osVersion</span><span class="sxs-lookup"><span data-stu-id="bb022-175">osVersion</span></span>|<span data-ttu-id="bb022-176">String</span><span class="sxs-lookup"><span data-stu-id="bb022-176">String</span></span>|<span data-ttu-id="bb022-177">Versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb022-177">Device operating system version.</span></span>|
|<span data-ttu-id="bb022-178">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="bb022-178">deploymentDuration</span></span>|<span data-ttu-id="bb022-179">Duração</span><span class="sxs-lookup"><span data-stu-id="bb022-179">Duration</span></span>|<span data-ttu-id="bb022-180">Duração da implantação do piloto automático, incluindo registro.</span><span class="sxs-lookup"><span data-stu-id="bb022-180">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="bb022-181">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="bb022-181">deploymentTotalDuration</span></span>|<span data-ttu-id="bb022-182">Duração</span><span class="sxs-lookup"><span data-stu-id="bb022-182">Duration</span></span>|<span data-ttu-id="bb022-183">Duração total da implantação na tela de registro na área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="bb022-183">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="bb022-184">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="bb022-184">devicePreparationDuration</span></span>|<span data-ttu-id="bb022-185">Duração</span><span class="sxs-lookup"><span data-stu-id="bb022-185">Duration</span></span>|<span data-ttu-id="bb022-186">Tempo gasto no registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb022-186">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="bb022-187">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="bb022-187">deviceSetupDuration</span></span>|<span data-ttu-id="bb022-188">Duração</span><span class="sxs-lookup"><span data-stu-id="bb022-188">Duration</span></span>|<span data-ttu-id="bb022-189">Tempo gasto em ESP de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb022-189">Time spent in device ESP.</span></span>|
|<span data-ttu-id="bb022-190">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="bb022-190">accountSetupDuration</span></span>|<span data-ttu-id="bb022-191">Duração</span><span class="sxs-lookup"><span data-stu-id="bb022-191">Duration</span></span>|<span data-ttu-id="bb022-192">Tempo gasto na ESP do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb022-192">Time spent in user ESP.</span></span>|
|<span data-ttu-id="bb022-193">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="bb022-193">deploymentStartDateTime</span></span>|<span data-ttu-id="bb022-194">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb022-194">DateTimeOffset</span></span>|<span data-ttu-id="bb022-195">Hora de início da implantação.</span><span class="sxs-lookup"><span data-stu-id="bb022-195">Deployment start time.</span></span>|
|<span data-ttu-id="bb022-196">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="bb022-196">deploymentEndDateTime</span></span>|<span data-ttu-id="bb022-197">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb022-197">DateTimeOffset</span></span>|<span data-ttu-id="bb022-198">Hora de término da implantação.</span><span class="sxs-lookup"><span data-stu-id="bb022-198">Deployment end time.</span></span>|
|<span data-ttu-id="bb022-199">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="bb022-199">targetedAppCount</span></span>|<span data-ttu-id="bb022-200">Int32</span><span class="sxs-lookup"><span data-stu-id="bb022-200">Int32</span></span>|<span data-ttu-id="bb022-201">Contagem de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="bb022-201">Count of applications targeted.</span></span>|
|<span data-ttu-id="bb022-202">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="bb022-202">targetedPolicyCount</span></span>|<span data-ttu-id="bb022-203">Int32</span><span class="sxs-lookup"><span data-stu-id="bb022-203">Int32</span></span>|<span data-ttu-id="bb022-204">Contagem de políticas direcionadas.</span><span class="sxs-lookup"><span data-stu-id="bb022-204">Count of policies targeted.</span></span>|
|<span data-ttu-id="bb022-205">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="bb022-205">enrollmentFailureDetails</span></span>|<span data-ttu-id="bb022-206">String</span><span class="sxs-lookup"><span data-stu-id="bb022-206">String</span></span>|<span data-ttu-id="bb022-207">Detalhes da falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="bb022-207">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="bb022-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb022-208">Response</span></span>
<span data-ttu-id="bb022-209">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb022-209">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb022-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb022-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb022-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb022-211">Request</span></span>
<span data-ttu-id="bb022-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb022-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb022-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb022-213">Response</span></span>
<span data-ttu-id="bb022-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb022-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





