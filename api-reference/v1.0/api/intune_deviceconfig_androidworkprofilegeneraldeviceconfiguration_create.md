# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="a196c-101">Create androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a196c-101">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a196c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a196c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a196c-103">Cria um novo objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a196c-103">Create a new [deviceConfigurationAssignment](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a196c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a196c-104">Prerequisites</span></span>
<span data-ttu-id="a196c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a196c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a196c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a196c-107">Permission type</span></span>|<span data-ttu-id="a196c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a196c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a196c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a196c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a196c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a196c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a196c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a196c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a196c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a196c-112">Not supported.</span></span>|
|<span data-ttu-id="a196c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a196c-113">Application</span></span>|<span data-ttu-id="a196c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a196c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a196c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a196c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a196c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a196c-116">Request headers</span></span>
|<span data-ttu-id="a196c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a196c-117">Header</span></span>|<span data-ttu-id="a196c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="a196c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a196c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="a196c-119">Authorization</span></span>|<span data-ttu-id="a196c-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="a196c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a196c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a196c-121">Accept</span></span>|<span data-ttu-id="a196c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a196c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a196c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a196c-123">Request body</span></span>
<span data-ttu-id="a196c-124">No corpo da solicitação, fornece uma representação JSON do objeto androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a196c-124">In the request body, supply a JSON representation for the deviceManagement object.</span></span>

