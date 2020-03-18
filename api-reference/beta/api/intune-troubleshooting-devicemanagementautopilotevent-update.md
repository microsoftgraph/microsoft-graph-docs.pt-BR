---
title: Atualizar deviceManagementAutopilotEvent
description: Atualiza as propriedades de um objeto deviceManagementAutopilotEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea3703d23eb45e9c91dd40cbd3cb3031b7e2cd30
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800232"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="095d7-103">Atualizar deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="095d7-103">Update deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="095d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="095d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="095d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="095d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="095d7-106">Atualiza as propriedades de um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="095d7-106">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="095d7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="095d7-107">Prerequisites</span></span>
<span data-ttu-id="095d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="095d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="095d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="095d7-110">Permission type</span></span>|<span data-ttu-id="095d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="095d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="095d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="095d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="095d7-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="095d7-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="095d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="095d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="095d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="095d7-115">Not supported.</span></span>|
|<span data-ttu-id="095d7-116">Application</span><span class="sxs-lookup"><span data-stu-id="095d7-116">Application</span></span>|<span data-ttu-id="095d7-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="095d7-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="095d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="095d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="095d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="095d7-119">Request headers</span></span>
|<span data-ttu-id="095d7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="095d7-120">Header</span></span>|<span data-ttu-id="095d7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="095d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="095d7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="095d7-122">Authorization</span></span>|<span data-ttu-id="095d7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="095d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="095d7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="095d7-124">Accept</span></span>|<span data-ttu-id="095d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="095d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="095d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="095d7-126">Request body</span></span>
<span data-ttu-id="095d7-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="095d7-127">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="095d7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span><span class="sxs-lookup"><span data-stu-id="095d7-128">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="095d7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="095d7-129">Property</span></span>|<span data-ttu-id="095d7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="095d7-130">Type</span></span>|<span data-ttu-id="095d7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="095d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="095d7-132">id</span><span class="sxs-lookup"><span data-stu-id="095d7-132">id</span></span>|<span data-ttu-id="095d7-133">String</span><span class="sxs-lookup"><span data-stu-id="095d7-133">String</span></span>|<span data-ttu-id="095d7-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="095d7-134">UUID for the object</span></span>|
|<span data-ttu-id="095d7-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="095d7-135">deviceId</span></span>|<span data-ttu-id="095d7-136">String</span><span class="sxs-lookup"><span data-stu-id="095d7-136">String</span></span>|<span data-ttu-id="095d7-137">ID de dispositivo associada ao objeto</span><span class="sxs-lookup"><span data-stu-id="095d7-137">Device id associated with the object</span></span>|
|<span data-ttu-id="095d7-138">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="095d7-138">eventDateTime</span></span>|<span data-ttu-id="095d7-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="095d7-139">DateTimeOffset</span></span>|<span data-ttu-id="095d7-140">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="095d7-140">Time when the event occurred .</span></span>|
|<span data-ttu-id="095d7-141">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="095d7-141">deviceRegisteredDateTime</span></span>|<span data-ttu-id="095d7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="095d7-142">DateTimeOffset</span></span>|<span data-ttu-id="095d7-143">Data de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="095d7-143">Device registration date.</span></span>|
|<span data-ttu-id="095d7-144">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="095d7-144">enrollmentStartDateTime</span></span>|<span data-ttu-id="095d7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="095d7-145">DateTimeOffset</span></span>|<span data-ttu-id="095d7-146">Data de início do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="095d7-146">Device enrollment start date.</span></span>|
|<span data-ttu-id="095d7-147">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="095d7-147">enrollmentType</span></span>|[<span data-ttu-id="095d7-148">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="095d7-148">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="095d7-149">Tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="095d7-149">Enrollment type.</span></span> <span data-ttu-id="095d7-150">Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="095d7-150">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="095d7-151">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="095d7-151">deviceSerialNumber</span></span>|<span data-ttu-id="095d7-152">String</span><span class="sxs-lookup"><span data-stu-id="095d7-152">String</span></span>|<span data-ttu-id="095d7-153">Número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="095d7-153">Device serial number.</span></span>|
|<span data-ttu-id="095d7-154">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="095d7-154">managedDeviceName</span></span>|<span data-ttu-id="095d7-155">String</span><span class="sxs-lookup"><span data-stu-id="095d7-155">String</span></span>|<span data-ttu-id="095d7-156">Nome do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="095d7-156">Managed device name.</span></span>|
|<span data-ttu-id="095d7-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="095d7-157">userPrincipalName</span></span>|<span data-ttu-id="095d7-158">String</span><span class="sxs-lookup"><span data-stu-id="095d7-158">String</span></span>|<span data-ttu-id="095d7-159">Nome principal do usuário usado para registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="095d7-159">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="095d7-160">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="095d7-160">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="095d7-161">String</span><span class="sxs-lookup"><span data-stu-id="095d7-161">String</span></span>|<span data-ttu-id="095d7-162">Nome do perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="095d7-162">Autopilot profile name.</span></span>|
|<span data-ttu-id="095d7-163">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="095d7-163">enrollmentState</span></span>|[<span data-ttu-id="095d7-164">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="095d7-164">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="095d7-165">Estado de registro como cadastrado, falhou.</span><span class="sxs-lookup"><span data-stu-id="095d7-165">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="095d7-166">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="095d7-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="095d7-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="095d7-167">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="095d7-168">String</span><span class="sxs-lookup"><span data-stu-id="095d7-168">String</span></span>|<span data-ttu-id="095d7-169">Nome do perfil da página de status do registro</span><span class="sxs-lookup"><span data-stu-id="095d7-169">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="095d7-170">DeploymentState</span><span class="sxs-lookup"><span data-stu-id="095d7-170">deploymentState</span></span>|[<span data-ttu-id="095d7-171">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="095d7-171">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="095d7-172">Estado de implantação como êxito, falha, InProgress, SuccessWithTimeout.</span><span class="sxs-lookup"><span data-stu-id="095d7-172">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="095d7-173">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="095d7-173">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="095d7-174">osVersion</span><span class="sxs-lookup"><span data-stu-id="095d7-174">osVersion</span></span>|<span data-ttu-id="095d7-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="095d7-175">String</span></span>|<span data-ttu-id="095d7-176">Versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="095d7-176">Device operating system version.</span></span>|
|<span data-ttu-id="095d7-177">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="095d7-177">deploymentDuration</span></span>|<span data-ttu-id="095d7-178">Duração</span><span class="sxs-lookup"><span data-stu-id="095d7-178">Duration</span></span>|<span data-ttu-id="095d7-179">Duração da implantação do piloto automático, incluindo registro.</span><span class="sxs-lookup"><span data-stu-id="095d7-179">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="095d7-180">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="095d7-180">deploymentTotalDuration</span></span>|<span data-ttu-id="095d7-181">Duração</span><span class="sxs-lookup"><span data-stu-id="095d7-181">Duration</span></span>|<span data-ttu-id="095d7-182">Duração total da implantação na tela de registro na área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="095d7-182">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="095d7-183">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="095d7-183">devicePreparationDuration</span></span>|<span data-ttu-id="095d7-184">Duração</span><span class="sxs-lookup"><span data-stu-id="095d7-184">Duration</span></span>|<span data-ttu-id="095d7-185">Tempo gasto no registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="095d7-185">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="095d7-186">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="095d7-186">deviceSetupDuration</span></span>|<span data-ttu-id="095d7-187">Duração</span><span class="sxs-lookup"><span data-stu-id="095d7-187">Duration</span></span>|<span data-ttu-id="095d7-188">Tempo gasto em ESP de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="095d7-188">Time spent in device ESP.</span></span>|
|<span data-ttu-id="095d7-189">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="095d7-189">accountSetupDuration</span></span>|<span data-ttu-id="095d7-190">Duração</span><span class="sxs-lookup"><span data-stu-id="095d7-190">Duration</span></span>|<span data-ttu-id="095d7-191">Tempo gasto na ESP do usuário.</span><span class="sxs-lookup"><span data-stu-id="095d7-191">Time spent in user ESP.</span></span>|
|<span data-ttu-id="095d7-192">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="095d7-192">deploymentStartDateTime</span></span>|<span data-ttu-id="095d7-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="095d7-193">DateTimeOffset</span></span>|<span data-ttu-id="095d7-194">Hora de início da implantação.</span><span class="sxs-lookup"><span data-stu-id="095d7-194">Deployment start time.</span></span>|
|<span data-ttu-id="095d7-195">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="095d7-195">deploymentEndDateTime</span></span>|<span data-ttu-id="095d7-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="095d7-196">DateTimeOffset</span></span>|<span data-ttu-id="095d7-197">Hora de término da implantação.</span><span class="sxs-lookup"><span data-stu-id="095d7-197">Deployment end time.</span></span>|
|<span data-ttu-id="095d7-198">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="095d7-198">targetedAppCount</span></span>|<span data-ttu-id="095d7-199">Int32</span><span class="sxs-lookup"><span data-stu-id="095d7-199">Int32</span></span>|<span data-ttu-id="095d7-200">Contagem de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="095d7-200">Count of applications targeted.</span></span>|
|<span data-ttu-id="095d7-201">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="095d7-201">targetedPolicyCount</span></span>|<span data-ttu-id="095d7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="095d7-202">Int32</span></span>|<span data-ttu-id="095d7-203">Contagem de políticas direcionadas.</span><span class="sxs-lookup"><span data-stu-id="095d7-203">Count of policies targeted.</span></span>|
|<span data-ttu-id="095d7-204">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="095d7-204">enrollmentFailureDetails</span></span>|<span data-ttu-id="095d7-205">String</span><span class="sxs-lookup"><span data-stu-id="095d7-205">String</span></span>|<span data-ttu-id="095d7-206">Detalhes da falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="095d7-206">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="095d7-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="095d7-207">Response</span></span>
<span data-ttu-id="095d7-208">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="095d7-208">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="095d7-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="095d7-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="095d7-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="095d7-210">Request</span></span>
<span data-ttu-id="095d7-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="095d7-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
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

### <a name="response"></a><span data-ttu-id="095d7-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="095d7-212">Response</span></span>
<span data-ttu-id="095d7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="095d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




