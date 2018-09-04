# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="1b814-101">Tipo de recurso windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="1b814-101">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="1b814-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b814-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b814-103">Política para proteção de informações do Windows para definir configurações de gerenciamento detalhadas</span><span class="sxs-lookup"><span data-stu-id="1b814-103">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="1b814-104">Herda de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1b814-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b814-105">Methods</span></span>
|<span data-ttu-id="1b814-106">Método</span><span class="sxs-lookup"><span data-stu-id="1b814-106">Method</span></span>|<span data-ttu-id="1b814-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b814-107">Return Type</span></span>|<span data-ttu-id="1b814-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b814-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b814-109">Listar windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="1b814-109">List windowsInformationProtections</span></span>](../api/intune_mam_windowsinformationprotection_list.md)|<span data-ttu-id="1b814-110">Coleção [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-110">[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="1b814-111">Listar propriedades e relações dos objetos [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="1b814-111">List properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="1b814-112">Obter windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="1b814-112">Get windowsInformationProtection</span></span>](../api/intune_mam_windowsinformationprotection_get.md)|[<span data-ttu-id="1b814-113">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="1b814-113">windowsInformationProtection</span></span>](../resources/intune_mam_windowsinformationprotection.md)|<span data-ttu-id="1b814-114">Ler propriedades e relações do objeto [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="1b814-114">Read properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="1b814-115">Ação assign</span><span class="sxs-lookup"><span data-stu-id="1b814-115">assign action</span></span>](../api/intune_mam_windowsinformationprotection_assign.md)|<span data-ttu-id="1b814-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b814-116">None</span></span>|<span data-ttu-id="1b814-117">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1b814-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1b814-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b814-118">Properties</span></span>
|<span data-ttu-id="1b814-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b814-119">Property</span></span>|<span data-ttu-id="1b814-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b814-120">Type</span></span>|<span data-ttu-id="1b814-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b814-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b814-122">displayName</span><span class="sxs-lookup"><span data-stu-id="1b814-122">displayName</span></span>|<span data-ttu-id="1b814-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b814-123">String</span></span>|<span data-ttu-id="1b814-124">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="1b814-124">Policy display name.</span></span> <span data-ttu-id="1b814-125">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-125">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b814-126">description</span><span class="sxs-lookup"><span data-stu-id="1b814-126">description</span></span>|<span data-ttu-id="1b814-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b814-127">String</span></span>|<span data-ttu-id="1b814-128">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="1b814-128">The policy's description.</span></span> <span data-ttu-id="1b814-129">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-129">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b814-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b814-130">createdDateTime</span></span>|<span data-ttu-id="1b814-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b814-131">DateTimeOffset</span></span>|<span data-ttu-id="1b814-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="1b814-132">The date and time the policy was created.</span></span> <span data-ttu-id="1b814-133">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-133">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b814-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b814-134">lastModifiedDateTime</span></span>|<span data-ttu-id="1b814-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b814-135">DateTimeOffset</span></span>|<span data-ttu-id="1b814-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="1b814-136">Last time the policy was modified.</span></span> <span data-ttu-id="1b814-137">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-137">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b814-138">id</span><span class="sxs-lookup"><span data-stu-id="1b814-138">id</span></span>|<span data-ttu-id="1b814-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b814-139">String</span></span>|<span data-ttu-id="1b814-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b814-140">Key of the entity.</span></span> <span data-ttu-id="1b814-141">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-141">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b814-142">version</span><span class="sxs-lookup"><span data-stu-id="1b814-142">version</span></span>|<span data-ttu-id="1b814-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b814-143">String</span></span>|<span data-ttu-id="1b814-144">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b814-144">Version of the entity.</span></span> <span data-ttu-id="1b814-145">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-145">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b814-146">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="1b814-146">enforcementLevel</span></span>|[<span data-ttu-id="1b814-147">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="1b814-147">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="1b814-148">Nível da imposição de WIP. Consulte a definição de Enum de valores suportados.</span><span class="sxs-lookup"><span data-stu-id="1b814-148">WIP enforcement level.See the Enum definition for supported values Possible values are: , , , .</span></span> <span data-ttu-id="1b814-149">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="1b814-149">The possible values are `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`, , , , , , , , or .</span></span>|
|<span data-ttu-id="1b814-150">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="1b814-150">enterpriseDomain</span></span>|<span data-ttu-id="1b814-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b814-151">String</span></span>|<span data-ttu-id="1b814-152">Domínio primário da empresa</span><span class="sxs-lookup"><span data-stu-id="1b814-152">Primary enterprise domain</span></span>|
|<span data-ttu-id="1b814-153">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="1b814-153">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="1b814-154">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-154">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1b814-155">Lista de domínios da empresa a serem protegidos</span><span class="sxs-lookup"><span data-stu-id="1b814-155">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="1b814-156">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="1b814-156">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="1b814-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b814-157">Boolean</span></span>|<span data-ttu-id="1b814-158">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada</span><span class="sxs-lookup"><span data-stu-id="1b814-158">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="1b814-159">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="1b814-159">dataRecoveryCertificate</span></span>|[<span data-ttu-id="1b814-160">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="1b814-160">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="1b814-161">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="1b814-161">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="1b814-162">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS)</span><span class="sxs-lookup"><span data-stu-id="1b814-162">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="1b814-163">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="1b814-163">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="1b814-164">Booleano</span><span class="sxs-lookup"><span data-stu-id="1b814-164">Boolean</span></span>|<span data-ttu-id="1b814-165">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1b814-165">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="1b814-166">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="1b814-166">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="1b814-167">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="1b814-167">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="1b814-168">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="1b814-168">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="1b814-169">Guid</span><span class="sxs-lookup"><span data-stu-id="1b814-169">Guid</span></span>|<span data-ttu-id="1b814-170">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="1b814-170">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="1b814-171">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso</span><span class="sxs-lookup"><span data-stu-id="1b814-171">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="1b814-172">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="1b814-172">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="1b814-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b814-173">Boolean</span></span>|<span data-ttu-id="1b814-174">Especifica se a criptografia do Azure RMS para WIP será permitida</span><span class="sxs-lookup"><span data-stu-id="1b814-174">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="1b814-175">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="1b814-175">iconsVisible</span></span>|<span data-ttu-id="1b814-176">Booleano</span><span class="sxs-lookup"><span data-stu-id="1b814-176">Boolean</span></span>|<span data-ttu-id="1b814-177">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="1b814-177">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="1b814-178">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP</span><span class="sxs-lookup"><span data-stu-id="1b814-178">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="1b814-179">protectedApps</span><span class="sxs-lookup"><span data-stu-id="1b814-179">protectedApps</span></span>|<span data-ttu-id="1b814-180">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-180">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="1b814-181">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia</span><span class="sxs-lookup"><span data-stu-id="1b814-181">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="1b814-182">exemptApps</span><span class="sxs-lookup"><span data-stu-id="1b814-182">exemptApps</span></span>|<span data-ttu-id="1b814-183">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-183">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="1b814-184">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="1b814-184">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="1b814-185">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="1b814-185">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="1b814-186">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="1b814-186">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="1b814-187">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-187">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1b814-188">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b814-188">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="1b814-189">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="1b814-189">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="1b814-190">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="1b814-190">enterpriseProxiedDomains</span></span>|<span data-ttu-id="1b814-191">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-191">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="1b814-192">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="1b814-192">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="1b814-193">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="1b814-193">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="1b814-194">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="1b814-194">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="1b814-195">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="1b814-195">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="1b814-196">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="1b814-196">enterpriseIPRanges</span></span>|<span data-ttu-id="1b814-197">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-197">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="1b814-198">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="1b814-198">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="1b814-199">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="1b814-199">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="1b814-200">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="1b814-200">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="1b814-201">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="1b814-201">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="1b814-202">Booleano</span><span class="sxs-lookup"><span data-stu-id="1b814-202">Boolean</span></span>|<span data-ttu-id="1b814-203">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="1b814-203">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="1b814-204">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="1b814-204">Default is false</span></span>|
|<span data-ttu-id="1b814-205">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="1b814-205">enterpriseProxyServers</span></span>|<span data-ttu-id="1b814-206">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-206">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1b814-207">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="1b814-207">This is a list of proxy servers.</span></span> <span data-ttu-id="1b814-208">Qualquer servidor que não esteja na lista é considerado não corporativo</span><span class="sxs-lookup"><span data-stu-id="1b814-208">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="1b814-209">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="1b814-209">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="1b814-210">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-210">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1b814-211">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="1b814-211">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="1b814-212">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="1b814-212">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="1b814-213">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="1b814-213">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="1b814-214">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b814-214">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="1b814-215">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies</span><span class="sxs-lookup"><span data-stu-id="1b814-215">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="1b814-216">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="1b814-216">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="1b814-217">Booleano</span><span class="sxs-lookup"><span data-stu-id="1b814-217">Boolean</span></span>|<span data-ttu-id="1b814-218">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1b814-218">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="1b814-219">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="1b814-219">Default is false</span></span>|
|<span data-ttu-id="1b814-220">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="1b814-220">neutralDomainResources</span></span>|<span data-ttu-id="1b814-221">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-221">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1b814-222">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal</span><span class="sxs-lookup"><span data-stu-id="1b814-222">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="1b814-223">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="1b814-223">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="1b814-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b814-224">Boolean</span></span>|<span data-ttu-id="1b814-225">Esta opção é para o indexador do Windows Search, para permitir ou não a indexação de itens</span><span class="sxs-lookup"><span data-stu-id="1b814-225">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="1b814-226">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="1b814-226">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="1b814-227">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-227">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="1b814-228">Especifica uma lista de extensões de arquivo, para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo</span><span class="sxs-lookup"><span data-stu-id="1b814-228">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="1b814-229">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1b814-229">isAssigned</span></span>|<span data-ttu-id="1b814-230">Booleano</span><span class="sxs-lookup"><span data-stu-id="1b814-230">Boolean</span></span>|<span data-ttu-id="1b814-231">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="1b814-231">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b814-232">Relações</span><span class="sxs-lookup"><span data-stu-id="1b814-232">Relationships</span></span>
|<span data-ttu-id="1b814-233">Relação</span><span class="sxs-lookup"><span data-stu-id="1b814-233">Relationship</span></span>|<span data-ttu-id="1b814-234">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b814-234">Type</span></span>|<span data-ttu-id="1b814-235">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b814-235">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b814-236">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="1b814-236">protectedAppLockerFiles</span></span>|<span data-ttu-id="1b814-237">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-237">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="1b814-238">Outra maneira de inserir aplicativos protegidos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="1b814-238">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="1b814-239">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="1b814-239">exemptAppLockerFiles</span></span>|<span data-ttu-id="1b814-240">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-240">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="1b814-241">Outra maneira de inserir aplicativos isentos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="1b814-241">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="1b814-242">assignments</span><span class="sxs-lookup"><span data-stu-id="1b814-242">assignments</span></span>|<span data-ttu-id="1b814-243">Coleção [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1b814-243">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="1b814-244">Propriedade de navegação para lista de grupos de segurança direcionados para política.</span><span class="sxs-lookup"><span data-stu-id="1b814-244">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b814-245">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b814-245">JSON Representation</span></span>
<span data-ttu-id="1b814-246">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b814-246">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppPolicy",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}-->
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
  "rightsManagementServicesTemplateId": "79199ed9-e50b-4257-8de4-70b9c8685061",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
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