<span data-ttu-id="a196c-125">A tabela a seguir mostra as propriedades necessárias ao criar androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a196c-125">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="a196c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a196c-126">Property</span></span>|<span data-ttu-id="a196c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a196c-127">Type</span></span>|<span data-ttu-id="a196c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a196c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a196c-129">id</span><span class="sxs-lookup"><span data-stu-id="a196c-129">id</span></span>|<span data-ttu-id="a196c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a196c-130">String</span></span>|<span data-ttu-id="a196c-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a196c-131">Key of the entity.</span></span> <span data-ttu-id="a196c-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a196c-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a196c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a196c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a196c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a196c-134">DateTimeOffset</span></span>|<span data-ttu-id="a196c-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a196c-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a196c-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a196c-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a196c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a196c-137">createdDateTime</span></span>|<span data-ttu-id="a196c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a196c-138">DateTimeOffset</span></span>|<span data-ttu-id="a196c-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a196c-139">DateTime the object was created.</span></span> <span data-ttu-id="a196c-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a196c-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a196c-141">descrição</span><span class="sxs-lookup"><span data-stu-id="a196c-141">description</span></span>|<span data-ttu-id="a196c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a196c-142">String</span></span>|<span data-ttu-id="a196c-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a196c-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a196c-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a196c-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a196c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a196c-145">displayName</span></span>|<span data-ttu-id="a196c-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a196c-146">String</span></span>|<span data-ttu-id="a196c-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a196c-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a196c-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a196c-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a196c-149">version</span><span class="sxs-lookup"><span data-stu-id="a196c-149">version</span></span>|<span data-ttu-id="a196c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-150">Int32</span></span>|<span data-ttu-id="a196c-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a196c-151">Version of the device configuration.</span></span> <span data-ttu-id="a196c-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a196c-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a196c-153">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a196c-153">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a196c-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-154">Boolean</span></span>|<span data-ttu-id="a196c-155">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="a196c-155">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a196c-156">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a196c-156">passwordBlockTrustAgents</span></span>|<span data-ttu-id="a196c-157">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-157">Boolean</span></span>|<span data-ttu-id="a196c-158">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="a196c-158">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="a196c-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a196c-159">passwordExpirationDays</span></span>|<span data-ttu-id="a196c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-160">Int32</span></span>|<span data-ttu-id="a196c-161">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="a196c-161">Number of days before the password expires.</span></span> <span data-ttu-id="a196c-162">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="a196c-162">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a196c-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a196c-163">passwordMinimumLength</span></span>|<span data-ttu-id="a196c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-164">Int32</span></span>|<span data-ttu-id="a196c-165">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="a196c-165">Minimum length of passwords.</span></span> <span data-ttu-id="a196c-166">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="a196c-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a196c-167">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a196c-167">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a196c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-168">Int32</span></span>|<span data-ttu-id="a196c-169">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="a196c-169">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a196c-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a196c-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a196c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-171">Int32</span></span>|<span data-ttu-id="a196c-172">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="a196c-172">Number of previous passwords to block.</span></span> <span data-ttu-id="a196c-173">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="a196c-173">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a196c-174">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a196c-174">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a196c-175">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-175">Int32</span></span>|<span data-ttu-id="a196c-176">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="a196c-176">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="a196c-177">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="a196c-177">Valid values 4 to 11</span></span>|
|<span data-ttu-id="a196c-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a196c-178">passwordRequiredType</span></span>|[<span data-ttu-id="a196c-179">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a196c-179">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="a196c-180">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="a196c-180">Type of password that is required.</span></span> <span data-ttu-id="a196c-181">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a196c-181">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a196c-182">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="a196c-182">workProfileDataSharingType</span></span>|[<span data-ttu-id="a196c-183">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="a196c-183">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="a196c-184">Tipo de dados de compartilhamento permitido.</span><span class="sxs-lookup"><span data-stu-id="a196c-184">Type of data sharing that is allowed.</span></span> <span data-ttu-id="a196c-185">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="a196c-185">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="a196c-186">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="a196c-186">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="a196c-187">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-187">Boolean</span></span>|<span data-ttu-id="a196c-188">Indica se deve ou não bloquear notificações enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="a196c-188">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="a196c-189">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="a196c-189">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="a196c-190">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-190">Boolean</span></span>|<span data-ttu-id="a196c-191">Impede que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-191">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="a196c-192">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="a196c-192">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="a196c-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-193">Boolean</span></span>|<span data-ttu-id="a196c-194">Permite que dispositivos bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="a196c-194">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="a196c-195">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="a196c-195">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="a196c-196">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-196">Boolean</span></span>|<span data-ttu-id="a196c-197">Bloqueia capturas de tela no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-197">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="a196c-198">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="a196c-198">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="a196c-199">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-199">Boolean</span></span>|<span data-ttu-id="a196c-200">Bloqueia a exibição de identificação de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="a196c-200">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="a196c-201">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="a196c-201">workProfileBlockCamera</span></span>|<span data-ttu-id="a196c-202">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-202">Boolean</span></span>|<span data-ttu-id="a196c-203">Bloqueia a câmera no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-203">Block work profile camera.</span></span>|
|<span data-ttu-id="a196c-204">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="a196c-204">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="a196c-205">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-205">Boolean</span></span>|<span data-ttu-id="a196c-206">Bloqueia a disponibilidade de contatos do perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="a196c-206">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="a196c-207">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="a196c-207">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="a196c-208">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-208">Boolean</span></span>|<span data-ttu-id="a196c-209">Booleano que indica se a configuração para impedir copiar/colar entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="a196c-209">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="a196c-210">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="a196c-210">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="a196c-211">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a196c-211">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="a196c-212">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="a196c-212">Type of password that is required.</span></span> <span data-ttu-id="a196c-213">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="a196c-213">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="a196c-214">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a196c-214">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a196c-215">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-215">Boolean</span></span>|<span data-ttu-id="a196c-216">Indica se o desbloqueio por impressão digital deve ou não ser bloqueado no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-216">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a196c-217">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a196c-217">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="a196c-218">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-218">Boolean</span></span>|<span data-ttu-id="a196c-219">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-219">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="a196c-220">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a196c-220">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="a196c-221">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-221">Int32</span></span>|<span data-ttu-id="a196c-222">Número de dias antes da expiração da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-222">Number of days before the password expires.</span></span> <span data-ttu-id="a196c-223">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="a196c-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a196c-224">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a196c-224">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="a196c-225">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-225">Int32</span></span>|<span data-ttu-id="a196c-226">Tamanho mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-226">Minimum length of work profile password.</span></span> <span data-ttu-id="a196c-227">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="a196c-227">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a196c-228">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="a196c-228">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="a196c-229">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-229">Int32</span></span>|<span data-ttu-id="a196c-230">Número mínimo de caracteres numéricos obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-230">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="a196c-231">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a196c-231">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a196c-232">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="a196c-232">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="a196c-233">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-233">Int32</span></span>|<span data-ttu-id="a196c-234">Número mínimo de caracteres não alfabéticos obrigatórios na senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-234">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="a196c-235">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a196c-235">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a196c-236">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="a196c-236">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="a196c-237">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-237">Int32</span></span>|<span data-ttu-id="a196c-238">Número mínimo de caracteres de alfabéticos obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-238">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="a196c-239">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a196c-239">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a196c-240">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="a196c-240">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="a196c-241">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-241">Int32</span></span>|<span data-ttu-id="a196c-242">Número mínimo de letras minúsculas obrigatórias na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-242">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="a196c-243">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a196c-243">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a196c-244">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="a196c-244">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="a196c-245">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-245">Int32</span></span>|<span data-ttu-id="a196c-246">Número mínimo de letras maiúsculas obrigatórias na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-246">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="a196c-247">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a196c-247">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a196c-248">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="a196c-248">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="a196c-249">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-249">Int32</span></span>|<span data-ttu-id="a196c-250">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a196c-250">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="a196c-251">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a196c-251">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a196c-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a196c-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a196c-253">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-253">Int32</span></span>|<span data-ttu-id="a196c-254">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="a196c-254">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a196c-255">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a196c-255">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a196c-256">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-256">Int32</span></span>|<span data-ttu-id="a196c-257">Número de senhas do perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="a196c-257">Number of previous passwords to block.</span></span> <span data-ttu-id="a196c-258">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="a196c-258">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a196c-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a196c-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a196c-260">Int32</span><span class="sxs-lookup"><span data-stu-id="a196c-260">Int32</span></span>|<span data-ttu-id="a196c-261">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos sejam excluídos.</span><span class="sxs-lookup"><span data-stu-id="a196c-261">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="a196c-262">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="a196c-262">Valid values 4 to 11</span></span>|
|<span data-ttu-id="a196c-263">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a196c-263">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="a196c-264">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a196c-264">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="a196c-265">Tipo de senha de perfil de trabalho obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a196c-265">Type of password that is required.</span></span> <span data-ttu-id="a196c-266">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a196c-266">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a196c-267">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="a196c-267">workProfileRequirePassword</span></span>|<span data-ttu-id="a196c-268">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-268">Boolean</span></span>|<span data-ttu-id="a196c-269">A senha é ou não obrigatória para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="a196c-269">Password is required or not for work profile</span></span>|
|<span data-ttu-id="a196c-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a196c-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="a196c-271">Booleano</span><span class="sxs-lookup"><span data-stu-id="a196c-271">Boolean</span></span>|<span data-ttu-id="a196c-272">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="a196c-272">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="a196c-273">Resposta</span><span class="sxs-lookup"><span data-stu-id="a196c-273">Response</span></span>
<span data-ttu-id="a196c-274">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a196c-274">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a196c-275">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a196c-275">Example</span></span>
### <a name="request"></a><span data-ttu-id="a196c-276">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a196c-276">Request</span></span>
<span data-ttu-id="a196c-277">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a196c-277">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1895

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="a196c-278">Resposta</span><span class="sxs-lookup"><span data-stu-id="a196c-278">Response</span></span>
<span data-ttu-id="a196c-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a196c-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








