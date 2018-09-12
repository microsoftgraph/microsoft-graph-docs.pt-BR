# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="2ad54-101">Criar sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ad54-101">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="2ad54-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2ad54-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ad54-103">Cria um novo objeto [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ad54-103">Create a new [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ad54-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ad54-104">Prerequisites</span></span>
<span data-ttu-id="2ad54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ad54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ad54-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ad54-107">Permission type</span></span>|<span data-ttu-id="2ad54-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ad54-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ad54-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ad54-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2ad54-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ad54-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ad54-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ad54-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ad54-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ad54-112">Not supported.</span></span>|
|<span data-ttu-id="2ad54-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ad54-113">Application</span></span>|<span data-ttu-id="2ad54-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ad54-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ad54-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ad54-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2ad54-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ad54-116">Request headers</span></span>
|<span data-ttu-id="2ad54-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ad54-117">Header</span></span>|<span data-ttu-id="2ad54-118">Valor</span><span class="sxs-lookup"><span data-stu-id="2ad54-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ad54-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ad54-119">Authorization</span></span>|<span data-ttu-id="2ad54-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="2ad54-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ad54-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ad54-121">Accept</span></span>|<span data-ttu-id="2ad54-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2ad54-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ad54-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ad54-123">Request body</span></span>
<span data-ttu-id="2ad54-124">No corpo da solicitação, forneça uma representação JSON do objeto sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2ad54-124">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="2ad54-125">A tabela a seguir mostra as propriedades que são necessárias ao criar sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2ad54-125">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="2ad54-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ad54-126">Property</span></span>|<span data-ttu-id="2ad54-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ad54-127">Type</span></span>|<span data-ttu-id="2ad54-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ad54-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad54-129">id</span><span class="sxs-lookup"><span data-stu-id="2ad54-129">id</span></span>|<span data-ttu-id="2ad54-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ad54-130">String</span></span>|<span data-ttu-id="2ad54-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2ad54-131">Key of the entity.</span></span> <span data-ttu-id="2ad54-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad54-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad54-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad54-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2ad54-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad54-134">DateTimeOffset</span></span>|<span data-ttu-id="2ad54-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2ad54-135">DateTime the object was last modified.</span></span> <span data-ttu-id="2ad54-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad54-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad54-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad54-137">createdDateTime</span></span>|<span data-ttu-id="2ad54-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad54-138">DateTimeOffset</span></span>|<span data-ttu-id="2ad54-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2ad54-139">DateTime the object was created.</span></span> <span data-ttu-id="2ad54-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad54-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad54-141">description</span><span class="sxs-lookup"><span data-stu-id="2ad54-141">description</span></span>|<span data-ttu-id="2ad54-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ad54-142">String</span></span>|<span data-ttu-id="2ad54-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ad54-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2ad54-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad54-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad54-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2ad54-145">displayName</span></span>|<span data-ttu-id="2ad54-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ad54-146">String</span></span>|<span data-ttu-id="2ad54-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ad54-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2ad54-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad54-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad54-149">version</span><span class="sxs-lookup"><span data-stu-id="2ad54-149">version</span></span>|<span data-ttu-id="2ad54-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad54-150">Int32</span></span>|<span data-ttu-id="2ad54-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ad54-151">Version of the device configuration.</span></span> <span data-ttu-id="2ad54-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ad54-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ad54-153">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="2ad54-153">accountManagerPolicy</span></span>|[<span data-ttu-id="2ad54-154">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="2ad54-154">sharedPCAccountManagerPolicy</span></span>](../resources/intune_deviceconfig_sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="2ad54-155">Especifica como as contas são gerenciadas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2ad54-155">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="2ad54-156">Aplica-se somente quando disableAccountManager é false.</span><span class="sxs-lookup"><span data-stu-id="2ad54-156">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="2ad54-157">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="2ad54-157">allowedAccounts</span></span>|[<span data-ttu-id="2ad54-158">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="2ad54-158">sharedPCAllowedAccountType</span></span>](../resources/intune_deviceconfig_sharedpcallowedaccounttype.md)|<span data-ttu-id="2ad54-p109">Indica quais tipos de contas têm permissão para usar em um PC compartilhado. Os valores possíveis são: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="2ad54-p109">Indicates which type of accounts are allowed to use on a shared PC. The possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="2ad54-161">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="2ad54-161">allowLocalStorage</span></span>|<span data-ttu-id="2ad54-162">Booleano</span><span class="sxs-lookup"><span data-stu-id="2ad54-162">Boolean</span></span>|<span data-ttu-id="2ad54-163">Especifica se o armazenamento local é permitido em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2ad54-163">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="2ad54-164">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="2ad54-164">disableAccountManager</span></span>|<span data-ttu-id="2ad54-165">Booleano</span><span class="sxs-lookup"><span data-stu-id="2ad54-165">Boolean</span></span>|<span data-ttu-id="2ad54-166">Desabilita o gerente de contas para o modo de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2ad54-166">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="2ad54-167">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="2ad54-167">disableEduPolicies</span></span>|<span data-ttu-id="2ad54-168">Booleano</span><span class="sxs-lookup"><span data-stu-id="2ad54-168">Boolean</span></span>|<span data-ttu-id="2ad54-169">Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="2ad54-169">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="2ad54-170">Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.</span><span class="sxs-lookup"><span data-stu-id="2ad54-170">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="2ad54-171">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="2ad54-171">disablePowerPolicies</span></span>|<span data-ttu-id="2ad54-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="2ad54-172">Boolean</span></span>|<span data-ttu-id="2ad54-173">Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="2ad54-173">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="2ad54-174">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="2ad54-174">disableSignInOnResume</span></span>|<span data-ttu-id="2ad54-175">Booleano</span><span class="sxs-lookup"><span data-stu-id="2ad54-175">Boolean</span></span>|<span data-ttu-id="2ad54-176">Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="2ad54-176">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="2ad54-177">enabled</span><span class="sxs-lookup"><span data-stu-id="2ad54-177">enabled</span></span>|<span data-ttu-id="2ad54-178">Booleano</span><span class="sxs-lookup"><span data-stu-id="2ad54-178">Boolean</span></span>|<span data-ttu-id="2ad54-179">Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="2ad54-179">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="2ad54-180">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="2ad54-180">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="2ad54-181">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad54-181">Int32</span></span>|<span data-ttu-id="2ad54-182">Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão.</span><span class="sxs-lookup"><span data-stu-id="2ad54-182">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="2ad54-183">Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.</span><span class="sxs-lookup"><span data-stu-id="2ad54-183">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="2ad54-184">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ad54-184">kioskAppDisplayName</span></span>|<span data-ttu-id="2ad54-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ad54-185">String</span></span>|<span data-ttu-id="2ad54-186">Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="2ad54-186">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="2ad54-187">Aplicável somente quando KioskAppUserModelId está definido.</span><span class="sxs-lookup"><span data-stu-id="2ad54-187">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="2ad54-188">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="2ad54-188">kioskAppUserModelId</span></span>|<span data-ttu-id="2ad54-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ad54-189">String</span></span>|<span data-ttu-id="2ad54-190">Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.</span><span class="sxs-lookup"><span data-stu-id="2ad54-190">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="2ad54-191">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="2ad54-191">maintenanceStartTime</span></span>|<span data-ttu-id="2ad54-192">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2ad54-192">TimeOfDay</span></span>|<span data-ttu-id="2ad54-193">Especifica o horário de início diário da hora de manutenção.</span><span class="sxs-lookup"><span data-stu-id="2ad54-193">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="2ad54-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ad54-194">Response</span></span>
<span data-ttu-id="2ad54-195">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ad54-195">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ad54-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ad54-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ad54-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ad54-197">Request</span></span>
<span data-ttu-id="2ad54-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ad54-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 924

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="2ad54-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ad54-199">Response</span></span>
<span data-ttu-id="2ad54-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ad54-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```








