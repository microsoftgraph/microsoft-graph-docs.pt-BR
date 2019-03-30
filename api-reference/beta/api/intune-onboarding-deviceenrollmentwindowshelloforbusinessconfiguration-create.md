---
title: Criar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Crie um novo objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f3e3188293455ca8ae7fd36b5040eec890df35d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985302"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="1e0b5-103">Criar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e0b5-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="1e0b5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e0b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e0b5-106">Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0b5-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e0b5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e0b5-107">Prerequisites</span></span>
<span data-ttu-id="1e0b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e0b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e0b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e0b5-110">Permission type</span></span>|<span data-ttu-id="1e0b5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e0b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e0b5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e0b5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1e0b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e0b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-115">Not supported.</span></span>|
|<span data-ttu-id="1e0b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e0b5-116">Application</span></span>|<span data-ttu-id="1e0b5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e0b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e0b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e0b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e0b5-119">Request headers</span></span>
|<span data-ttu-id="1e0b5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e0b5-120">Header</span></span>|<span data-ttu-id="1e0b5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e0b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e0b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e0b5-122">Authorization</span></span>|<span data-ttu-id="1e0b5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e0b5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e0b5-124">Accept</span></span>|<span data-ttu-id="1e0b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e0b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e0b5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e0b5-126">Request body</span></span>
<span data-ttu-id="1e0b5-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="1e0b5-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="1e0b5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e0b5-129">Property</span></span>|<span data-ttu-id="1e0b5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e0b5-130">Type</span></span>|<span data-ttu-id="1e0b5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e0b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e0b5-132">id</span><span class="sxs-lookup"><span data-stu-id="1e0b5-132">id</span></span>|<span data-ttu-id="1e0b5-133">String</span><span class="sxs-lookup"><span data-stu-id="1e0b5-133">String</span></span>|<span data-ttu-id="1e0b5-134">ID da configuração da página de status de registro herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e0b5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1e0b5-135">displayName</span></span>|<span data-ttu-id="1e0b5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e0b5-136">String</span></span>|<span data-ttu-id="1e0b5-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e0b5-138">description</span><span class="sxs-lookup"><span data-stu-id="1e0b5-138">description</span></span>|<span data-ttu-id="1e0b5-139">String</span><span class="sxs-lookup"><span data-stu-id="1e0b5-139">String</span></span>|<span data-ttu-id="1e0b5-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e0b5-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="1e0b5-141">priority</span></span>|<span data-ttu-id="1e0b5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1e0b5-142">Int32</span></span>|<span data-ttu-id="1e0b5-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e0b5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e0b5-144">createdDateTime</span></span>|<span data-ttu-id="1e0b5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e0b5-145">DateTimeOffset</span></span>|<span data-ttu-id="1e0b5-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e0b5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e0b5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="1e0b5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e0b5-148">DateTimeOffset</span></span>|<span data-ttu-id="1e0b5-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e0b5-150">versão</span><span class="sxs-lookup"><span data-stu-id="1e0b5-150">version</span></span>|<span data-ttu-id="1e0b5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1e0b5-151">Int32</span></span>|<span data-ttu-id="1e0b5-152">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e0b5-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1e0b5-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1e0b5-153">pinMinimumLength</span></span>|<span data-ttu-id="1e0b5-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1e0b5-154">Int32</span></span>|<span data-ttu-id="1e0b5-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e0b5-155">Not yet documented</span></span>|
|<span data-ttu-id="1e0b5-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="1e0b5-156">pinMaximumLength</span></span>|<span data-ttu-id="1e0b5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="1e0b5-157">Int32</span></span>|<span data-ttu-id="1e0b5-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e0b5-158">Not yet documented</span></span>|
|<span data-ttu-id="1e0b5-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1e0b5-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="1e0b5-160">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1e0b5-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1e0b5-161">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-161">Not yet documented.</span></span> <span data-ttu-id="1e0b5-162">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1e0b5-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1e0b5-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="1e0b5-164">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1e0b5-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1e0b5-165">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-165">Not yet documented.</span></span> <span data-ttu-id="1e0b5-166">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1e0b5-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1e0b5-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="1e0b5-168">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1e0b5-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1e0b5-169">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-169">Not yet documented.</span></span> <span data-ttu-id="1e0b5-170">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1e0b5-171">state</span><span class="sxs-lookup"><span data-stu-id="1e0b5-171">state</span></span>|[<span data-ttu-id="1e0b5-172">habilitação</span><span class="sxs-lookup"><span data-stu-id="1e0b5-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1e0b5-173">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-173">Not yet documented.</span></span> <span data-ttu-id="1e0b5-174">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1e0b5-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="1e0b5-175">securityDeviceRequired</span></span>|<span data-ttu-id="1e0b5-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e0b5-176">Boolean</span></span>|<span data-ttu-id="1e0b5-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e0b5-177">Not yet documented</span></span>|
|<span data-ttu-id="1e0b5-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="1e0b5-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="1e0b5-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e0b5-179">Boolean</span></span>|<span data-ttu-id="1e0b5-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e0b5-180">Not yet documented</span></span>|
|<span data-ttu-id="1e0b5-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="1e0b5-181">remotePassportEnabled</span></span>|<span data-ttu-id="1e0b5-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e0b5-182">Boolean</span></span>|<span data-ttu-id="1e0b5-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e0b5-183">Not yet documented</span></span>|
|<span data-ttu-id="1e0b5-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="1e0b5-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="1e0b5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1e0b5-185">Int32</span></span>|<span data-ttu-id="1e0b5-186">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e0b5-186">Not yet documented</span></span>|
|<span data-ttu-id="1e0b5-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="1e0b5-187">pinExpirationInDays</span></span>|<span data-ttu-id="1e0b5-188">Int32</span><span class="sxs-lookup"><span data-stu-id="1e0b5-188">Int32</span></span>|<span data-ttu-id="1e0b5-189">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1e0b5-189">Not yet documented</span></span>|
|<span data-ttu-id="1e0b5-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="1e0b5-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="1e0b5-191">habilitação</span><span class="sxs-lookup"><span data-stu-id="1e0b5-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1e0b5-192">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-192">Not yet documented.</span></span> <span data-ttu-id="1e0b5-193">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="1e0b5-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e0b5-194">Response</span></span>
<span data-ttu-id="1e0b5-195">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e0b5-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e0b5-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e0b5-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e0b5-197">Request</span></span>
<span data-ttu-id="1e0b5-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e0b5-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e0b5-199">Response</span></span>
<span data-ttu-id="1e0b5-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e0b5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




