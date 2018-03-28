# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="b6b69-101">Criar deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6b69-101">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="b6b69-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b6b69-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6b69-103">Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b6b69-103">Create a new [plannerBucket](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6b69-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6b69-104">Prerequisites</span></span>
<span data-ttu-id="b6b69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b6b69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b6b69-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6b69-107">Permission type</span></span>|<span data-ttu-id="b6b69-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6b69-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6b69-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6b69-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b6b69-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6b69-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6b69-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6b69-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6b69-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6b69-112">Not supported.</span></span>|
|<span data-ttu-id="b6b69-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6b69-113">Application</span></span>|<span data-ttu-id="b6b69-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6b69-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6b69-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6b69-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b6b69-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b69-116">Request headers</span></span>
|<span data-ttu-id="b6b69-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6b69-117">Header</span></span>|<span data-ttu-id="b6b69-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b6b69-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6b69-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6b69-119">Authorization</span></span>|<span data-ttu-id="b6b69-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6b69-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b6b69-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b6b69-121">Accept</span></span>|<span data-ttu-id="b6b69-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b6b69-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6b69-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b69-123">Request body</span></span>
<span data-ttu-id="b6b69-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b6b69-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b6b69-125">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b6b69-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="b6b69-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6b69-126">Property</span></span>|<span data-ttu-id="b6b69-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6b69-127">Type</span></span>|<span data-ttu-id="b6b69-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6b69-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6b69-129">id</span><span class="sxs-lookup"><span data-stu-id="b6b69-129">id</span></span>|<span data-ttu-id="b6b69-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b69-130">String</span></span>|<span data-ttu-id="b6b69-131">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6b69-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b6b69-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b6b69-132">displayName</span></span>|<span data-ttu-id="b6b69-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b69-133">String</span></span>|<span data-ttu-id="b6b69-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6b69-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b6b69-135">description</span><span class="sxs-lookup"><span data-stu-id="b6b69-135">description</span></span>|<span data-ttu-id="b6b69-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b69-136">String</span></span>|<span data-ttu-id="b6b69-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6b69-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b6b69-138">prioridade</span><span class="sxs-lookup"><span data-stu-id="b6b69-138">priority</span></span>|<span data-ttu-id="b6b69-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b69-139">Int32</span></span>|<span data-ttu-id="b6b69-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6b69-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b6b69-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6b69-141">createdDateTime</span></span>|<span data-ttu-id="b6b69-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6b69-142">DateTimeOffset</span></span>|<span data-ttu-id="b6b69-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6b69-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b6b69-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6b69-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b6b69-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6b69-145">DateTimeOffset</span></span>|<span data-ttu-id="b6b69-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6b69-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b6b69-147">version</span><span class="sxs-lookup"><span data-stu-id="b6b69-147">version</span></span>|<span data-ttu-id="b6b69-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b69-148">Int32</span></span>|<span data-ttu-id="b6b69-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6b69-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b6b69-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b6b69-150">pinMinimumLength</span></span>|<span data-ttu-id="b6b69-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b69-151">Int32</span></span>|<span data-ttu-id="b6b69-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6b69-152">Not yet documented</span></span>|
|<span data-ttu-id="b6b69-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="b6b69-153">pinMaximumLength</span></span>|<span data-ttu-id="b6b69-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b69-154">Int32</span></span>|<span data-ttu-id="b6b69-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6b69-155">Not yet documented</span></span>|
|<span data-ttu-id="b6b69-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b6b69-156">pinUppercaseCharactersUsage</span></span>|<span data-ttu-id="b6b69-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b69-157">String</span></span>|<span data-ttu-id="b6b69-158">Ainda não documentado Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="b6b69-158">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b6b69-159">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b6b69-159">pinLowercaseCharactersUsage</span></span>|<span data-ttu-id="b6b69-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b69-160">String</span></span>|<span data-ttu-id="b6b69-161">Ainda não documentado Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="b6b69-161">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b6b69-162">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="b6b69-162">pinSpecialCharactersUsage</span></span>|<span data-ttu-id="b6b69-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b69-163">String</span></span>|<span data-ttu-id="b6b69-164">Ainda não documentado Os valores possíveis são: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="b6b69-164">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="b6b69-165">state</span><span class="sxs-lookup"><span data-stu-id="b6b69-165">state</span></span>|<span data-ttu-id="b6b69-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b69-166">String</span></span>|<span data-ttu-id="b6b69-167">Ainda não documentado Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b6b69-167">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b6b69-168">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="b6b69-168">securityDeviceRequired</span></span>|<span data-ttu-id="b6b69-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6b69-169">Boolean</span></span>|<span data-ttu-id="b6b69-170">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6b69-170">Not yet documented</span></span>|
|<span data-ttu-id="b6b69-171">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="b6b69-171">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="b6b69-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6b69-172">Boolean</span></span>|<span data-ttu-id="b6b69-173">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6b69-173">Not yet documented</span></span>|
|<span data-ttu-id="b6b69-174">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="b6b69-174">remotePassportEnabled</span></span>|<span data-ttu-id="b6b69-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6b69-175">Boolean</span></span>|<span data-ttu-id="b6b69-176">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6b69-176">Not yet documented</span></span>|
|<span data-ttu-id="b6b69-177">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="b6b69-177">pinPreviousBlockCount</span></span>|<span data-ttu-id="b6b69-178">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b69-178">Int32</span></span>|<span data-ttu-id="b6b69-179">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6b69-179">Not yet documented</span></span>|
|<span data-ttu-id="b6b69-180">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="b6b69-180">pinExpirationInDays</span></span>|<span data-ttu-id="b6b69-181">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b69-181">Int32</span></span>|<span data-ttu-id="b6b69-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6b69-182">Not yet documented</span></span>|
|<span data-ttu-id="b6b69-183">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="b6b69-183">enhancedBiometricsState</span></span>|<span data-ttu-id="b6b69-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b69-184">String</span></span>|<span data-ttu-id="b6b69-185">Ainda não documentado Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b6b69-185">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="b6b69-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6b69-186">Response</span></span>
<span data-ttu-id="b6b69-187">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6b69-187">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6b69-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6b69-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6b69-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b69-189">Request</span></span>
<span data-ttu-id="b6b69-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6b69-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="b6b69-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6b69-191">Response</span></span>
<span data-ttu-id="b6b69-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6b69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



