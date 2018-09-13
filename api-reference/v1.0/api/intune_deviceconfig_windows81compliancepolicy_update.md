# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="bb841-101">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bb841-101">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="bb841-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bb841-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb841-103">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bb841-103">Update the properties of a [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb841-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb841-104">Prerequisites</span></span>
<span data-ttu-id="bb841-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bb841-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb841-107">Permission type</span></span>|<span data-ttu-id="bb841-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb841-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb841-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb841-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bb841-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb841-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb841-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb841-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb841-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb841-112">Not supported.</span></span>|
|<span data-ttu-id="bb841-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb841-113">Application</span></span>|<span data-ttu-id="bb841-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb841-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb841-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb841-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="bb841-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb841-116">Request headers</span></span>
|<span data-ttu-id="bb841-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb841-117">Header</span></span>|<span data-ttu-id="bb841-118">Valor</span><span class="sxs-lookup"><span data-stu-id="bb841-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb841-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb841-119">Authorization</span></span>|<span data-ttu-id="bb841-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="bb841-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb841-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb841-121">Accept</span></span>|<span data-ttu-id="bb841-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bb841-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb841-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb841-123">Request body</span></span>
<span data-ttu-id="bb841-124">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bb841-124">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="bb841-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bb841-125">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="bb841-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb841-126">Property</span></span>|<span data-ttu-id="bb841-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb841-127">Type</span></span>|<span data-ttu-id="bb841-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb841-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb841-129">id</span><span class="sxs-lookup"><span data-stu-id="bb841-129">id</span></span>|<span data-ttu-id="bb841-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb841-130">String</span></span>|<span data-ttu-id="bb841-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb841-131">Key of the entity.</span></span> <span data-ttu-id="bb841-132">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb841-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bb841-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb841-133">createdDateTime</span></span>|<span data-ttu-id="bb841-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb841-134">DateTimeOffset</span></span>|<span data-ttu-id="bb841-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bb841-135">DateTime the object was created.</span></span> <span data-ttu-id="bb841-136">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb841-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bb841-137">description</span><span class="sxs-lookup"><span data-stu-id="bb841-137">description</span></span>|<span data-ttu-id="bb841-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb841-138">String</span></span>|<span data-ttu-id="bb841-139">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb841-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb841-140">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb841-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bb841-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb841-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bb841-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb841-142">DateTimeOffset</span></span>|<span data-ttu-id="bb841-143">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bb841-143">DateTime the object was last modified.</span></span> <span data-ttu-id="bb841-144">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb841-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bb841-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bb841-145">displayName</span></span>|<span data-ttu-id="bb841-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb841-146">String</span></span>|<span data-ttu-id="bb841-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb841-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb841-148">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb841-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bb841-149">version</span><span class="sxs-lookup"><span data-stu-id="bb841-149">version</span></span>|<span data-ttu-id="bb841-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bb841-150">Int32</span></span>|<span data-ttu-id="bb841-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb841-151">Version of the device configuration.</span></span> <span data-ttu-id="bb841-152">Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb841-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bb841-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bb841-153">passwordRequired</span></span>|<span data-ttu-id="bb841-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb841-154">Boolean</span></span>|<span data-ttu-id="bb841-155">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="bb841-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="bb841-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bb841-156">passwordBlockSimple</span></span>|<span data-ttu-id="bb841-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb841-157">Boolean</span></span>|<span data-ttu-id="bb841-158">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bb841-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="bb841-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bb841-159">passwordExpirationDays</span></span>|<span data-ttu-id="bb841-160">Int32</span><span class="sxs-lookup"><span data-stu-id="bb841-160">Int32</span></span>|<span data-ttu-id="bb841-161">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="bb841-161">Password expiration in days.</span></span>|
|<span data-ttu-id="bb841-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bb841-162">passwordMinimumLength</span></span>|<span data-ttu-id="bb841-163">Int32</span><span class="sxs-lookup"><span data-stu-id="bb841-163">Int32</span></span>|<span data-ttu-id="bb841-164">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="bb841-164">The minimum password length.</span></span>|
|<span data-ttu-id="bb841-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bb841-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bb841-166">Int32</span><span class="sxs-lookup"><span data-stu-id="bb841-166">Int32</span></span>|<span data-ttu-id="bb841-167">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="bb841-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bb841-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bb841-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bb841-169">Int32</span><span class="sxs-lookup"><span data-stu-id="bb841-169">Int32</span></span>|<span data-ttu-id="bb841-170">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="bb841-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bb841-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bb841-171">passwordRequiredType</span></span>|[<span data-ttu-id="bb841-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bb841-172">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="bb841-p108">O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bb841-p108">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bb841-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bb841-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bb841-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bb841-176">Int32</span></span>|<span data-ttu-id="bb841-177">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="bb841-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="bb841-178">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="bb841-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="bb841-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bb841-179">osMinimumVersion</span></span>|<span data-ttu-id="bb841-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb841-180">String</span></span>|<span data-ttu-id="bb841-181">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="bb841-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="bb841-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bb841-182">osMaximumVersion</span></span>|<span data-ttu-id="bb841-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb841-183">String</span></span>|<span data-ttu-id="bb841-184">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="bb841-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="bb841-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bb841-185">storageRequireEncryption</span></span>|<span data-ttu-id="bb841-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb841-186">Boolean</span></span>|<span data-ttu-id="bb841-187">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="bb841-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="bb841-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb841-188">Response</span></span>
<span data-ttu-id="bb841-189">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb841-189">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb841-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb841-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb841-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb841-191">Request</span></span>
<span data-ttu-id="bb841-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb841-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb841-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb841-193">Response</span></span>
<span data-ttu-id="bb841-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb841-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








