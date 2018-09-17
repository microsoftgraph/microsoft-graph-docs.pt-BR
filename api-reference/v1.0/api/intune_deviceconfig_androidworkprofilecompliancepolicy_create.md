# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="69abc-101">Criar androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="69abc-101">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="69abc-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="69abc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69abc-103">Criar um novo objeto [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="69abc-103">Create a new [editionUpgradeConfiguration](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69abc-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69abc-104">Prerequisites</span></span>
<span data-ttu-id="69abc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="69abc-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69abc-107">Permission type</span></span>|<span data-ttu-id="69abc-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69abc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69abc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69abc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="69abc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69abc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69abc-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69abc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69abc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69abc-112">Not supported.</span></span>|
|<span data-ttu-id="69abc-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69abc-113">Application</span></span>|<span data-ttu-id="69abc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69abc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69abc-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69abc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="69abc-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69abc-116">Request headers</span></span>
|<span data-ttu-id="69abc-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69abc-117">Header</span></span>|<span data-ttu-id="69abc-118">Valor</span><span class="sxs-lookup"><span data-stu-id="69abc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69abc-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="69abc-119">Authorization</span></span>|<span data-ttu-id="69abc-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="69abc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69abc-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69abc-121">Accept</span></span>|<span data-ttu-id="69abc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="69abc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69abc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69abc-123">Request body</span></span>
<span data-ttu-id="69abc-124">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="69abc-124">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="69abc-125">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="69abc-125">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="69abc-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69abc-126">Property</span></span>|<span data-ttu-id="69abc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="69abc-127">Type</span></span>|<span data-ttu-id="69abc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="69abc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69abc-129">id</span><span class="sxs-lookup"><span data-stu-id="69abc-129">id</span></span>|<span data-ttu-id="69abc-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abc-130">String</span></span>|<span data-ttu-id="69abc-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="69abc-131">Key of the entity.</span></span> <span data-ttu-id="69abc-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69abc-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69abc-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69abc-133">createdDateTime</span></span>|<span data-ttu-id="69abc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69abc-134">DateTimeOffset</span></span>|<span data-ttu-id="69abc-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="69abc-135">DateTime the object was created.</span></span> <span data-ttu-id="69abc-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69abc-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69abc-137">descrição</span><span class="sxs-lookup"><span data-stu-id="69abc-137">description</span></span>|<span data-ttu-id="69abc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abc-138">String</span></span>|<span data-ttu-id="69abc-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69abc-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="69abc-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69abc-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69abc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69abc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="69abc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69abc-142">DateTimeOffset</span></span>|<span data-ttu-id="69abc-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="69abc-143">DateTime the object was last modified.</span></span> <span data-ttu-id="69abc-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69abc-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69abc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="69abc-145">displayName</span></span>|<span data-ttu-id="69abc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abc-146">String</span></span>|<span data-ttu-id="69abc-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69abc-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="69abc-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69abc-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69abc-149">versão</span><span class="sxs-lookup"><span data-stu-id="69abc-149">version</span></span>|<span data-ttu-id="69abc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="69abc-150">Int32</span></span>|<span data-ttu-id="69abc-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69abc-151">Version of the device configuration.</span></span> <span data-ttu-id="69abc-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="69abc-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="69abc-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="69abc-153">passwordRequired</span></span>|<span data-ttu-id="69abc-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-154">Boolean</span></span>|<span data-ttu-id="69abc-155">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69abc-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="69abc-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="69abc-156">passwordMinimumLength</span></span>|<span data-ttu-id="69abc-157">Int32</span><span class="sxs-lookup"><span data-stu-id="69abc-157">Int32</span></span>|<span data-ttu-id="69abc-158">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="69abc-158">Minimum password length.</span></span> <span data-ttu-id="69abc-159">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="69abc-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="69abc-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="69abc-160">passwordRequiredType</span></span>|[<span data-ttu-id="69abc-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="69abc-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="69abc-162">Tipo de caracteres da senha.</span><span class="sxs-lookup"><span data-stu-id="69abc-162">Type of characters in password Possible values are: , , , , , , , .</span></span> <span data-ttu-id="69abc-163">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="69abc-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="69abc-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="69abc-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="69abc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="69abc-165">Int32</span></span>|<span data-ttu-id="69abc-166">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="69abc-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="69abc-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="69abc-167">passwordExpirationDays</span></span>|<span data-ttu-id="69abc-168">Int32</span><span class="sxs-lookup"><span data-stu-id="69abc-168">Int32</span></span>|<span data-ttu-id="69abc-169">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="69abc-169">Number of days before the password expires.</span></span> <span data-ttu-id="69abc-170">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="69abc-170">Valid values 1 to 365</span></span>|
|<span data-ttu-id="69abc-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="69abc-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="69abc-172">Int32</span><span class="sxs-lookup"><span data-stu-id="69abc-172">Int32</span></span>|<span data-ttu-id="69abc-173">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="69abc-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="69abc-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="69abc-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="69abc-175">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-175">Boolean</span></span>|<span data-ttu-id="69abc-176">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="69abc-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="69abc-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="69abc-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="69abc-178">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-178">Boolean</span></span>|<span data-ttu-id="69abc-179">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="69abc-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="69abc-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="69abc-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="69abc-181">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-181">Boolean</span></span>|<span data-ttu-id="69abc-182">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="69abc-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="69abc-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="69abc-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="69abc-184">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-184">Boolean</span></span>|<span data-ttu-id="69abc-185">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="69abc-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="69abc-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="69abc-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="69abc-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="69abc-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="69abc-188">Exige o nível mínimo de risco de Proteção contra ameaças móveis para relatar a não conformidade.</span><span class="sxs-lookup"><span data-stu-id="69abc-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="69abc-189">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="69abc-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="69abc-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="69abc-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="69abc-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-191">Boolean</span></span>|<span data-ttu-id="69abc-192">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="69abc-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="69abc-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="69abc-193">osMinimumVersion</span></span>|<span data-ttu-id="69abc-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abc-194">String</span></span>|<span data-ttu-id="69abc-195">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="69abc-195">Minimum Android version.</span></span>|
|<span data-ttu-id="69abc-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="69abc-196">osMaximumVersion</span></span>|<span data-ttu-id="69abc-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abc-197">String</span></span>|<span data-ttu-id="69abc-198">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="69abc-198">Maximum Android version.</span></span>|
|<span data-ttu-id="69abc-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="69abc-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="69abc-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abc-200">String</span></span>|<span data-ttu-id="69abc-201">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="69abc-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="69abc-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="69abc-202">storageRequireEncryption</span></span>|<span data-ttu-id="69abc-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-203">Boolean</span></span>|<span data-ttu-id="69abc-204">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="69abc-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="69abc-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="69abc-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="69abc-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-206">Boolean</span></span>|<span data-ttu-id="69abc-207">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="69abc-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="69abc-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="69abc-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="69abc-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-209">Boolean</span></span>|<span data-ttu-id="69abc-210">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="69abc-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="69abc-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="69abc-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="69abc-212">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-212">Boolean</span></span>|<span data-ttu-id="69abc-213">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69abc-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="69abc-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="69abc-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="69abc-215">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-215">Boolean</span></span>|<span data-ttu-id="69abc-216">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="69abc-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="69abc-217">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="69abc-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="69abc-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="69abc-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="69abc-219">Booleano</span><span class="sxs-lookup"><span data-stu-id="69abc-219">Boolean</span></span>|<span data-ttu-id="69abc-220">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="69abc-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="69abc-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="69abc-221">Response</span></span>
<span data-ttu-id="69abc-222">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69abc-222">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69abc-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69abc-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="69abc-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69abc-224">Request</span></span>
<span data-ttu-id="69abc-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69abc-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1234

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="69abc-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="69abc-226">Response</span></span>
<span data-ttu-id="69abc-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69abc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "4e385271-5271-4e38-7152-384e7152384e",
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








