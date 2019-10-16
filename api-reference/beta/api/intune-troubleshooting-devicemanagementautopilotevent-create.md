---
title: Criar deviceManagementAutopilotEvent
description: Criar um novo objeto deviceManagementAutopilotEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e848613bab1975ad30ee595a7f796d3a04ef7bf
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536767"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="84774-103">Criar deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="84774-103">Create deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="84774-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84774-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84774-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84774-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84774-106">Criar um novo objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="84774-106">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84774-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84774-107">Prerequisites</span></span>
<span data-ttu-id="84774-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84774-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84774-110">Permission type</span></span>|<span data-ttu-id="84774-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84774-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84774-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84774-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84774-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84774-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="84774-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84774-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84774-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84774-115">Not supported.</span></span>|
|<span data-ttu-id="84774-116">Application</span><span class="sxs-lookup"><span data-stu-id="84774-116">Application</span></span>|<span data-ttu-id="84774-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84774-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84774-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84774-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="84774-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84774-119">Request headers</span></span>
|<span data-ttu-id="84774-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84774-120">Header</span></span>|<span data-ttu-id="84774-121">Valor</span><span class="sxs-lookup"><span data-stu-id="84774-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84774-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="84774-122">Authorization</span></span>|<span data-ttu-id="84774-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84774-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84774-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84774-124">Accept</span></span>|<span data-ttu-id="84774-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84774-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84774-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84774-126">Request body</span></span>
<span data-ttu-id="84774-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="84774-127">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="84774-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="84774-128">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="84774-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84774-129">Property</span></span>|<span data-ttu-id="84774-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="84774-130">Type</span></span>|<span data-ttu-id="84774-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="84774-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84774-132">id</span><span class="sxs-lookup"><span data-stu-id="84774-132">id</span></span>|<span data-ttu-id="84774-133">String</span><span class="sxs-lookup"><span data-stu-id="84774-133">String</span></span>|<span data-ttu-id="84774-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="84774-134">UUID for the object</span></span>|
|<span data-ttu-id="84774-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="84774-135">eventDateTime</span></span>|<span data-ttu-id="84774-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84774-136">DateTimeOffset</span></span>|<span data-ttu-id="84774-137">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="84774-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="84774-138">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="84774-138">deviceRegisteredDateTime</span></span>|<span data-ttu-id="84774-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84774-139">DateTimeOffset</span></span>|<span data-ttu-id="84774-140">Data de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84774-140">Device registration date.</span></span>|
|<span data-ttu-id="84774-141">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="84774-141">enrollmentStartDateTime</span></span>|<span data-ttu-id="84774-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84774-142">DateTimeOffset</span></span>|<span data-ttu-id="84774-143">Data de início do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84774-143">Device enrollment start date.</span></span>|
|<span data-ttu-id="84774-144">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="84774-144">enrollmentType</span></span>|[<span data-ttu-id="84774-145">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="84774-145">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="84774-146">Tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="84774-146">Enrollment type.</span></span> <span data-ttu-id="84774-147">Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="84774-147">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="84774-148">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="84774-148">deviceSerialNumber</span></span>|<span data-ttu-id="84774-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84774-149">String</span></span>|<span data-ttu-id="84774-150">Número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84774-150">Device serial number.</span></span>|
|<span data-ttu-id="84774-151">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="84774-151">managedDeviceName</span></span>|<span data-ttu-id="84774-152">String</span><span class="sxs-lookup"><span data-stu-id="84774-152">String</span></span>|<span data-ttu-id="84774-153">Nome do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="84774-153">Managed device name.</span></span>|
|<span data-ttu-id="84774-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84774-154">userPrincipalName</span></span>|<span data-ttu-id="84774-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84774-155">String</span></span>|<span data-ttu-id="84774-156">Nome principal do usuário usado para registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84774-156">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="84774-157">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="84774-157">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="84774-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84774-158">String</span></span>|<span data-ttu-id="84774-159">Nome do perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="84774-159">Autopilot profile name.</span></span>|
|<span data-ttu-id="84774-160">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="84774-160">enrollmentState</span></span>|[<span data-ttu-id="84774-161">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="84774-161">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="84774-162">Estado de registro como cadastrado, falhou.</span><span class="sxs-lookup"><span data-stu-id="84774-162">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="84774-163">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="84774-163">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="84774-164">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="84774-164">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="84774-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84774-165">String</span></span>|<span data-ttu-id="84774-166">Nome do perfil da página de status do registro</span><span class="sxs-lookup"><span data-stu-id="84774-166">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="84774-167">DeploymentState</span><span class="sxs-lookup"><span data-stu-id="84774-167">deploymentState</span></span>|[<span data-ttu-id="84774-168">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="84774-168">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="84774-169">Estado de implantação como êxito, falha, InProgress, SuccessWithTimeout.</span><span class="sxs-lookup"><span data-stu-id="84774-169">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="84774-170">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="84774-170">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="84774-171">osVersion</span><span class="sxs-lookup"><span data-stu-id="84774-171">osVersion</span></span>|<span data-ttu-id="84774-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84774-172">String</span></span>|<span data-ttu-id="84774-173">Versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84774-173">Device operating system version.</span></span>|
|<span data-ttu-id="84774-174">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="84774-174">deploymentDuration</span></span>|<span data-ttu-id="84774-175">Duração</span><span class="sxs-lookup"><span data-stu-id="84774-175">Duration</span></span>|<span data-ttu-id="84774-176">Duração da implantação do piloto automático, incluindo registro.</span><span class="sxs-lookup"><span data-stu-id="84774-176">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="84774-177">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="84774-177">deploymentTotalDuration</span></span>|<span data-ttu-id="84774-178">Duração</span><span class="sxs-lookup"><span data-stu-id="84774-178">Duration</span></span>|<span data-ttu-id="84774-179">Duração total da implantação na tela de registro na área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84774-179">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="84774-180">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="84774-180">devicePreparationDuration</span></span>|<span data-ttu-id="84774-181">Duração</span><span class="sxs-lookup"><span data-stu-id="84774-181">Duration</span></span>|<span data-ttu-id="84774-182">Tempo gasto no registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84774-182">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="84774-183">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="84774-183">deviceSetupDuration</span></span>|<span data-ttu-id="84774-184">Duração</span><span class="sxs-lookup"><span data-stu-id="84774-184">Duration</span></span>|<span data-ttu-id="84774-185">Tempo gasto em ESP de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84774-185">Time spent in device ESP.</span></span>|
|<span data-ttu-id="84774-186">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="84774-186">accountSetupDuration</span></span>|<span data-ttu-id="84774-187">Duração</span><span class="sxs-lookup"><span data-stu-id="84774-187">Duration</span></span>|<span data-ttu-id="84774-188">Tempo gasto na ESP do usuário.</span><span class="sxs-lookup"><span data-stu-id="84774-188">Time spent in user ESP.</span></span>|
|<span data-ttu-id="84774-189">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="84774-189">deploymentStartDateTime</span></span>|<span data-ttu-id="84774-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84774-190">DateTimeOffset</span></span>|<span data-ttu-id="84774-191">Hora de início da implantação.</span><span class="sxs-lookup"><span data-stu-id="84774-191">Deployment start time.</span></span>|
|<span data-ttu-id="84774-192">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="84774-192">deploymentEndDateTime</span></span>|<span data-ttu-id="84774-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84774-193">DateTimeOffset</span></span>|<span data-ttu-id="84774-194">Hora de término da implantação.</span><span class="sxs-lookup"><span data-stu-id="84774-194">Deployment end time.</span></span>|
|<span data-ttu-id="84774-195">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="84774-195">targetedAppCount</span></span>|<span data-ttu-id="84774-196">Int32</span><span class="sxs-lookup"><span data-stu-id="84774-196">Int32</span></span>|<span data-ttu-id="84774-197">Contagem de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="84774-197">Count of applications targeted.</span></span>|
|<span data-ttu-id="84774-198">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="84774-198">targetedPolicyCount</span></span>|<span data-ttu-id="84774-199">Int32</span><span class="sxs-lookup"><span data-stu-id="84774-199">Int32</span></span>|<span data-ttu-id="84774-200">Contagem de políticas direcionadas.</span><span class="sxs-lookup"><span data-stu-id="84774-200">Count of policies targeted.</span></span>|
|<span data-ttu-id="84774-201">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="84774-201">enrollmentFailureDetails</span></span>|<span data-ttu-id="84774-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84774-202">String</span></span>|<span data-ttu-id="84774-203">Detalhes da falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="84774-203">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="84774-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="84774-204">Response</span></span>
<span data-ttu-id="84774-205">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84774-205">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84774-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84774-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="84774-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84774-207">Request</span></span>
<span data-ttu-id="84774-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84774-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1323

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
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

### <a name="response"></a><span data-ttu-id="84774-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="84774-209">Response</span></span>
<span data-ttu-id="84774-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84774-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1372

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
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






