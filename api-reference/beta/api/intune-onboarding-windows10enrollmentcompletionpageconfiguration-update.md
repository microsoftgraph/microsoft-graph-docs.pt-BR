---
title: Atualizar windows10EnrollmentCompletionPageConfiguration
description: Atualiza as propriedades de um objeto windows10EnrollmentCompletionPageConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3221c76298c65c47edbf56b5924bc9b78750db89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995703"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="4e23a-103">Atualizar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="4e23a-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="4e23a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e23a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e23a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e23a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e23a-106">Atualiza as propriedades de um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4e23a-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e23a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e23a-107">Prerequisites</span></span>
<span data-ttu-id="4e23a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e23a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e23a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e23a-110">Permission type</span></span>|<span data-ttu-id="4e23a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e23a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e23a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e23a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e23a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e23a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4e23a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e23a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e23a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e23a-115">Not supported.</span></span>|
|<span data-ttu-id="4e23a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e23a-116">Application</span></span>|<span data-ttu-id="4e23a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e23a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e23a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e23a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4e23a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e23a-119">Request headers</span></span>
|<span data-ttu-id="4e23a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e23a-120">Header</span></span>|<span data-ttu-id="4e23a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4e23a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e23a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e23a-122">Authorization</span></span>|<span data-ttu-id="4e23a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e23a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e23a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e23a-124">Accept</span></span>|<span data-ttu-id="4e23a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e23a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e23a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e23a-126">Request body</span></span>
<span data-ttu-id="4e23a-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4e23a-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="4e23a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e23a-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="4e23a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e23a-129">Property</span></span>|<span data-ttu-id="4e23a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e23a-130">Type</span></span>|<span data-ttu-id="4e23a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e23a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e23a-132">id</span><span class="sxs-lookup"><span data-stu-id="4e23a-132">id</span></span>|<span data-ttu-id="4e23a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e23a-133">String</span></span>|<span data-ttu-id="4e23a-134">Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e23a-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4e23a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4e23a-135">displayName</span></span>|<span data-ttu-id="4e23a-136">String</span><span class="sxs-lookup"><span data-stu-id="4e23a-136">String</span></span>|<span data-ttu-id="4e23a-137">O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e23a-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4e23a-138">descrição</span><span class="sxs-lookup"><span data-stu-id="4e23a-138">description</span></span>|<span data-ttu-id="4e23a-139">String</span><span class="sxs-lookup"><span data-stu-id="4e23a-139">String</span></span>|<span data-ttu-id="4e23a-140">A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e23a-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4e23a-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="4e23a-141">priority</span></span>|<span data-ttu-id="4e23a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4e23a-142">Int32</span></span>|<span data-ttu-id="4e23a-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="4e23a-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="4e23a-144">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="4e23a-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="4e23a-145">Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e23a-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4e23a-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e23a-146">createdDateTime</span></span>|<span data-ttu-id="4e23a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e23a-147">DateTimeOffset</span></span>|<span data-ttu-id="4e23a-148">Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e23a-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4e23a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e23a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4e23a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e23a-150">DateTimeOffset</span></span>|<span data-ttu-id="4e23a-151">Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e23a-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4e23a-152">versão</span><span class="sxs-lookup"><span data-stu-id="4e23a-152">version</span></span>|<span data-ttu-id="4e23a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4e23a-153">Int32</span></span>|<span data-ttu-id="4e23a-154">A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e23a-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4e23a-155">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="4e23a-155">showInstallationProgress</span></span>|<span data-ttu-id="4e23a-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e23a-156">Boolean</span></span>|<span data-ttu-id="4e23a-157">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="4e23a-157">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="4e23a-158">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="4e23a-158">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="4e23a-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e23a-159">Boolean</span></span>|<span data-ttu-id="4e23a-160">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="4e23a-160">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="4e23a-161">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="4e23a-161">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="4e23a-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e23a-162">Boolean</span></span>|<span data-ttu-id="4e23a-163">Permitir ou bloquear falha de redefinição de dispositivo na instalação</span><span class="sxs-lookup"><span data-stu-id="4e23a-163">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="4e23a-164">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="4e23a-164">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="4e23a-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e23a-165">Boolean</span></span>|<span data-ttu-id="4e23a-166">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="4e23a-166">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="4e23a-167">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="4e23a-167">customErrorMessage</span></span>|<span data-ttu-id="4e23a-168">String</span><span class="sxs-lookup"><span data-stu-id="4e23a-168">String</span></span>|<span data-ttu-id="4e23a-169">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="4e23a-169">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="4e23a-170">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="4e23a-170">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="4e23a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="4e23a-171">Int32</span></span>|<span data-ttu-id="4e23a-172">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="4e23a-172">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="4e23a-173">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="4e23a-173">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="4e23a-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e23a-174">Boolean</span></span>|<span data-ttu-id="4e23a-175">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="4e23a-175">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="4e23a-176">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="4e23a-176">selectedMobileAppIds</span></span>|<span data-ttu-id="4e23a-177">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e23a-177">String collection</span></span>|<span data-ttu-id="4e23a-178">Aplicativos selecionados para acompanhar o status de instalação</span><span class="sxs-lookup"><span data-stu-id="4e23a-178">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="4e23a-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e23a-179">Response</span></span>
<span data-ttu-id="4e23a-180">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e23a-180">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e23a-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e23a-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e23a-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e23a-182">Request</span></span>
<span data-ttu-id="4e23a-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e23a-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 583

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="4e23a-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e23a-184">Response</span></span>
<span data-ttu-id="4e23a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e23a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 755

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
  ]
}
```





