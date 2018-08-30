# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="94aca-101">Criar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="94aca-101">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="94aca-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="94aca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94aca-103">Cria um novo objeto [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="94aca-103">Create a new [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94aca-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94aca-104">Prerequisites</span></span>
<span data-ttu-id="94aca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="94aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94aca-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94aca-107">Permission type</span></span>|<span data-ttu-id="94aca-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94aca-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94aca-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94aca-109">Delegated (work or school account)</span></span>|<span data-ttu-id="94aca-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94aca-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94aca-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94aca-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94aca-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94aca-112">Not supported.</span></span>|
|<span data-ttu-id="94aca-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94aca-113">Application</span></span>|<span data-ttu-id="94aca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94aca-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94aca-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94aca-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="94aca-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94aca-116">Request headers</span></span>
|<span data-ttu-id="94aca-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94aca-117">Header</span></span>|<span data-ttu-id="94aca-118">Valor</span><span class="sxs-lookup"><span data-stu-id="94aca-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94aca-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="94aca-119">Authorization</span></span>|<span data-ttu-id="94aca-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="94aca-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94aca-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94aca-121">Accept</span></span>|<span data-ttu-id="94aca-122">application/json</span><span class="sxs-lookup"><span data-stu-id="94aca-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94aca-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94aca-123">Request body</span></span>
<span data-ttu-id="94aca-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="94aca-124">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="94aca-125">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="94aca-125">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="94aca-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94aca-126">Property</span></span>|<span data-ttu-id="94aca-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="94aca-127">Type</span></span>|<span data-ttu-id="94aca-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="94aca-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94aca-129">id</span><span class="sxs-lookup"><span data-stu-id="94aca-129">id</span></span>|<span data-ttu-id="94aca-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94aca-130">String</span></span>|<span data-ttu-id="94aca-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="94aca-131">Key of the entity.</span></span> <span data-ttu-id="94aca-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="94aca-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="94aca-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94aca-133">createdDateTime</span></span>|<span data-ttu-id="94aca-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94aca-134">DateTimeOffset</span></span>|<span data-ttu-id="94aca-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="94aca-135">DateTime the object was created.</span></span> <span data-ttu-id="94aca-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="94aca-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="94aca-137">description</span><span class="sxs-lookup"><span data-stu-id="94aca-137">description</span></span>|<span data-ttu-id="94aca-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94aca-138">String</span></span>|<span data-ttu-id="94aca-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94aca-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="94aca-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="94aca-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="94aca-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94aca-141">lastModifiedDateTime</span></span>|<span data-ttu-id="94aca-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94aca-142">DateTimeOffset</span></span>|<span data-ttu-id="94aca-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="94aca-143">DateTime the object was last modified.</span></span> <span data-ttu-id="94aca-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="94aca-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="94aca-145">displayName</span><span class="sxs-lookup"><span data-stu-id="94aca-145">displayName</span></span>|<span data-ttu-id="94aca-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94aca-146">String</span></span>|<span data-ttu-id="94aca-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94aca-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="94aca-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="94aca-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="94aca-149">version</span><span class="sxs-lookup"><span data-stu-id="94aca-149">version</span></span>|<span data-ttu-id="94aca-150">Int32</span><span class="sxs-lookup"><span data-stu-id="94aca-150">Int32</span></span>|<span data-ttu-id="94aca-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94aca-151">Version of the device configuration.</span></span> <span data-ttu-id="94aca-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="94aca-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="94aca-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="94aca-153">passwordBlockSimple</span></span>|<span data-ttu-id="94aca-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="94aca-154">Boolean</span></span>|<span data-ttu-id="94aca-155">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="94aca-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="94aca-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="94aca-156">passwordExpirationDays</span></span>|<span data-ttu-id="94aca-157">Int32</span><span class="sxs-lookup"><span data-stu-id="94aca-157">Int32</span></span>|<span data-ttu-id="94aca-158">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="94aca-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="94aca-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="94aca-159">passwordMinimumLength</span></span>|<span data-ttu-id="94aca-160">Int32</span><span class="sxs-lookup"><span data-stu-id="94aca-160">Int32</span></span>|<span data-ttu-id="94aca-161">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="94aca-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="94aca-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="94aca-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="94aca-163">Int32</span><span class="sxs-lookup"><span data-stu-id="94aca-163">Int32</span></span>|<span data-ttu-id="94aca-164">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="94aca-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="94aca-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="94aca-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="94aca-166">Int32</span><span class="sxs-lookup"><span data-stu-id="94aca-166">Int32</span></span>|<span data-ttu-id="94aca-167">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="94aca-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="94aca-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="94aca-168">passwordRequiredType</span></span>|[<span data-ttu-id="94aca-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="94aca-169">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="94aca-170">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="94aca-170">The required password type.</span></span> <span data-ttu-id="94aca-171">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="94aca-171">The possible values are:</span></span>|
|<span data-ttu-id="94aca-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="94aca-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="94aca-173">Int32</span><span class="sxs-lookup"><span data-stu-id="94aca-173">Int32</span></span>|<span data-ttu-id="94aca-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="94aca-174">Number of previous passwords to block.</span></span> <span data-ttu-id="94aca-175">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="94aca-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="94aca-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="94aca-176">passwordRequired</span></span>|<span data-ttu-id="94aca-177">Booleano</span><span class="sxs-lookup"><span data-stu-id="94aca-177">Boolean</span></span>|<span data-ttu-id="94aca-178">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="94aca-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="94aca-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="94aca-179">osMinimumVersion</span></span>|<span data-ttu-id="94aca-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94aca-180">String</span></span>|<span data-ttu-id="94aca-181">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="94aca-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="94aca-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="94aca-182">osMaximumVersion</span></span>|<span data-ttu-id="94aca-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94aca-183">String</span></span>|<span data-ttu-id="94aca-184">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="94aca-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="94aca-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="94aca-185">storageRequireEncryption</span></span>|<span data-ttu-id="94aca-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="94aca-186">Boolean</span></span>|<span data-ttu-id="94aca-187">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="94aca-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="94aca-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="94aca-188">Response</span></span>
<span data-ttu-id="94aca-189">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94aca-189">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94aca-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94aca-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="94aca-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94aca-191">Request</span></span>
<span data-ttu-id="94aca-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94aca-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 671

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="94aca-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="94aca-193">Response</span></span>
<span data-ttu-id="94aca-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94aca-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



