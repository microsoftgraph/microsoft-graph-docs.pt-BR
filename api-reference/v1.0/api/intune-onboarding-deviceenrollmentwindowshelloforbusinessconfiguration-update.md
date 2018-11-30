---
title: Atualizar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Atualize as propriedades de um objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
ms.openlocfilehash: f91067a57dc4da7dc7d4850f72fbe267f364c6e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007504"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="c324e-103">Atualizar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="c324e-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="c324e-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c324e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c324e-105">Atualize as propriedades de um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c324e-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c324e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c324e-106">Prerequisites</span></span>
<span data-ttu-id="c324e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c324e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c324e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c324e-109">Permission type</span></span>|<span data-ttu-id="c324e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c324e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c324e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c324e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c324e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c324e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c324e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c324e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c324e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c324e-114">Not supported.</span></span>|
|<span data-ttu-id="c324e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c324e-115">Application</span></span>|<span data-ttu-id="c324e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c324e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c324e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c324e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c324e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c324e-118">Request headers</span></span>
|<span data-ttu-id="c324e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c324e-119">Header</span></span>|<span data-ttu-id="c324e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c324e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c324e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c324e-121">Authorization</span></span>|<span data-ttu-id="c324e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c324e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c324e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c324e-123">Accept</span></span>|<span data-ttu-id="c324e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c324e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c324e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c324e-125">Request body</span></span>
<span data-ttu-id="c324e-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c324e-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="c324e-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c324e-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="c324e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c324e-128">Property</span></span>|<span data-ttu-id="c324e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c324e-129">Type</span></span>|<span data-ttu-id="c324e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c324e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c324e-131">id</span><span class="sxs-lookup"><span data-stu-id="c324e-131">id</span></span>|<span data-ttu-id="c324e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c324e-132">String</span></span>|<span data-ttu-id="c324e-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c324e-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c324e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c324e-134">displayName</span></span>|<span data-ttu-id="c324e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c324e-135">String</span></span>|<span data-ttu-id="c324e-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c324e-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c324e-137">description</span><span class="sxs-lookup"><span data-stu-id="c324e-137">description</span></span>|<span data-ttu-id="c324e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c324e-138">String</span></span>|<span data-ttu-id="c324e-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c324e-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c324e-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="c324e-140">priority</span></span>|<span data-ttu-id="c324e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c324e-141">Int32</span></span>|<span data-ttu-id="c324e-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c324e-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c324e-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c324e-143">createdDateTime</span></span>|<span data-ttu-id="c324e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c324e-144">DateTimeOffset</span></span>|<span data-ttu-id="c324e-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c324e-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c324e-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c324e-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c324e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c324e-147">DateTimeOffset</span></span>|<span data-ttu-id="c324e-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c324e-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c324e-149">version</span><span class="sxs-lookup"><span data-stu-id="c324e-149">version</span></span>|<span data-ttu-id="c324e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c324e-150">Int32</span></span>|<span data-ttu-id="c324e-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c324e-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c324e-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c324e-152">pinMinimumLength</span></span>|<span data-ttu-id="c324e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c324e-153">Int32</span></span>|<span data-ttu-id="c324e-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c324e-154">Not yet documented</span></span>|
|<span data-ttu-id="c324e-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="c324e-155">pinMaximumLength</span></span>|<span data-ttu-id="c324e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c324e-156">Int32</span></span>|<span data-ttu-id="c324e-157">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c324e-157">Not yet documented</span></span>|
|<span data-ttu-id="c324e-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c324e-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="c324e-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="c324e-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c324e-160">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="c324e-160">Not yet documented.</span></span> <span data-ttu-id="c324e-161">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="c324e-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c324e-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c324e-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="c324e-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="c324e-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c324e-164">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="c324e-164">Not yet documented.</span></span> <span data-ttu-id="c324e-165">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="c324e-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c324e-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c324e-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="c324e-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="c324e-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c324e-168">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="c324e-168">Not yet documented.</span></span> <span data-ttu-id="c324e-169">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="c324e-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c324e-170">state</span><span class="sxs-lookup"><span data-stu-id="c324e-170">state</span></span>|[<span data-ttu-id="c324e-171">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="c324e-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="c324e-172">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="c324e-172">Not yet documented.</span></span> <span data-ttu-id="c324e-173">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c324e-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="c324e-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="c324e-174">securityDeviceRequired</span></span>|<span data-ttu-id="c324e-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="c324e-175">Boolean</span></span>|<span data-ttu-id="c324e-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c324e-176">Not yet documented</span></span>|
|<span data-ttu-id="c324e-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="c324e-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="c324e-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="c324e-178">Boolean</span></span>|<span data-ttu-id="c324e-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c324e-179">Not yet documented</span></span>|
|<span data-ttu-id="c324e-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="c324e-180">remotePassportEnabled</span></span>|<span data-ttu-id="c324e-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="c324e-181">Boolean</span></span>|<span data-ttu-id="c324e-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c324e-182">Not yet documented</span></span>|
|<span data-ttu-id="c324e-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="c324e-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="c324e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c324e-184">Int32</span></span>|<span data-ttu-id="c324e-185">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c324e-185">Not yet documented</span></span>|
|<span data-ttu-id="c324e-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="c324e-186">pinExpirationInDays</span></span>|<span data-ttu-id="c324e-187">Int32</span><span class="sxs-lookup"><span data-stu-id="c324e-187">Int32</span></span>|<span data-ttu-id="c324e-188">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c324e-188">Not yet documented</span></span>|
|<span data-ttu-id="c324e-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="c324e-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="c324e-190">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="c324e-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="c324e-191">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="c324e-191">Not yet documented.</span></span> <span data-ttu-id="c324e-192">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c324e-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="c324e-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="c324e-193">Response</span></span>
<span data-ttu-id="c324e-194">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c324e-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c324e-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c324e-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="c324e-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c324e-196">Request</span></span>
<span data-ttu-id="c324e-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c324e-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c324e-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="c324e-198">Response</span></span>
<span data-ttu-id="c324e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c324e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



