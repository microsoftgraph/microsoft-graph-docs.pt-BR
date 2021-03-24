---
title: Criar windows10EnrollmentCompletionPageConfiguration
description: Crie um novo objeto windows10EnrollmentCompletionPageConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a5198792f852a30591e8212b76bf627a63f99f7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134974"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="802ef-103">Criar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="802ef-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="802ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="802ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="802ef-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="802ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="802ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="802ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="802ef-107">Crie um novo [objeto windows10EnrollmentCompletionPageConfiguration.](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="802ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="802ef-108">Prerequisites</span></span>
<span data-ttu-id="802ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="802ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="802ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="802ef-111">Permission type</span></span>|<span data-ttu-id="802ef-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="802ef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="802ef-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="802ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="802ef-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="802ef-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="802ef-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="802ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="802ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="802ef-116">Not supported.</span></span>|
|<span data-ttu-id="802ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="802ef-117">Application</span></span>|<span data-ttu-id="802ef-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="802ef-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="802ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="802ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="802ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="802ef-120">Request headers</span></span>
|<span data-ttu-id="802ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="802ef-121">Header</span></span>|<span data-ttu-id="802ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="802ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="802ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="802ef-123">Authorization</span></span>|<span data-ttu-id="802ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="802ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="802ef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="802ef-125">Accept</span></span>|<span data-ttu-id="802ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="802ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="802ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="802ef-127">Request body</span></span>
<span data-ttu-id="802ef-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="802ef-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="802ef-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="802ef-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="802ef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="802ef-130">Property</span></span>|<span data-ttu-id="802ef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="802ef-131">Type</span></span>|<span data-ttu-id="802ef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="802ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="802ef-133">id</span><span class="sxs-lookup"><span data-stu-id="802ef-133">id</span></span>|<span data-ttu-id="802ef-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="802ef-134">String</span></span>|<span data-ttu-id="802ef-135">Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="802ef-136">displayName</span><span class="sxs-lookup"><span data-stu-id="802ef-136">displayName</span></span>|<span data-ttu-id="802ef-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="802ef-137">String</span></span>|<span data-ttu-id="802ef-138">O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="802ef-139">descrição</span><span class="sxs-lookup"><span data-stu-id="802ef-139">description</span></span>|<span data-ttu-id="802ef-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="802ef-140">String</span></span>|<span data-ttu-id="802ef-141">A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="802ef-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="802ef-142">priority</span></span>|<span data-ttu-id="802ef-143">Int32</span><span class="sxs-lookup"><span data-stu-id="802ef-143">Int32</span></span>|<span data-ttu-id="802ef-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="802ef-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="802ef-145">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="802ef-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="802ef-146">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="802ef-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="802ef-147">createdDateTime</span></span>|<span data-ttu-id="802ef-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="802ef-148">DateTimeOffset</span></span>|<span data-ttu-id="802ef-149">Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="802ef-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="802ef-150">lastModifiedDateTime</span></span>|<span data-ttu-id="802ef-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="802ef-151">DateTimeOffset</span></span>|<span data-ttu-id="802ef-152">Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="802ef-153">versão</span><span class="sxs-lookup"><span data-stu-id="802ef-153">version</span></span>|<span data-ttu-id="802ef-154">Int32</span><span class="sxs-lookup"><span data-stu-id="802ef-154">Int32</span></span>|<span data-ttu-id="802ef-155">A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="802ef-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="802ef-156">roleScopeTagIds</span></span>|<span data-ttu-id="802ef-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="802ef-157">String collection</span></span>|<span data-ttu-id="802ef-158">Marcas de escopo de função opcionais para as restrições de registro.</span><span class="sxs-lookup"><span data-stu-id="802ef-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="802ef-159">Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="802ef-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="802ef-160">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="802ef-160">showInstallationProgress</span></span>|<span data-ttu-id="802ef-161">Booleano</span><span class="sxs-lookup"><span data-stu-id="802ef-161">Boolean</span></span>|<span data-ttu-id="802ef-162">Mostrar ou ocultar o progresso da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="802ef-162">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="802ef-163">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="802ef-163">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="802ef-164">Booleano</span><span class="sxs-lookup"><span data-stu-id="802ef-164">Boolean</span></span>|<span data-ttu-id="802ef-165">Permitir que o usuário repetir a instalação na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="802ef-165">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="802ef-166">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="802ef-166">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="802ef-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="802ef-167">Boolean</span></span>|<span data-ttu-id="802ef-168">Permitir ou bloquear a redefinição do dispositivo na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="802ef-168">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="802ef-169">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="802ef-169">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="802ef-170">Booleano</span><span class="sxs-lookup"><span data-stu-id="802ef-170">Boolean</span></span>|<span data-ttu-id="802ef-171">Permitir ou bloquear o conjunto de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="802ef-171">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="802ef-172">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="802ef-172">customErrorMessage</span></span>|<span data-ttu-id="802ef-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="802ef-173">String</span></span>|<span data-ttu-id="802ef-174">Definir mensagem de erro personalizada para mostrar após a falha na instalação</span><span class="sxs-lookup"><span data-stu-id="802ef-174">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="802ef-175">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="802ef-175">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="802ef-176">Int32</span><span class="sxs-lookup"><span data-stu-id="802ef-176">Int32</span></span>|<span data-ttu-id="802ef-177">Definir o tempo de tempo de duração da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="802ef-177">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="802ef-178">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="802ef-178">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="802ef-179">Booleano</span><span class="sxs-lookup"><span data-stu-id="802ef-179">Boolean</span></span>|<span data-ttu-id="802ef-180">Permitir que o usuário continue usando o dispositivo na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="802ef-180">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="802ef-181">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="802ef-181">selectedMobileAppIds</span></span>|<span data-ttu-id="802ef-182">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="802ef-182">String collection</span></span>|<span data-ttu-id="802ef-183">Aplicativos selecionados para rastrear o status da instalação</span><span class="sxs-lookup"><span data-stu-id="802ef-183">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="802ef-184">trackInstallProgressForAutopilotOnly</span><span class="sxs-lookup"><span data-stu-id="802ef-184">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="802ef-185">Booleano</span><span class="sxs-lookup"><span data-stu-id="802ef-185">Boolean</span></span>|<span data-ttu-id="802ef-186">Mostrar apenas o progresso da instalação para cenários de registro do Piloto Automático</span><span class="sxs-lookup"><span data-stu-id="802ef-186">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="802ef-187">disableUserStatusTrackingAfterFirstUser</span><span class="sxs-lookup"><span data-stu-id="802ef-187">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="802ef-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="802ef-188">Boolean</span></span>|<span data-ttu-id="802ef-189">Mostrar apenas o progresso da instalação para o primeiro registro de postagem do usuário</span><span class="sxs-lookup"><span data-stu-id="802ef-189">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="802ef-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="802ef-190">Response</span></span>
<span data-ttu-id="802ef-191">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="802ef-191">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="802ef-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="802ef-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="802ef-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="802ef-193">Request</span></span>
<span data-ttu-id="802ef-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="802ef-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="802ef-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="802ef-195">Response</span></span>
<span data-ttu-id="802ef-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="802ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 918

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




