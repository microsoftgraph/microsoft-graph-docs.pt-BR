---
title: Criar deviceManagementAutopilotEvent
description: Crie um novo objeto deviceManagementAutopilotEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce61e72124fc58b710d17d246827e65edf133b38
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156027"
---
# <a name="create-devicemanagementautopilotevent"></a><span data-ttu-id="efa37-103">Criar deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="efa37-103">Create deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="efa37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efa37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efa37-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="efa37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efa37-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efa37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa37-107">Crie um novo [objeto deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)</span><span class="sxs-lookup"><span data-stu-id="efa37-107">Create a new [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efa37-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efa37-108">Prerequisites</span></span>
<span data-ttu-id="efa37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efa37-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efa37-111">Permission type</span></span>|<span data-ttu-id="efa37-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efa37-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efa37-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efa37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efa37-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa37-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="efa37-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efa37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efa37-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efa37-116">Not supported.</span></span>|
|<span data-ttu-id="efa37-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efa37-117">Application</span></span>|<span data-ttu-id="efa37-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa37-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efa37-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efa37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="efa37-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efa37-120">Request headers</span></span>
|<span data-ttu-id="efa37-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efa37-121">Header</span></span>|<span data-ttu-id="efa37-122">Valor</span><span class="sxs-lookup"><span data-stu-id="efa37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efa37-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efa37-123">Authorization</span></span>|<span data-ttu-id="efa37-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efa37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efa37-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efa37-125">Accept</span></span>|<span data-ttu-id="efa37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efa37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efa37-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efa37-127">Request body</span></span>
<span data-ttu-id="efa37-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="efa37-128">In the request body, supply a JSON representation for the deviceManagementAutopilotEvent object.</span></span>

<span data-ttu-id="efa37-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotEvent.</span><span class="sxs-lookup"><span data-stu-id="efa37-129">The following table shows the properties that are required when you create the deviceManagementAutopilotEvent.</span></span>

