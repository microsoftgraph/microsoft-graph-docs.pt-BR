---
title: Atualizar windows10EnrollmentCompletionPageConfiguration
description: Atualize as propriedades de um objeto windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9cc7d2cff8563d5e720e23c7f49bd88c42f47ec3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870075"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="5a738-103">Atualizar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a738-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="5a738-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a738-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a738-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a738-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a738-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5a738-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a738-107">Atualize as propriedades de um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5a738-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a738-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a738-108">Prerequisites</span></span>
<span data-ttu-id="5a738-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a738-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a738-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a738-111">Permission type</span></span>|<span data-ttu-id="5a738-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a738-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a738-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a738-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a738-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a738-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5a738-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a738-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a738-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a738-116">Not supported.</span></span>|
|<span data-ttu-id="5a738-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a738-117">Application</span></span>|<span data-ttu-id="5a738-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a738-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a738-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a738-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5a738-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a738-120">Request headers</span></span>
|<span data-ttu-id="5a738-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a738-121">Header</span></span>|<span data-ttu-id="5a738-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5a738-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a738-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a738-123">Authorization</span></span>|<span data-ttu-id="5a738-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a738-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a738-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a738-125">Accept</span></span>|<span data-ttu-id="5a738-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a738-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a738-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a738-127">Request body</span></span>
<span data-ttu-id="5a738-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5a738-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="5a738-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a738-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="5a738-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a738-130">Property</span></span>|<span data-ttu-id="5a738-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a738-131">Type</span></span>|<span data-ttu-id="5a738-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a738-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a738-133">id</span><span class="sxs-lookup"><span data-stu-id="5a738-133">id</span></span>|<span data-ttu-id="5a738-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a738-134">String</span></span>|<span data-ttu-id="5a738-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a738-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5a738-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5a738-136">displayName</span></span>|<span data-ttu-id="5a738-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a738-137">String</span></span>|<span data-ttu-id="5a738-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a738-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5a738-139">description</span><span class="sxs-lookup"><span data-stu-id="5a738-139">description</span></span>|<span data-ttu-id="5a738-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a738-140">String</span></span>|<span data-ttu-id="5a738-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a738-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5a738-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="5a738-142">priority</span></span>|<span data-ttu-id="5a738-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5a738-143">Int32</span></span>|<span data-ttu-id="5a738-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a738-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5a738-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a738-145">createdDateTime</span></span>|<span data-ttu-id="5a738-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a738-146">DateTimeOffset</span></span>|<span data-ttu-id="5a738-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a738-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5a738-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a738-148">lastModifiedDateTime</span></span>|<span data-ttu-id="5a738-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a738-149">DateTimeOffset</span></span>|<span data-ttu-id="5a738-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a738-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5a738-151">version</span><span class="sxs-lookup"><span data-stu-id="5a738-151">version</span></span>|<span data-ttu-id="5a738-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5a738-152">Int32</span></span>|<span data-ttu-id="5a738-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a738-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5a738-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="5a738-154">showInstallationProgress</span></span>|<span data-ttu-id="5a738-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a738-155">Boolean</span></span>|<span data-ttu-id="5a738-156">Mostrar ou ocultar o progresso da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="5a738-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="5a738-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="5a738-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="5a738-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a738-158">Boolean</span></span>|<span data-ttu-id="5a738-159">Permitir que o usuário repetir a instalação em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="5a738-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="5a738-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="5a738-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="5a738-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a738-161">Boolean</span></span>|<span data-ttu-id="5a738-162">Permitir ou bloquear o dispositivo redefinir em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="5a738-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="5a738-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="5a738-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="5a738-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a738-164">Boolean</span></span>|<span data-ttu-id="5a738-165">Permitir ou bloquear o conjunto de log em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="5a738-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="5a738-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="5a738-166">customErrorMessage</span></span>|<span data-ttu-id="5a738-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a738-167">String</span></span>|<span data-ttu-id="5a738-168">Definir a mensagem de erro personalizada para mostrar após a falha de instalação</span><span class="sxs-lookup"><span data-stu-id="5a738-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="5a738-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="5a738-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="5a738-170">Int32</span><span class="sxs-lookup"><span data-stu-id="5a738-170">Int32</span></span>|<span data-ttu-id="5a738-171">Definir tempo limite de progresso de instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="5a738-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="5a738-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="5a738-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="5a738-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a738-173">Boolean</span></span>|<span data-ttu-id="5a738-174">Permitir que o usuário continue a usar o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="5a738-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="5a738-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="5a738-175">selectedMobileAppIds</span></span>|<span data-ttu-id="5a738-176">String collection</span><span class="sxs-lookup"><span data-stu-id="5a738-176">String collection</span></span>|<span data-ttu-id="5a738-177">Aplicativos selecionados para rastrear o status de instalação</span><span class="sxs-lookup"><span data-stu-id="5a738-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="5a738-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a738-178">Response</span></span>
<span data-ttu-id="5a738-179">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a738-179">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a738-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a738-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a738-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a738-181">Request</span></span>
<span data-ttu-id="5a738-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a738-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5a738-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a738-183">Response</span></span>
<span data-ttu-id="5a738-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a738-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





