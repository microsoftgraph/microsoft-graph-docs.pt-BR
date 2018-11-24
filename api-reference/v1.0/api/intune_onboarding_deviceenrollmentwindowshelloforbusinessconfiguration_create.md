# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="82724-101">Criar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="82724-101">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="82724-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="82724-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82724-103">Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82724-103">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82724-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82724-104">Prerequisites</span></span>
<span data-ttu-id="82724-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="82724-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="82724-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82724-107">Permission type</span></span>|<span data-ttu-id="82724-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82724-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82724-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82724-109">Delegated (work or school account)</span></span>|<span data-ttu-id="82724-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82724-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82724-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82724-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82724-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82724-112">Not supported.</span></span>|
|<span data-ttu-id="82724-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82724-113">Application</span></span>|<span data-ttu-id="82724-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82724-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82724-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82724-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="82724-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82724-116">Request headers</span></span>
|<span data-ttu-id="82724-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82724-117">Header</span></span>|<span data-ttu-id="82724-118">Valor</span><span class="sxs-lookup"><span data-stu-id="82724-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82724-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="82724-119">Authorization</span></span>|<span data-ttu-id="82724-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82724-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82724-121">Accept</span><span class="sxs-lookup"><span data-stu-id="82724-121">Accept</span></span>|<span data-ttu-id="82724-122">application/json</span><span class="sxs-lookup"><span data-stu-id="82724-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82724-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82724-123">Request body</span></span>
<span data-ttu-id="82724-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="82724-124">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="82724-125">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="82724-125">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="82724-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82724-126">Property</span></span>|<span data-ttu-id="82724-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="82724-127">Type</span></span>|<span data-ttu-id="82724-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="82724-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82724-129">id</span><span class="sxs-lookup"><span data-stu-id="82724-129">id</span></span>|<span data-ttu-id="82724-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82724-130">String</span></span>|<span data-ttu-id="82724-131">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82724-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="82724-132">displayName</span><span class="sxs-lookup"><span data-stu-id="82724-132">displayName</span></span>|<span data-ttu-id="82724-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82724-133">String</span></span>|<span data-ttu-id="82724-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82724-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="82724-135">description</span><span class="sxs-lookup"><span data-stu-id="82724-135">description</span></span>|<span data-ttu-id="82724-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82724-136">String</span></span>|<span data-ttu-id="82724-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82724-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="82724-138">prioridade</span><span class="sxs-lookup"><span data-stu-id="82724-138">priority</span></span>|<span data-ttu-id="82724-139">Int32</span><span class="sxs-lookup"><span data-stu-id="82724-139">Int32</span></span>|<span data-ttu-id="82724-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82724-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="82724-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82724-141">createdDateTime</span></span>|<span data-ttu-id="82724-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82724-142">DateTimeOffset</span></span>|<span data-ttu-id="82724-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82724-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="82724-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82724-144">lastModifiedDateTime</span></span>|<span data-ttu-id="82724-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82724-145">DateTimeOffset</span></span>|<span data-ttu-id="82724-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82724-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="82724-147">version</span><span class="sxs-lookup"><span data-stu-id="82724-147">version</span></span>|<span data-ttu-id="82724-148">Int32</span><span class="sxs-lookup"><span data-stu-id="82724-148">Int32</span></span>|<span data-ttu-id="82724-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82724-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="82724-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="82724-150">pinMinimumLength</span></span>|<span data-ttu-id="82724-151">Int32</span><span class="sxs-lookup"><span data-stu-id="82724-151">Int32</span></span>|<span data-ttu-id="82724-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82724-152">Not yet documented</span></span>|
|<span data-ttu-id="82724-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="82724-153">pinMaximumLength</span></span>|<span data-ttu-id="82724-154">Int32</span><span class="sxs-lookup"><span data-stu-id="82724-154">Int32</span></span>|<span data-ttu-id="82724-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82724-155">Not yet documented</span></span>|
|<span data-ttu-id="82724-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82724-156">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="82724-157">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="82724-157">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="82724-158">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="82724-158">Not yet documented.</span></span> <span data-ttu-id="82724-159">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="82724-159">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="82724-160">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82724-160">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="82724-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="82724-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="82724-162">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="82724-162">Not yet documented.</span></span> <span data-ttu-id="82724-163">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="82724-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="82724-164">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="82724-164">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="82724-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="82724-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="82724-166">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="82724-166">Not yet documented.</span></span> <span data-ttu-id="82724-167">Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="82724-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="82724-168">state</span><span class="sxs-lookup"><span data-stu-id="82724-168">state</span></span>|[<span data-ttu-id="82724-169">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="82724-169">enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="82724-170">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="82724-170">Not yet documented.</span></span> <span data-ttu-id="82724-171">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="82724-171">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="82724-172">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="82724-172">securityDeviceRequired</span></span>|<span data-ttu-id="82724-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="82724-173">Boolean</span></span>|<span data-ttu-id="82724-174">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82724-174">Not yet documented</span></span>|
|<span data-ttu-id="82724-175">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="82724-175">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="82724-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="82724-176">Boolean</span></span>|<span data-ttu-id="82724-177">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82724-177">Not yet documented</span></span>|
|<span data-ttu-id="82724-178">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="82724-178">remotePassportEnabled</span></span>|<span data-ttu-id="82724-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="82724-179">Boolean</span></span>|<span data-ttu-id="82724-180">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82724-180">Not yet documented</span></span>|
|<span data-ttu-id="82724-181">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="82724-181">pinPreviousBlockCount</span></span>|<span data-ttu-id="82724-182">Int32</span><span class="sxs-lookup"><span data-stu-id="82724-182">Int32</span></span>|<span data-ttu-id="82724-183">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82724-183">Not yet documented</span></span>|
|<span data-ttu-id="82724-184">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="82724-184">pinExpirationInDays</span></span>|<span data-ttu-id="82724-185">Int32</span><span class="sxs-lookup"><span data-stu-id="82724-185">Int32</span></span>|<span data-ttu-id="82724-186">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="82724-186">Not yet documented</span></span>|
|<span data-ttu-id="82724-187">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="82724-187">enhancedBiometricsState</span></span>|[<span data-ttu-id="82724-188">Habilitação de</span><span class="sxs-lookup"><span data-stu-id="82724-188">enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="82724-189">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="82724-189">Not yet documented.</span></span> <span data-ttu-id="82724-190">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="82724-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="82724-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="82724-191">Response</span></span>
<span data-ttu-id="82724-192">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82724-192">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82724-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82724-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="82724-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82724-194">Request</span></span>
<span data-ttu-id="82724-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82724-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82724-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="82724-196">Response</span></span>
<span data-ttu-id="82724-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82724-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



