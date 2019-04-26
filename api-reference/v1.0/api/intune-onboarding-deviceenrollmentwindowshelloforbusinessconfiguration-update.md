---
title: Atualizar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Atualize as propriedades de um objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3225f7fe36f5ec8a66df8424a06d8569b7c92efd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561625"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="07bbc-103">Atualizar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="07bbc-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="07bbc-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07bbc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07bbc-105">Atualize as propriedades de um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07bbc-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07bbc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07bbc-106">Prerequisites</span></span>
<span data-ttu-id="07bbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07bbc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07bbc-109">Permission type</span></span>|<span data-ttu-id="07bbc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07bbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07bbc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07bbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="07bbc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07bbc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="07bbc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07bbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07bbc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07bbc-114">Not supported.</span></span>|
|<span data-ttu-id="07bbc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07bbc-115">Application</span></span>|<span data-ttu-id="07bbc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07bbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07bbc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07bbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="07bbc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07bbc-118">Request headers</span></span>
|<span data-ttu-id="07bbc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07bbc-119">Header</span></span>|<span data-ttu-id="07bbc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="07bbc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07bbc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="07bbc-121">Authorization</span></span>|<span data-ttu-id="07bbc-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07bbc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07bbc-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07bbc-123">Accept</span></span>|<span data-ttu-id="07bbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="07bbc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07bbc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07bbc-125">Request body</span></span>
<span data-ttu-id="07bbc-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07bbc-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="07bbc-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07bbc-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="07bbc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07bbc-128">Property</span></span>|<span data-ttu-id="07bbc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="07bbc-129">Type</span></span>|<span data-ttu-id="07bbc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="07bbc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07bbc-131">id</span><span class="sxs-lookup"><span data-stu-id="07bbc-131">id</span></span>|<span data-ttu-id="07bbc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07bbc-132">String</span></span>|<span data-ttu-id="07bbc-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07bbc-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="07bbc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="07bbc-134">displayName</span></span>|<span data-ttu-id="07bbc-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07bbc-135">String</span></span>|<span data-ttu-id="07bbc-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07bbc-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="07bbc-137">description</span><span class="sxs-lookup"><span data-stu-id="07bbc-137">description</span></span>|<span data-ttu-id="07bbc-138">String</span><span class="sxs-lookup"><span data-stu-id="07bbc-138">String</span></span>|<span data-ttu-id="07bbc-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07bbc-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="07bbc-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="07bbc-140">priority</span></span>|<span data-ttu-id="07bbc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="07bbc-141">Int32</span></span>|<span data-ttu-id="07bbc-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07bbc-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="07bbc-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07bbc-143">createdDateTime</span></span>|<span data-ttu-id="07bbc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07bbc-144">DateTimeOffset</span></span>|<span data-ttu-id="07bbc-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07bbc-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="07bbc-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07bbc-146">lastModifiedDateTime</span></span>|<span data-ttu-id="07bbc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07bbc-147">DateTimeOffset</span></span>|<span data-ttu-id="07bbc-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07bbc-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="07bbc-149">versão</span><span class="sxs-lookup"><span data-stu-id="07bbc-149">version</span></span>|<span data-ttu-id="07bbc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="07bbc-150">Int32</span></span>|<span data-ttu-id="07bbc-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07bbc-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="07bbc-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="07bbc-152">pinMinimumLength</span></span>|<span data-ttu-id="07bbc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="07bbc-153">Int32</span></span>|<span data-ttu-id="07bbc-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07bbc-154">Not yet documented</span></span>|
|<span data-ttu-id="07bbc-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="07bbc-155">pinMaximumLength</span></span>|<span data-ttu-id="07bbc-156">Int32</span><span class="sxs-lookup"><span data-stu-id="07bbc-156">Int32</span></span>|<span data-ttu-id="07bbc-157">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07bbc-157">Not yet documented</span></span>|
|<span data-ttu-id="07bbc-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="07bbc-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="07bbc-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="07bbc-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="07bbc-160">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="07bbc-160">Not yet documented.</span></span> <span data-ttu-id="07bbc-161">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="07bbc-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="07bbc-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="07bbc-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="07bbc-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="07bbc-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="07bbc-164">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="07bbc-164">Not yet documented.</span></span> <span data-ttu-id="07bbc-165">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="07bbc-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="07bbc-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="07bbc-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="07bbc-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="07bbc-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="07bbc-168">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="07bbc-168">Not yet documented.</span></span> <span data-ttu-id="07bbc-169">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="07bbc-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="07bbc-170">estado</span><span class="sxs-lookup"><span data-stu-id="07bbc-170">state</span></span>|[<span data-ttu-id="07bbc-171">habilitação</span><span class="sxs-lookup"><span data-stu-id="07bbc-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="07bbc-172">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="07bbc-172">Not yet documented.</span></span> <span data-ttu-id="07bbc-173">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="07bbc-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="07bbc-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="07bbc-174">securityDeviceRequired</span></span>|<span data-ttu-id="07bbc-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="07bbc-175">Boolean</span></span>|<span data-ttu-id="07bbc-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07bbc-176">Not yet documented</span></span>|
|<span data-ttu-id="07bbc-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="07bbc-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="07bbc-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="07bbc-178">Boolean</span></span>|<span data-ttu-id="07bbc-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07bbc-179">Not yet documented</span></span>|
|<span data-ttu-id="07bbc-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="07bbc-180">remotePassportEnabled</span></span>|<span data-ttu-id="07bbc-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="07bbc-181">Boolean</span></span>|<span data-ttu-id="07bbc-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07bbc-182">Not yet documented</span></span>|
|<span data-ttu-id="07bbc-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="07bbc-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="07bbc-184">Int32</span><span class="sxs-lookup"><span data-stu-id="07bbc-184">Int32</span></span>|<span data-ttu-id="07bbc-185">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07bbc-185">Not yet documented</span></span>|
|<span data-ttu-id="07bbc-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="07bbc-186">pinExpirationInDays</span></span>|<span data-ttu-id="07bbc-187">Int32</span><span class="sxs-lookup"><span data-stu-id="07bbc-187">Int32</span></span>|<span data-ttu-id="07bbc-188">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07bbc-188">Not yet documented</span></span>|
|<span data-ttu-id="07bbc-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="07bbc-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="07bbc-190">habilitação</span><span class="sxs-lookup"><span data-stu-id="07bbc-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="07bbc-191">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="07bbc-191">Not yet documented.</span></span> <span data-ttu-id="07bbc-192">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="07bbc-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="07bbc-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="07bbc-193">Response</span></span>
<span data-ttu-id="07bbc-194">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07bbc-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07bbc-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07bbc-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="07bbc-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07bbc-196">Request</span></span>
<span data-ttu-id="07bbc-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07bbc-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07bbc-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="07bbc-198">Response</span></span>
<span data-ttu-id="07bbc-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07bbc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



