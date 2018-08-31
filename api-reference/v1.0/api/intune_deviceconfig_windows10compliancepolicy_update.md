# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="06bcc-101">Atualizar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="06bcc-101">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="06bcc-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06bcc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06bcc-103">Atualiza as propriedades de um objeto [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06bcc-103">Update the properties of a [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06bcc-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06bcc-104">Prerequisites</span></span>
<span data-ttu-id="06bcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="06bcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06bcc-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06bcc-107">Permission type</span></span>|<span data-ttu-id="06bcc-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06bcc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06bcc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06bcc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="06bcc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06bcc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06bcc-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06bcc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06bcc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06bcc-112">Not supported.</span></span>|
|<span data-ttu-id="06bcc-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06bcc-113">Application</span></span>|<span data-ttu-id="06bcc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06bcc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06bcc-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06bcc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="06bcc-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06bcc-116">Request headers</span></span>
|<span data-ttu-id="06bcc-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06bcc-117">Header</span></span>|<span data-ttu-id="06bcc-118">Valor</span><span class="sxs-lookup"><span data-stu-id="06bcc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06bcc-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="06bcc-119">Authorization</span></span>|<span data-ttu-id="06bcc-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="06bcc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06bcc-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06bcc-121">Accept</span></span>|<span data-ttu-id="06bcc-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="06bcc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06bcc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06bcc-123">Request body</span></span>
<span data-ttu-id="06bcc-124">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06bcc-124">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="06bcc-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06bcc-125">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="06bcc-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06bcc-126">Property</span></span>|<span data-ttu-id="06bcc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="06bcc-127">Type</span></span>|<span data-ttu-id="06bcc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="06bcc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06bcc-129">id</span><span class="sxs-lookup"><span data-stu-id="06bcc-129">id</span></span>|<span data-ttu-id="06bcc-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06bcc-130">String</span></span>|<span data-ttu-id="06bcc-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06bcc-131">Key of the entity.</span></span> <span data-ttu-id="06bcc-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06bcc-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06bcc-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06bcc-133">createdDateTime</span></span>|<span data-ttu-id="06bcc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06bcc-134">DateTimeOffset</span></span>|<span data-ttu-id="06bcc-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="06bcc-135">DateTime the object was created.</span></span> <span data-ttu-id="06bcc-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06bcc-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06bcc-137">description</span><span class="sxs-lookup"><span data-stu-id="06bcc-137">description</span></span>|<span data-ttu-id="06bcc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06bcc-138">String</span></span>|<span data-ttu-id="06bcc-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06bcc-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06bcc-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06bcc-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06bcc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06bcc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="06bcc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06bcc-142">DateTimeOffset</span></span>|<span data-ttu-id="06bcc-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="06bcc-143">DateTime the object was last modified.</span></span> <span data-ttu-id="06bcc-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06bcc-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06bcc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="06bcc-145">displayName</span></span>|<span data-ttu-id="06bcc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06bcc-146">String</span></span>|<span data-ttu-id="06bcc-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06bcc-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06bcc-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06bcc-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06bcc-149">version</span><span class="sxs-lookup"><span data-stu-id="06bcc-149">version</span></span>|<span data-ttu-id="06bcc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="06bcc-150">Int32</span></span>|<span data-ttu-id="06bcc-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06bcc-151">Version of the device configuration.</span></span> <span data-ttu-id="06bcc-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06bcc-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06bcc-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="06bcc-153">passwordRequired</span></span>|<span data-ttu-id="06bcc-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="06bcc-154">Boolean</span></span>|<span data-ttu-id="06bcc-155">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="06bcc-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="06bcc-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="06bcc-156">passwordBlockSimple</span></span>|<span data-ttu-id="06bcc-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="06bcc-157">Boolean</span></span>|<span data-ttu-id="06bcc-158">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="06bcc-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="06bcc-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="06bcc-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="06bcc-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="06bcc-160">Boolean</span></span>|<span data-ttu-id="06bcc-161">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="06bcc-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="06bcc-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="06bcc-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="06bcc-163">Int32</span><span class="sxs-lookup"><span data-stu-id="06bcc-163">Int32</span></span>|<span data-ttu-id="06bcc-164">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="06bcc-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="06bcc-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="06bcc-165">passwordExpirationDays</span></span>|<span data-ttu-id="06bcc-166">Int32</span><span class="sxs-lookup"><span data-stu-id="06bcc-166">Int32</span></span>|<span data-ttu-id="06bcc-167">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="06bcc-167">The password expiration in days.</span></span>|
|<span data-ttu-id="06bcc-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="06bcc-168">passwordMinimumLength</span></span>|<span data-ttu-id="06bcc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="06bcc-169">Int32</span></span>|<span data-ttu-id="06bcc-170">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="06bcc-170">The minimum password length.</span></span>|
|<span data-ttu-id="06bcc-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="06bcc-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="06bcc-172">Int32</span><span class="sxs-lookup"><span data-stu-id="06bcc-172">Int32</span></span>|<span data-ttu-id="06bcc-173">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="06bcc-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="06bcc-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="06bcc-174">passwordRequiredType</span></span>|[<span data-ttu-id="06bcc-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="06bcc-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="06bcc-176">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="06bcc-176">The required password type.</span></span> <span data-ttu-id="06bcc-177">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="06bcc-177">The possible values are:</span></span>|
|<span data-ttu-id="06bcc-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="06bcc-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="06bcc-179">Int32</span><span class="sxs-lookup"><span data-stu-id="06bcc-179">Int32</span></span>|<span data-ttu-id="06bcc-180">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="06bcc-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="06bcc-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="06bcc-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="06bcc-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="06bcc-182">Boolean</span></span>|<span data-ttu-id="06bcc-183">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="06bcc-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="06bcc-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="06bcc-184">osMinimumVersion</span></span>|<span data-ttu-id="06bcc-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06bcc-185">String</span></span>|<span data-ttu-id="06bcc-186">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="06bcc-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="06bcc-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="06bcc-187">osMaximumVersion</span></span>|<span data-ttu-id="06bcc-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06bcc-188">String</span></span>|<span data-ttu-id="06bcc-189">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="06bcc-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="06bcc-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="06bcc-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="06bcc-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06bcc-191">String</span></span>|<span data-ttu-id="06bcc-192">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="06bcc-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="06bcc-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="06bcc-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="06bcc-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06bcc-194">String</span></span>|<span data-ttu-id="06bcc-195">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="06bcc-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="06bcc-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="06bcc-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="06bcc-197">Booleano</span><span class="sxs-lookup"><span data-stu-id="06bcc-197">Boolean</span></span>|<span data-ttu-id="06bcc-198">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="06bcc-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="06bcc-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="06bcc-199">bitLockerEnabled</span></span>|<span data-ttu-id="06bcc-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="06bcc-200">Boolean</span></span>|<span data-ttu-id="06bcc-201">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="06bcc-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="06bcc-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="06bcc-202">secureBootEnabled</span></span>|<span data-ttu-id="06bcc-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="06bcc-203">Boolean</span></span>|<span data-ttu-id="06bcc-204">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="06bcc-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="06bcc-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="06bcc-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="06bcc-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="06bcc-206">Boolean</span></span>|<span data-ttu-id="06bcc-207">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="06bcc-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="06bcc-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="06bcc-208">storageRequireEncryption</span></span>|<span data-ttu-id="06bcc-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="06bcc-209">Boolean</span></span>|<span data-ttu-id="06bcc-210">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="06bcc-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="06bcc-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="06bcc-211">Response</span></span>
<span data-ttu-id="06bcc-212">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06bcc-212">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06bcc-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06bcc-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="06bcc-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06bcc-214">Request</span></span>
<span data-ttu-id="06bcc-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06bcc-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="06bcc-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="06bcc-216">Response</span></span>
<span data-ttu-id="06bcc-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06bcc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



