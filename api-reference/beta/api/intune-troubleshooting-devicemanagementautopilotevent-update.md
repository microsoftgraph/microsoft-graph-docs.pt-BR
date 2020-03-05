---
title: Atualizar deviceManagementAutopilotEvent
description: Atualiza as propriedades de um objeto deviceManagementAutopilotEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db30ad9e855ae7371b055e033e4b1d8c6036125d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457710"
---
# <a name="update-devicemanagementautopilotevent"></a><span data-ttu-id="a49d8-103">Atualizar deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="a49d8-103">Update deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="a49d8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a49d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a49d8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a49d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a49d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a49d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a49d8-107">Atualiza as propriedades de um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="a49d8-107">Update the properties of a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a49d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a49d8-108">Prerequisites</span></span>
<span data-ttu-id="a49d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a49d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a49d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a49d8-111">Permission type</span></span>|<span data-ttu-id="a49d8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a49d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a49d8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a49d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a49d8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a49d8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a49d8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a49d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a49d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a49d8-116">Not supported.</span></span>|
|<span data-ttu-id="a49d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a49d8-117">Application</span></span>|<span data-ttu-id="a49d8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a49d8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a49d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a49d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="request-headers"></a><span data-ttu-id="a49d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a49d8-120">Request headers</span></span>
|<span data-ttu-id="a49d8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a49d8-121">Header</span></span>|<span data-ttu-id="a49d8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a49d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a49d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a49d8-123">Authorization</span></span>|<span data-ttu-id="a49d8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a49d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a49d8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a49d8-125">Accept</span></span>|<span data-ttu-id="a49d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a49d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a49d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a49d8-127">Request body</span></span>
<span data-ttu-id="a49d8-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="a49d8-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

<span data-ttu-id="a49d8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span><span class="sxs-lookup"><span data-stu-id="a49d8-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).</span></span>

