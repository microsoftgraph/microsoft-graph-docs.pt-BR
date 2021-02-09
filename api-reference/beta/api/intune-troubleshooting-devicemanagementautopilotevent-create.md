---
title: Criar deviceManagementAutopilotEvent
description: Crie um novo objeto deviceManagementAutopilotEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 411e7dd15a8f3fe75d726f0caab38c7592b3a8a6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159210"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="07d0f-103">Criar deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="07d0f-103">Create deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="07d0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07d0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07d0f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07d0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07d0f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07d0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07d0f-107">Crie um novo [objeto deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)</span><span class="sxs-lookup"><span data-stu-id="07d0f-107">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07d0f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07d0f-108">Prerequisites</span></span>
<span data-ttu-id="07d0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d0f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07d0f-111">Permission type</span></span>|<span data-ttu-id="07d0f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07d0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07d0f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07d0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07d0f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d0f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="07d0f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07d0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07d0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07d0f-116">Not supported.</span></span>|
|<span data-ttu-id="07d0f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07d0f-117">Application</span></span>|<span data-ttu-id="07d0f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d0f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07d0f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07d0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="07d0f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07d0f-120">Request headers</span></span>
|<span data-ttu-id="07d0f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07d0f-121">Header</span></span>|<span data-ttu-id="07d0f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="07d0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07d0f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07d0f-123">Authorization</span></span>|<span data-ttu-id="07d0f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07d0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07d0f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07d0f-125">Accept</span></span>|<span data-ttu-id="07d0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07d0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07d0f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07d0f-127">Request body</span></span>
<span data-ttu-id="07d0f-128">No corpo da solicitação, fornece uma representação JSON do objeto deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="07d0f-128">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="07d0f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="07d0f-129">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="07d0f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07d0f-130">Property</span></span>|<span data-ttu-id="07d0f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="07d0f-131">Type</span></span>|<span data-ttu-id="07d0f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="07d0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07d0f-133">id</span><span class="sxs-lookup"><span data-stu-id="07d0f-133">id</span></span>|<span data-ttu-id="07d0f-134">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-134">String</span></span>|<span data-ttu-id="07d0f-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="07d0f-135">UUID for the object</span></span>|
|<span data-ttu-id="07d0f-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="07d0f-136">deviceId</span></span>|<span data-ttu-id="07d0f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07d0f-137">String</span></span>|<span data-ttu-id="07d0f-138">ID do dispositivo associada ao objeto</span><span class="sxs-lookup"><span data-stu-id="07d0f-138">Device id associated with the object</span></span>|
|<span data-ttu-id="07d0f-139">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="07d0f-139">eventDateTime</span></span>|<span data-ttu-id="07d0f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d0f-140">DateTimeOffset</span></span>|<span data-ttu-id="07d0f-141">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="07d0f-141">Time when the event occurred .</span></span>|
|<span data-ttu-id="07d0f-142">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="07d0f-142">deviceRegisteredDateTime</span></span>|<span data-ttu-id="07d0f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d0f-143">DateTimeOffset</span></span>|<span data-ttu-id="07d0f-144">Data de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07d0f-144">Device registration date.</span></span>|
|<span data-ttu-id="07d0f-145">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="07d0f-145">enrollmentStartDateTime</span></span>|<span data-ttu-id="07d0f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d0f-146">DateTimeOffset</span></span>|<span data-ttu-id="07d0f-147">Data de início do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07d0f-147">Device enrollment start date.</span></span>|
|<span data-ttu-id="07d0f-148">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="07d0f-148">enrollmentType</span></span>|[<span data-ttu-id="07d0f-149">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="07d0f-149">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="07d0f-150">Tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="07d0f-150">Enrollment type.</span></span> <span data-ttu-id="07d0f-151">Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="07d0f-151">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="07d0f-152">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="07d0f-152">deviceSerialNumber</span></span>|<span data-ttu-id="07d0f-153">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-153">String</span></span>|<span data-ttu-id="07d0f-154">Número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07d0f-154">Device serial number.</span></span>|
|<span data-ttu-id="07d0f-155">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="07d0f-155">managedDeviceName</span></span>|<span data-ttu-id="07d0f-156">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-156">String</span></span>|<span data-ttu-id="07d0f-157">Nome do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="07d0f-157">Managed device name.</span></span>|
|<span data-ttu-id="07d0f-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="07d0f-158">userPrincipalName</span></span>|<span data-ttu-id="07d0f-159">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-159">String</span></span>|<span data-ttu-id="07d0f-160">Nome principal do usuário usado para registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07d0f-160">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="07d0f-161">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="07d0f-161">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="07d0f-162">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-162">String</span></span>|<span data-ttu-id="07d0f-163">Nome do perfil do Autopilot.</span><span class="sxs-lookup"><span data-stu-id="07d0f-163">Autopilot profile name.</span></span>|
|<span data-ttu-id="07d0f-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="07d0f-164">enrollmentState</span></span>|[<span data-ttu-id="07d0f-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="07d0f-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="07d0f-166">Estado de registro como Registro, Falha.</span><span class="sxs-lookup"><span data-stu-id="07d0f-166">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="07d0f-167">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="07d0f-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="07d0f-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="07d0f-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="07d0f-169">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-169">String</span></span>|<span data-ttu-id="07d0f-170">Nome do perfil da Página de Status do Registro</span><span class="sxs-lookup"><span data-stu-id="07d0f-170">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="07d0f-171">windows10EnrollmentCompletionPageConfigurationId</span><span class="sxs-lookup"><span data-stu-id="07d0f-171">windows10EnrollmentCompletionPageConfigurationId</span></span>|<span data-ttu-id="07d0f-172">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-172">String</span></span>|<span data-ttu-id="07d0f-173">ID do perfil da Página de Status do Registro</span><span class="sxs-lookup"><span data-stu-id="07d0f-173">Enrollment Status Page profile ID</span></span>|
|<span data-ttu-id="07d0f-174">deploymentState</span><span class="sxs-lookup"><span data-stu-id="07d0f-174">deploymentState</span></span>|[<span data-ttu-id="07d0f-175">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="07d0f-175">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="07d0f-176">Estado de implantação como Êxito, Falha, InProgress, SuccessWithTimeout.</span><span class="sxs-lookup"><span data-stu-id="07d0f-176">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="07d0f-177">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="07d0f-177">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="07d0f-178">deviceSetupStatus</span><span class="sxs-lookup"><span data-stu-id="07d0f-178">deviceSetupStatus</span></span>|[<span data-ttu-id="07d0f-179">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="07d0f-179">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="07d0f-180">Status de implantação da fase de configuração do dispositivo da página de status do registro.</span><span class="sxs-lookup"><span data-stu-id="07d0f-180">Deployment status for the enrollment status page device setup phase.</span></span> <span data-ttu-id="07d0f-181">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="07d0f-181">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="07d0f-182">accountSetupStatus</span><span class="sxs-lookup"><span data-stu-id="07d0f-182">accountSetupStatus</span></span>|[<span data-ttu-id="07d0f-183">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="07d0f-183">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="07d0f-184">Status de implantação da fase de configuração da conta da página de status do registro.</span><span class="sxs-lookup"><span data-stu-id="07d0f-184">Deployment status for the enrollment status page account setup phase.</span></span> <span data-ttu-id="07d0f-185">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="07d0f-185">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="07d0f-186">osVersion</span><span class="sxs-lookup"><span data-stu-id="07d0f-186">osVersion</span></span>|<span data-ttu-id="07d0f-187">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-187">String</span></span>|<span data-ttu-id="07d0f-188">Versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07d0f-188">Device operating system version.</span></span>|
|<span data-ttu-id="07d0f-189">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="07d0f-189">deploymentDuration</span></span>|<span data-ttu-id="07d0f-190">Duration</span><span class="sxs-lookup"><span data-stu-id="07d0f-190">Duration</span></span>|<span data-ttu-id="07d0f-191">Duração da implantação do Autopilot, incluindo o registro.</span><span class="sxs-lookup"><span data-stu-id="07d0f-191">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="07d0f-192">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="07d0f-192">deploymentTotalDuration</span></span>|<span data-ttu-id="07d0f-193">Duration</span><span class="sxs-lookup"><span data-stu-id="07d0f-193">Duration</span></span>|<span data-ttu-id="07d0f-194">Duração total da implantação do registro na tela área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="07d0f-194">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="07d0f-195">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="07d0f-195">devicePreparationDuration</span></span>|<span data-ttu-id="07d0f-196">Duration</span><span class="sxs-lookup"><span data-stu-id="07d0f-196">Duration</span></span>|<span data-ttu-id="07d0f-197">Tempo gasto no registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07d0f-197">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="07d0f-198">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="07d0f-198">deviceSetupDuration</span></span>|<span data-ttu-id="07d0f-199">Duration</span><span class="sxs-lookup"><span data-stu-id="07d0f-199">Duration</span></span>|<span data-ttu-id="07d0f-200">Tempo gasto no dispositivo ESP.</span><span class="sxs-lookup"><span data-stu-id="07d0f-200">Time spent in device ESP.</span></span>|
|<span data-ttu-id="07d0f-201">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="07d0f-201">accountSetupDuration</span></span>|<span data-ttu-id="07d0f-202">Duration</span><span class="sxs-lookup"><span data-stu-id="07d0f-202">Duration</span></span>|<span data-ttu-id="07d0f-203">Tempo gasto no ESP do usuário.</span><span class="sxs-lookup"><span data-stu-id="07d0f-203">Time spent in user ESP.</span></span>|
|<span data-ttu-id="07d0f-204">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="07d0f-204">deploymentStartDateTime</span></span>|<span data-ttu-id="07d0f-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d0f-205">DateTimeOffset</span></span>|<span data-ttu-id="07d0f-206">Hora de início da implantação.</span><span class="sxs-lookup"><span data-stu-id="07d0f-206">Deployment start time.</span></span>|
|<span data-ttu-id="07d0f-207">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="07d0f-207">deploymentEndDateTime</span></span>|<span data-ttu-id="07d0f-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d0f-208">DateTimeOffset</span></span>|<span data-ttu-id="07d0f-209">Hora de término da implantação.</span><span class="sxs-lookup"><span data-stu-id="07d0f-209">Deployment end time.</span></span>|
|<span data-ttu-id="07d0f-210">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="07d0f-210">targetedAppCount</span></span>|<span data-ttu-id="07d0f-211">Int32</span><span class="sxs-lookup"><span data-stu-id="07d0f-211">Int32</span></span>|<span data-ttu-id="07d0f-212">Contagem de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="07d0f-212">Count of applications targeted.</span></span>|
|<span data-ttu-id="07d0f-213">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="07d0f-213">targetedPolicyCount</span></span>|<span data-ttu-id="07d0f-214">Int32</span><span class="sxs-lookup"><span data-stu-id="07d0f-214">Int32</span></span>|<span data-ttu-id="07d0f-215">Contagem de políticas direcionadas.</span><span class="sxs-lookup"><span data-stu-id="07d0f-215">Count of policies targeted.</span></span>|
|<span data-ttu-id="07d0f-216">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="07d0f-216">enrollmentFailureDetails</span></span>|<span data-ttu-id="07d0f-217">String</span><span class="sxs-lookup"><span data-stu-id="07d0f-217">String</span></span>|<span data-ttu-id="07d0f-218">Detalhes da falha do registro.</span><span class="sxs-lookup"><span data-stu-id="07d0f-218">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="07d0f-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="07d0f-219">Response</span></span>
<span data-ttu-id="07d0f-220">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07d0f-220">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07d0f-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07d0f-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="07d0f-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07d0f-222">Request</span></span>
<span data-ttu-id="07d0f-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07d0f-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1545

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
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
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

### <a name="response"></a><span data-ttu-id="07d0f-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="07d0f-224">Response</span></span>
<span data-ttu-id="07d0f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07d0f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1594

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
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
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




