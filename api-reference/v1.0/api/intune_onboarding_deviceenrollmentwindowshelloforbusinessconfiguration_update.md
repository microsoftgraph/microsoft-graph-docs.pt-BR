# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="edbd4-101">Atualizar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="edbd4-101">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="edbd4-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="edbd4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edbd4-103">Atualize as propriedades de um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edbd4-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edbd4-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="edbd4-104">Prerequisites</span></span>
<span data-ttu-id="edbd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="edbd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="edbd4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edbd4-107">Permission type</span></span>|<span data-ttu-id="edbd4-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="edbd4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edbd4-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edbd4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="edbd4-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbd4-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="edbd4-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edbd4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edbd4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edbd4-112">Not supported.</span></span>|
|<span data-ttu-id="edbd4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="edbd4-113">Application</span></span>|<span data-ttu-id="edbd4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edbd4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edbd4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edbd4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="edbd4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edbd4-116">Request headers</span></span>
|<span data-ttu-id="edbd4-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="edbd4-117">Header</span></span>|<span data-ttu-id="edbd4-118">Valor</span><span class="sxs-lookup"><span data-stu-id="edbd4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edbd4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="edbd4-119">Authorization</span></span>|<span data-ttu-id="edbd4-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edbd4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="edbd4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="edbd4-121">Accept</span></span>|<span data-ttu-id="edbd4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="edbd4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edbd4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edbd4-123">Request body</span></span>
<span data-ttu-id="edbd4-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edbd4-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="edbd4-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edbd4-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="edbd4-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edbd4-126">Property</span></span>|<span data-ttu-id="edbd4-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="edbd4-127">Type</span></span>|<span data-ttu-id="edbd4-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="edbd4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edbd4-129">id</span><span class="sxs-lookup"><span data-stu-id="edbd4-129">id</span></span>|<span data-ttu-id="edbd4-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbd4-130">String</span></span>|<span data-ttu-id="edbd4-131">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edbd4-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edbd4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="edbd4-132">displayName</span></span>|<span data-ttu-id="edbd4-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbd4-133">String</span></span>|<span data-ttu-id="edbd4-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edbd4-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edbd4-135">description</span><span class="sxs-lookup"><span data-stu-id="edbd4-135">description</span></span>|<span data-ttu-id="edbd4-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbd4-136">String</span></span>|<span data-ttu-id="edbd4-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edbd4-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edbd4-138">prioridade</span><span class="sxs-lookup"><span data-stu-id="edbd4-138">priority</span></span>|<span data-ttu-id="edbd4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="edbd4-139">Int32</span></span>|<span data-ttu-id="edbd4-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edbd4-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edbd4-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edbd4-141">createdDateTime</span></span>|<span data-ttu-id="edbd4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edbd4-142">DateTimeOffset</span></span>|<span data-ttu-id="edbd4-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edbd4-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edbd4-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edbd4-144">lastModifiedDateTime</span></span>|<span data-ttu-id="edbd4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edbd4-145">DateTimeOffset</span></span>|<span data-ttu-id="edbd4-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edbd4-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edbd4-147">version</span><span class="sxs-lookup"><span data-stu-id="edbd4-147">version</span></span>|<span data-ttu-id="edbd4-148">Int32</span><span class="sxs-lookup"><span data-stu-id="edbd4-148">Int32</span></span>|<span data-ttu-id="edbd4-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edbd4-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edbd4-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="edbd4-150">pinMinimumLength</span></span>|<span data-ttu-id="edbd4-151">Int32</span><span class="sxs-lookup"><span data-stu-id="edbd4-151">Int32</span></span>|<span data-ttu-id="edbd4-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="edbd4-152">Not yet documented</span></span>|
|<span data-ttu-id="edbd4-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="edbd4-153">pinMaximumLength</span></span>|<span data-ttu-id="edbd4-154">Int32</span><span class="sxs-lookup"><span data-stu-id="edbd4-154">Int32</span></span>|<span data-ttu-id="edbd4-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="edbd4-155">Not yet documented</span></span>|
|<span data-ttu-id="edbd4-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="edbd4-156">pinUppercaseCharactersUsage</span></span>|<span data-ttu-id="edbd4-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbd4-157">String</span></span>|<span data-ttu-id="edbd4-158">Ainda não documentado Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="edbd4-158">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="edbd4-159">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="edbd4-159">pinLowercaseCharactersUsage</span></span>|<span data-ttu-id="edbd4-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbd4-160">String</span></span>|<span data-ttu-id="edbd4-161">Ainda não documentado Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="edbd4-161">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="edbd4-162">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="edbd4-162">pinSpecialCharactersUsage</span></span>|<span data-ttu-id="edbd4-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbd4-163">String</span></span>|<span data-ttu-id="edbd4-164">Ainda não documentado Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="edbd4-164">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="edbd4-165">state</span><span class="sxs-lookup"><span data-stu-id="edbd4-165">state</span></span>|<span data-ttu-id="edbd4-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbd4-166">String</span></span>|<span data-ttu-id="edbd4-167">Ainda não documentado Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="edbd4-167">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="edbd4-168">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="edbd4-168">securityDeviceRequired</span></span>|<span data-ttu-id="edbd4-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="edbd4-169">Boolean</span></span>|<span data-ttu-id="edbd4-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="edbd4-170">Not yet documented</span></span>|
|<span data-ttu-id="edbd4-171">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="edbd4-171">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="edbd4-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="edbd4-172">Boolean</span></span>|<span data-ttu-id="edbd4-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="edbd4-173">Not yet documented</span></span>|
|<span data-ttu-id="edbd4-174">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="edbd4-174">remotePassportEnabled</span></span>|<span data-ttu-id="edbd4-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="edbd4-175">Boolean</span></span>|<span data-ttu-id="edbd4-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="edbd4-176">Not yet documented</span></span>|
|<span data-ttu-id="edbd4-177">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="edbd4-177">pinPreviousBlockCount</span></span>|<span data-ttu-id="edbd4-178">Int32</span><span class="sxs-lookup"><span data-stu-id="edbd4-178">Int32</span></span>|<span data-ttu-id="edbd4-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="edbd4-179">Not yet documented</span></span>|
|<span data-ttu-id="edbd4-180">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="edbd4-180">pinExpirationInDays</span></span>|<span data-ttu-id="edbd4-181">Int32</span><span class="sxs-lookup"><span data-stu-id="edbd4-181">Int32</span></span>|<span data-ttu-id="edbd4-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="edbd4-182">Not yet documented</span></span>|
|<span data-ttu-id="edbd4-183">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="edbd4-183">enhancedBiometricsState</span></span>|<span data-ttu-id="edbd4-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edbd4-184">String</span></span>|<span data-ttu-id="edbd4-185">Ainda não documentado Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="edbd4-185">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="edbd4-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="edbd4-186">Response</span></span>
<span data-ttu-id="edbd4-187">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="edbd4-187">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edbd4-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="edbd4-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="edbd4-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edbd4-189">Request</span></span>
<span data-ttu-id="edbd4-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="edbd4-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 602

{
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

### <a name="response"></a><span data-ttu-id="edbd4-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="edbd4-191">Response</span></span>
<span data-ttu-id="edbd4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edbd4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



