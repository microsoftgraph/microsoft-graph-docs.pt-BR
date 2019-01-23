---
title: Criar windows10EnrollmentCompletionPageConfiguration
description: Crie um novo objeto de windows10EnrollmentCompletionPageConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4e7797ac1cd3ca46724c046e43bfa1fa1649ebb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411355"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="9a696-103">Criar windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a696-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="9a696-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a696-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a696-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a696-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a696-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9a696-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a696-107">Crie um novo objeto de [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9a696-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a696-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a696-108">Prerequisites</span></span>
<span data-ttu-id="9a696-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a696-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a696-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a696-111">Permission type</span></span>|<span data-ttu-id="9a696-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a696-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a696-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a696-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a696-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a696-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a696-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a696-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a696-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a696-116">Not supported.</span></span>|
|<span data-ttu-id="9a696-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a696-117">Application</span></span>|<span data-ttu-id="9a696-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a696-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a696-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a696-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9a696-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a696-120">Request headers</span></span>
|<span data-ttu-id="9a696-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a696-121">Header</span></span>|<span data-ttu-id="9a696-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a696-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a696-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a696-123">Authorization</span></span>|<span data-ttu-id="9a696-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a696-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a696-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a696-125">Accept</span></span>|<span data-ttu-id="9a696-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a696-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a696-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a696-127">Request body</span></span>
<span data-ttu-id="9a696-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9a696-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="9a696-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9a696-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="9a696-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a696-130">Property</span></span>|<span data-ttu-id="9a696-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a696-131">Type</span></span>|<span data-ttu-id="9a696-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a696-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a696-133">id</span><span class="sxs-lookup"><span data-stu-id="9a696-133">id</span></span>|<span data-ttu-id="9a696-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a696-134">String</span></span>|<span data-ttu-id="9a696-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a696-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a696-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9a696-136">displayName</span></span>|<span data-ttu-id="9a696-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a696-137">String</span></span>|<span data-ttu-id="9a696-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a696-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a696-139">description</span><span class="sxs-lookup"><span data-stu-id="9a696-139">description</span></span>|<span data-ttu-id="9a696-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a696-140">String</span></span>|<span data-ttu-id="9a696-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a696-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a696-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="9a696-142">priority</span></span>|<span data-ttu-id="9a696-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9a696-143">Int32</span></span>|<span data-ttu-id="9a696-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a696-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a696-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a696-145">createdDateTime</span></span>|<span data-ttu-id="9a696-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a696-146">DateTimeOffset</span></span>|<span data-ttu-id="9a696-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a696-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a696-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a696-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9a696-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a696-149">DateTimeOffset</span></span>|<span data-ttu-id="9a696-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a696-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a696-151">version</span><span class="sxs-lookup"><span data-stu-id="9a696-151">version</span></span>|<span data-ttu-id="9a696-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9a696-152">Int32</span></span>|<span data-ttu-id="9a696-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a696-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a696-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="9a696-154">showInstallationProgress</span></span>|<span data-ttu-id="9a696-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a696-155">Boolean</span></span>|<span data-ttu-id="9a696-156">Mostrar ou ocultar o progresso da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="9a696-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="9a696-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="9a696-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="9a696-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a696-158">Boolean</span></span>|<span data-ttu-id="9a696-159">Permitir que o usuário repetir a instalação em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="9a696-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="9a696-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="9a696-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="9a696-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a696-161">Boolean</span></span>|<span data-ttu-id="9a696-162">Permitir ou bloquear o dispositivo redefinir em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="9a696-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="9a696-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="9a696-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="9a696-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a696-164">Boolean</span></span>|<span data-ttu-id="9a696-165">Permitir ou bloquear o conjunto de log em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="9a696-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="9a696-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="9a696-166">customErrorMessage</span></span>|<span data-ttu-id="9a696-167">String</span><span class="sxs-lookup"><span data-stu-id="9a696-167">String</span></span>|<span data-ttu-id="9a696-168">Definir a mensagem de erro personalizada para mostrar após a falha de instalação</span><span class="sxs-lookup"><span data-stu-id="9a696-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="9a696-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="9a696-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="9a696-170">Int32</span><span class="sxs-lookup"><span data-stu-id="9a696-170">Int32</span></span>|<span data-ttu-id="9a696-171">Definir tempo limite de progresso de instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="9a696-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="9a696-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="9a696-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="9a696-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a696-173">Boolean</span></span>|<span data-ttu-id="9a696-174">Permitir que o usuário continue a usar o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="9a696-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="9a696-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="9a696-175">selectedMobileAppIds</span></span>|<span data-ttu-id="9a696-176">String collection</span><span class="sxs-lookup"><span data-stu-id="9a696-176">String collection</span></span>|<span data-ttu-id="9a696-177">Aplicativos selecionados para rastrear o status de instalação</span><span class="sxs-lookup"><span data-stu-id="9a696-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="9a696-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a696-178">Response</span></span>
<span data-ttu-id="9a696-179">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a696-179">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a696-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a696-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a696-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a696-181">Request</span></span>
<span data-ttu-id="9a696-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a696-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a696-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a696-183">Response</span></span>
<span data-ttu-id="9a696-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a696-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




