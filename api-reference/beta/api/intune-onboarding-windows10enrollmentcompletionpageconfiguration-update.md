---
title: Atualizar windows10EnrollmentCompletionPageConfiguration
description: Atualize as propriedades de um objeto windows10EnrollmentCompletionPageConfiguration.
ms.openlocfilehash: b3566d7b476c17557bdfc15f8ff9d86763123ab2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039228"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="a6dcd-103">Atualizar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6dcd-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="a6dcd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6dcd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6dcd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6dcd-107">Atualize as propriedades de um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a6dcd-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6dcd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6dcd-108">Prerequisites</span></span>
<span data-ttu-id="a6dcd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6dcd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6dcd-111">Permission type</span></span>|<span data-ttu-id="a6dcd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6dcd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6dcd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6dcd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6dcd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6dcd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-116">Not supported.</span></span>|
|<span data-ttu-id="a6dcd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6dcd-117">Application</span></span>|<span data-ttu-id="a6dcd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6dcd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6dcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6dcd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-120">Request headers</span></span>
|<span data-ttu-id="a6dcd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6dcd-121">Header</span></span>|<span data-ttu-id="a6dcd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6dcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6dcd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6dcd-123">Authorization</span></span>|<span data-ttu-id="a6dcd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6dcd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6dcd-125">Accept</span></span>|<span data-ttu-id="a6dcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6dcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6dcd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-127">Request body</span></span>
<span data-ttu-id="a6dcd-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a6dcd-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="a6dcd-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6dcd-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="a6dcd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6dcd-130">Property</span></span>|<span data-ttu-id="a6dcd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6dcd-131">Type</span></span>|<span data-ttu-id="a6dcd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6dcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6dcd-133">id</span><span class="sxs-lookup"><span data-stu-id="a6dcd-133">id</span></span>|<span data-ttu-id="a6dcd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6dcd-134">String</span></span>|<span data-ttu-id="a6dcd-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6dcd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a6dcd-136">displayName</span></span>|<span data-ttu-id="a6dcd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6dcd-137">String</span></span>|<span data-ttu-id="a6dcd-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6dcd-139">description</span><span class="sxs-lookup"><span data-stu-id="a6dcd-139">description</span></span>|<span data-ttu-id="a6dcd-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6dcd-140">String</span></span>|<span data-ttu-id="a6dcd-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6dcd-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="a6dcd-142">priority</span></span>|<span data-ttu-id="a6dcd-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a6dcd-143">Int32</span></span>|<span data-ttu-id="a6dcd-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6dcd-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6dcd-145">createdDateTime</span></span>|<span data-ttu-id="a6dcd-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6dcd-146">DateTimeOffset</span></span>|<span data-ttu-id="a6dcd-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6dcd-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6dcd-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a6dcd-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6dcd-149">DateTimeOffset</span></span>|<span data-ttu-id="a6dcd-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6dcd-151">version</span><span class="sxs-lookup"><span data-stu-id="a6dcd-151">version</span></span>|<span data-ttu-id="a6dcd-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a6dcd-152">Int32</span></span>|<span data-ttu-id="a6dcd-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6dcd-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a6dcd-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="a6dcd-154">showInstallationProgress</span></span>|<span data-ttu-id="a6dcd-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6dcd-155">Boolean</span></span>|<span data-ttu-id="a6dcd-156">Mostrar ou ocultar o progresso da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="a6dcd-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="a6dcd-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="a6dcd-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="a6dcd-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6dcd-158">Boolean</span></span>|<span data-ttu-id="a6dcd-159">Permitir que o usuário repetir a instalação em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="a6dcd-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="a6dcd-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="a6dcd-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6dcd-161">Boolean</span></span>|<span data-ttu-id="a6dcd-162">Permitir ou bloquear o dispositivo redefinir em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="a6dcd-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="a6dcd-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="a6dcd-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6dcd-164">Boolean</span></span>|<span data-ttu-id="a6dcd-165">Permitir ou bloquear o conjunto de log em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="a6dcd-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="a6dcd-166">customErrorMessage</span></span>|<span data-ttu-id="a6dcd-167">String</span><span class="sxs-lookup"><span data-stu-id="a6dcd-167">String</span></span>|<span data-ttu-id="a6dcd-168">Definir a mensagem de erro personalizada para mostrar após a falha de instalação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="a6dcd-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a6dcd-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="a6dcd-170">Int32</span><span class="sxs-lookup"><span data-stu-id="a6dcd-170">Int32</span></span>|<span data-ttu-id="a6dcd-171">Definir tempo limite de progresso de instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="a6dcd-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="a6dcd-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="a6dcd-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="a6dcd-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6dcd-173">Boolean</span></span>|<span data-ttu-id="a6dcd-174">Permitir que o usuário continue a usar o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="a6dcd-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="a6dcd-175">selectedMobileAppIds</span></span>|<span data-ttu-id="a6dcd-176">String collection</span><span class="sxs-lookup"><span data-stu-id="a6dcd-176">String collection</span></span>|<span data-ttu-id="a6dcd-177">Aplicativos selecionados para rastrear o status de instalação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="a6dcd-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6dcd-178">Response</span></span>
<span data-ttu-id="a6dcd-179">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-179">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6dcd-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6dcd-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6dcd-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6dcd-181">Request</span></span>
<span data-ttu-id="a6dcd-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 562

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="a6dcd-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6dcd-183">Response</span></span>
<span data-ttu-id="a6dcd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6dcd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





