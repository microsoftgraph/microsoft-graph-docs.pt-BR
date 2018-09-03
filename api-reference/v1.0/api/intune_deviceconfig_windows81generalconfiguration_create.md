# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="92dfb-101">Criar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="92dfb-101">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="92dfb-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="92dfb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92dfb-103">Criar um novo objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92dfb-103">Create a new [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92dfb-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92dfb-104">Prerequisites</span></span>
<span data-ttu-id="92dfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="92dfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="92dfb-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92dfb-107">Permission type</span></span>|<span data-ttu-id="92dfb-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92dfb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92dfb-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92dfb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="92dfb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92dfb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92dfb-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92dfb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92dfb-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92dfb-112">Not supported.</span></span>|
|<span data-ttu-id="92dfb-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92dfb-113">Application</span></span>|<span data-ttu-id="92dfb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92dfb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92dfb-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92dfb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="92dfb-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92dfb-116">Request headers</span></span>
|<span data-ttu-id="92dfb-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92dfb-117">Header</span></span>|<span data-ttu-id="92dfb-118">Valor</span><span class="sxs-lookup"><span data-stu-id="92dfb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92dfb-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="92dfb-119">Authorization</span></span>|<span data-ttu-id="92dfb-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="92dfb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92dfb-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92dfb-121">Accept</span></span>|<span data-ttu-id="92dfb-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="92dfb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92dfb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92dfb-123">Request body</span></span>
<span data-ttu-id="92dfb-124">No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="92dfb-124">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="92dfb-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="92dfb-125">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="92dfb-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92dfb-126">Property</span></span>|<span data-ttu-id="92dfb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="92dfb-127">Type</span></span>|<span data-ttu-id="92dfb-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="92dfb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92dfb-129">id</span><span class="sxs-lookup"><span data-stu-id="92dfb-129">id</span></span>|<span data-ttu-id="92dfb-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92dfb-130">String</span></span>|<span data-ttu-id="92dfb-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92dfb-131">Key of the entity.</span></span> <span data-ttu-id="92dfb-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92dfb-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92dfb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92dfb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="92dfb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92dfb-134">DateTimeOffset</span></span>|<span data-ttu-id="92dfb-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="92dfb-135">DateTime the object was last modified.</span></span> <span data-ttu-id="92dfb-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92dfb-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92dfb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92dfb-137">createdDateTime</span></span>|<span data-ttu-id="92dfb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92dfb-138">DateTimeOffset</span></span>|<span data-ttu-id="92dfb-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="92dfb-139">DateTime the object was created.</span></span> <span data-ttu-id="92dfb-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92dfb-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92dfb-141">description</span><span class="sxs-lookup"><span data-stu-id="92dfb-141">description</span></span>|<span data-ttu-id="92dfb-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92dfb-142">String</span></span>|<span data-ttu-id="92dfb-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92dfb-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92dfb-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92dfb-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92dfb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="92dfb-145">displayName</span></span>|<span data-ttu-id="92dfb-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92dfb-146">String</span></span>|<span data-ttu-id="92dfb-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92dfb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92dfb-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92dfb-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92dfb-149">version</span><span class="sxs-lookup"><span data-stu-id="92dfb-149">version</span></span>|<span data-ttu-id="92dfb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="92dfb-150">Int32</span></span>|<span data-ttu-id="92dfb-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92dfb-151">Version of the device configuration.</span></span> <span data-ttu-id="92dfb-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92dfb-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92dfb-153">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="92dfb-153">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="92dfb-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-154">Boolean</span></span>|<span data-ttu-id="92dfb-155">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="92dfb-155">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="92dfb-156">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="92dfb-156">applyOnlyToWindows81</span></span>|<span data-ttu-id="92dfb-157">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-157">Boolean</span></span>|<span data-ttu-id="92dfb-158">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="92dfb-158">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="92dfb-159">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92dfb-159">This property is read-only.</span></span>|
|<span data-ttu-id="92dfb-160">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="92dfb-160">browserBlockAutofill</span></span>|<span data-ttu-id="92dfb-161">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-161">Boolean</span></span>|<span data-ttu-id="92dfb-162">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="92dfb-162">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="92dfb-163">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="92dfb-163">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="92dfb-164">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-164">Boolean</span></span>|<span data-ttu-id="92dfb-165">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="92dfb-165">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="92dfb-166">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="92dfb-166">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="92dfb-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-167">Boolean</span></span>|<span data-ttu-id="92dfb-168">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="92dfb-168">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="92dfb-169">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="92dfb-169">browserBlockJavaScript</span></span>|<span data-ttu-id="92dfb-170">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-170">Boolean</span></span>|<span data-ttu-id="92dfb-171">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="92dfb-171">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="92dfb-172">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="92dfb-172">browserBlockPlugins</span></span>|<span data-ttu-id="92dfb-173">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-173">Boolean</span></span>|<span data-ttu-id="92dfb-174">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="92dfb-174">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="92dfb-175">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="92dfb-175">browserBlockPopups</span></span>|<span data-ttu-id="92dfb-176">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-176">Boolean</span></span>|<span data-ttu-id="92dfb-177">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="92dfb-177">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="92dfb-178">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="92dfb-178">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="92dfb-179">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-179">Boolean</span></span>|<span data-ttu-id="92dfb-180">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="92dfb-180">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="92dfb-181">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="92dfb-181">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="92dfb-182">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-182">Boolean</span></span>|<span data-ttu-id="92dfb-183">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="92dfb-183">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="92dfb-184">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="92dfb-184">browserRequireSmartScreen</span></span>|<span data-ttu-id="92dfb-185">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-185">Boolean</span></span>|<span data-ttu-id="92dfb-186">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="92dfb-186">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="92dfb-187">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="92dfb-187">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="92dfb-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92dfb-188">String</span></span>|<span data-ttu-id="92dfb-189">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="92dfb-189">The enterprise mode site list location.</span></span> <span data-ttu-id="92dfb-190">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="92dfb-190">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="92dfb-191">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="92dfb-191">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="92dfb-192">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="92dfb-192">internetSiteSecurityLevel</span></span>](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|<span data-ttu-id="92dfb-193">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="92dfb-193">The internet security level.</span></span> <span data-ttu-id="92dfb-194">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="92dfb-194">The possible values are `userDefined`, `medium`, `mediumHigh`, `high`, , , , , , , , or .</span></span>|
|<span data-ttu-id="92dfb-195">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="92dfb-195">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="92dfb-196">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="92dfb-196">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="92dfb-197">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="92dfb-197">The Intranet security level.</span></span> <span data-ttu-id="92dfb-198">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="92dfb-198">The possible values are `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`, , , , , , or .</span></span>|
|<span data-ttu-id="92dfb-199">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="92dfb-199">browserLoggingReportLocation</span></span>|<span data-ttu-id="92dfb-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92dfb-200">String</span></span>|<span data-ttu-id="92dfb-201">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="92dfb-201">The logging report location.</span></span>|
|<span data-ttu-id="92dfb-202">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="92dfb-202">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="92dfb-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-203">Boolean</span></span>|<span data-ttu-id="92dfb-204">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="92dfb-204">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="92dfb-205">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="92dfb-205">browserRequireFirewall</span></span>|<span data-ttu-id="92dfb-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-206">Boolean</span></span>|<span data-ttu-id="92dfb-207">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="92dfb-207">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="92dfb-208">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="92dfb-208">browserRequireFraudWarning</span></span>|<span data-ttu-id="92dfb-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-209">Boolean</span></span>|<span data-ttu-id="92dfb-210">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="92dfb-210">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="92dfb-211">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="92dfb-211">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="92dfb-212">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="92dfb-212">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="92dfb-213">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="92dfb-213">The trusted sites security level.</span></span> <span data-ttu-id="92dfb-214">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="92dfb-214">The possible values are `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`, , , , , , or .</span></span>|
|<span data-ttu-id="92dfb-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="92dfb-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="92dfb-216">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-216">Boolean</span></span>|<span data-ttu-id="92dfb-217">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="92dfb-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="92dfb-218">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="92dfb-218">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="92dfb-219">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-219">Boolean</span></span>|<span data-ttu-id="92dfb-220">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="92dfb-220">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="92dfb-221">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="92dfb-221">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="92dfb-222">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-222">Boolean</span></span>|<span data-ttu-id="92dfb-223">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="92dfb-223">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="92dfb-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="92dfb-224">passwordExpirationDays</span></span>|<span data-ttu-id="92dfb-225">Int32</span><span class="sxs-lookup"><span data-stu-id="92dfb-225">Int32</span></span>|<span data-ttu-id="92dfb-226">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="92dfb-226">Password expiration in days.</span></span>|
|<span data-ttu-id="92dfb-227">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="92dfb-227">passwordMinimumLength</span></span>|<span data-ttu-id="92dfb-228">Int32</span><span class="sxs-lookup"><span data-stu-id="92dfb-228">Int32</span></span>|<span data-ttu-id="92dfb-229">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="92dfb-229">The minimum password length.</span></span>|
|<span data-ttu-id="92dfb-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="92dfb-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="92dfb-231">Int32</span><span class="sxs-lookup"><span data-stu-id="92dfb-231">Int32</span></span>|<span data-ttu-id="92dfb-232">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="92dfb-232">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="92dfb-233">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="92dfb-233">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="92dfb-234">Int32</span><span class="sxs-lookup"><span data-stu-id="92dfb-234">Int32</span></span>|<span data-ttu-id="92dfb-235">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="92dfb-235">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="92dfb-236">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="92dfb-236">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="92dfb-237">Int32</span><span class="sxs-lookup"><span data-stu-id="92dfb-237">Int32</span></span>|<span data-ttu-id="92dfb-238">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="92dfb-238">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="92dfb-239">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="92dfb-239">Valid values 0 to 24</span></span>|
|<span data-ttu-id="92dfb-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="92dfb-240">passwordRequiredType</span></span>|[<span data-ttu-id="92dfb-241">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="92dfb-241">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="92dfb-242">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="92dfb-242">The required password type.</span></span> <span data-ttu-id="92dfb-243">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="92dfb-243">The possible values are:</span></span>|
|<span data-ttu-id="92dfb-244">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="92dfb-244">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="92dfb-245">Int32</span><span class="sxs-lookup"><span data-stu-id="92dfb-245">Int32</span></span>|<span data-ttu-id="92dfb-246">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="92dfb-246">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="92dfb-247">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="92dfb-247">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="92dfb-248">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-248">Boolean</span></span>|<span data-ttu-id="92dfb-249">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="92dfb-249">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="92dfb-250">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="92dfb-250">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="92dfb-251">Booleano</span><span class="sxs-lookup"><span data-stu-id="92dfb-251">Boolean</span></span>|<span data-ttu-id="92dfb-252">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="92dfb-252">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="92dfb-253">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="92dfb-253">userAccountControlSettings</span></span>|[<span data-ttu-id="92dfb-254">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="92dfb-254">windowsUserAccountControlSettings</span></span>](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|<span data-ttu-id="92dfb-255">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="92dfb-255">The user account control settings.</span></span> <span data-ttu-id="92dfb-256">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="92dfb-256">The possible values are `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`, , , , , , , or .</span></span>|
|<span data-ttu-id="92dfb-257">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="92dfb-257">workFoldersUrl</span></span>|<span data-ttu-id="92dfb-258">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92dfb-258">String</span></span>|<span data-ttu-id="92dfb-259">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="92dfb-259">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="92dfb-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="92dfb-260">Response</span></span>
<span data-ttu-id="92dfb-261">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92dfb-261">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92dfb-262">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92dfb-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="92dfb-263">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92dfb-263">Request</span></span>
<span data-ttu-id="92dfb-264">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92dfb-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1757

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="92dfb-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="92dfb-265">Response</span></span>
<span data-ttu-id="92dfb-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92dfb-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```



