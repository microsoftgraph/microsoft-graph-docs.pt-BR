# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="69169-101">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="69169-101">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="69169-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="69169-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69169-103">Cria um novo objeto [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="69169-103">Create a new [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69169-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69169-104">Prerequisites</span></span>
<span data-ttu-id="69169-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69169-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="69169-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69169-107">Permission type</span></span>|<span data-ttu-id="69169-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69169-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69169-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69169-109">Delegated (work or school account)</span></span>|<span data-ttu-id="69169-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69169-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69169-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69169-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69169-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69169-112">Not supported.</span></span>|
|<span data-ttu-id="69169-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69169-113">Application</span></span>|<span data-ttu-id="69169-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69169-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69169-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69169-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="69169-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69169-116">Request headers</span></span>
|<span data-ttu-id="69169-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69169-117">Header</span></span>|<span data-ttu-id="69169-118">Valor</span><span class="sxs-lookup"><span data-stu-id="69169-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69169-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="69169-119">Authorization</span></span>|<span data-ttu-id="69169-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69169-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69169-121">Accept</span><span class="sxs-lookup"><span data-stu-id="69169-121">Accept</span></span>|<span data-ttu-id="69169-122">application/json</span><span class="sxs-lookup"><span data-stu-id="69169-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69169-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69169-123">Request body</span></span>
<span data-ttu-id="69169-124">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="69169-124">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="69169-125">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="69169-125">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="69169-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69169-126">Property</span></span>|<span data-ttu-id="69169-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="69169-127">Type</span></span>|<span data-ttu-id="69169-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="69169-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69169-129">id</span><span class="sxs-lookup"><span data-stu-id="69169-129">id</span></span>|<span data-ttu-id="69169-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69169-130">String</span></span>|<span data-ttu-id="69169-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="69169-131">Key of the entity.</span></span> <span data-ttu-id="69169-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69169-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69169-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69169-133">createdDateTime</span></span>|<span data-ttu-id="69169-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69169-134">DateTimeOffset</span></span>|<span data-ttu-id="69169-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="69169-135">DateTime the object was created.</span></span> <span data-ttu-id="69169-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69169-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69169-137">description</span><span class="sxs-lookup"><span data-stu-id="69169-137">description</span></span>|<span data-ttu-id="69169-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69169-138">String</span></span>|<span data-ttu-id="69169-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69169-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="69169-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69169-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69169-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69169-141">lastModifiedDateTime</span></span>|<span data-ttu-id="69169-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69169-142">DateTimeOffset</span></span>|<span data-ttu-id="69169-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="69169-143">DateTime the object was last modified.</span></span> <span data-ttu-id="69169-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69169-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69169-145">displayName</span><span class="sxs-lookup"><span data-stu-id="69169-145">displayName</span></span>|<span data-ttu-id="69169-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69169-146">String</span></span>|<span data-ttu-id="69169-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69169-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="69169-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69169-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69169-149">version</span><span class="sxs-lookup"><span data-stu-id="69169-149">version</span></span>|<span data-ttu-id="69169-150">Int32</span><span class="sxs-lookup"><span data-stu-id="69169-150">Int32</span></span>|<span data-ttu-id="69169-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69169-151">Version of the device configuration.</span></span> <span data-ttu-id="69169-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69169-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69169-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="69169-153">passwordRequired</span></span>|<span data-ttu-id="69169-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-154">Boolean</span></span>|<span data-ttu-id="69169-155">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69169-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="69169-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="69169-156">passwordMinimumLength</span></span>|<span data-ttu-id="69169-157">Int32</span><span class="sxs-lookup"><span data-stu-id="69169-157">Int32</span></span>|<span data-ttu-id="69169-158">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="69169-158">Minimum password length.</span></span> <span data-ttu-id="69169-159">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="69169-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="69169-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="69169-160">passwordRequiredType</span></span>|[<span data-ttu-id="69169-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="69169-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="69169-162">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="69169-162">Type of characters in password.</span></span> <span data-ttu-id="69169-163">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="69169-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="69169-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="69169-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="69169-165">Int32</span><span class="sxs-lookup"><span data-stu-id="69169-165">Int32</span></span>|<span data-ttu-id="69169-166">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="69169-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="69169-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="69169-167">passwordExpirationDays</span></span>|<span data-ttu-id="69169-168">Int32</span><span class="sxs-lookup"><span data-stu-id="69169-168">Int32</span></span>|<span data-ttu-id="69169-169">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="69169-169">Number of days before the password expires.</span></span> <span data-ttu-id="69169-170">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="69169-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="69169-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="69169-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="69169-172">Int32</span><span class="sxs-lookup"><span data-stu-id="69169-172">Int32</span></span>|<span data-ttu-id="69169-173">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="69169-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="69169-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="69169-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="69169-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-175">Boolean</span></span>|<span data-ttu-id="69169-176">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="69169-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="69169-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="69169-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="69169-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-178">Boolean</span></span>|<span data-ttu-id="69169-179">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="69169-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="69169-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="69169-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="69169-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-181">Boolean</span></span>|<span data-ttu-id="69169-182">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="69169-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="69169-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="69169-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="69169-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-184">Boolean</span></span>|<span data-ttu-id="69169-185">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="69169-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="69169-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="69169-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="69169-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="69169-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="69169-188">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="69169-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="69169-189">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="69169-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="69169-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="69169-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="69169-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-191">Boolean</span></span>|<span data-ttu-id="69169-192">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="69169-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="69169-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="69169-193">osMinimumVersion</span></span>|<span data-ttu-id="69169-194">String</span><span class="sxs-lookup"><span data-stu-id="69169-194">String</span></span>|<span data-ttu-id="69169-195">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="69169-195">Minimum Android version.</span></span>|
|<span data-ttu-id="69169-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="69169-196">osMaximumVersion</span></span>|<span data-ttu-id="69169-197">String</span><span class="sxs-lookup"><span data-stu-id="69169-197">String</span></span>|<span data-ttu-id="69169-198">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="69169-198">Maximum Android version.</span></span>|
|<span data-ttu-id="69169-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="69169-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="69169-200">String</span><span class="sxs-lookup"><span data-stu-id="69169-200">String</span></span>|<span data-ttu-id="69169-201">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="69169-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="69169-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="69169-202">storageRequireEncryption</span></span>|<span data-ttu-id="69169-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-203">Boolean</span></span>|<span data-ttu-id="69169-204">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="69169-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="69169-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="69169-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="69169-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-206">Boolean</span></span>|<span data-ttu-id="69169-207">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="69169-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="69169-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="69169-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="69169-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-209">Boolean</span></span>|<span data-ttu-id="69169-210">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="69169-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="69169-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="69169-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="69169-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-212">Boolean</span></span>|<span data-ttu-id="69169-213">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69169-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="69169-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="69169-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="69169-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-215">Boolean</span></span>|<span data-ttu-id="69169-216">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="69169-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="69169-217">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="69169-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="69169-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="69169-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="69169-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="69169-219">Boolean</span></span>|<span data-ttu-id="69169-220">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="69169-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="69169-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="69169-221">Response</span></span>
<span data-ttu-id="69169-222">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69169-222">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69169-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69169-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="69169-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69169-224">Request</span></span>
<span data-ttu-id="69169-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69169-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="69169-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="69169-226">Response</span></span>
<span data-ttu-id="69169-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69169-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



