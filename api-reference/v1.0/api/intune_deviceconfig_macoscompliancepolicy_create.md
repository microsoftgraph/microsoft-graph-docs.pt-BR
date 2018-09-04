# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="0fb27-101">Criar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0fb27-101">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="0fb27-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0fb27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fb27-103">Cria um novo objeto [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fb27-103">Create a new [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0fb27-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fb27-104">Prerequisites</span></span>
<span data-ttu-id="0fb27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0fb27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0fb27-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fb27-107">Permission type</span></span>|<span data-ttu-id="0fb27-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0fb27-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fb27-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fb27-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0fb27-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb27-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fb27-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fb27-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fb27-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fb27-112">Not supported.</span></span>|
|<span data-ttu-id="0fb27-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fb27-113">Application</span></span>|<span data-ttu-id="0fb27-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fb27-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fb27-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fb27-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0fb27-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb27-116">Request headers</span></span>
|<span data-ttu-id="0fb27-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fb27-117">Header</span></span>|<span data-ttu-id="0fb27-118">Valor</span><span class="sxs-lookup"><span data-stu-id="0fb27-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fb27-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fb27-119">Authorization</span></span>|<span data-ttu-id="0fb27-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="0fb27-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fb27-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fb27-121">Accept</span></span>|<span data-ttu-id="0fb27-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0fb27-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fb27-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb27-123">Request body</span></span>
<span data-ttu-id="0fb27-124">No corpo da solicitação, forneça uma representação JSON do objeto macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="0fb27-124">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="0fb27-125">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="0fb27-125">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="0fb27-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fb27-126">Property</span></span>|<span data-ttu-id="0fb27-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fb27-127">Type</span></span>|<span data-ttu-id="0fb27-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fb27-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb27-129">id</span><span class="sxs-lookup"><span data-stu-id="0fb27-129">id</span></span>|<span data-ttu-id="0fb27-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fb27-130">String</span></span>|<span data-ttu-id="0fb27-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0fb27-131">Key of the entity.</span></span> <span data-ttu-id="0fb27-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0fb27-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb27-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fb27-133">createdDateTime</span></span>|<span data-ttu-id="0fb27-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fb27-134">DateTimeOffset</span></span>|<span data-ttu-id="0fb27-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0fb27-135">DateTime the object was created.</span></span> <span data-ttu-id="0fb27-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0fb27-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb27-137">description</span><span class="sxs-lookup"><span data-stu-id="0fb27-137">description</span></span>|<span data-ttu-id="0fb27-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fb27-138">String</span></span>|<span data-ttu-id="0fb27-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0fb27-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0fb27-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0fb27-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb27-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fb27-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0fb27-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fb27-142">DateTimeOffset</span></span>|<span data-ttu-id="0fb27-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0fb27-143">DateTime the object was last modified.</span></span> <span data-ttu-id="0fb27-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0fb27-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb27-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0fb27-145">displayName</span></span>|<span data-ttu-id="0fb27-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fb27-146">String</span></span>|<span data-ttu-id="0fb27-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0fb27-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0fb27-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0fb27-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb27-149">version</span><span class="sxs-lookup"><span data-stu-id="0fb27-149">version</span></span>|<span data-ttu-id="0fb27-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb27-150">Int32</span></span>|<span data-ttu-id="0fb27-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0fb27-151">Version of the device configuration.</span></span> <span data-ttu-id="0fb27-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0fb27-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb27-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0fb27-153">passwordRequired</span></span>|<span data-ttu-id="0fb27-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="0fb27-154">Boolean</span></span>|<span data-ttu-id="0fb27-155">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="0fb27-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="0fb27-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0fb27-156">passwordBlockSimple</span></span>|<span data-ttu-id="0fb27-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="0fb27-157">Boolean</span></span>|<span data-ttu-id="0fb27-158">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="0fb27-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="0fb27-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0fb27-159">passwordExpirationDays</span></span>|<span data-ttu-id="0fb27-160">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb27-160">Int32</span></span>|<span data-ttu-id="0fb27-161">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="0fb27-161">Number of days before the password expires.</span></span> <span data-ttu-id="0fb27-162">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="0fb27-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0fb27-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0fb27-163">passwordMinimumLength</span></span>|<span data-ttu-id="0fb27-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb27-164">Int32</span></span>|<span data-ttu-id="0fb27-165">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="0fb27-165">Minimum length of password.</span></span> <span data-ttu-id="0fb27-166">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="0fb27-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="0fb27-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0fb27-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0fb27-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb27-168">Int32</span></span>|<span data-ttu-id="0fb27-169">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="0fb27-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0fb27-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0fb27-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0fb27-171">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb27-171">Int32</span></span>|<span data-ttu-id="0fb27-172">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="0fb27-172">Number of previous passwords to block.</span></span> <span data-ttu-id="0fb27-173">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="0fb27-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0fb27-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0fb27-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0fb27-175">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb27-175">Int32</span></span>|<span data-ttu-id="0fb27-176">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="0fb27-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0fb27-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0fb27-177">passwordRequiredType</span></span>|[<span data-ttu-id="0fb27-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0fb27-178">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="0fb27-179">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="0fb27-179">The required password type.</span></span> <span data-ttu-id="0fb27-180">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0fb27-180">The possible values are:</span></span>|
|<span data-ttu-id="0fb27-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0fb27-181">osMinimumVersion</span></span>|<span data-ttu-id="0fb27-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fb27-182">String</span></span>|<span data-ttu-id="0fb27-183">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="0fb27-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="0fb27-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0fb27-184">osMaximumVersion</span></span>|<span data-ttu-id="0fb27-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fb27-185">String</span></span>|<span data-ttu-id="0fb27-186">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="0fb27-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="0fb27-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0fb27-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="0fb27-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="0fb27-188">Boolean</span></span>|<span data-ttu-id="0fb27-189">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="0fb27-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="0fb27-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0fb27-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0fb27-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="0fb27-191">Boolean</span></span>|<span data-ttu-id="0fb27-192">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="0fb27-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="0fb27-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0fb27-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0fb27-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0fb27-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="0fb27-195">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="0fb27-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0fb27-196">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0fb27-196">The possible values are `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`, , , , , , or .</span></span>|
|<span data-ttu-id="0fb27-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0fb27-197">storageRequireEncryption</span></span>|<span data-ttu-id="0fb27-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="0fb27-198">Boolean</span></span>|<span data-ttu-id="0fb27-199">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="0fb27-199">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="0fb27-200">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="0fb27-200">firewallEnabled</span></span>|<span data-ttu-id="0fb27-201">Booleano</span><span class="sxs-lookup"><span data-stu-id="0fb27-201">Boolean</span></span>|<span data-ttu-id="0fb27-202">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="0fb27-202">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="0fb27-203">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="0fb27-203">firewallBlockAllIncoming</span></span>|<span data-ttu-id="0fb27-204">Booleano</span><span class="sxs-lookup"><span data-stu-id="0fb27-204">Boolean</span></span>|<span data-ttu-id="0fb27-205">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="0fb27-205">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="0fb27-206">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="0fb27-206">firewallEnableStealthMode</span></span>|<span data-ttu-id="0fb27-207">Booleano</span><span class="sxs-lookup"><span data-stu-id="0fb27-207">Boolean</span></span>|<span data-ttu-id="0fb27-208">Corresponde à "Habilitar modo furtivo".</span><span class="sxs-lookup"><span data-stu-id="0fb27-208">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="0fb27-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fb27-209">Response</span></span>
<span data-ttu-id="0fb27-210">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fb27-210">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fb27-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fb27-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="0fb27-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb27-212">Request</span></span>
<span data-ttu-id="0fb27-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fb27-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 913

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="0fb27-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fb27-214">Response</span></span>
<span data-ttu-id="0fb27-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fb27-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



