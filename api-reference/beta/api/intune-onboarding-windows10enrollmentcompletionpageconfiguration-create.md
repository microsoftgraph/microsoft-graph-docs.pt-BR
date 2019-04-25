---
title: Criar windows10EnrollmentCompletionPageConfiguration
description: Criar um novo objeto windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c2edde71ba4ec8b61fe8894f05b0a6501df053c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528040"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="f6903-103">Criar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="f6903-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="f6903-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6903-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6903-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6903-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6903-106">Criar um novo objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f6903-106">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6903-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6903-107">Prerequisites</span></span>
<span data-ttu-id="f6903-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6903-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6903-110">Permission type</span></span>|<span data-ttu-id="f6903-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f6903-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6903-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6903-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6903-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6903-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f6903-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6903-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6903-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6903-115">Not supported.</span></span>|
|<span data-ttu-id="f6903-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6903-116">Application</span></span>|<span data-ttu-id="f6903-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6903-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6903-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6903-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f6903-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6903-119">Request headers</span></span>
|<span data-ttu-id="f6903-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6903-120">Header</span></span>|<span data-ttu-id="f6903-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f6903-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6903-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6903-122">Authorization</span></span>|<span data-ttu-id="f6903-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6903-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6903-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6903-124">Accept</span></span>|<span data-ttu-id="f6903-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6903-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6903-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6903-126">Request body</span></span>
<span data-ttu-id="f6903-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f6903-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="f6903-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f6903-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="f6903-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6903-129">Property</span></span>|<span data-ttu-id="f6903-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6903-130">Type</span></span>|<span data-ttu-id="f6903-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6903-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6903-132">id</span><span class="sxs-lookup"><span data-stu-id="f6903-132">id</span></span>|<span data-ttu-id="f6903-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6903-133">String</span></span>|<span data-ttu-id="f6903-134">ID da configuração da página de status de registro herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6903-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f6903-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f6903-135">displayName</span></span>|<span data-ttu-id="f6903-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6903-136">String</span></span>|<span data-ttu-id="f6903-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6903-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f6903-138">description</span><span class="sxs-lookup"><span data-stu-id="f6903-138">description</span></span>|<span data-ttu-id="f6903-139">String</span><span class="sxs-lookup"><span data-stu-id="f6903-139">String</span></span>|<span data-ttu-id="f6903-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6903-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f6903-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="f6903-141">priority</span></span>|<span data-ttu-id="f6903-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f6903-142">Int32</span></span>|<span data-ttu-id="f6903-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6903-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f6903-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6903-144">createdDateTime</span></span>|<span data-ttu-id="f6903-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6903-145">DateTimeOffset</span></span>|<span data-ttu-id="f6903-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6903-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f6903-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6903-147">lastModifiedDateTime</span></span>|<span data-ttu-id="f6903-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6903-148">DateTimeOffset</span></span>|<span data-ttu-id="f6903-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6903-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f6903-150">versão</span><span class="sxs-lookup"><span data-stu-id="f6903-150">version</span></span>|<span data-ttu-id="f6903-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f6903-151">Int32</span></span>|<span data-ttu-id="f6903-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6903-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f6903-153">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="f6903-153">showInstallationProgress</span></span>|<span data-ttu-id="f6903-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6903-154">Boolean</span></span>|<span data-ttu-id="f6903-155">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="f6903-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="f6903-156">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="f6903-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="f6903-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6903-157">Boolean</span></span>|<span data-ttu-id="f6903-158">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="f6903-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="f6903-159">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f6903-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="f6903-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6903-160">Boolean</span></span>|<span data-ttu-id="f6903-161">Permitir ou bloquear falha de redefinição de dispositivo na instalação</span><span class="sxs-lookup"><span data-stu-id="f6903-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="f6903-162">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f6903-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="f6903-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6903-163">Boolean</span></span>|<span data-ttu-id="f6903-164">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="f6903-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="f6903-165">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="f6903-165">customErrorMessage</span></span>|<span data-ttu-id="f6903-166">String</span><span class="sxs-lookup"><span data-stu-id="f6903-166">String</span></span>|<span data-ttu-id="f6903-167">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="f6903-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="f6903-168">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="f6903-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="f6903-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f6903-169">Int32</span></span>|<span data-ttu-id="f6903-170">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="f6903-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="f6903-171">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f6903-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="f6903-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6903-172">Boolean</span></span>|<span data-ttu-id="f6903-173">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="f6903-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="f6903-174">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="f6903-174">selectedMobileAppIds</span></span>|<span data-ttu-id="f6903-175">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6903-175">String collection</span></span>|<span data-ttu-id="f6903-176">Aplicativos selecionados para acompanhar o status de instalação</span><span class="sxs-lookup"><span data-stu-id="f6903-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="f6903-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6903-177">Response</span></span>
<span data-ttu-id="f6903-178">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6903-178">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6903-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6903-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6903-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6903-180">Request</span></span>
<span data-ttu-id="f6903-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6903-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="f6903-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6903-182">Response</span></span>
<span data-ttu-id="f6903-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6903-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