|<span data-ttu-id="efa37-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efa37-130">Property</span></span>|<span data-ttu-id="efa37-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efa37-131">Type</span></span>|<span data-ttu-id="efa37-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efa37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa37-133">id</span><span class="sxs-lookup"><span data-stu-id="efa37-133">id</span></span>|<span data-ttu-id="efa37-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa37-134">String</span></span>|<span data-ttu-id="efa37-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="efa37-135">UUID for the object</span></span>|
|<span data-ttu-id="efa37-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="efa37-136">deviceId</span></span>|<span data-ttu-id="efa37-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa37-137">String</span></span>|<span data-ttu-id="efa37-138">ID do dispositivo associada ao objeto</span><span class="sxs-lookup"><span data-stu-id="efa37-138">Device id associated with the object</span></span>|
|<span data-ttu-id="efa37-139">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="efa37-139">eventDateTime</span></span>|<span data-ttu-id="efa37-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa37-140">DateTimeOffset</span></span>|<span data-ttu-id="efa37-141">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="efa37-141">Time when the event occurred .</span></span>|
|<span data-ttu-id="efa37-142">deviceRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="efa37-142">deviceRegisteredDateTime</span></span>|<span data-ttu-id="efa37-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa37-143">DateTimeOffset</span></span>|<span data-ttu-id="efa37-144">Data do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa37-144">Device registration date.</span></span>|
|<span data-ttu-id="efa37-145">enrollmentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="efa37-145">enrollmentStartDateTime</span></span>|<span data-ttu-id="efa37-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa37-146">DateTimeOffset</span></span>|<span data-ttu-id="efa37-147">Data de início do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa37-147">Device enrollment start date.</span></span>|
|<span data-ttu-id="efa37-148">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="efa37-148">enrollmentType</span></span>|[<span data-ttu-id="efa37-149">windowsAutopilotEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="efa37-149">windowsAutopilotEnrollmentType</span></span>](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|<span data-ttu-id="efa37-150">Tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="efa37-150">Enrollment type.</span></span> <span data-ttu-id="efa37-151">Os valores possíveis são: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span><span class="sxs-lookup"><span data-stu-id="efa37-151">Possible values are: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.</span></span>|
|<span data-ttu-id="efa37-152">deviceSerialNumber</span><span class="sxs-lookup"><span data-stu-id="efa37-152">deviceSerialNumber</span></span>|<span data-ttu-id="efa37-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa37-153">String</span></span>|<span data-ttu-id="efa37-154">Número de série do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa37-154">Device serial number.</span></span>|
|<span data-ttu-id="efa37-155">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="efa37-155">managedDeviceName</span></span>|<span data-ttu-id="efa37-156">String</span><span class="sxs-lookup"><span data-stu-id="efa37-156">String</span></span>|<span data-ttu-id="efa37-157">Nome do dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="efa37-157">Managed device name.</span></span>|
|<span data-ttu-id="efa37-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="efa37-158">userPrincipalName</span></span>|<span data-ttu-id="efa37-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa37-159">String</span></span>|<span data-ttu-id="efa37-160">Nome principal do usuário usado para registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa37-160">User principal name used to enroll the device.</span></span>|
|<span data-ttu-id="efa37-161">windowsAutopilotDeploymentProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="efa37-161">windowsAutopilotDeploymentProfileDisplayName</span></span>|<span data-ttu-id="efa37-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa37-162">String</span></span>|<span data-ttu-id="efa37-163">Nome do perfil do piloto automático.</span><span class="sxs-lookup"><span data-stu-id="efa37-163">Autopilot profile name.</span></span>|
|<span data-ttu-id="efa37-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="efa37-164">enrollmentState</span></span>|[<span data-ttu-id="efa37-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="efa37-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="efa37-166">Estado de registro como Inscrito, Falha.</span><span class="sxs-lookup"><span data-stu-id="efa37-166">Enrollment state like Enrolled, Failed.</span></span> <span data-ttu-id="efa37-167">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="efa37-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="efa37-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span><span class="sxs-lookup"><span data-stu-id="efa37-168">windows10EnrollmentCompletionPageConfigurationDisplayName</span></span>|<span data-ttu-id="efa37-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa37-169">String</span></span>|<span data-ttu-id="efa37-170">Nome do perfil da Página de Status do Registro</span><span class="sxs-lookup"><span data-stu-id="efa37-170">Enrollment Status Page profile name</span></span>|
|<span data-ttu-id="efa37-171">windows10EnrollmentCompletionPageConfigurationId</span><span class="sxs-lookup"><span data-stu-id="efa37-171">windows10EnrollmentCompletionPageConfigurationId</span></span>|<span data-ttu-id="efa37-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa37-172">String</span></span>|<span data-ttu-id="efa37-173">ID do perfil da página de status de registro</span><span class="sxs-lookup"><span data-stu-id="efa37-173">Enrollment Status Page profile ID</span></span>|
|<span data-ttu-id="efa37-174">deploymentState</span><span class="sxs-lookup"><span data-stu-id="efa37-174">deploymentState</span></span>|[<span data-ttu-id="efa37-175">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="efa37-175">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="efa37-176">Estado de implantação como Sucesso, Falha, InProgress, SuccessWithTimeout.</span><span class="sxs-lookup"><span data-stu-id="efa37-176">Deployment state like Success, Failure, InProgress, SuccessWithTimeout.</span></span> <span data-ttu-id="efa37-177">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="efa37-177">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="efa37-178">deviceSetupStatus</span><span class="sxs-lookup"><span data-stu-id="efa37-178">deviceSetupStatus</span></span>|[<span data-ttu-id="efa37-179">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="efa37-179">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="efa37-180">Status de implantação para a fase de configuração do dispositivo de página de status de registro.</span><span class="sxs-lookup"><span data-stu-id="efa37-180">Deployment status for the enrollment status page device setup phase.</span></span> <span data-ttu-id="efa37-181">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="efa37-181">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="efa37-182">accountSetupStatus</span><span class="sxs-lookup"><span data-stu-id="efa37-182">accountSetupStatus</span></span>|[<span data-ttu-id="efa37-183">windowsAutopilotDeploymentState</span><span class="sxs-lookup"><span data-stu-id="efa37-183">windowsAutopilotDeploymentState</span></span>](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|<span data-ttu-id="efa37-184">Status de implantação para a fase de configuração da conta de página de status de registro.</span><span class="sxs-lookup"><span data-stu-id="efa37-184">Deployment status for the enrollment status page account setup phase.</span></span> <span data-ttu-id="efa37-185">Os valores possíveis são: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="efa37-185">Possible values are: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.</span></span>|
|<span data-ttu-id="efa37-186">osVersion</span><span class="sxs-lookup"><span data-stu-id="efa37-186">osVersion</span></span>|<span data-ttu-id="efa37-187">String</span><span class="sxs-lookup"><span data-stu-id="efa37-187">String</span></span>|<span data-ttu-id="efa37-188">Versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa37-188">Device operating system version.</span></span>|
|<span data-ttu-id="efa37-189">deploymentDuration</span><span class="sxs-lookup"><span data-stu-id="efa37-189">deploymentDuration</span></span>|<span data-ttu-id="efa37-190">Duration</span><span class="sxs-lookup"><span data-stu-id="efa37-190">Duration</span></span>|<span data-ttu-id="efa37-191">Duração da implantação do piloto automático, incluindo o registro.</span><span class="sxs-lookup"><span data-stu-id="efa37-191">Autopilot deployment duration including enrollment.</span></span>|
|<span data-ttu-id="efa37-192">deploymentTotalDuration</span><span class="sxs-lookup"><span data-stu-id="efa37-192">deploymentTotalDuration</span></span>|<span data-ttu-id="efa37-193">Duration</span><span class="sxs-lookup"><span data-stu-id="efa37-193">Duration</span></span>|<span data-ttu-id="efa37-194">Duração total da implantação do registro na tela da Área de Trabalho.</span><span class="sxs-lookup"><span data-stu-id="efa37-194">Total deployment duration from enrollment to Desktop screen.</span></span>|
|<span data-ttu-id="efa37-195">devicePreparationDuration</span><span class="sxs-lookup"><span data-stu-id="efa37-195">devicePreparationDuration</span></span>|<span data-ttu-id="efa37-196">Duration</span><span class="sxs-lookup"><span data-stu-id="efa37-196">Duration</span></span>|<span data-ttu-id="efa37-197">Tempo gasto no registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa37-197">Time spent in device enrollment.</span></span>|
|<span data-ttu-id="efa37-198">deviceSetupDuration</span><span class="sxs-lookup"><span data-stu-id="efa37-198">deviceSetupDuration</span></span>|<span data-ttu-id="efa37-199">Duration</span><span class="sxs-lookup"><span data-stu-id="efa37-199">Duration</span></span>|<span data-ttu-id="efa37-200">Tempo gasto no ESP do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa37-200">Time spent in device ESP.</span></span>|
|<span data-ttu-id="efa37-201">accountSetupDuration</span><span class="sxs-lookup"><span data-stu-id="efa37-201">accountSetupDuration</span></span>|<span data-ttu-id="efa37-202">Duration</span><span class="sxs-lookup"><span data-stu-id="efa37-202">Duration</span></span>|<span data-ttu-id="efa37-203">Tempo gasto no ESP do usuário.</span><span class="sxs-lookup"><span data-stu-id="efa37-203">Time spent in user ESP.</span></span>|
|<span data-ttu-id="efa37-204">deploymentStartDateTime</span><span class="sxs-lookup"><span data-stu-id="efa37-204">deploymentStartDateTime</span></span>|<span data-ttu-id="efa37-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa37-205">DateTimeOffset</span></span>|<span data-ttu-id="efa37-206">Hora de início da implantação.</span><span class="sxs-lookup"><span data-stu-id="efa37-206">Deployment start time.</span></span>|
|<span data-ttu-id="efa37-207">deploymentEndDateTime</span><span class="sxs-lookup"><span data-stu-id="efa37-207">deploymentEndDateTime</span></span>|<span data-ttu-id="efa37-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa37-208">DateTimeOffset</span></span>|<span data-ttu-id="efa37-209">Hora de término da implantação.</span><span class="sxs-lookup"><span data-stu-id="efa37-209">Deployment end time.</span></span>|
|<span data-ttu-id="efa37-210">targetedAppCount</span><span class="sxs-lookup"><span data-stu-id="efa37-210">targetedAppCount</span></span>|<span data-ttu-id="efa37-211">Int32</span><span class="sxs-lookup"><span data-stu-id="efa37-211">Int32</span></span>|<span data-ttu-id="efa37-212">Contagem de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="efa37-212">Count of applications targeted.</span></span>|
|<span data-ttu-id="efa37-213">targetedPolicyCount</span><span class="sxs-lookup"><span data-stu-id="efa37-213">targetedPolicyCount</span></span>|<span data-ttu-id="efa37-214">Int32</span><span class="sxs-lookup"><span data-stu-id="efa37-214">Int32</span></span>|<span data-ttu-id="efa37-215">Contagem de políticas direcionadas.</span><span class="sxs-lookup"><span data-stu-id="efa37-215">Count of policies targeted.</span></span>|
|<span data-ttu-id="efa37-216">enrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="efa37-216">enrollmentFailureDetails</span></span>|<span data-ttu-id="efa37-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa37-217">String</span></span>|<span data-ttu-id="efa37-218">Detalhes de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="efa37-218">Enrollment failure details.</span></span>|



## <a name="response"></a><span data-ttu-id="efa37-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="efa37-219">Response</span></span>
<span data-ttu-id="efa37-220">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efa37-220">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efa37-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efa37-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="efa37-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efa37-222">Request</span></span>
<span data-ttu-id="efa37-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efa37-223">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efa37-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="efa37-224">Response</span></span>
<span data-ttu-id="efa37-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efa37-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




