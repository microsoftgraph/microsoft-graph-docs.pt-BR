---
title: Criar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Crie um novo objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbd45a72db4b226ec23cdd8221cbb16cb27ba771
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362551"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="05879-103">Criar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="05879-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="05879-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05879-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05879-105">Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05879-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05879-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05879-106">Prerequisites</span></span>
<span data-ttu-id="05879-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05879-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05879-109">Permission type</span></span>|<span data-ttu-id="05879-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05879-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05879-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05879-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05879-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05879-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="05879-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05879-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05879-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05879-114">Not supported.</span></span>|
|<span data-ttu-id="05879-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05879-115">Application</span></span>|<span data-ttu-id="05879-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05879-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05879-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05879-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="05879-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05879-118">Request headers</span></span>
|<span data-ttu-id="05879-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05879-119">Header</span></span>|<span data-ttu-id="05879-120">Valor</span><span class="sxs-lookup"><span data-stu-id="05879-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05879-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="05879-121">Authorization</span></span>|<span data-ttu-id="05879-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05879-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05879-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05879-123">Accept</span></span>|<span data-ttu-id="05879-124">application/json</span><span class="sxs-lookup"><span data-stu-id="05879-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05879-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05879-125">Request body</span></span>
<span data-ttu-id="05879-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05879-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="05879-127">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05879-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="05879-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05879-128">Property</span></span>|<span data-ttu-id="05879-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="05879-129">Type</span></span>|<span data-ttu-id="05879-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="05879-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05879-131">id</span><span class="sxs-lookup"><span data-stu-id="05879-131">id</span></span>|<span data-ttu-id="05879-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05879-132">String</span></span>|<span data-ttu-id="05879-133">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05879-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="05879-134">displayName</span><span class="sxs-lookup"><span data-stu-id="05879-134">displayName</span></span>|<span data-ttu-id="05879-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05879-135">String</span></span>|<span data-ttu-id="05879-136">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05879-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="05879-137">descrição</span><span class="sxs-lookup"><span data-stu-id="05879-137">description</span></span>|<span data-ttu-id="05879-138">String</span><span class="sxs-lookup"><span data-stu-id="05879-138">String</span></span>|<span data-ttu-id="05879-139">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05879-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="05879-140">prioridade</span><span class="sxs-lookup"><span data-stu-id="05879-140">priority</span></span>|<span data-ttu-id="05879-141">Int32</span><span class="sxs-lookup"><span data-stu-id="05879-141">Int32</span></span>|<span data-ttu-id="05879-142">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05879-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="05879-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05879-143">createdDateTime</span></span>|<span data-ttu-id="05879-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05879-144">DateTimeOffset</span></span>|<span data-ttu-id="05879-145">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05879-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="05879-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05879-146">lastModifiedDateTime</span></span>|<span data-ttu-id="05879-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05879-147">DateTimeOffset</span></span>|<span data-ttu-id="05879-148">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05879-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="05879-149">versão</span><span class="sxs-lookup"><span data-stu-id="05879-149">version</span></span>|<span data-ttu-id="05879-150">Int32</span><span class="sxs-lookup"><span data-stu-id="05879-150">Int32</span></span>|<span data-ttu-id="05879-151">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05879-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="05879-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="05879-152">pinMinimumLength</span></span>|<span data-ttu-id="05879-153">Int32</span><span class="sxs-lookup"><span data-stu-id="05879-153">Int32</span></span>|<span data-ttu-id="05879-154">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05879-154">Not yet documented</span></span>|
|<span data-ttu-id="05879-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="05879-155">pinMaximumLength</span></span>|<span data-ttu-id="05879-156">Int32</span><span class="sxs-lookup"><span data-stu-id="05879-156">Int32</span></span>|<span data-ttu-id="05879-157">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05879-157">Not yet documented</span></span>|
|<span data-ttu-id="05879-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="05879-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="05879-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="05879-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="05879-160">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="05879-160">Not yet documented.</span></span> <span data-ttu-id="05879-161">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="05879-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="05879-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="05879-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="05879-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="05879-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="05879-164">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="05879-164">Not yet documented.</span></span> <span data-ttu-id="05879-165">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="05879-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="05879-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="05879-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="05879-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="05879-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="05879-168">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="05879-168">Not yet documented.</span></span> <span data-ttu-id="05879-169">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="05879-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="05879-170">state</span><span class="sxs-lookup"><span data-stu-id="05879-170">state</span></span>|[<span data-ttu-id="05879-171">habilitação</span><span class="sxs-lookup"><span data-stu-id="05879-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="05879-172">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="05879-172">Not yet documented.</span></span> <span data-ttu-id="05879-173">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="05879-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="05879-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="05879-174">securityDeviceRequired</span></span>|<span data-ttu-id="05879-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="05879-175">Boolean</span></span>|<span data-ttu-id="05879-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05879-176">Not yet documented</span></span>|
|<span data-ttu-id="05879-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="05879-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="05879-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="05879-178">Boolean</span></span>|<span data-ttu-id="05879-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05879-179">Not yet documented</span></span>|
|<span data-ttu-id="05879-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="05879-180">remotePassportEnabled</span></span>|<span data-ttu-id="05879-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="05879-181">Boolean</span></span>|<span data-ttu-id="05879-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05879-182">Not yet documented</span></span>|
|<span data-ttu-id="05879-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="05879-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="05879-184">Int32</span><span class="sxs-lookup"><span data-stu-id="05879-184">Int32</span></span>|<span data-ttu-id="05879-185">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05879-185">Not yet documented</span></span>|
|<span data-ttu-id="05879-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="05879-186">pinExpirationInDays</span></span>|<span data-ttu-id="05879-187">Int32</span><span class="sxs-lookup"><span data-stu-id="05879-187">Int32</span></span>|<span data-ttu-id="05879-188">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05879-188">Not yet documented</span></span>|
|<span data-ttu-id="05879-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="05879-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="05879-190">habilitação</span><span class="sxs-lookup"><span data-stu-id="05879-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="05879-191">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="05879-191">Not yet documented.</span></span> <span data-ttu-id="05879-192">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="05879-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="05879-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="05879-193">Response</span></span>
<span data-ttu-id="05879-194">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05879-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05879-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05879-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="05879-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05879-196">Request</span></span>
<span data-ttu-id="05879-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05879-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05879-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="05879-198">Response</span></span>
<span data-ttu-id="05879-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05879-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




