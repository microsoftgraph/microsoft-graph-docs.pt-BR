---
title: Atualizar windows10EnrollmentCompletionPageConfiguration
description: Atualiza as propriedades de um objeto windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 862ec01be1bd6b99351d9b01f16797ae4a376e75
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981129"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="7599d-103">Atualizar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="7599d-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="7599d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7599d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7599d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7599d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7599d-106">Atualiza as propriedades de um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7599d-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7599d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7599d-107">Prerequisites</span></span>
<span data-ttu-id="7599d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7599d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7599d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7599d-110">Permission type</span></span>|<span data-ttu-id="7599d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7599d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7599d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7599d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7599d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7599d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7599d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7599d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7599d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7599d-115">Not supported.</span></span>|
|<span data-ttu-id="7599d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7599d-116">Application</span></span>|<span data-ttu-id="7599d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7599d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7599d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7599d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7599d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7599d-119">Request headers</span></span>
|<span data-ttu-id="7599d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7599d-120">Header</span></span>|<span data-ttu-id="7599d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7599d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7599d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7599d-122">Authorization</span></span>|<span data-ttu-id="7599d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7599d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7599d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7599d-124">Accept</span></span>|<span data-ttu-id="7599d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7599d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7599d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7599d-126">Request body</span></span>
<span data-ttu-id="7599d-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7599d-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="7599d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7599d-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="7599d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7599d-129">Property</span></span>|<span data-ttu-id="7599d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7599d-130">Type</span></span>|<span data-ttu-id="7599d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7599d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7599d-132">id</span><span class="sxs-lookup"><span data-stu-id="7599d-132">id</span></span>|<span data-ttu-id="7599d-133">String</span><span class="sxs-lookup"><span data-stu-id="7599d-133">String</span></span>|<span data-ttu-id="7599d-134">ID da configuração da página de status de registro herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7599d-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7599d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7599d-135">displayName</span></span>|<span data-ttu-id="7599d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7599d-136">String</span></span>|<span data-ttu-id="7599d-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7599d-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7599d-138">descrição</span><span class="sxs-lookup"><span data-stu-id="7599d-138">description</span></span>|<span data-ttu-id="7599d-139">String</span><span class="sxs-lookup"><span data-stu-id="7599d-139">String</span></span>|<span data-ttu-id="7599d-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7599d-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7599d-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="7599d-141">priority</span></span>|<span data-ttu-id="7599d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7599d-142">Int32</span></span>|<span data-ttu-id="7599d-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7599d-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7599d-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7599d-144">createdDateTime</span></span>|<span data-ttu-id="7599d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7599d-145">DateTimeOffset</span></span>|<span data-ttu-id="7599d-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7599d-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7599d-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7599d-147">lastModifiedDateTime</span></span>|<span data-ttu-id="7599d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7599d-148">DateTimeOffset</span></span>|<span data-ttu-id="7599d-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7599d-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7599d-150">versão</span><span class="sxs-lookup"><span data-stu-id="7599d-150">version</span></span>|<span data-ttu-id="7599d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7599d-151">Int32</span></span>|<span data-ttu-id="7599d-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7599d-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7599d-153">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="7599d-153">showInstallationProgress</span></span>|<span data-ttu-id="7599d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7599d-154">Boolean</span></span>|<span data-ttu-id="7599d-155">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="7599d-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="7599d-156">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="7599d-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="7599d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="7599d-157">Boolean</span></span>|<span data-ttu-id="7599d-158">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="7599d-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="7599d-159">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7599d-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="7599d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7599d-160">Boolean</span></span>|<span data-ttu-id="7599d-161">Permitir ou bloquear falha de redefinição de dispositivo na instalação</span><span class="sxs-lookup"><span data-stu-id="7599d-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="7599d-162">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7599d-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="7599d-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="7599d-163">Boolean</span></span>|<span data-ttu-id="7599d-164">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="7599d-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="7599d-165">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="7599d-165">customErrorMessage</span></span>|<span data-ttu-id="7599d-166">String</span><span class="sxs-lookup"><span data-stu-id="7599d-166">String</span></span>|<span data-ttu-id="7599d-167">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="7599d-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="7599d-168">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7599d-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="7599d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7599d-169">Int32</span></span>|<span data-ttu-id="7599d-170">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="7599d-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="7599d-171">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7599d-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="7599d-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="7599d-172">Boolean</span></span>|<span data-ttu-id="7599d-173">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="7599d-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="7599d-174">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="7599d-174">selectedMobileAppIds</span></span>|<span data-ttu-id="7599d-175">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7599d-175">String collection</span></span>|<span data-ttu-id="7599d-176">Aplicativos selecionados para acompanhar o status de instalação</span><span class="sxs-lookup"><span data-stu-id="7599d-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="7599d-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="7599d-177">Response</span></span>
<span data-ttu-id="7599d-178">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7599d-178">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7599d-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7599d-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="7599d-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7599d-180">Request</span></span>
<span data-ttu-id="7599d-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7599d-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7599d-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="7599d-182">Response</span></span>
<span data-ttu-id="7599d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7599d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




