---
title: Criar windows10EnrollmentCompletionPageConfiguration
description: Criar um novo objeto windows10EnrollmentCompletionPageConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3efa2a669ac11123bd4480b7a3092717528c932
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461631"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="caef0-103">Criar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="caef0-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="caef0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="caef0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="caef0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="caef0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caef0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="caef0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caef0-107">Criar um novo objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="caef0-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="caef0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="caef0-108">Prerequisites</span></span>
<span data-ttu-id="caef0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caef0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caef0-111">Permission type</span></span>|<span data-ttu-id="caef0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="caef0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caef0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caef0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="caef0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caef0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="caef0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caef0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caef0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caef0-116">Not supported.</span></span>|
|<span data-ttu-id="caef0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caef0-117">Application</span></span>|<span data-ttu-id="caef0-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caef0-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="caef0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caef0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="caef0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caef0-120">Request headers</span></span>
|<span data-ttu-id="caef0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="caef0-121">Header</span></span>|<span data-ttu-id="caef0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="caef0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caef0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="caef0-123">Authorization</span></span>|<span data-ttu-id="caef0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caef0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caef0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="caef0-125">Accept</span></span>|<span data-ttu-id="caef0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="caef0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caef0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caef0-127">Request body</span></span>
<span data-ttu-id="caef0-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="caef0-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="caef0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="caef0-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="caef0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="caef0-130">Property</span></span>|<span data-ttu-id="caef0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="caef0-131">Type</span></span>|<span data-ttu-id="caef0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="caef0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caef0-133">id</span><span class="sxs-lookup"><span data-stu-id="caef0-133">id</span></span>|<span data-ttu-id="caef0-134">String</span><span class="sxs-lookup"><span data-stu-id="caef0-134">String</span></span>|<span data-ttu-id="caef0-135">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="caef0-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="caef0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="caef0-136">displayName</span></span>|<span data-ttu-id="caef0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="caef0-137">String</span></span>|<span data-ttu-id="caef0-138">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="caef0-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="caef0-139">description</span><span class="sxs-lookup"><span data-stu-id="caef0-139">description</span></span>|<span data-ttu-id="caef0-140">String</span><span class="sxs-lookup"><span data-stu-id="caef0-140">String</span></span>|<span data-ttu-id="caef0-141">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="caef0-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="caef0-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="caef0-142">priority</span></span>|<span data-ttu-id="caef0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="caef0-143">Int32</span></span>|<span data-ttu-id="caef0-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="caef0-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="caef0-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="caef0-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="caef0-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="caef0-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="caef0-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="caef0-147">createdDateTime</span></span>|<span data-ttu-id="caef0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caef0-148">DateTimeOffset</span></span>|<span data-ttu-id="caef0-149">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="caef0-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="caef0-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="caef0-150">lastModifiedDateTime</span></span>|<span data-ttu-id="caef0-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caef0-151">DateTimeOffset</span></span>|<span data-ttu-id="caef0-152">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="caef0-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="caef0-153">versão</span><span class="sxs-lookup"><span data-stu-id="caef0-153">version</span></span>|<span data-ttu-id="caef0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="caef0-154">Int32</span></span>|<span data-ttu-id="caef0-155">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="caef0-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="caef0-156">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="caef0-156">showInstallationProgress</span></span>|<span data-ttu-id="caef0-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="caef0-157">Boolean</span></span>|<span data-ttu-id="caef0-158">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="caef0-158">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="caef0-159">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="caef0-159">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="caef0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="caef0-160">Boolean</span></span>|<span data-ttu-id="caef0-161">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="caef0-161">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="caef0-162">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="caef0-162">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="caef0-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="caef0-163">Boolean</span></span>|<span data-ttu-id="caef0-164">Permitir ou bloquear falha de redefinição de dispositivo na instalação</span><span class="sxs-lookup"><span data-stu-id="caef0-164">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="caef0-165">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="caef0-165">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="caef0-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="caef0-166">Boolean</span></span>|<span data-ttu-id="caef0-167">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="caef0-167">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="caef0-168">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="caef0-168">customErrorMessage</span></span>|<span data-ttu-id="caef0-169">String</span><span class="sxs-lookup"><span data-stu-id="caef0-169">String</span></span>|<span data-ttu-id="caef0-170">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="caef0-170">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="caef0-171">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="caef0-171">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="caef0-172">Int32</span><span class="sxs-lookup"><span data-stu-id="caef0-172">Int32</span></span>|<span data-ttu-id="caef0-173">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="caef0-173">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="caef0-174">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="caef0-174">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="caef0-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="caef0-175">Boolean</span></span>|<span data-ttu-id="caef0-176">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="caef0-176">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="caef0-177">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="caef0-177">selectedMobileAppIds</span></span>|<span data-ttu-id="caef0-178">String collection</span><span class="sxs-lookup"><span data-stu-id="caef0-178">String collection</span></span>|<span data-ttu-id="caef0-179">Aplicativos selecionados para acompanhar o status de instalação</span><span class="sxs-lookup"><span data-stu-id="caef0-179">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="caef0-180">trackInstallProgressForAutopilotOnly</span><span class="sxs-lookup"><span data-stu-id="caef0-180">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="caef0-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="caef0-181">Boolean</span></span>|<span data-ttu-id="caef0-182">Mostrar apenas o progresso da instalação dos cenários de registro do piloto automático</span><span class="sxs-lookup"><span data-stu-id="caef0-182">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="caef0-183">disableUserStatusTrackingAfterFirstUser</span><span class="sxs-lookup"><span data-stu-id="caef0-183">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="caef0-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="caef0-184">Boolean</span></span>|<span data-ttu-id="caef0-185">Mostrar apenas o progresso da instalação para o primeiro registro post de usuário</span><span class="sxs-lookup"><span data-stu-id="caef0-185">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="caef0-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="caef0-186">Response</span></span>
<span data-ttu-id="caef0-187">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caef0-187">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caef0-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="caef0-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="caef0-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caef0-189">Request</span></span>
<span data-ttu-id="caef0-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="caef0-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="caef0-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="caef0-191">Response</span></span>
<span data-ttu-id="caef0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="caef0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





