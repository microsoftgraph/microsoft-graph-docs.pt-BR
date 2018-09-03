# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="bc378-101">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bc378-101">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="bc378-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc378-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc378-103">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc378-103">Update the properties of a [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc378-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc378-104">Prerequisites</span></span>
<span data-ttu-id="bc378-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc378-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc378-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc378-107">Permission type</span></span>|<span data-ttu-id="bc378-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc378-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc378-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc378-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bc378-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc378-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc378-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc378-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc378-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc378-112">Not supported.</span></span>|
|<span data-ttu-id="bc378-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc378-113">Application</span></span>|<span data-ttu-id="bc378-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc378-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc378-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc378-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="bc378-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc378-116">Request headers</span></span>
|<span data-ttu-id="bc378-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc378-117">Header</span></span>|<span data-ttu-id="bc378-118">Valor</span><span class="sxs-lookup"><span data-stu-id="bc378-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc378-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc378-119">Authorization</span></span>|<span data-ttu-id="bc378-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="bc378-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc378-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc378-121">Accept</span></span>|<span data-ttu-id="bc378-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bc378-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc378-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc378-123">Request body</span></span>
<span data-ttu-id="bc378-124">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc378-124">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="bc378-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc378-125">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="bc378-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc378-126">Property</span></span>|<span data-ttu-id="bc378-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc378-127">Type</span></span>|<span data-ttu-id="bc378-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc378-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc378-129">id</span><span class="sxs-lookup"><span data-stu-id="bc378-129">id</span></span>|<span data-ttu-id="bc378-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc378-130">String</span></span>|<span data-ttu-id="bc378-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bc378-131">Key of the entity.</span></span> <span data-ttu-id="bc378-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc378-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc378-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc378-133">createdDateTime</span></span>|<span data-ttu-id="bc378-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc378-134">DateTimeOffset</span></span>|<span data-ttu-id="bc378-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bc378-135">DateTime the object was created.</span></span> <span data-ttu-id="bc378-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc378-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc378-137">description</span><span class="sxs-lookup"><span data-stu-id="bc378-137">description</span></span>|<span data-ttu-id="bc378-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc378-138">String</span></span>|<span data-ttu-id="bc378-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc378-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bc378-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc378-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc378-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc378-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bc378-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc378-142">DateTimeOffset</span></span>|<span data-ttu-id="bc378-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bc378-143">DateTime the object was last modified.</span></span> <span data-ttu-id="bc378-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc378-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc378-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bc378-145">displayName</span></span>|<span data-ttu-id="bc378-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc378-146">String</span></span>|<span data-ttu-id="bc378-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc378-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bc378-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc378-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc378-149">version</span><span class="sxs-lookup"><span data-stu-id="bc378-149">version</span></span>|<span data-ttu-id="bc378-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bc378-150">Int32</span></span>|<span data-ttu-id="bc378-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc378-151">Version of the device configuration.</span></span> <span data-ttu-id="bc378-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc378-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc378-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bc378-153">passwordRequired</span></span>|<span data-ttu-id="bc378-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc378-154">Boolean</span></span>|<span data-ttu-id="bc378-155">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="bc378-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="bc378-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bc378-156">passwordBlockSimple</span></span>|<span data-ttu-id="bc378-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc378-157">Boolean</span></span>|<span data-ttu-id="bc378-158">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc378-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="bc378-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bc378-159">passwordExpirationDays</span></span>|<span data-ttu-id="bc378-160">Int32</span><span class="sxs-lookup"><span data-stu-id="bc378-160">Int32</span></span>|<span data-ttu-id="bc378-161">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="bc378-161">Password expiration in days.</span></span>|
|<span data-ttu-id="bc378-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bc378-162">passwordMinimumLength</span></span>|<span data-ttu-id="bc378-163">Int32</span><span class="sxs-lookup"><span data-stu-id="bc378-163">Int32</span></span>|<span data-ttu-id="bc378-164">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="bc378-164">The minimum password length.</span></span>|
|<span data-ttu-id="bc378-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bc378-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bc378-166">Int32</span><span class="sxs-lookup"><span data-stu-id="bc378-166">Int32</span></span>|<span data-ttu-id="bc378-167">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="bc378-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bc378-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bc378-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bc378-169">Int32</span><span class="sxs-lookup"><span data-stu-id="bc378-169">Int32</span></span>|<span data-ttu-id="bc378-170">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="bc378-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bc378-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bc378-171">passwordRequiredType</span></span>|[<span data-ttu-id="bc378-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bc378-172">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="bc378-173">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="bc378-173">The required password type.</span></span> <span data-ttu-id="bc378-174">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bc378-174">The possible values are:</span></span>|
|<span data-ttu-id="bc378-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bc378-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bc378-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bc378-176">Int32</span></span>|<span data-ttu-id="bc378-177">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="bc378-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="bc378-178">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="bc378-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="bc378-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bc378-179">osMinimumVersion</span></span>|<span data-ttu-id="bc378-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc378-180">String</span></span>|<span data-ttu-id="bc378-181">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="bc378-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="bc378-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bc378-182">osMaximumVersion</span></span>|<span data-ttu-id="bc378-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc378-183">String</span></span>|<span data-ttu-id="bc378-184">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="bc378-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="bc378-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bc378-185">storageRequireEncryption</span></span>|<span data-ttu-id="bc378-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc378-186">Boolean</span></span>|<span data-ttu-id="bc378-187">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="bc378-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="bc378-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc378-188">Response</span></span>
<span data-ttu-id="bc378-189">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc378-189">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc378-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc378-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc378-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc378-191">Request</span></span>
<span data-ttu-id="bc378-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc378-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="bc378-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc378-193">Response</span></span>
<span data-ttu-id="bc378-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc378-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



