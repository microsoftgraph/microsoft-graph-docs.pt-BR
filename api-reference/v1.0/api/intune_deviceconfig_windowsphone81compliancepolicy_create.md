# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="06091-101">Criar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="06091-101">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="06091-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06091-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06091-103">Cria um novo objeto [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06091-103">Create a new [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06091-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06091-104">Prerequisites</span></span>
<span data-ttu-id="06091-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="06091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06091-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06091-107">Permission type</span></span>|<span data-ttu-id="06091-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06091-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06091-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06091-109">Delegated (work or school account)</span></span>|<span data-ttu-id="06091-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06091-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06091-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06091-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06091-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06091-112">Not supported.</span></span>|
|<span data-ttu-id="06091-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06091-113">Application</span></span>|<span data-ttu-id="06091-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06091-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06091-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06091-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="06091-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06091-116">Request headers</span></span>
|<span data-ttu-id="06091-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06091-117">Header</span></span>|<span data-ttu-id="06091-118">Valor</span><span class="sxs-lookup"><span data-stu-id="06091-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06091-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="06091-119">Authorization</span></span>|<span data-ttu-id="06091-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="06091-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06091-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06091-121">Accept</span></span>|<span data-ttu-id="06091-122">application/json</span><span class="sxs-lookup"><span data-stu-id="06091-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06091-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06091-123">Request body</span></span>
<span data-ttu-id="06091-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="06091-124">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="06091-125">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="06091-125">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="06091-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06091-126">Property</span></span>|<span data-ttu-id="06091-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="06091-127">Type</span></span>|<span data-ttu-id="06091-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="06091-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06091-129">id</span><span class="sxs-lookup"><span data-stu-id="06091-129">id</span></span>|<span data-ttu-id="06091-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06091-130">String</span></span>|<span data-ttu-id="06091-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06091-131">Key of the entity.</span></span> <span data-ttu-id="06091-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06091-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06091-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06091-133">createdDateTime</span></span>|<span data-ttu-id="06091-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06091-134">DateTimeOffset</span></span>|<span data-ttu-id="06091-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="06091-135">DateTime the object was created.</span></span> <span data-ttu-id="06091-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06091-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06091-137">description</span><span class="sxs-lookup"><span data-stu-id="06091-137">description</span></span>|<span data-ttu-id="06091-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06091-138">String</span></span>|<span data-ttu-id="06091-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06091-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06091-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06091-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06091-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06091-141">lastModifiedDateTime</span></span>|<span data-ttu-id="06091-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06091-142">DateTimeOffset</span></span>|<span data-ttu-id="06091-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="06091-143">DateTime the object was last modified.</span></span> <span data-ttu-id="06091-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06091-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06091-145">displayName</span><span class="sxs-lookup"><span data-stu-id="06091-145">displayName</span></span>|<span data-ttu-id="06091-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06091-146">String</span></span>|<span data-ttu-id="06091-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06091-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06091-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06091-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06091-149">version</span><span class="sxs-lookup"><span data-stu-id="06091-149">version</span></span>|<span data-ttu-id="06091-150">Int32</span><span class="sxs-lookup"><span data-stu-id="06091-150">Int32</span></span>|<span data-ttu-id="06091-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06091-151">Version of the device configuration.</span></span> <span data-ttu-id="06091-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06091-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06091-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="06091-153">passwordBlockSimple</span></span>|<span data-ttu-id="06091-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="06091-154">Boolean</span></span>|<span data-ttu-id="06091-155">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="06091-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="06091-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="06091-156">passwordExpirationDays</span></span>|<span data-ttu-id="06091-157">Int32</span><span class="sxs-lookup"><span data-stu-id="06091-157">Int32</span></span>|<span data-ttu-id="06091-158">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="06091-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="06091-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="06091-159">passwordMinimumLength</span></span>|<span data-ttu-id="06091-160">Int32</span><span class="sxs-lookup"><span data-stu-id="06091-160">Int32</span></span>|<span data-ttu-id="06091-161">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="06091-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="06091-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="06091-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="06091-163">Int32</span><span class="sxs-lookup"><span data-stu-id="06091-163">Int32</span></span>|<span data-ttu-id="06091-164">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="06091-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="06091-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="06091-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="06091-166">Int32</span><span class="sxs-lookup"><span data-stu-id="06091-166">Int32</span></span>|<span data-ttu-id="06091-167">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="06091-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="06091-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="06091-168">passwordRequiredType</span></span>|[<span data-ttu-id="06091-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="06091-169">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="06091-p108">O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="06091-p108">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="06091-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="06091-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="06091-173">Int32</span><span class="sxs-lookup"><span data-stu-id="06091-173">Int32</span></span>|<span data-ttu-id="06091-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="06091-174">Number of previous passwords to block.</span></span> <span data-ttu-id="06091-175">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="06091-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="06091-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="06091-176">passwordRequired</span></span>|<span data-ttu-id="06091-177">Booleano</span><span class="sxs-lookup"><span data-stu-id="06091-177">Boolean</span></span>|<span data-ttu-id="06091-178">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="06091-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="06091-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="06091-179">osMinimumVersion</span></span>|<span data-ttu-id="06091-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06091-180">String</span></span>|<span data-ttu-id="06091-181">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="06091-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="06091-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="06091-182">osMaximumVersion</span></span>|<span data-ttu-id="06091-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06091-183">String</span></span>|<span data-ttu-id="06091-184">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="06091-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="06091-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="06091-185">storageRequireEncryption</span></span>|<span data-ttu-id="06091-186">Booleano</span><span class="sxs-lookup"><span data-stu-id="06091-186">Boolean</span></span>|<span data-ttu-id="06091-187">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="06091-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="06091-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="06091-188">Response</span></span>
<span data-ttu-id="06091-189">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06091-189">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06091-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06091-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="06091-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06091-191">Request</span></span>
<span data-ttu-id="06091-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06091-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06091-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="06091-193">Response</span></span>
<span data-ttu-id="06091-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06091-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








