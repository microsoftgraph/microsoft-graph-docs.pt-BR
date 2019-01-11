---
title: Criar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Crie um novo objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd395803e5940855c3eb21e5ca1ca8b8b1ec3bdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829488"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="58513-103">Criar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="58513-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="58513-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="58513-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58513-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="58513-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58513-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="58513-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58513-107">Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58513-107">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58513-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58513-108">Prerequisites</span></span>
<span data-ttu-id="58513-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58513-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58513-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58513-111">Permission type</span></span>|<span data-ttu-id="58513-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58513-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58513-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58513-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58513-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58513-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58513-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58513-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58513-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58513-116">Not supported.</span></span>|
|<span data-ttu-id="58513-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58513-117">Application</span></span>|<span data-ttu-id="58513-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58513-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58513-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58513-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="58513-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58513-120">Request headers</span></span>
|<span data-ttu-id="58513-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58513-121">Header</span></span>|<span data-ttu-id="58513-122">Valor</span><span class="sxs-lookup"><span data-stu-id="58513-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58513-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58513-123">Authorization</span></span>|<span data-ttu-id="58513-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58513-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58513-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58513-125">Accept</span></span>|<span data-ttu-id="58513-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58513-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58513-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58513-127">Request body</span></span>
<span data-ttu-id="58513-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="58513-128">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="58513-129">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="58513-129">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="58513-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58513-130">Property</span></span>|<span data-ttu-id="58513-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="58513-131">Type</span></span>|<span data-ttu-id="58513-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="58513-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58513-133">id</span><span class="sxs-lookup"><span data-stu-id="58513-133">id</span></span>|<span data-ttu-id="58513-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58513-134">String</span></span>|<span data-ttu-id="58513-135">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58513-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="58513-136">displayName</span><span class="sxs-lookup"><span data-stu-id="58513-136">displayName</span></span>|<span data-ttu-id="58513-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58513-137">String</span></span>|<span data-ttu-id="58513-138">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58513-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="58513-139">description</span><span class="sxs-lookup"><span data-stu-id="58513-139">description</span></span>|<span data-ttu-id="58513-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58513-140">String</span></span>|<span data-ttu-id="58513-141">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58513-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="58513-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="58513-142">priority</span></span>|<span data-ttu-id="58513-143">Int32</span><span class="sxs-lookup"><span data-stu-id="58513-143">Int32</span></span>|<span data-ttu-id="58513-144">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58513-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="58513-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58513-145">createdDateTime</span></span>|<span data-ttu-id="58513-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58513-146">DateTimeOffset</span></span>|<span data-ttu-id="58513-147">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58513-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="58513-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58513-148">lastModifiedDateTime</span></span>|<span data-ttu-id="58513-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58513-149">DateTimeOffset</span></span>|<span data-ttu-id="58513-150">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58513-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="58513-151">version</span><span class="sxs-lookup"><span data-stu-id="58513-151">version</span></span>|<span data-ttu-id="58513-152">Int32</span><span class="sxs-lookup"><span data-stu-id="58513-152">Int32</span></span>|<span data-ttu-id="58513-153">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58513-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="58513-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="58513-154">pinMinimumLength</span></span>|<span data-ttu-id="58513-155">Int32</span><span class="sxs-lookup"><span data-stu-id="58513-155">Int32</span></span>|<span data-ttu-id="58513-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58513-156">Not yet documented</span></span>|
|<span data-ttu-id="58513-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="58513-157">pinMaximumLength</span></span>|<span data-ttu-id="58513-158">Int32</span><span class="sxs-lookup"><span data-stu-id="58513-158">Int32</span></span>|<span data-ttu-id="58513-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58513-159">Not yet documented</span></span>|
|<span data-ttu-id="58513-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="58513-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="58513-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="58513-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="58513-162">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="58513-162">Not yet documented.</span></span> <span data-ttu-id="58513-163">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="58513-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="58513-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="58513-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="58513-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="58513-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="58513-166">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="58513-166">Not yet documented.</span></span> <span data-ttu-id="58513-167">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="58513-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="58513-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="58513-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="58513-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="58513-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="58513-170">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="58513-170">Not yet documented.</span></span> <span data-ttu-id="58513-171">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="58513-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="58513-172">estado</span><span class="sxs-lookup"><span data-stu-id="58513-172">state</span></span>|[<span data-ttu-id="58513-173">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="58513-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="58513-174">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="58513-174">Not yet documented.</span></span> <span data-ttu-id="58513-175">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="58513-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="58513-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="58513-176">securityDeviceRequired</span></span>|<span data-ttu-id="58513-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="58513-177">Boolean</span></span>|<span data-ttu-id="58513-178">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58513-178">Not yet documented</span></span>|
|<span data-ttu-id="58513-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="58513-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="58513-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="58513-180">Boolean</span></span>|<span data-ttu-id="58513-181">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58513-181">Not yet documented</span></span>|
|<span data-ttu-id="58513-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="58513-182">remotePassportEnabled</span></span>|<span data-ttu-id="58513-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="58513-183">Boolean</span></span>|<span data-ttu-id="58513-184">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58513-184">Not yet documented</span></span>|
|<span data-ttu-id="58513-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="58513-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="58513-186">Int32</span><span class="sxs-lookup"><span data-stu-id="58513-186">Int32</span></span>|<span data-ttu-id="58513-187">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58513-187">Not yet documented</span></span>|
|<span data-ttu-id="58513-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="58513-188">pinExpirationInDays</span></span>|<span data-ttu-id="58513-189">Int32</span><span class="sxs-lookup"><span data-stu-id="58513-189">Int32</span></span>|<span data-ttu-id="58513-190">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58513-190">Not yet documented</span></span>|
|<span data-ttu-id="58513-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="58513-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="58513-192">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="58513-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="58513-193">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="58513-193">Not yet documented.</span></span> <span data-ttu-id="58513-194">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="58513-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="58513-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="58513-195">Response</span></span>
<span data-ttu-id="58513-196">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58513-196">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58513-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58513-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="58513-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58513-198">Request</span></span>
<span data-ttu-id="58513-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58513-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 693

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="58513-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="58513-200">Response</span></span>
<span data-ttu-id="58513-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58513-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