|<span data-ttu-id="a49d8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a49d8-130">Property</span></span>|<span data-ttu-id="a49d8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a49d8-131">Type</span></span>|<span data-ttu-id="a49d8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a49d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a49d8-133">id</span><span class="sxs-lookup"><span data-stu-id="a49d8-133">id</span></span>|<span data-ttu-id="a49d8-134">String</span><span class="sxs-lookup"><span data-stu-id="a49d8-134">String</span></span>|<span data-ttu-id="a49d8-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="a49d8-135">UUID for the object</span></span>|
|<span data-ttu-id="a49d8-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a49d8-136">eventDateTime</span></span>|<span data-ttu-id="a49d8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49d8-137">DateTimeOffset</span></span>|<span data-ttu-id="a49d8-138">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="a49d8-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="a49d8-139">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="a49d8-139">deviceRegisteredDateTime</span></span>|<span data-ttu-id="a49d8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49d8-140">DateTimeOffset</span></span>|<span data-ttu-id="a49d8-141">Data de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a49d8-141">Device registration date.</span></span>|
|<span data-ttu-id="a49d8-142">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a49d8-142">enrollmentStartDateTime</span></span>|<span data-ttu-id="a49d8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49d8-143">DateTimeOffset</span></span>|<span data-ttu-id="a49d8-144">Data de início do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a49d8-144">Device enrollment start date.</span></span>|
|<span data-ttu-id="a49d8-145">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="a49d8-145">enrollmentType</span></span>|[<span data-ttu-id="a49d8-146">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a49d8-146">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="a49d8-147">Tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="a49d8-147">Enrollment type.</span></span> <span data-ttu-id="a49d8-148">Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="a49d8-148">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="a49d8-149">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="a49d8-149">deviceSerialNumber</span></span>|<span data-ttu-id="a49d8-150">String</span><span class="sxs-lookup"><span data-stu-id="a49d8-150">String</span></span>|<span data-ttu-id="a49d8-151">Número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a49d8-151">Device serial number.</span></span>|
|<span data-ttu-id="a49d8-152">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="a49d8-152">managedDeviceName</span></span>|<span data-ttu-id="a49d8-153">String</span><span class="sxs-lookup"><span data-stu-id="a49d8-153">String</span></span>|<span data-ttu-id="a49d8-154">Nome do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="a49d8-154">Managed device name.</span></span>|
|<span data-ttu-id="a49d8-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a49d8-155">userPrincipalName</span></span>|<span data-ttu-id="a49d8-156">String</span><span class="sxs-lookup"><span data-stu-id="a49d8-156">String</span></span>|<span data-ttu-id="a49d8-157">Nome principal do usuário usado para registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a49d8-157">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="a49d8-158">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="a49d8-158">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="a49d8-159">String</span><span class="sxs-lookup"><span data-stu-id="a49d8-159">String</span></span>|<span data-ttu-id="a49d8-160">Nome do perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="a49d8-160">Autopilot profile name.</span></span>|
|<span data-ttu-id="a49d8-161">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="a49d8-161">enrollmentState</span></span>|[<span data-ttu-id="a49d8-162">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="a49d8-162">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="a49d8-163">Estado de registro como cadastrado, falhou.</span><span class="sxs-lookup"><span data-stu-id="a49d8-163">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="a49d8-164">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="a49d8-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a49d8-165">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="a49d8-165">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="a49d8-166">String</span><span class="sxs-lookup"><span data-stu-id="a49d8-166">String</span></span>|<span data-ttu-id="a49d8-167">Nome do perfil da página de status do registro</span><span class="sxs-lookup"><span data-stu-id="a49d8-167">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="a49d8-168">DeploymentState</span><span class="sxs-lookup"><span data-stu-id="a49d8-168">deploymentState</span></span>|[<span data-ttu-id="a49d8-169">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="a49d8-169">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="a49d8-170">Estado de implantação como êxito, falha, InProgress, SuccessWithTimeout.</span><span class="sxs-lookup"><span data-stu-id="a49d8-170">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="a49d8-171">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span><span class="sxs-lookup"><span data-stu-id="a49d8-171">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.</span></span>|
|<span data-ttu-id="a49d8-172">osVersion</span><span class="sxs-lookup"><span data-stu-id="a49d8-172">osVersion</span></span>|<span data-ttu-id="a49d8-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a49d8-173">String</span></span>|<span data-ttu-id="a49d8-174">Versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a49d8-174">Device operating system version.</span></span>|
|<span data-ttu-id="a49d8-175">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="a49d8-175">deploymentDuration</span></span>|<span data-ttu-id="a49d8-176">Duração</span><span class="sxs-lookup"><span data-stu-id="a49d8-176">Duration</span></span>|<span data-ttu-id="a49d8-177">Duração da implantação do piloto automático, incluindo registro.</span><span class="sxs-lookup"><span data-stu-id="a49d8-177">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="a49d8-178">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="a49d8-178">deploymentTotalDuration</span></span>|<span data-ttu-id="a49d8-179">Duração</span><span class="sxs-lookup"><span data-stu-id="a49d8-179">Duration</span></span>|<span data-ttu-id="a49d8-180">Duração total da implantação na tela de registro na área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a49d8-180">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="a49d8-181">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="a49d8-181">devicePreparationDuration</span></span>|<span data-ttu-id="a49d8-182">Duração</span><span class="sxs-lookup"><span data-stu-id="a49d8-182">Duration</span></span>|<span data-ttu-id="a49d8-183">Tempo gasto no registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a49d8-183">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="a49d8-184">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="a49d8-184">deviceSetupDuration</span></span>|<span data-ttu-id="a49d8-185">Duração</span><span class="sxs-lookup"><span data-stu-id="a49d8-185">Duration</span></span>|<span data-ttu-id="a49d8-186">Tempo gasto em ESP de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a49d8-186">Time spent in device ESP.</span></span>|
|<span data-ttu-id="a49d8-187">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="a49d8-187">accountSetupDuration</span></span>|<span data-ttu-id="a49d8-188">Duração</span><span class="sxs-lookup"><span data-stu-id="a49d8-188">Duration</span></span>|<span data-ttu-id="a49d8-189">Tempo gasto na ESP do usuário.</span><span class="sxs-lookup"><span data-stu-id="a49d8-189">Time spent in user ESP.</span></span>|
|<span data-ttu-id="a49d8-190">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a49d8-190">deploymentStartDateTime</span></span>|<span data-ttu-id="a49d8-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49d8-191">DateTimeOffset</span></span>|<span data-ttu-id="a49d8-192">Hora de início da implantação.</span><span class="sxs-lookup"><span data-stu-id="a49d8-192">Deployment start time.</span></span>|
|<span data-ttu-id="a49d8-193">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="a49d8-193">deploymentEndDateTime</span></span>|<span data-ttu-id="a49d8-194">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49d8-194">DateTimeOffset</span></span>|<span data-ttu-id="a49d8-195">Hora de término da implantação.</span><span class="sxs-lookup"><span data-stu-id="a49d8-195">Deployment end time.</span></span>|
|<span data-ttu-id="a49d8-196">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="a49d8-196">targetedAppCount</span></span>|<span data-ttu-id="a49d8-197">Int32</span><span class="sxs-lookup"><span data-stu-id="a49d8-197">Int32</span></span>|<span data-ttu-id="a49d8-198">Contagem de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="a49d8-198">Count of applications targeted.</span></span>|
|<span data-ttu-id="a49d8-199">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="a49d8-199">targetedPolicyCount</span></span>|<span data-ttu-id="a49d8-200">Int32</span><span class="sxs-lookup"><span data-stu-id="a49d8-200">Int32</span></span>|<span data-ttu-id="a49d8-201">Contagem de políticas direcionadas.</span><span class="sxs-lookup"><span data-stu-id="a49d8-201">Count of policies targeted.</span></span>|
|<span data-ttu-id="a49d8-202">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="a49d8-202">enrollmentFailureDetails</span></span>|<span data-ttu-id="a49d8-203">String</span><span class="sxs-lookup"><span data-stu-id="a49d8-203">String</span></span>|<span data-ttu-id="a49d8-204">Detalhes da falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="a49d8-204">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="a49d8-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="a49d8-205">Response</span></span>
<span data-ttu-id="a49d8-206">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a49d8-206">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a49d8-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a49d8-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="a49d8-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a49d8-208">Request</span></span>
<span data-ttu-id="a49d8-209">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a49d8-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
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

### <a name="response"></a><span data-ttu-id="a49d8-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="a49d8-210">Response</span></span>
<span data-ttu-id="a49d8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a49d8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





