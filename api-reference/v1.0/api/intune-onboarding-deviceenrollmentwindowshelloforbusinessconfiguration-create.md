---
title: Criar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Crie um novo objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dfdc22edcd04638c5b5f7a332ede550feae98352
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512612"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="64ea7-103">Criar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="64ea7-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="64ea7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64ea7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64ea7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64ea7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64ea7-106">Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64ea7-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64ea7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64ea7-107">Prerequisites</span></span>
<span data-ttu-id="64ea7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64ea7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64ea7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64ea7-110">Permission type</span></span>|<span data-ttu-id="64ea7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64ea7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64ea7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64ea7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64ea7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64ea7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="64ea7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64ea7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64ea7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64ea7-115">Not supported.</span></span>|
|<span data-ttu-id="64ea7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64ea7-116">Application</span></span>|<span data-ttu-id="64ea7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64ea7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64ea7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64ea7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64ea7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64ea7-119">Request headers</span></span>
|<span data-ttu-id="64ea7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64ea7-120">Header</span></span>|<span data-ttu-id="64ea7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="64ea7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64ea7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64ea7-122">Authorization</span></span>|<span data-ttu-id="64ea7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64ea7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64ea7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64ea7-124">Accept</span></span>|<span data-ttu-id="64ea7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64ea7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64ea7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64ea7-126">Request body</span></span>
<span data-ttu-id="64ea7-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="64ea7-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="64ea7-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="64ea7-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="64ea7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64ea7-129">Property</span></span>|<span data-ttu-id="64ea7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="64ea7-130">Type</span></span>|<span data-ttu-id="64ea7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="64ea7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64ea7-132">id</span><span class="sxs-lookup"><span data-stu-id="64ea7-132">id</span></span>|<span data-ttu-id="64ea7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64ea7-133">String</span></span>|<span data-ttu-id="64ea7-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64ea7-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="64ea7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="64ea7-135">displayName</span></span>|<span data-ttu-id="64ea7-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64ea7-136">String</span></span>|<span data-ttu-id="64ea7-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64ea7-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="64ea7-138">description</span><span class="sxs-lookup"><span data-stu-id="64ea7-138">description</span></span>|<span data-ttu-id="64ea7-139">String</span><span class="sxs-lookup"><span data-stu-id="64ea7-139">String</span></span>|<span data-ttu-id="64ea7-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64ea7-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="64ea7-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="64ea7-141">priority</span></span>|<span data-ttu-id="64ea7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="64ea7-142">Int32</span></span>|<span data-ttu-id="64ea7-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64ea7-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="64ea7-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64ea7-144">createdDateTime</span></span>|<span data-ttu-id="64ea7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64ea7-145">DateTimeOffset</span></span>|<span data-ttu-id="64ea7-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64ea7-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="64ea7-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64ea7-147">lastModifiedDateTime</span></span>|<span data-ttu-id="64ea7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64ea7-148">DateTimeOffset</span></span>|<span data-ttu-id="64ea7-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64ea7-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="64ea7-150">versão</span><span class="sxs-lookup"><span data-stu-id="64ea7-150">version</span></span>|<span data-ttu-id="64ea7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="64ea7-151">Int32</span></span>|<span data-ttu-id="64ea7-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64ea7-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="64ea7-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="64ea7-153">pinMinimumLength</span></span>|<span data-ttu-id="64ea7-154">Int32</span><span class="sxs-lookup"><span data-stu-id="64ea7-154">Int32</span></span>|<span data-ttu-id="64ea7-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64ea7-155">Not yet documented</span></span>|
|<span data-ttu-id="64ea7-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="64ea7-156">pinMaximumLength</span></span>|<span data-ttu-id="64ea7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="64ea7-157">Int32</span></span>|<span data-ttu-id="64ea7-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64ea7-158">Not yet documented</span></span>|
|<span data-ttu-id="64ea7-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="64ea7-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="64ea7-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="64ea7-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="64ea7-161">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="64ea7-161">Not yet documented.</span></span> <span data-ttu-id="64ea7-162">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="64ea7-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="64ea7-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="64ea7-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="64ea7-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="64ea7-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="64ea7-165">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="64ea7-165">Not yet documented.</span></span> <span data-ttu-id="64ea7-166">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="64ea7-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="64ea7-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="64ea7-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="64ea7-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="64ea7-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="64ea7-169">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="64ea7-169">Not yet documented.</span></span> <span data-ttu-id="64ea7-170">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="64ea7-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="64ea7-171">state</span><span class="sxs-lookup"><span data-stu-id="64ea7-171">state</span></span>|[<span data-ttu-id="64ea7-172">habilitação</span><span class="sxs-lookup"><span data-stu-id="64ea7-172">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="64ea7-173">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="64ea7-173">Not yet documented.</span></span> <span data-ttu-id="64ea7-174">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64ea7-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="64ea7-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="64ea7-175">securityDeviceRequired</span></span>|<span data-ttu-id="64ea7-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="64ea7-176">Boolean</span></span>|<span data-ttu-id="64ea7-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64ea7-177">Not yet documented</span></span>|
|<span data-ttu-id="64ea7-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="64ea7-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="64ea7-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="64ea7-179">Boolean</span></span>|<span data-ttu-id="64ea7-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64ea7-180">Not yet documented</span></span>|
|<span data-ttu-id="64ea7-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="64ea7-181">remotePassportEnabled</span></span>|<span data-ttu-id="64ea7-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="64ea7-182">Boolean</span></span>|<span data-ttu-id="64ea7-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64ea7-183">Not yet documented</span></span>|
|<span data-ttu-id="64ea7-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="64ea7-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="64ea7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="64ea7-185">Int32</span></span>|<span data-ttu-id="64ea7-186">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64ea7-186">Not yet documented</span></span>|
|<span data-ttu-id="64ea7-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="64ea7-187">pinExpirationInDays</span></span>|<span data-ttu-id="64ea7-188">Int32</span><span class="sxs-lookup"><span data-stu-id="64ea7-188">Int32</span></span>|<span data-ttu-id="64ea7-189">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64ea7-189">Not yet documented</span></span>|
|<span data-ttu-id="64ea7-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="64ea7-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="64ea7-191">habilitação</span><span class="sxs-lookup"><span data-stu-id="64ea7-191">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="64ea7-192">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="64ea7-192">Not yet documented.</span></span> <span data-ttu-id="64ea7-193">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="64ea7-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="64ea7-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="64ea7-194">Response</span></span>
<span data-ttu-id="64ea7-195">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64ea7-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64ea7-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64ea7-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="64ea7-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64ea7-197">Request</span></span>
<span data-ttu-id="64ea7-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64ea7-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64ea7-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="64ea7-199">Response</span></span>
<span data-ttu-id="64ea7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64ea7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




