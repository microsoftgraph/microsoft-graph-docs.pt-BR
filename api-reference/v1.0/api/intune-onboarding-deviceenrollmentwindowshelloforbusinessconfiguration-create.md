---
title: Criar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Crie um novo objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f86fd9fc1a8028ab983dce46998046b1515c761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983076"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="fd492-103">Criar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd492-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="fd492-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fd492-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd492-105">Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd492-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd492-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd492-106">Prerequisites</span></span>
<span data-ttu-id="fd492-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd492-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd492-109">Permission type</span></span>|<span data-ttu-id="fd492-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd492-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd492-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd492-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd492-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd492-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd492-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd492-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd492-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd492-114">Not supported.</span></span>|
|<span data-ttu-id="fd492-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd492-115">Application</span></span>|<span data-ttu-id="fd492-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd492-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd492-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd492-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fd492-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd492-118">Request headers</span></span>
|<span data-ttu-id="fd492-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd492-119">Header</span></span>|<span data-ttu-id="fd492-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fd492-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd492-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd492-121">Authorization</span></span>|<span data-ttu-id="fd492-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd492-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd492-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd492-123">Accept</span></span>|<span data-ttu-id="fd492-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd492-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd492-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd492-125">Request body</span></span>
<span data-ttu-id="fd492-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fd492-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="fd492-127">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fd492-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="fd492-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd492-128">Property</span></span>|<span data-ttu-id="fd492-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd492-129">Type</span></span>|<span data-ttu-id="fd492-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd492-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd492-131">id</span><span class="sxs-lookup"><span data-stu-id="fd492-131">id</span></span>|<span data-ttu-id="fd492-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd492-132">String</span></span>|<span data-ttu-id="fd492-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd492-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd492-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fd492-134">displayName</span></span>|<span data-ttu-id="fd492-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd492-135">String</span></span>|<span data-ttu-id="fd492-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd492-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd492-137">description</span><span class="sxs-lookup"><span data-stu-id="fd492-137">description</span></span>|<span data-ttu-id="fd492-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd492-138">String</span></span>|<span data-ttu-id="fd492-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd492-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd492-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="fd492-140">priority</span></span>|<span data-ttu-id="fd492-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fd492-141">Int32</span></span>|<span data-ttu-id="fd492-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd492-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd492-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd492-143">createdDateTime</span></span>|<span data-ttu-id="fd492-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd492-144">DateTimeOffset</span></span>|<span data-ttu-id="fd492-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd492-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd492-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd492-146">lastModifiedDateTime</span></span>|<span data-ttu-id="fd492-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd492-147">DateTimeOffset</span></span>|<span data-ttu-id="fd492-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd492-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd492-149">version</span><span class="sxs-lookup"><span data-stu-id="fd492-149">version</span></span>|<span data-ttu-id="fd492-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fd492-150">Int32</span></span>|<span data-ttu-id="fd492-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd492-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fd492-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fd492-152">pinMinimumLength</span></span>|<span data-ttu-id="fd492-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fd492-153">Int32</span></span>|<span data-ttu-id="fd492-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd492-154">Not yet documented</span></span>|
|<span data-ttu-id="fd492-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="fd492-155">pinMaximumLength</span></span>|<span data-ttu-id="fd492-156">Int32</span><span class="sxs-lookup"><span data-stu-id="fd492-156">Int32</span></span>|<span data-ttu-id="fd492-157">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd492-157">Not yet documented</span></span>|
|<span data-ttu-id="fd492-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fd492-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="fd492-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="fd492-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="fd492-160">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="fd492-160">Not yet documented.</span></span> <span data-ttu-id="fd492-161">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="fd492-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="fd492-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fd492-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="fd492-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="fd492-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="fd492-164">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="fd492-164">Not yet documented.</span></span> <span data-ttu-id="fd492-165">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="fd492-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="fd492-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fd492-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="fd492-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="fd492-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="fd492-168">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="fd492-168">Not yet documented.</span></span> <span data-ttu-id="fd492-169">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="fd492-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="fd492-170">estado</span><span class="sxs-lookup"><span data-stu-id="fd492-170">state</span></span>|[<span data-ttu-id="fd492-171">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="fd492-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="fd492-172">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="fd492-172">Not yet documented.</span></span> <span data-ttu-id="fd492-173">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="fd492-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fd492-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="fd492-174">securityDeviceRequired</span></span>|<span data-ttu-id="fd492-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd492-175">Boolean</span></span>|<span data-ttu-id="fd492-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd492-176">Not yet documented</span></span>|
|<span data-ttu-id="fd492-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="fd492-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="fd492-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd492-178">Boolean</span></span>|<span data-ttu-id="fd492-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd492-179">Not yet documented</span></span>|
|<span data-ttu-id="fd492-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="fd492-180">remotePassportEnabled</span></span>|<span data-ttu-id="fd492-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd492-181">Boolean</span></span>|<span data-ttu-id="fd492-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd492-182">Not yet documented</span></span>|
|<span data-ttu-id="fd492-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="fd492-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="fd492-184">Int32</span><span class="sxs-lookup"><span data-stu-id="fd492-184">Int32</span></span>|<span data-ttu-id="fd492-185">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd492-185">Not yet documented</span></span>|
|<span data-ttu-id="fd492-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="fd492-186">pinExpirationInDays</span></span>|<span data-ttu-id="fd492-187">Int32</span><span class="sxs-lookup"><span data-stu-id="fd492-187">Int32</span></span>|<span data-ttu-id="fd492-188">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fd492-188">Not yet documented</span></span>|
|<span data-ttu-id="fd492-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="fd492-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="fd492-190">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="fd492-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="fd492-191">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="fd492-191">Not yet documented.</span></span> <span data-ttu-id="fd492-192">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="fd492-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="fd492-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd492-193">Response</span></span>
<span data-ttu-id="fd492-194">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd492-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd492-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd492-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd492-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd492-196">Request</span></span>
<span data-ttu-id="fd492-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd492-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="fd492-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd492-198">Response</span></span>
<span data-ttu-id="fd492-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd492-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



