---
title: Criar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Crie um novo objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6198de8729f38517ac2110e6c20e19b620b206bf
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800711"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="6d5f6-103">Criar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d5f6-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="6d5f6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d5f6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d5f6-106">Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d5f6-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d5f6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d5f6-107">Prerequisites</span></span>
<span data-ttu-id="6d5f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d5f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d5f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d5f6-110">Permission type</span></span>|<span data-ttu-id="6d5f6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d5f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d5f6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d5f6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6d5f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d5f6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-115">Not supported.</span></span>|
|<span data-ttu-id="6d5f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d5f6-116">Application</span></span>|<span data-ttu-id="6d5f6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d5f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d5f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6d5f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d5f6-119">Request headers</span></span>
|<span data-ttu-id="6d5f6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d5f6-120">Header</span></span>|<span data-ttu-id="6d5f6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6d5f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d5f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d5f6-122">Authorization</span></span>|<span data-ttu-id="6d5f6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d5f6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d5f6-124">Accept</span></span>|<span data-ttu-id="6d5f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d5f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d5f6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d5f6-126">Request body</span></span>
<span data-ttu-id="6d5f6-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="6d5f6-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="6d5f6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d5f6-129">Property</span></span>|<span data-ttu-id="6d5f6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d5f6-130">Type</span></span>|<span data-ttu-id="6d5f6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d5f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d5f6-132">id</span><span class="sxs-lookup"><span data-stu-id="6d5f6-132">id</span></span>|<span data-ttu-id="6d5f6-133">String</span><span class="sxs-lookup"><span data-stu-id="6d5f6-133">String</span></span>|<span data-ttu-id="6d5f6-134">ID da configuração da página de status de registro herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d5f6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6d5f6-135">displayName</span></span>|<span data-ttu-id="6d5f6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d5f6-136">String</span></span>|<span data-ttu-id="6d5f6-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d5f6-138">description</span><span class="sxs-lookup"><span data-stu-id="6d5f6-138">description</span></span>|<span data-ttu-id="6d5f6-139">String</span><span class="sxs-lookup"><span data-stu-id="6d5f6-139">String</span></span>|<span data-ttu-id="6d5f6-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d5f6-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="6d5f6-141">priority</span></span>|<span data-ttu-id="6d5f6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5f6-142">Int32</span></span>|<span data-ttu-id="6d5f6-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d5f6-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d5f6-144">createdDateTime</span></span>|<span data-ttu-id="6d5f6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d5f6-145">DateTimeOffset</span></span>|<span data-ttu-id="6d5f6-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d5f6-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d5f6-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6d5f6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d5f6-148">DateTimeOffset</span></span>|<span data-ttu-id="6d5f6-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d5f6-150">versão</span><span class="sxs-lookup"><span data-stu-id="6d5f6-150">version</span></span>|<span data-ttu-id="6d5f6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5f6-151">Int32</span></span>|<span data-ttu-id="6d5f6-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d5f6-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6d5f6-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6d5f6-153">pinMinimumLength</span></span>|<span data-ttu-id="6d5f6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5f6-154">Int32</span></span>|<span data-ttu-id="6d5f6-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d5f6-155">Not yet documented</span></span>|
|<span data-ttu-id="6d5f6-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="6d5f6-156">pinMaximumLength</span></span>|<span data-ttu-id="6d5f6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5f6-157">Int32</span></span>|<span data-ttu-id="6d5f6-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d5f6-158">Not yet documented</span></span>|
|<span data-ttu-id="6d5f6-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6d5f6-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="6d5f6-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6d5f6-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6d5f6-161">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-161">Not yet documented.</span></span> <span data-ttu-id="6d5f6-162">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6d5f6-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6d5f6-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="6d5f6-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6d5f6-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6d5f6-165">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-165">Not yet documented.</span></span> <span data-ttu-id="6d5f6-166">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6d5f6-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="6d5f6-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="6d5f6-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="6d5f6-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="6d5f6-169">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-169">Not yet documented.</span></span> <span data-ttu-id="6d5f6-170">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="6d5f6-171">state</span><span class="sxs-lookup"><span data-stu-id="6d5f6-171">state</span></span>|[<span data-ttu-id="6d5f6-172">habilitação</span><span class="sxs-lookup"><span data-stu-id="6d5f6-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="6d5f6-173">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-173">Not yet documented.</span></span> <span data-ttu-id="6d5f6-174">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="6d5f6-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="6d5f6-175">securityDeviceRequired</span></span>|<span data-ttu-id="6d5f6-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d5f6-176">Boolean</span></span>|<span data-ttu-id="6d5f6-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d5f6-177">Not yet documented</span></span>|
|<span data-ttu-id="6d5f6-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="6d5f6-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="6d5f6-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d5f6-179">Boolean</span></span>|<span data-ttu-id="6d5f6-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d5f6-180">Not yet documented</span></span>|
|<span data-ttu-id="6d5f6-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="6d5f6-181">remotePassportEnabled</span></span>|<span data-ttu-id="6d5f6-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d5f6-182">Boolean</span></span>|<span data-ttu-id="6d5f6-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d5f6-183">Not yet documented</span></span>|
|<span data-ttu-id="6d5f6-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="6d5f6-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="6d5f6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5f6-185">Int32</span></span>|<span data-ttu-id="6d5f6-186">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d5f6-186">Not yet documented</span></span>|
|<span data-ttu-id="6d5f6-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="6d5f6-187">pinExpirationInDays</span></span>|<span data-ttu-id="6d5f6-188">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5f6-188">Int32</span></span>|<span data-ttu-id="6d5f6-189">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d5f6-189">Not yet documented</span></span>|
|<span data-ttu-id="6d5f6-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="6d5f6-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="6d5f6-191">habilitação</span><span class="sxs-lookup"><span data-stu-id="6d5f6-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="6d5f6-192">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-192">Not yet documented.</span></span> <span data-ttu-id="6d5f6-193">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="6d5f6-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d5f6-194">Response</span></span>
<span data-ttu-id="6d5f6-195">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d5f6-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d5f6-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d5f6-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d5f6-197">Request</span></span>
<span data-ttu-id="6d5f6-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="6d5f6-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d5f6-199">Response</span></span>
<span data-ttu-id="6d5f6-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d5f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```





