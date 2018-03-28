# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="23eae-101">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="23eae-101">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="23eae-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="23eae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23eae-103">Cria um novo objeto [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="23eae-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23eae-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23eae-104">Prerequisites</span></span>
<span data-ttu-id="23eae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="23eae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23eae-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23eae-107">Permission type</span></span>|<span data-ttu-id="23eae-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23eae-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23eae-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23eae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="23eae-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23eae-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23eae-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23eae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23eae-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23eae-112">Not supported.</span></span>|
|<span data-ttu-id="23eae-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23eae-113">Application</span></span>|<span data-ttu-id="23eae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23eae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23eae-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23eae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="23eae-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23eae-116">Request headers</span></span>
|<span data-ttu-id="23eae-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23eae-117">Header</span></span>|<span data-ttu-id="23eae-118">Valor</span><span class="sxs-lookup"><span data-stu-id="23eae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23eae-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="23eae-119">Authorization</span></span>|<span data-ttu-id="23eae-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23eae-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="23eae-121">Accept</span><span class="sxs-lookup"><span data-stu-id="23eae-121">Accept</span></span>|<span data-ttu-id="23eae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="23eae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23eae-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23eae-123">Request body</span></span>
<span data-ttu-id="23eae-124">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="23eae-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="23eae-125">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="23eae-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="23eae-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23eae-126">Property</span></span>|<span data-ttu-id="23eae-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="23eae-127">Type</span></span>|<span data-ttu-id="23eae-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="23eae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23eae-129">id</span><span class="sxs-lookup"><span data-stu-id="23eae-129">id</span></span>|<span data-ttu-id="23eae-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23eae-130">String</span></span>|<span data-ttu-id="23eae-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="23eae-131">Key of the setting.</span></span> <span data-ttu-id="23eae-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23eae-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23eae-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23eae-133">createdDateTime</span></span>|<span data-ttu-id="23eae-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23eae-134">DateTimeOffset</span></span>|<span data-ttu-id="23eae-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="23eae-135">DateTime the object was created.</span></span> <span data-ttu-id="23eae-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23eae-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23eae-137">description</span><span class="sxs-lookup"><span data-stu-id="23eae-137">description</span></span>|<span data-ttu-id="23eae-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23eae-138">String</span></span>|<span data-ttu-id="23eae-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23eae-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23eae-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23eae-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23eae-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23eae-141">lastModifiedDateTime</span></span>|<span data-ttu-id="23eae-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23eae-142">DateTimeOffset</span></span>|<span data-ttu-id="23eae-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="23eae-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="23eae-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23eae-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23eae-145">displayName</span><span class="sxs-lookup"><span data-stu-id="23eae-145">displayName</span></span>|<span data-ttu-id="23eae-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23eae-146">String</span></span>|<span data-ttu-id="23eae-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23eae-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23eae-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23eae-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23eae-149">version</span><span class="sxs-lookup"><span data-stu-id="23eae-149">version</span></span>|<span data-ttu-id="23eae-150">Int32</span><span class="sxs-lookup"><span data-stu-id="23eae-150">Int32</span></span>|<span data-ttu-id="23eae-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23eae-151">Version of the device configuration.</span></span> <span data-ttu-id="23eae-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23eae-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23eae-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="23eae-153">passwordRequired</span></span>|<span data-ttu-id="23eae-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-154">Boolean</span></span>|<span data-ttu-id="23eae-155">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23eae-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="23eae-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="23eae-156">passwordMinimumLength</span></span>|<span data-ttu-id="23eae-157">Int32</span><span class="sxs-lookup"><span data-stu-id="23eae-157">Int32</span></span>|<span data-ttu-id="23eae-158">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="23eae-158">Minimum password length.</span></span> <span data-ttu-id="23eae-159">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="23eae-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="23eae-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="23eae-160">passwordRequiredType</span></span>|<span data-ttu-id="23eae-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23eae-161">String</span></span>|<span data-ttu-id="23eae-162">Tipo de caracteres na senha Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="23eae-162">Type of characters in password Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="23eae-163">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="23eae-163">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="23eae-164">Int32</span><span class="sxs-lookup"><span data-stu-id="23eae-164">Int32</span></span>|<span data-ttu-id="23eae-165">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="23eae-165">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="23eae-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="23eae-166">passwordExpirationDays</span></span>|<span data-ttu-id="23eae-167">Int32</span><span class="sxs-lookup"><span data-stu-id="23eae-167">Int32</span></span>|<span data-ttu-id="23eae-168">Número de dias antes que a senha expire.</span><span class="sxs-lookup"><span data-stu-id="23eae-168">Number of days before the password expires.</span></span> <span data-ttu-id="23eae-169">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="23eae-169">Valid values 1 to 365</span></span>|
|<span data-ttu-id="23eae-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="23eae-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="23eae-171">Int32</span><span class="sxs-lookup"><span data-stu-id="23eae-171">Int32</span></span>|<span data-ttu-id="23eae-172">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="23eae-172">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="23eae-173">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="23eae-173">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="23eae-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-174">Boolean</span></span>|<span data-ttu-id="23eae-175">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="23eae-175">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="23eae-176">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="23eae-176">securityDisableUsbDebugging</span></span>|<span data-ttu-id="23eae-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-177">Boolean</span></span>|<span data-ttu-id="23eae-178">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="23eae-178">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="23eae-179">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="23eae-179">securityRequireVerifyApps</span></span>|<span data-ttu-id="23eae-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-180">Boolean</span></span>|<span data-ttu-id="23eae-181">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="23eae-181">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="23eae-182">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="23eae-182">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="23eae-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-183">Boolean</span></span>|<span data-ttu-id="23eae-184">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="23eae-184">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="23eae-185">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="23eae-185">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="23eae-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23eae-186">String</span></span>|<span data-ttu-id="23eae-187">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="23eae-187">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="23eae-188">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="23eae-188">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="23eae-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="23eae-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="23eae-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-190">Boolean</span></span>|<span data-ttu-id="23eae-191">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="23eae-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="23eae-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="23eae-192">osMinimumVersion</span></span>|<span data-ttu-id="23eae-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23eae-193">String</span></span>|<span data-ttu-id="23eae-194">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="23eae-194">Minimum Android version.</span></span>|
|<span data-ttu-id="23eae-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="23eae-195">osMaximumVersion</span></span>|<span data-ttu-id="23eae-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23eae-196">String</span></span>|<span data-ttu-id="23eae-197">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="23eae-197">Maximum Android version.</span></span>|
|<span data-ttu-id="23eae-198">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="23eae-198">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="23eae-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23eae-199">String</span></span>|<span data-ttu-id="23eae-200">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="23eae-200">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="23eae-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="23eae-201">storageRequireEncryption</span></span>|<span data-ttu-id="23eae-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-202">Boolean</span></span>|<span data-ttu-id="23eae-203">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="23eae-203">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="23eae-204">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="23eae-204">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="23eae-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-205">Boolean</span></span>|<span data-ttu-id="23eae-206">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="23eae-206">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="23eae-207">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="23eae-207">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="23eae-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-208">Boolean</span></span>|<span data-ttu-id="23eae-209">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="23eae-209">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="23eae-210">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="23eae-210">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="23eae-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-211">Boolean</span></span>|<span data-ttu-id="23eae-212">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23eae-212">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="23eae-213">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="23eae-213">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="23eae-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-214">Boolean</span></span>|<span data-ttu-id="23eae-215">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="23eae-215">Require the device to have up to date security providers.</span></span> <span data-ttu-id="23eae-216">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="23eae-216">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="23eae-217">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="23eae-217">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="23eae-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="23eae-218">Boolean</span></span>|<span data-ttu-id="23eae-219">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="23eae-219">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="23eae-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="23eae-220">Response</span></span>
<span data-ttu-id="23eae-221">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23eae-221">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23eae-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23eae-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="23eae-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23eae-223">Request</span></span>
<span data-ttu-id="23eae-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23eae-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="23eae-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="23eae-225">Response</span></span>
<span data-ttu-id="23eae-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23eae-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```



