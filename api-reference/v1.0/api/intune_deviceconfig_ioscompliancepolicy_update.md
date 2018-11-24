# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="9e84a-101">Atualizar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9e84a-101">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="9e84a-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9e84a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e84a-103">Atualiza as propriedades de um objeto [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e84a-103">Update the properties of a [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e84a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e84a-104">Prerequisites</span></span>
<span data-ttu-id="9e84a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9e84a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9e84a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e84a-107">Permission type</span></span>|<span data-ttu-id="9e84a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e84a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e84a-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e84a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9e84a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e84a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e84a-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e84a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e84a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e84a-112">Not supported.</span></span>|
|<span data-ttu-id="9e84a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e84a-113">Application</span></span>|<span data-ttu-id="9e84a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e84a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e84a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e84a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9e84a-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e84a-116">Request headers</span></span>
|<span data-ttu-id="9e84a-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e84a-117">Header</span></span>|<span data-ttu-id="9e84a-118">Valor</span><span class="sxs-lookup"><span data-stu-id="9e84a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e84a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e84a-119">Authorization</span></span>|<span data-ttu-id="9e84a-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e84a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e84a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9e84a-121">Accept</span></span>|<span data-ttu-id="9e84a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9e84a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e84a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e84a-123">Request body</span></span>
<span data-ttu-id="9e84a-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e84a-124">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="9e84a-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e84a-125">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="9e84a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e84a-126">Property</span></span>|<span data-ttu-id="9e84a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e84a-127">Type</span></span>|<span data-ttu-id="9e84a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e84a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e84a-129">id</span><span class="sxs-lookup"><span data-stu-id="9e84a-129">id</span></span>|<span data-ttu-id="9e84a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e84a-130">String</span></span>|<span data-ttu-id="9e84a-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e84a-131">Key of the entity.</span></span> <span data-ttu-id="9e84a-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e84a-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e84a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e84a-133">createdDateTime</span></span>|<span data-ttu-id="9e84a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e84a-134">DateTimeOffset</span></span>|<span data-ttu-id="9e84a-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9e84a-135">DateTime the object was created.</span></span> <span data-ttu-id="9e84a-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e84a-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e84a-137">description</span><span class="sxs-lookup"><span data-stu-id="9e84a-137">description</span></span>|<span data-ttu-id="9e84a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e84a-138">String</span></span>|<span data-ttu-id="9e84a-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e84a-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e84a-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e84a-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e84a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e84a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="9e84a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e84a-142">DateTimeOffset</span></span>|<span data-ttu-id="9e84a-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9e84a-143">DateTime the object was last modified.</span></span> <span data-ttu-id="9e84a-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e84a-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e84a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="9e84a-145">displayName</span></span>|<span data-ttu-id="9e84a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e84a-146">String</span></span>|<span data-ttu-id="9e84a-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e84a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e84a-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e84a-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e84a-149">version</span><span class="sxs-lookup"><span data-stu-id="9e84a-149">version</span></span>|<span data-ttu-id="9e84a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9e84a-150">Int32</span></span>|<span data-ttu-id="9e84a-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e84a-151">Version of the device configuration.</span></span> <span data-ttu-id="9e84a-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e84a-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e84a-153">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9e84a-153">passcodeBlockSimple</span></span>|<span data-ttu-id="9e84a-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e84a-154">Boolean</span></span>|<span data-ttu-id="9e84a-155">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="9e84a-155">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="9e84a-156">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9e84a-156">passcodeExpirationDays</span></span>|<span data-ttu-id="9e84a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9e84a-157">Int32</span></span>|<span data-ttu-id="9e84a-158">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="9e84a-158">Number of days before the passcode expires.</span></span> <span data-ttu-id="9e84a-159">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="9e84a-159">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="9e84a-160">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9e84a-160">passcodeMinimumLength</span></span>|<span data-ttu-id="9e84a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9e84a-161">Int32</span></span>|<span data-ttu-id="9e84a-162">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="9e84a-162">Minimum length of passcode.</span></span> <span data-ttu-id="9e84a-163">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="9e84a-163">Valid values 4 to 14</span></span>|
|<span data-ttu-id="9e84a-164">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9e84a-164">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9e84a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9e84a-165">Int32</span></span>|<span data-ttu-id="9e84a-166">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="9e84a-166">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="9e84a-167">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="9e84a-167">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="9e84a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="9e84a-168">Int32</span></span>|<span data-ttu-id="9e84a-169">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="9e84a-169">Number of previous passcodes to block.</span></span> <span data-ttu-id="9e84a-170">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="9e84a-170">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9e84a-171">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9e84a-171">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="9e84a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="9e84a-172">Int32</span></span>|<span data-ttu-id="9e84a-173">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="9e84a-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9e84a-174">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="9e84a-174">passcodeRequiredType</span></span>|[<span data-ttu-id="9e84a-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9e84a-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="9e84a-176">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="9e84a-176">The required passcode type.</span></span> <span data-ttu-id="9e84a-177">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="9e84a-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9e84a-178">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="9e84a-178">passcodeRequired</span></span>|<span data-ttu-id="9e84a-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e84a-179">Boolean</span></span>|<span data-ttu-id="9e84a-180">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="9e84a-180">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="9e84a-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9e84a-181">osMinimumVersion</span></span>|<span data-ttu-id="9e84a-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e84a-182">String</span></span>|<span data-ttu-id="9e84a-183">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="9e84a-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="9e84a-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9e84a-184">osMaximumVersion</span></span>|<span data-ttu-id="9e84a-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e84a-185">String</span></span>|<span data-ttu-id="9e84a-186">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="9e84a-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="9e84a-187">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="9e84a-187">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="9e84a-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e84a-188">Boolean</span></span>|<span data-ttu-id="9e84a-189">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="9e84a-189">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="9e84a-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9e84a-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9e84a-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e84a-191">Boolean</span></span>|<span data-ttu-id="9e84a-192">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="9e84a-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="9e84a-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9e84a-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9e84a-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9e84a-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="9e84a-195">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="9e84a-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9e84a-196">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="9e84a-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9e84a-197">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="9e84a-197">managedEmailProfileRequired</span></span>|<span data-ttu-id="9e84a-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e84a-198">Boolean</span></span>|<span data-ttu-id="9e84a-199">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="9e84a-199">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="9e84a-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e84a-200">Response</span></span>
<span data-ttu-id="9e84a-201">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e84a-201">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e84a-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e84a-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e84a-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e84a-203">Request</span></span>
<span data-ttu-id="9e84a-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e84a-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="9e84a-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e84a-205">Response</span></span>
<span data-ttu-id="9e84a-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e84a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```



