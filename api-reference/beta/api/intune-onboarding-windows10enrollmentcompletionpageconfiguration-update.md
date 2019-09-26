---
title: Atualizar windows10EnrollmentCompletionPageConfiguration
description: Atualiza as propriedades de um objeto windows10EnrollmentCompletionPageConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43193d8bac87dff093435c5961b29fa28e723bb6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37190072"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="29a88-103">Atualizar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="29a88-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="29a88-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29a88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29a88-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29a88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29a88-106">Atualiza as propriedades de um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="29a88-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29a88-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29a88-107">Prerequisites</span></span>
<span data-ttu-id="29a88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29a88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29a88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29a88-110">Permission type</span></span>|<span data-ttu-id="29a88-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29a88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29a88-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29a88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29a88-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29a88-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="29a88-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29a88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29a88-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29a88-115">Not supported.</span></span>|
|<span data-ttu-id="29a88-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29a88-116">Application</span></span>|<span data-ttu-id="29a88-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29a88-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29a88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29a88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29a88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29a88-119">Request headers</span></span>
|<span data-ttu-id="29a88-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29a88-120">Header</span></span>|<span data-ttu-id="29a88-121">Valor</span><span class="sxs-lookup"><span data-stu-id="29a88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29a88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="29a88-122">Authorization</span></span>|<span data-ttu-id="29a88-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29a88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29a88-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29a88-124">Accept</span></span>|<span data-ttu-id="29a88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29a88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29a88-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29a88-126">Request body</span></span>
<span data-ttu-id="29a88-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="29a88-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="29a88-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29a88-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="29a88-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29a88-129">Property</span></span>|<span data-ttu-id="29a88-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="29a88-130">Type</span></span>|<span data-ttu-id="29a88-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="29a88-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a88-132">id</span><span class="sxs-lookup"><span data-stu-id="29a88-132">id</span></span>|<span data-ttu-id="29a88-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29a88-133">String</span></span>|<span data-ttu-id="29a88-134">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29a88-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29a88-135">displayName</span><span class="sxs-lookup"><span data-stu-id="29a88-135">displayName</span></span>|<span data-ttu-id="29a88-136">String</span><span class="sxs-lookup"><span data-stu-id="29a88-136">String</span></span>|<span data-ttu-id="29a88-137">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29a88-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29a88-138">descrição</span><span class="sxs-lookup"><span data-stu-id="29a88-138">description</span></span>|<span data-ttu-id="29a88-139">String</span><span class="sxs-lookup"><span data-stu-id="29a88-139">String</span></span>|<span data-ttu-id="29a88-140">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29a88-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29a88-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="29a88-141">priority</span></span>|<span data-ttu-id="29a88-142">Int32</span><span class="sxs-lookup"><span data-stu-id="29a88-142">Int32</span></span>|<span data-ttu-id="29a88-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="29a88-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="29a88-144">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="29a88-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="29a88-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29a88-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29a88-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29a88-146">createdDateTime</span></span>|<span data-ttu-id="29a88-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29a88-147">DateTimeOffset</span></span>|<span data-ttu-id="29a88-148">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29a88-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29a88-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29a88-149">lastModifiedDateTime</span></span>|<span data-ttu-id="29a88-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29a88-150">DateTimeOffset</span></span>|<span data-ttu-id="29a88-151">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29a88-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29a88-152">versão</span><span class="sxs-lookup"><span data-stu-id="29a88-152">version</span></span>|<span data-ttu-id="29a88-153">Int32</span><span class="sxs-lookup"><span data-stu-id="29a88-153">Int32</span></span>|<span data-ttu-id="29a88-154">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29a88-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29a88-155">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="29a88-155">showInstallationProgress</span></span>|<span data-ttu-id="29a88-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="29a88-156">Boolean</span></span>|<span data-ttu-id="29a88-157">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="29a88-157">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="29a88-158">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="29a88-158">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="29a88-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="29a88-159">Boolean</span></span>|<span data-ttu-id="29a88-160">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="29a88-160">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="29a88-161">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="29a88-161">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="29a88-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="29a88-162">Boolean</span></span>|<span data-ttu-id="29a88-163">Permitir ou bloquear falha de redefinição de dispositivo na instalação</span><span class="sxs-lookup"><span data-stu-id="29a88-163">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="29a88-164">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="29a88-164">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="29a88-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="29a88-165">Boolean</span></span>|<span data-ttu-id="29a88-166">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="29a88-166">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="29a88-167">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="29a88-167">customErrorMessage</span></span>|<span data-ttu-id="29a88-168">String</span><span class="sxs-lookup"><span data-stu-id="29a88-168">String</span></span>|<span data-ttu-id="29a88-169">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="29a88-169">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="29a88-170">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="29a88-170">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="29a88-171">Int32</span><span class="sxs-lookup"><span data-stu-id="29a88-171">Int32</span></span>|<span data-ttu-id="29a88-172">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="29a88-172">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="29a88-173">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="29a88-173">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="29a88-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="29a88-174">Boolean</span></span>|<span data-ttu-id="29a88-175">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="29a88-175">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="29a88-176">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="29a88-176">selectedMobileAppIds</span></span>|<span data-ttu-id="29a88-177">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="29a88-177">String collection</span></span>|<span data-ttu-id="29a88-178">Aplicativos selecionados para acompanhar o status de instalação</span><span class="sxs-lookup"><span data-stu-id="29a88-178">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="29a88-179">trackInstallProgressForAutopilotOnly</span><span class="sxs-lookup"><span data-stu-id="29a88-179">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="29a88-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="29a88-180">Boolean</span></span>|<span data-ttu-id="29a88-181">Mostrar apenas o progresso da instalação dos cenários de registro do piloto automático</span><span class="sxs-lookup"><span data-stu-id="29a88-181">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="29a88-182">disableUserStatusTrackingAfterFirstUser</span><span class="sxs-lookup"><span data-stu-id="29a88-182">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="29a88-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="29a88-183">Boolean</span></span>|<span data-ttu-id="29a88-184">Mostrar apenas o progresso da instalação para o primeiro registro post de usuário</span><span class="sxs-lookup"><span data-stu-id="29a88-184">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="29a88-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="29a88-185">Response</span></span>
<span data-ttu-id="29a88-186">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29a88-186">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29a88-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29a88-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="29a88-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29a88-188">Request</span></span>
<span data-ttu-id="29a88-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29a88-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 684

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```

### <a name="response"></a><span data-ttu-id="29a88-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="29a88-190">Response</span></span>
<span data-ttu-id="29a88-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29a88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 856

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```




