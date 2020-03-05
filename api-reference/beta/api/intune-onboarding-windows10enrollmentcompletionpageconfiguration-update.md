---
title: Atualizar windows10EnrollmentCompletionPageConfiguration
description: Atualiza as propriedades de um objeto windows10EnrollmentCompletionPageConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9524480c41d3e915e4767ce958052b1ebb45bd7c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461568"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="304fe-103">Atualizar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="304fe-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="304fe-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="304fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="304fe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="304fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="304fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="304fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="304fe-107">Atualiza as propriedades de um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="304fe-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="304fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="304fe-108">Prerequisites</span></span>
<span data-ttu-id="304fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="304fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="304fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="304fe-111">Permission type</span></span>|<span data-ttu-id="304fe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="304fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="304fe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="304fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="304fe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304fe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="304fe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="304fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="304fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="304fe-116">Not supported.</span></span>|
|<span data-ttu-id="304fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="304fe-117">Application</span></span>|<span data-ttu-id="304fe-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304fe-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="304fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="304fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="304fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="304fe-120">Request headers</span></span>
|<span data-ttu-id="304fe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="304fe-121">Header</span></span>|<span data-ttu-id="304fe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="304fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="304fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="304fe-123">Authorization</span></span>|<span data-ttu-id="304fe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="304fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="304fe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="304fe-125">Accept</span></span>|<span data-ttu-id="304fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="304fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="304fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="304fe-127">Request body</span></span>
<span data-ttu-id="304fe-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="304fe-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="304fe-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="304fe-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="304fe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="304fe-130">Property</span></span>|<span data-ttu-id="304fe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="304fe-131">Type</span></span>|<span data-ttu-id="304fe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="304fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="304fe-133">id</span><span class="sxs-lookup"><span data-stu-id="304fe-133">id</span></span>|<span data-ttu-id="304fe-134">String</span><span class="sxs-lookup"><span data-stu-id="304fe-134">String</span></span>|<span data-ttu-id="304fe-135">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="304fe-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="304fe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="304fe-136">displayName</span></span>|<span data-ttu-id="304fe-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="304fe-137">String</span></span>|<span data-ttu-id="304fe-138">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="304fe-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="304fe-139">description</span><span class="sxs-lookup"><span data-stu-id="304fe-139">description</span></span>|<span data-ttu-id="304fe-140">String</span><span class="sxs-lookup"><span data-stu-id="304fe-140">String</span></span>|<span data-ttu-id="304fe-141">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="304fe-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="304fe-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="304fe-142">priority</span></span>|<span data-ttu-id="304fe-143">Int32</span><span class="sxs-lookup"><span data-stu-id="304fe-143">Int32</span></span>|<span data-ttu-id="304fe-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="304fe-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="304fe-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="304fe-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="304fe-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="304fe-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="304fe-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="304fe-147">createdDateTime</span></span>|<span data-ttu-id="304fe-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="304fe-148">DateTimeOffset</span></span>|<span data-ttu-id="304fe-149">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="304fe-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="304fe-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="304fe-150">lastModifiedDateTime</span></span>|<span data-ttu-id="304fe-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="304fe-151">DateTimeOffset</span></span>|<span data-ttu-id="304fe-152">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="304fe-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="304fe-153">versão</span><span class="sxs-lookup"><span data-stu-id="304fe-153">version</span></span>|<span data-ttu-id="304fe-154">Int32</span><span class="sxs-lookup"><span data-stu-id="304fe-154">Int32</span></span>|<span data-ttu-id="304fe-155">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="304fe-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="304fe-156">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="304fe-156">showInstallationProgress</span></span>|<span data-ttu-id="304fe-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="304fe-157">Boolean</span></span>|<span data-ttu-id="304fe-158">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="304fe-158">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="304fe-159">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="304fe-159">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="304fe-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="304fe-160">Boolean</span></span>|<span data-ttu-id="304fe-161">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="304fe-161">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="304fe-162">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="304fe-162">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="304fe-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="304fe-163">Boolean</span></span>|<span data-ttu-id="304fe-164">Permitir ou bloquear falha de redefinição de dispositivo na instalação</span><span class="sxs-lookup"><span data-stu-id="304fe-164">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="304fe-165">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="304fe-165">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="304fe-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="304fe-166">Boolean</span></span>|<span data-ttu-id="304fe-167">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="304fe-167">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="304fe-168">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="304fe-168">customErrorMessage</span></span>|<span data-ttu-id="304fe-169">String</span><span class="sxs-lookup"><span data-stu-id="304fe-169">String</span></span>|<span data-ttu-id="304fe-170">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="304fe-170">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="304fe-171">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="304fe-171">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="304fe-172">Int32</span><span class="sxs-lookup"><span data-stu-id="304fe-172">Int32</span></span>|<span data-ttu-id="304fe-173">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="304fe-173">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="304fe-174">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="304fe-174">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="304fe-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="304fe-175">Boolean</span></span>|<span data-ttu-id="304fe-176">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="304fe-176">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="304fe-177">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="304fe-177">selectedMobileAppIds</span></span>|<span data-ttu-id="304fe-178">String collection</span><span class="sxs-lookup"><span data-stu-id="304fe-178">String collection</span></span>|<span data-ttu-id="304fe-179">Aplicativos selecionados para acompanhar o status de instalação</span><span class="sxs-lookup"><span data-stu-id="304fe-179">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="304fe-180">trackInstallProgressForAutopilotOnly</span><span class="sxs-lookup"><span data-stu-id="304fe-180">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="304fe-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="304fe-181">Boolean</span></span>|<span data-ttu-id="304fe-182">Mostrar apenas o progresso da instalação dos cenários de registro do piloto automático</span><span class="sxs-lookup"><span data-stu-id="304fe-182">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="304fe-183">disableUserStatusTrackingAfterFirstUser</span><span class="sxs-lookup"><span data-stu-id="304fe-183">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="304fe-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="304fe-184">Boolean</span></span>|<span data-ttu-id="304fe-185">Mostrar apenas o progresso da instalação para o primeiro registro post de usuário</span><span class="sxs-lookup"><span data-stu-id="304fe-185">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="304fe-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="304fe-186">Response</span></span>
<span data-ttu-id="304fe-187">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="304fe-187">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="304fe-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="304fe-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="304fe-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="304fe-189">Request</span></span>
<span data-ttu-id="304fe-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="304fe-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="304fe-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="304fe-191">Response</span></span>
<span data-ttu-id="304fe-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="304fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





