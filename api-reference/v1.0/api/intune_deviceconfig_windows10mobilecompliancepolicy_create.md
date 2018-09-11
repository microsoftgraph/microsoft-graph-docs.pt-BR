# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="caddd-101">Criar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="caddd-101">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="caddd-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="caddd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caddd-103">Cria um novo objeto [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="caddd-103">Create a new [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="caddd-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="caddd-104">Prerequisites</span></span>
<span data-ttu-id="caddd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="caddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="caddd-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caddd-107">Permission type</span></span>|<span data-ttu-id="caddd-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="caddd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caddd-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caddd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="caddd-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caddd-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="caddd-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caddd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caddd-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caddd-112">Not supported.</span></span>|
|<span data-ttu-id="caddd-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caddd-113">Application</span></span>|<span data-ttu-id="caddd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caddd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caddd-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caddd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="caddd-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caddd-116">Request headers</span></span>
|<span data-ttu-id="caddd-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="caddd-117">Header</span></span>|<span data-ttu-id="caddd-118">Valor</span><span class="sxs-lookup"><span data-stu-id="caddd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caddd-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="caddd-119">Authorization</span></span>|<span data-ttu-id="caddd-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="caddd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caddd-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="caddd-121">Accept</span></span>|<span data-ttu-id="caddd-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="caddd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caddd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caddd-123">Request body</span></span>
<span data-ttu-id="caddd-124">No corpo da solicitação, forneça uma representação JSON do objeto windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="caddd-124">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="caddd-125">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="caddd-125">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="caddd-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="caddd-126">Property</span></span>|<span data-ttu-id="caddd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="caddd-127">Type</span></span>|<span data-ttu-id="caddd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="caddd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caddd-129">id</span><span class="sxs-lookup"><span data-stu-id="caddd-129">id</span></span>|<span data-ttu-id="caddd-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="caddd-130">String</span></span>|<span data-ttu-id="caddd-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="caddd-131">Key of the entity.</span></span> <span data-ttu-id="caddd-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="caddd-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="caddd-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="caddd-133">createdDateTime</span></span>|<span data-ttu-id="caddd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caddd-134">DateTimeOffset</span></span>|<span data-ttu-id="caddd-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="caddd-135">DateTime the object was created.</span></span> <span data-ttu-id="caddd-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="caddd-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="caddd-137">descrição</span><span class="sxs-lookup"><span data-stu-id="caddd-137">description</span></span>|<span data-ttu-id="caddd-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="caddd-138">String</span></span>|<span data-ttu-id="caddd-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="caddd-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="caddd-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="caddd-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="caddd-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="caddd-141">lastModifiedDateTime</span></span>|<span data-ttu-id="caddd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caddd-142">DateTimeOffset</span></span>|<span data-ttu-id="caddd-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="caddd-143">DateTime the object was last modified.</span></span> <span data-ttu-id="caddd-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="caddd-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="caddd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="caddd-145">displayName</span></span>|<span data-ttu-id="caddd-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="caddd-146">String</span></span>|<span data-ttu-id="caddd-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="caddd-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="caddd-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="caddd-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="caddd-149">versão</span><span class="sxs-lookup"><span data-stu-id="caddd-149">version</span></span>|<span data-ttu-id="caddd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="caddd-150">Int32</span></span>|<span data-ttu-id="caddd-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="caddd-151">Version of the device configuration.</span></span> <span data-ttu-id="caddd-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="caddd-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="caddd-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="caddd-153">passwordRequired</span></span>|<span data-ttu-id="caddd-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="caddd-154">Boolean</span></span>|<span data-ttu-id="caddd-155">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="caddd-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="caddd-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="caddd-156">passwordBlockSimple</span></span>|<span data-ttu-id="caddd-157">Booleano</span><span class="sxs-lookup"><span data-stu-id="caddd-157">Boolean</span></span>|<span data-ttu-id="caddd-158">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="caddd-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="caddd-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="caddd-159">passwordMinimumLength</span></span>|<span data-ttu-id="caddd-160">Int32</span><span class="sxs-lookup"><span data-stu-id="caddd-160">Int32</span></span>|<span data-ttu-id="caddd-161">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="caddd-161">Minimum password length.</span></span> <span data-ttu-id="caddd-162">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="caddd-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="caddd-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="caddd-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="caddd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="caddd-164">Int32</span></span>|<span data-ttu-id="caddd-165">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="caddd-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="caddd-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="caddd-166">passwordRequiredType</span></span>|[<span data-ttu-id="caddd-167">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="caddd-167">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="caddd-p109">O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="caddd-p109">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="caddd-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="caddd-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="caddd-171">Int32</span><span class="sxs-lookup"><span data-stu-id="caddd-171">Int32</span></span>|<span data-ttu-id="caddd-172">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="caddd-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="caddd-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="caddd-173">passwordExpirationDays</span></span>|<span data-ttu-id="caddd-174">Int32</span><span class="sxs-lookup"><span data-stu-id="caddd-174">Int32</span></span>|<span data-ttu-id="caddd-175">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="caddd-175">Number of days before password expiration.</span></span> <span data-ttu-id="caddd-176">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="caddd-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="caddd-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="caddd-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="caddd-178">Int32</span><span class="sxs-lookup"><span data-stu-id="caddd-178">Int32</span></span>|<span data-ttu-id="caddd-179">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="caddd-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="caddd-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="caddd-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="caddd-181">Booleano</span><span class="sxs-lookup"><span data-stu-id="caddd-181">Boolean</span></span>|<span data-ttu-id="caddd-182">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="caddd-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="caddd-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="caddd-183">osMinimumVersion</span></span>|<span data-ttu-id="caddd-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="caddd-184">String</span></span>|<span data-ttu-id="caddd-185">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="caddd-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="caddd-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="caddd-186">osMaximumVersion</span></span>|<span data-ttu-id="caddd-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="caddd-187">String</span></span>|<span data-ttu-id="caddd-188">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="caddd-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="caddd-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="caddd-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="caddd-190">Booleano</span><span class="sxs-lookup"><span data-stu-id="caddd-190">Boolean</span></span>|<span data-ttu-id="caddd-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="caddd-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="caddd-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="caddd-192">bitLockerEnabled</span></span>|<span data-ttu-id="caddd-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="caddd-193">Boolean</span></span>|<span data-ttu-id="caddd-194">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="caddd-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="caddd-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="caddd-195">secureBootEnabled</span></span>|<span data-ttu-id="caddd-196">Booleano</span><span class="sxs-lookup"><span data-stu-id="caddd-196">Boolean</span></span>|<span data-ttu-id="caddd-197">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="caddd-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="caddd-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="caddd-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="caddd-199">Booleano</span><span class="sxs-lookup"><span data-stu-id="caddd-199">Boolean</span></span>|<span data-ttu-id="caddd-200">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="caddd-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="caddd-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="caddd-201">storageRequireEncryption</span></span>|<span data-ttu-id="caddd-202">Booleano</span><span class="sxs-lookup"><span data-stu-id="caddd-202">Boolean</span></span>|<span data-ttu-id="caddd-203">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="caddd-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="caddd-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="caddd-204">Response</span></span>
<span data-ttu-id="caddd-205">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caddd-205">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caddd-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="caddd-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="caddd-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caddd-207">Request</span></span>
<span data-ttu-id="caddd-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="caddd-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 856

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="caddd-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="caddd-209">Response</span></span>
<span data-ttu-id="caddd-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="caddd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```








