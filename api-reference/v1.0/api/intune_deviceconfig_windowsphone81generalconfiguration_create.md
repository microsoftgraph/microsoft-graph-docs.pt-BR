# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="4d555-101">Criar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4d555-101">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="4d555-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d555-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d555-103">Criar um novo objeto [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d555-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d555-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d555-104">Prerequisites</span></span>
<span data-ttu-id="4d555-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d555-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4d555-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d555-107">Permission type</span></span>|<span data-ttu-id="4d555-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d555-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d555-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d555-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4d555-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d555-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d555-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d555-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d555-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d555-112">Not supported.</span></span>|
|<span data-ttu-id="4d555-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d555-113">Application</span></span>|<span data-ttu-id="4d555-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d555-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d555-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d555-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4d555-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d555-116">Request headers</span></span>
|<span data-ttu-id="4d555-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d555-117">Header</span></span>|<span data-ttu-id="4d555-118">Valor</span><span class="sxs-lookup"><span data-stu-id="4d555-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d555-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d555-119">Authorization</span></span>|<span data-ttu-id="4d555-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d555-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4d555-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d555-121">Accept</span></span>|<span data-ttu-id="4d555-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4d555-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d555-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d555-123">Request body</span></span>
<span data-ttu-id="4d555-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4d555-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="4d555-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4d555-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="4d555-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d555-126">Property</span></span>|<span data-ttu-id="4d555-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d555-127">Type</span></span>|<span data-ttu-id="4d555-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d555-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d555-129">id</span><span class="sxs-lookup"><span data-stu-id="4d555-129">id</span></span>|<span data-ttu-id="4d555-130">String</span><span class="sxs-lookup"><span data-stu-id="4d555-130">String</span></span>|<span data-ttu-id="4d555-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4d555-131">Key of the setting.</span></span> <span data-ttu-id="4d555-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d555-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d555-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d555-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4d555-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d555-134">DateTimeOffset</span></span>|<span data-ttu-id="4d555-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4d555-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="4d555-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d555-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d555-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d555-137">createdDateTime</span></span>|<span data-ttu-id="4d555-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d555-138">DateTimeOffset</span></span>|<span data-ttu-id="4d555-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4d555-139">DateTime the object was created.</span></span> <span data-ttu-id="4d555-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d555-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d555-141">descrição</span><span class="sxs-lookup"><span data-stu-id="4d555-141">description</span></span>|<span data-ttu-id="4d555-142">String</span><span class="sxs-lookup"><span data-stu-id="4d555-142">String</span></span>|<span data-ttu-id="4d555-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d555-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4d555-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d555-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d555-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4d555-145">displayName</span></span>|<span data-ttu-id="4d555-146">String</span><span class="sxs-lookup"><span data-stu-id="4d555-146">String</span></span>|<span data-ttu-id="4d555-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d555-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4d555-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d555-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d555-149">version</span><span class="sxs-lookup"><span data-stu-id="4d555-149">version</span></span>|<span data-ttu-id="4d555-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4d555-150">Int32</span></span>|<span data-ttu-id="4d555-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d555-151">Version of the device configuration.</span></span> <span data-ttu-id="4d555-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4d555-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d555-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4d555-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4d555-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-154">Boolean</span></span>|<span data-ttu-id="4d555-155">Valor que indica se esta política se aplica somente ao Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="4d555-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="4d555-156">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4d555-156">This property is read-only.</span></span>|
|<span data-ttu-id="4d555-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4d555-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="4d555-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-158">Boolean</span></span>|<span data-ttu-id="4d555-159">Indica se a função copiar/colar deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4d555-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="4d555-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-160">bluetoothBlocked</span></span>|<span data-ttu-id="4d555-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-161">Boolean</span></span>|<span data-ttu-id="4d555-162">Indica se o bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="4d555-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-163">cameraBlocked</span></span>|<span data-ttu-id="4d555-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-164">Boolean</span></span>|<span data-ttu-id="4d555-165">Indica se a câmera deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4d555-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="4d555-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="4d555-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="4d555-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-167">Boolean</span></span>|<span data-ttu-id="4d555-168">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="4d555-169">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4d555-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4d555-170">compliantAppsList</span></span>|<span data-ttu-id="4d555-171">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4d555-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="4d555-172">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="4d555-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4d555-173">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="4d555-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4d555-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4d555-174">compliantAppListType</span></span>|<span data-ttu-id="4d555-175">String</span><span class="sxs-lookup"><span data-stu-id="4d555-175">String</span></span>|<span data-ttu-id="4d555-176">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="4d555-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="4d555-177">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="4d555-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4d555-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4d555-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4d555-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-179">Boolean</span></span>|<span data-ttu-id="4d555-180">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4d555-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="4d555-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="4d555-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-182">Boolean</span></span>|<span data-ttu-id="4d555-183">Indica se as contas de email personalizadas devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="4d555-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="4d555-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-184">locationServicesBlocked</span></span>|<span data-ttu-id="4d555-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-185">Boolean</span></span>|<span data-ttu-id="4d555-186">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4d555-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4d555-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="4d555-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-188">Boolean</span></span>|<span data-ttu-id="4d555-189">Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="4d555-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-190">nfcBlocked</span></span>|<span data-ttu-id="4d555-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-191">Boolean</span></span>|<span data-ttu-id="4d555-192">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4d555-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4d555-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4d555-193">passwordBlockSimple</span></span>|<span data-ttu-id="4d555-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-194">Boolean</span></span>|<span data-ttu-id="4d555-195">Indica se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4d555-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4d555-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4d555-196">passwordExpirationDays</span></span>|<span data-ttu-id="4d555-197">Int32</span><span class="sxs-lookup"><span data-stu-id="4d555-197">Int32</span></span>|<span data-ttu-id="4d555-198">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="4d555-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="4d555-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4d555-199">passwordMinimumLength</span></span>|<span data-ttu-id="4d555-200">Int32</span><span class="sxs-lookup"><span data-stu-id="4d555-200">Int32</span></span>|<span data-ttu-id="4d555-201">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="4d555-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="4d555-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4d555-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4d555-203">Int32</span><span class="sxs-lookup"><span data-stu-id="4d555-203">Int32</span></span>|<span data-ttu-id="4d555-204">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="4d555-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="4d555-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4d555-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4d555-206">Int32</span><span class="sxs-lookup"><span data-stu-id="4d555-206">Int32</span></span>|<span data-ttu-id="4d555-207">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="4d555-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="4d555-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4d555-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4d555-209">Int32</span><span class="sxs-lookup"><span data-stu-id="4d555-209">Int32</span></span>|<span data-ttu-id="4d555-210">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="4d555-210">Number of previous passwords to block.</span></span> <span data-ttu-id="4d555-211">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="4d555-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4d555-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4d555-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4d555-213">Int32</span><span class="sxs-lookup"><span data-stu-id="4d555-213">Int32</span></span>|<span data-ttu-id="4d555-214">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="4d555-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="4d555-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4d555-215">passwordRequiredType</span></span>|<span data-ttu-id="4d555-216">String</span><span class="sxs-lookup"><span data-stu-id="4d555-216">String</span></span>|<span data-ttu-id="4d555-217">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="4d555-217">Password type that is required.</span></span> <span data-ttu-id="4d555-218">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4d555-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4d555-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4d555-219">passwordRequired</span></span>|<span data-ttu-id="4d555-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-220">Boolean</span></span>|<span data-ttu-id="4d555-221">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="4d555-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4d555-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-222">screenCaptureBlocked</span></span>|<span data-ttu-id="4d555-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-223">Boolean</span></span>|<span data-ttu-id="4d555-224">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="4d555-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4d555-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4d555-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4d555-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-226">Boolean</span></span>|<span data-ttu-id="4d555-227">Indica se o armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="4d555-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4d555-228">storageRequireEncryption</span></span>|<span data-ttu-id="4d555-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-229">Boolean</span></span>|<span data-ttu-id="4d555-230">Indica se a criptografia é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="4d555-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="4d555-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-231">webBrowserBlocked</span></span>|<span data-ttu-id="4d555-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-232">Boolean</span></span>|<span data-ttu-id="4d555-233">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4d555-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-234">wifiBlocked</span></span>|<span data-ttu-id="4d555-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-235">Boolean</span></span>|<span data-ttu-id="4d555-236">Indica se o Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="4d555-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="4d555-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="4d555-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-238">Boolean</span></span>|<span data-ttu-id="4d555-239">Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4d555-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="4d555-240">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4d555-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="4d555-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="4d555-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-242">Boolean</span></span>|<span data-ttu-id="4d555-243">Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4d555-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="4d555-244">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4d555-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4d555-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4d555-245">windowsStoreBlocked</span></span>|<span data-ttu-id="4d555-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d555-246">Boolean</span></span>|<span data-ttu-id="4d555-247">Indica se a Windows Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4d555-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="4d555-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d555-248">Response</span></span>
<span data-ttu-id="4d555-249">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d555-249">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d555-250">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d555-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d555-251">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d555-251">Request</span></span>
<span data-ttu-id="4d555-252">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d555-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1525

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="4d555-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d555-253">Response</span></span>
<span data-ttu-id="4d555-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d555-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



