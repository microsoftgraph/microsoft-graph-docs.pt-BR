# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="35954-101">Criar mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="35954-101">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="35954-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="35954-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35954-103">Cria um novo objeto [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="35954-103">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35954-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35954-104">Prerequisites</span></span>
<span data-ttu-id="35954-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="35954-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="35954-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35954-107">Permission type</span></span>|<span data-ttu-id="35954-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35954-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35954-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35954-109">Delegated (work or school account)</span></span>|<span data-ttu-id="35954-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35954-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="35954-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35954-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35954-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35954-112">Not supported.</span></span>|
|<span data-ttu-id="35954-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35954-113">Application</span></span>|<span data-ttu-id="35954-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35954-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35954-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35954-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="35954-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35954-116">Request headers</span></span>
|<span data-ttu-id="35954-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35954-117">Header</span></span>|<span data-ttu-id="35954-118">Valor</span><span class="sxs-lookup"><span data-stu-id="35954-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35954-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="35954-119">Authorization</span></span>|<span data-ttu-id="35954-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35954-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35954-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35954-121">Accept</span></span>|<span data-ttu-id="35954-122">application/json</span><span class="sxs-lookup"><span data-stu-id="35954-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35954-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35954-123">Request body</span></span>
<span data-ttu-id="35954-124">No corpo da solicitação, forneça uma representação JSON do objeto mdmWindowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="35954-124">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="35954-125">A tabela a seguir mostra as propriedades que são necessárias ao criar mdmWindowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="35954-125">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="35954-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35954-126">Property</span></span>|<span data-ttu-id="35954-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="35954-127">Type</span></span>|<span data-ttu-id="35954-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="35954-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35954-129">displayName</span><span class="sxs-lookup"><span data-stu-id="35954-129">displayName</span></span>|<span data-ttu-id="35954-130">String</span><span class="sxs-lookup"><span data-stu-id="35954-130">String</span></span>|<span data-ttu-id="35954-131">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="35954-131">Policy display name.</span></span> <span data-ttu-id="35954-132">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35954-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="35954-133">descrição</span><span class="sxs-lookup"><span data-stu-id="35954-133">description</span></span>|<span data-ttu-id="35954-134">String</span><span class="sxs-lookup"><span data-stu-id="35954-134">String</span></span>|<span data-ttu-id="35954-135">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="35954-135">The policy's description.</span></span> <span data-ttu-id="35954-136">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35954-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="35954-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35954-137">createdDateTime</span></span>|<span data-ttu-id="35954-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35954-138">DateTimeOffset</span></span>|<span data-ttu-id="35954-139">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="35954-139">The date and time the policy was created.</span></span> <span data-ttu-id="35954-140">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35954-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="35954-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35954-141">lastModifiedDateTime</span></span>|<span data-ttu-id="35954-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35954-142">DateTimeOffset</span></span>|<span data-ttu-id="35954-143">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="35954-143">Last time the policy was modified.</span></span> <span data-ttu-id="35954-144">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35954-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="35954-145">id</span><span class="sxs-lookup"><span data-stu-id="35954-145">id</span></span>|<span data-ttu-id="35954-146">String</span><span class="sxs-lookup"><span data-stu-id="35954-146">String</span></span>|<span data-ttu-id="35954-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="35954-147">Key of the entity.</span></span> <span data-ttu-id="35954-148">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35954-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="35954-149">version</span><span class="sxs-lookup"><span data-stu-id="35954-149">version</span></span>|<span data-ttu-id="35954-150">String</span><span class="sxs-lookup"><span data-stu-id="35954-150">String</span></span>|<span data-ttu-id="35954-151">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="35954-151">Version of the entity.</span></span> <span data-ttu-id="35954-152">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35954-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="35954-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="35954-153">enforcementLevel</span></span>|[<span data-ttu-id="35954-154">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="35954-154">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="35954-155">Nível da imposição de WIP. Consulte a definição de Enum de valores suportados Inherited de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="35954-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span></span> <span data-ttu-id="35954-156">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="35954-156">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="35954-157">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="35954-157">enterpriseDomain</span></span>|<span data-ttu-id="35954-158">String</span><span class="sxs-lookup"><span data-stu-id="35954-158">String</span></span>|<span data-ttu-id="35954-159">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-159">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-160">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="35954-160">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="35954-161">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-161">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="35954-162">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-162">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-163">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="35954-163">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="35954-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="35954-164">Boolean</span></span>|<span data-ttu-id="35954-165">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-165">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-166">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="35954-166">dataRecoveryCertificate</span></span>|[<span data-ttu-id="35954-167">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="35954-167">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="35954-168">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="35954-168">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="35954-169">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-169">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-170">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="35954-170">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="35954-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="35954-171">Boolean</span></span>|<span data-ttu-id="35954-172">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="35954-172">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="35954-173">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="35954-173">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="35954-174">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="35954-174">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="35954-175">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-175">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-176">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="35954-176">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="35954-177">Guid</span><span class="sxs-lookup"><span data-stu-id="35954-177">Guid</span></span>|<span data-ttu-id="35954-178">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="35954-178">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="35954-179">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-179">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-180">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="35954-180">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="35954-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="35954-181">Boolean</span></span>|<span data-ttu-id="35954-182">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-182">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-183">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="35954-183">iconsVisible</span></span>|<span data-ttu-id="35954-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="35954-184">Boolean</span></span>|<span data-ttu-id="35954-185">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="35954-185">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="35954-186">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-186">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-187">protectedApps</span><span class="sxs-lookup"><span data-stu-id="35954-187">protectedApps</span></span>|<span data-ttu-id="35954-188">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="35954-188">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="35954-189">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-189">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-190">exemptApps</span><span class="sxs-lookup"><span data-stu-id="35954-190">exemptApps</span></span>|<span data-ttu-id="35954-191">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="35954-191">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="35954-192">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="35954-192">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="35954-193">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="35954-193">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="35954-194">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-194">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-195">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="35954-195">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="35954-196">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-196">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="35954-197">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="35954-197">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="35954-198">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-198">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-199">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="35954-199">enterpriseProxiedDomains</span></span>|<span data-ttu-id="35954-200">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-200">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="35954-201">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="35954-201">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="35954-202">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="35954-202">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="35954-203">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="35954-203">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="35954-204">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-204">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-205">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="35954-205">enterpriseIPRanges</span></span>|<span data-ttu-id="35954-206">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-206">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="35954-207">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="35954-207">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="35954-208">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="35954-208">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="35954-209">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-209">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-210">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="35954-210">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="35954-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="35954-211">Boolean</span></span>|<span data-ttu-id="35954-212">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="35954-212">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="35954-213">A padrão é false Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-213">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-214">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="35954-214">enterpriseProxyServers</span></span>|<span data-ttu-id="35954-215">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-215">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="35954-216">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="35954-216">This is a list of proxy servers.</span></span> <span data-ttu-id="35954-217">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-217">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-218">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="35954-218">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="35954-219">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-219">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="35954-220">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="35954-220">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="35954-221">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="35954-221">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="35954-222">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="35954-222">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="35954-223">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="35954-223">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="35954-224">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-224">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-225">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="35954-225">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="35954-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="35954-226">Boolean</span></span>|<span data-ttu-id="35954-227">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="35954-227">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="35954-228">A padrão é false Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-228">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-229">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="35954-229">neutralDomainResources</span></span>|<span data-ttu-id="35954-230">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-230">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="35954-231">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-231">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-232">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="35954-232">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="35954-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="35954-233">Boolean</span></span>|<span data-ttu-id="35954-234">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-234">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-235">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="35954-235">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="35954-236">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-236">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="35954-237">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-237">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="35954-238">isAssigned</span><span class="sxs-lookup"><span data-stu-id="35954-238">isAssigned</span></span>|<span data-ttu-id="35954-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="35954-239">Boolean</span></span>|<span data-ttu-id="35954-240">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="35954-240">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="35954-241">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="35954-241">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="35954-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="35954-242">Response</span></span>
<span data-ttu-id="35954-243">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35954-243">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35954-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35954-244">Example</span></span>
### <a name="request"></a><span data-ttu-id="35954-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35954-245">Request</span></span>
<span data-ttu-id="35954-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35954-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3905

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="35954-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="35954-247">Response</span></span>
<span data-ttu-id="35954-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35954-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4077

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
  "version": "Version value",
  "enforcementLevel": "encryptAndAuditOnly",
  "enterpriseDomain": "Enterprise Domain value",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "Subject Name value",
    "description": "Description value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "certificate": "Y2VydGlmaWNhdGU="
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisherName": "Publisher Name value",
      "productName": "Product Name value",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "Display Name value",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "Ip Address Or FQDN value",
          "proxy": "Proxy value"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "Display Name value",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "Display Name value",
      "resources": [
        "Resources value"
      ]
    }
  ],
  "isAssigned": true
}
```



