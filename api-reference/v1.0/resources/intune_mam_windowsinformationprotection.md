# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="4e402-101">Tipo de recurso windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="4e402-101">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="4e402-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4e402-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e402-103">Política para proteção de informações do Windows para definir configurações de gerenciamento detalhadas</span><span class="sxs-lookup"><span data-stu-id="4e402-103">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="4e402-104">Herda de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4e402-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4e402-105">Methods</span></span>
|<span data-ttu-id="4e402-106">Método</span><span class="sxs-lookup"><span data-stu-id="4e402-106">Method</span></span>|<span data-ttu-id="4e402-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4e402-107">Return Type</span></span>|<span data-ttu-id="4e402-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e402-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4e402-109">Listar windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="4e402-109">List windowsInformationProtections</span></span>](../api/intune_mam_windowsinformationprotection_list.md)|<span data-ttu-id="4e402-110">Coleção [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="4e402-111">Listar propriedades e relações dos objetos [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4e402-111">List properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="4e402-112">Obter windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="4e402-112">Get windowsInformationProtection</span></span>](../api/intune_mam_windowsinformationprotection_get.md)|[<span data-ttu-id="4e402-113">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="4e402-113">windowsInformationProtection</span></span>](../resources/intune_mam_windowsinformationprotection.md)|<span data-ttu-id="4e402-114">Ler propriedades e relações do objeto [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4e402-114">Read properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="4e402-115">Ação assign</span><span class="sxs-lookup"><span data-stu-id="4e402-115">assign action</span></span>](../api/intune_mam_windowsinformationprotection_assign.md)|<span data-ttu-id="4e402-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e402-116">None</span></span>|<span data-ttu-id="4e402-117">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e402-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4e402-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e402-118">Properties</span></span>
|<span data-ttu-id="4e402-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e402-119">Property</span></span>|<span data-ttu-id="4e402-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e402-120">Type</span></span>|<span data-ttu-id="4e402-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e402-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e402-122">displayName</span><span class="sxs-lookup"><span data-stu-id="4e402-122">displayName</span></span>|<span data-ttu-id="4e402-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e402-123">String</span></span>|<span data-ttu-id="4e402-124">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="4e402-124">Policy display name.</span></span> <span data-ttu-id="4e402-125">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-125">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4e402-126">description</span><span class="sxs-lookup"><span data-stu-id="4e402-126">description</span></span>|<span data-ttu-id="4e402-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e402-127">String</span></span>|<span data-ttu-id="4e402-128">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="4e402-128">The policy's description.</span></span> <span data-ttu-id="4e402-129">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-129">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4e402-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e402-130">createdDateTime</span></span>|<span data-ttu-id="4e402-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e402-131">DateTimeOffset</span></span>|<span data-ttu-id="4e402-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="4e402-132">The date and time the policy was created.</span></span> <span data-ttu-id="4e402-133">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-133">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4e402-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e402-134">lastModifiedDateTime</span></span>|<span data-ttu-id="4e402-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e402-135">DateTimeOffset</span></span>|<span data-ttu-id="4e402-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="4e402-136">Last time the policy was modified.</span></span> <span data-ttu-id="4e402-137">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-137">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4e402-138">id</span><span class="sxs-lookup"><span data-stu-id="4e402-138">id</span></span>|<span data-ttu-id="4e402-139">String</span><span class="sxs-lookup"><span data-stu-id="4e402-139">String</span></span>|<span data-ttu-id="4e402-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e402-140">Key of the entity.</span></span> <span data-ttu-id="4e402-141">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-141">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4e402-142">version</span><span class="sxs-lookup"><span data-stu-id="4e402-142">version</span></span>|<span data-ttu-id="4e402-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e402-143">String</span></span>|<span data-ttu-id="4e402-144">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e402-144">Version of the entity.</span></span> <span data-ttu-id="4e402-145">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-145">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="4e402-146">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="4e402-146">enforcementLevel</span></span>|<span data-ttu-id="4e402-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e402-147">String</span></span>|<span data-ttu-id="4e402-148">Nível de imposição WIP. Confira a definição de enumeração para valores compatíveis Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="4e402-148">WIP enforcement level.See the Enum definition for supported values Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="4e402-149">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="4e402-149">enterpriseDomain</span></span>|<span data-ttu-id="4e402-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e402-150">String</span></span>|<span data-ttu-id="4e402-151">Domínio primário da empresa</span><span class="sxs-lookup"><span data-stu-id="4e402-151">Primary enterprise domain</span></span>|
|<span data-ttu-id="4e402-152">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="4e402-152">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="4e402-153">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-153">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4e402-154">Lista de domínios da empresa a serem protegidos</span><span class="sxs-lookup"><span data-stu-id="4e402-154">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="4e402-155">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="4e402-155">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="4e402-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e402-156">Boolean</span></span>|<span data-ttu-id="4e402-157">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada</span><span class="sxs-lookup"><span data-stu-id="4e402-157">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="4e402-158">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4e402-158">dataRecoveryCertificate</span></span>|[<span data-ttu-id="4e402-159">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4e402-159">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="4e402-160">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="4e402-160">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="4e402-161">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS)</span><span class="sxs-lookup"><span data-stu-id="4e402-161">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="4e402-162">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="4e402-162">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="4e402-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e402-163">Boolean</span></span>|<span data-ttu-id="4e402-164">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4e402-164">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="4e402-165">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="4e402-165">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="4e402-166">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="4e402-166">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="4e402-167">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="4e402-167">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="4e402-168">Guid</span><span class="sxs-lookup"><span data-stu-id="4e402-168">Guid</span></span>|<span data-ttu-id="4e402-169">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="4e402-169">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="4e402-170">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso</span><span class="sxs-lookup"><span data-stu-id="4e402-170">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="4e402-171">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="4e402-171">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="4e402-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e402-172">Boolean</span></span>|<span data-ttu-id="4e402-173">Especifica se a criptografia do Azure RMS para WIP será permitida</span><span class="sxs-lookup"><span data-stu-id="4e402-173">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="4e402-174">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="4e402-174">iconsVisible</span></span>|<span data-ttu-id="4e402-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e402-175">Boolean</span></span>|<span data-ttu-id="4e402-176">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="4e402-176">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="4e402-177">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP</span><span class="sxs-lookup"><span data-stu-id="4e402-177">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="4e402-178">protectedApps</span><span class="sxs-lookup"><span data-stu-id="4e402-178">protectedApps</span></span>|<span data-ttu-id="4e402-179">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-179">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="4e402-180">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia</span><span class="sxs-lookup"><span data-stu-id="4e402-180">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="4e402-181">exemptApps</span><span class="sxs-lookup"><span data-stu-id="4e402-181">exemptApps</span></span>|<span data-ttu-id="4e402-182">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-182">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="4e402-183">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="4e402-183">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="4e402-184">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="4e402-184">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="4e402-185">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="4e402-185">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="4e402-186">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-186">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4e402-187">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="4e402-187">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="4e402-188">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="4e402-188">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="4e402-189">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="4e402-189">enterpriseProxiedDomains</span></span>|<span data-ttu-id="4e402-190">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-190">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="4e402-191">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="4e402-191">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="4e402-192">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="4e402-192">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="4e402-193">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="4e402-193">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="4e402-194">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="4e402-194">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="4e402-195">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="4e402-195">enterpriseIPRanges</span></span>|<span data-ttu-id="4e402-196">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-196">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="4e402-197">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="4e402-197">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="4e402-198">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="4e402-198">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="4e402-199">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="4e402-199">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="4e402-200">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="4e402-200">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="4e402-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e402-201">Boolean</span></span>|<span data-ttu-id="4e402-202">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="4e402-202">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="4e402-203">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="4e402-203">Default is false</span></span>|
|<span data-ttu-id="4e402-204">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="4e402-204">enterpriseProxyServers</span></span>|<span data-ttu-id="4e402-205">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-205">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4e402-206">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="4e402-206">This is a list of proxy servers.</span></span> <span data-ttu-id="4e402-207">Qualquer servidor que não esteja na lista é considerado não corporativo</span><span class="sxs-lookup"><span data-stu-id="4e402-207">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="4e402-208">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="4e402-208">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="4e402-209">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-209">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4e402-210">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="4e402-210">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="4e402-211">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="4e402-211">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="4e402-212">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="4e402-212">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="4e402-213">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="4e402-213">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="4e402-214">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies</span><span class="sxs-lookup"><span data-stu-id="4e402-214">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="4e402-215">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="4e402-215">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="4e402-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e402-216">Boolean</span></span>|<span data-ttu-id="4e402-217">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4e402-217">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="4e402-218">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="4e402-218">Default is false</span></span>|
|<span data-ttu-id="4e402-219">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="4e402-219">neutralDomainResources</span></span>|<span data-ttu-id="4e402-220">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-220">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4e402-221">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal</span><span class="sxs-lookup"><span data-stu-id="4e402-221">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="4e402-222">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="4e402-222">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="4e402-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e402-223">Boolean</span></span>|<span data-ttu-id="4e402-224">Esta opção é para o indexador do Windows Search, para permitir ou não a indexação de itens</span><span class="sxs-lookup"><span data-stu-id="4e402-224">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="4e402-225">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="4e402-225">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="4e402-226">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-226">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="4e402-227">Especifica uma lista de extensões de arquivo, para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo</span><span class="sxs-lookup"><span data-stu-id="4e402-227">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="4e402-228">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4e402-228">isAssigned</span></span>|<span data-ttu-id="4e402-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e402-229">Boolean</span></span>|<span data-ttu-id="4e402-230">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="4e402-230">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e402-231">Relações</span><span class="sxs-lookup"><span data-stu-id="4e402-231">Relationships</span></span>
|<span data-ttu-id="4e402-232">Relação</span><span class="sxs-lookup"><span data-stu-id="4e402-232">Relationship</span></span>|<span data-ttu-id="4e402-233">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e402-233">Type</span></span>|<span data-ttu-id="4e402-234">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e402-234">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e402-235">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="4e402-235">protectedAppLockerFiles</span></span>|<span data-ttu-id="4e402-236">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-236">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="4e402-237">Outra maneira de inserir aplicativos protegidos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="4e402-237">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="4e402-238">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="4e402-238">exemptAppLockerFiles</span></span>|<span data-ttu-id="4e402-239">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="4e402-239">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="4e402-240">Outra maneira de inserir aplicativos isentos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="4e402-240">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="4e402-241">assignments</span><span class="sxs-lookup"><span data-stu-id="4e402-241">assignments</span></span>|<span data-ttu-id="4e402-242">Coleção targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4e402-242">targetedManagedAppPolicyAssignment collection</span></span>|<span data-ttu-id="4e402-243">Propriedade de navegação para lista de grupos de segurança direcionados para política.</span><span class="sxs-lookup"><span data-stu-id="4e402-243">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e402-244">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e402-244">JSON Representation</span></span>
<span data-ttu-id="4e402-245">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e402-245">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```



