# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="771ab-101">Criar windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="771ab-101">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="771ab-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="771ab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="771ab-103">Cria um novo objeto [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="771ab-103">Create a new [plannerBucket](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="771ab-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="771ab-104">Prerequisites</span></span>
<span data-ttu-id="771ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="771ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="771ab-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="771ab-107">Permission type</span></span>|<span data-ttu-id="771ab-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="771ab-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="771ab-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="771ab-109">Delegated (work or school account)</span></span>|<span data-ttu-id="771ab-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771ab-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="771ab-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="771ab-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="771ab-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="771ab-112">Not supported.</span></span>|
|<span data-ttu-id="771ab-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="771ab-113">Application</span></span>|<span data-ttu-id="771ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="771ab-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="771ab-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="771ab-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="771ab-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="771ab-116">Request headers</span></span>
|<span data-ttu-id="771ab-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="771ab-117">Header</span></span>|<span data-ttu-id="771ab-118">Valor</span><span class="sxs-lookup"><span data-stu-id="771ab-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="771ab-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="771ab-119">Authorization</span></span>|<span data-ttu-id="771ab-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="771ab-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="771ab-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="771ab-121">Accept</span></span>|<span data-ttu-id="771ab-122">application/json</span><span class="sxs-lookup"><span data-stu-id="771ab-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="771ab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="771ab-123">Request body</span></span>
<span data-ttu-id="771ab-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="771ab-124">In the request body, supply a JSON representation of calendar object.</span></span>

<span data-ttu-id="771ab-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="771ab-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="771ab-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="771ab-126">Property</span></span>|<span data-ttu-id="771ab-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="771ab-127">Type</span></span>|<span data-ttu-id="771ab-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="771ab-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="771ab-129">displayName</span><span class="sxs-lookup"><span data-stu-id="771ab-129">displayName</span></span>|<span data-ttu-id="771ab-130">String</span><span class="sxs-lookup"><span data-stu-id="771ab-130">String</span></span>|<span data-ttu-id="771ab-131">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="771ab-131">Policy display name.</span></span> <span data-ttu-id="771ab-132">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="771ab-133">descrição</span><span class="sxs-lookup"><span data-stu-id="771ab-133">description</span></span>|<span data-ttu-id="771ab-134">String</span><span class="sxs-lookup"><span data-stu-id="771ab-134">String</span></span>|<span data-ttu-id="771ab-135">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="771ab-135">The policy's description.</span></span> <span data-ttu-id="771ab-136">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="771ab-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="771ab-137">createdDateTime</span></span>|<span data-ttu-id="771ab-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="771ab-138">DateTimeOffset</span></span>|<span data-ttu-id="771ab-139">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="771ab-139">The date and time the group was created.</span></span> <span data-ttu-id="771ab-140">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="771ab-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="771ab-141">lastModifiedDateTime</span></span>|<span data-ttu-id="771ab-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="771ab-142">DateTimeOffset</span></span>|<span data-ttu-id="771ab-143">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="771ab-143">Last time the policy was modified.</span></span> <span data-ttu-id="771ab-144">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="771ab-145">id</span><span class="sxs-lookup"><span data-stu-id="771ab-145">id</span></span>|<span data-ttu-id="771ab-146">String</span><span class="sxs-lookup"><span data-stu-id="771ab-146">String</span></span>|<span data-ttu-id="771ab-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="771ab-147">Key of the setting.</span></span> <span data-ttu-id="771ab-148">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="771ab-149">version</span><span class="sxs-lookup"><span data-stu-id="771ab-149">version</span></span>|<span data-ttu-id="771ab-150">String</span><span class="sxs-lookup"><span data-stu-id="771ab-150">String</span></span>|<span data-ttu-id="771ab-151">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="771ab-151">Version of the entity.</span></span> <span data-ttu-id="771ab-152">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="771ab-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="771ab-153">enforcementLevel</span></span>|<span data-ttu-id="771ab-154">String</span><span class="sxs-lookup"><span data-stu-id="771ab-154">String</span></span>|<span data-ttu-id="771ab-155">Nível de imposição WIP. Confira a definição de enumeração para valores compatíveis Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="771ab-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="771ab-156">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="771ab-156">enterpriseDomain</span></span>|<span data-ttu-id="771ab-157">String</span><span class="sxs-lookup"><span data-stu-id="771ab-157">String</span></span>|<span data-ttu-id="771ab-158">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-158">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-159">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="771ab-159">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="771ab-160">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-160">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="771ab-161">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-161">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-162">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="771ab-162">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="771ab-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-163">Boolean</span></span>|<span data-ttu-id="771ab-164">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-164">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-165">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="771ab-165">dataRecoveryCertificate</span></span>|[<span data-ttu-id="771ab-166">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="771ab-166">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="771ab-167">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="771ab-167">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="771ab-168">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-168">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-169">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="771ab-169">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="771ab-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-170">Boolean</span></span>|<span data-ttu-id="771ab-171">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="771ab-171">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="771ab-172">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="771ab-172">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="771ab-173">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="771ab-173">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="771ab-174">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-174">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="771ab-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="771ab-176">Guid</span><span class="sxs-lookup"><span data-stu-id="771ab-176">Guid</span></span>|<span data-ttu-id="771ab-177">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="771ab-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="771ab-178">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="771ab-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="771ab-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-180">Boolean</span></span>|<span data-ttu-id="771ab-181">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-181">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="771ab-182">iconsVisible</span></span>|<span data-ttu-id="771ab-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-183">Boolean</span></span>|<span data-ttu-id="771ab-184">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="771ab-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="771ab-185">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="771ab-186">protectedApps</span></span>|<span data-ttu-id="771ab-187">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-187">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="771ab-188">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="771ab-189">exemptApps</span></span>|<span data-ttu-id="771ab-190">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-190">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="771ab-191">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="771ab-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="771ab-192">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="771ab-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="771ab-193">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-193">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="771ab-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="771ab-195">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-195">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="771ab-196">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="771ab-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="771ab-197">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="771ab-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="771ab-199">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="771ab-200">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="771ab-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="771ab-201">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="771ab-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="771ab-202">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="771ab-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="771ab-203">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="771ab-204">enterpriseIPRanges</span></span>|<span data-ttu-id="771ab-205">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="771ab-206">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="771ab-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="771ab-207">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="771ab-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="771ab-208">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-208">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="771ab-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="771ab-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-210">Boolean</span></span>|<span data-ttu-id="771ab-211">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="771ab-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="771ab-212">A padrão é false Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-212">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="771ab-213">enterpriseProxyServers</span></span>|<span data-ttu-id="771ab-214">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-214">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="771ab-215">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="771ab-215">This is a list of proxy servers.</span></span> <span data-ttu-id="771ab-216">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-216">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="771ab-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="771ab-218">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-218">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="771ab-219">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="771ab-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="771ab-220">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="771ab-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="771ab-221">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="771ab-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="771ab-222">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="771ab-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="771ab-223">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="771ab-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="771ab-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-225">Boolean</span></span>|<span data-ttu-id="771ab-226">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="771ab-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="771ab-227">A padrão é false Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-227">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="771ab-228">neutralDomainResources</span></span>|<span data-ttu-id="771ab-229">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-229">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="771ab-230">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-230">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="771ab-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="771ab-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-232">Boolean</span></span>|<span data-ttu-id="771ab-233">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="771ab-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="771ab-235">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-235">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="771ab-236">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="771ab-237">isAssigned</span></span>|<span data-ttu-id="771ab-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-238">Boolean</span></span>|<span data-ttu-id="771ab-239">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="771ab-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="771ab-240">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="771ab-240">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="771ab-241">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="771ab-241">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="771ab-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-242">Boolean</span></span>|<span data-ttu-id="771ab-243">Nova propriedade em RS2, documentação pendente</span><span class="sxs-lookup"><span data-stu-id="771ab-243">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="771ab-244">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="771ab-244">mdmEnrollmentUrl</span></span>|<span data-ttu-id="771ab-245">String</span><span class="sxs-lookup"><span data-stu-id="771ab-245">String</span></span>|<span data-ttu-id="771ab-246">Url do registro do MDM</span><span class="sxs-lookup"><span data-stu-id="771ab-246">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="771ab-247">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="771ab-247">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="771ab-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="771ab-248">Boolean</span></span>|<span data-ttu-id="771ab-249">Valor booliano que define o Windows Hello para Empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="771ab-249">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="771ab-250">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="771ab-250">pinMinimumLength</span></span>|<span data-ttu-id="771ab-251">Int32</span><span class="sxs-lookup"><span data-stu-id="771ab-251">Int32</span></span>|<span data-ttu-id="771ab-252">Valor inteiro que define o número mínimo de caracteres necessários para o PIN.</span><span class="sxs-lookup"><span data-stu-id="771ab-252">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="771ab-253">O valor padrão é 4.</span><span class="sxs-lookup"><span data-stu-id="771ab-253">Default value is 4.</span></span> <span data-ttu-id="771ab-254">O menor número que é possível definir para essa configuração de política é 4.</span><span class="sxs-lookup"><span data-stu-id="771ab-254">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="771ab-255">O maior número que é possível definir deve ser menor que o número configurado na política de comprimento máximo do PIN ou menor que 127, seja qual for o menor.</span><span class="sxs-lookup"><span data-stu-id="771ab-255">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="771ab-256">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="771ab-256">pinUppercaseLetters</span></span>|<span data-ttu-id="771ab-257">String</span><span class="sxs-lookup"><span data-stu-id="771ab-257">String</span></span>|<span data-ttu-id="771ab-258">Valor inteiro que configura o uso de letras maiúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="771ab-258">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="771ab-259">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="771ab-259">Default is NotAllow.</span></span> <span data-ttu-id="771ab-260">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="771ab-260">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="771ab-261">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="771ab-261">pinLowercaseLetters</span></span>|<span data-ttu-id="771ab-262">String</span><span class="sxs-lookup"><span data-stu-id="771ab-262">String</span></span>|<span data-ttu-id="771ab-263">Valor inteiro que configura o uso de letras minúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="771ab-263">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="771ab-264">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="771ab-264">Default is NotAllow.</span></span> <span data-ttu-id="771ab-265">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="771ab-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="771ab-266">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="771ab-266">pinSpecialCharacters</span></span>|<span data-ttu-id="771ab-267">String</span><span class="sxs-lookup"><span data-stu-id="771ab-267">String</span></span>|<span data-ttu-id="771ab-268">Valor inteiro que configura o uso de caracteres especiais no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="771ab-268">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="771ab-269">Os caracteres especiais válidos para o PIN do Windows Hello para Empresas incluem: !</span><span class="sxs-lookup"><span data-stu-id="771ab-269">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="771ab-270">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="771ab-270">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="771ab-271">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="771ab-271">/ : ; < = > ?</span></span><span data-ttu-id="771ab-272"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="771ab-272"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="771ab-273">} ~.</span><span class="sxs-lookup"><span data-stu-id="771ab-273">=, ==</span></span> <span data-ttu-id="771ab-274">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="771ab-274">Default is NotAllow.</span></span> <span data-ttu-id="771ab-275">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="771ab-275">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="771ab-276">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="771ab-276">pinExpirationDays</span></span>|<span data-ttu-id="771ab-277">Int32</span><span class="sxs-lookup"><span data-stu-id="771ab-277">Int32</span></span>|<span data-ttu-id="771ab-278">O valor inteiro especifica o período de tempo (em dias) em que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="771ab-278">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="771ab-279">O maior número que é possível definir para essa configuração de política é 730.</span><span class="sxs-lookup"><span data-stu-id="771ab-279">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="771ab-280">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="771ab-280">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="771ab-281">Se essa política for definida como 0, o PIN do usuário nunca irá expirar.</span><span class="sxs-lookup"><span data-stu-id="771ab-281">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="771ab-282">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="771ab-282">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="771ab-283">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="771ab-283">Default is 0.</span></span>|
|<span data-ttu-id="771ab-284">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="771ab-284">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="771ab-285">Int32</span><span class="sxs-lookup"><span data-stu-id="771ab-285">Int32</span></span>|<span data-ttu-id="771ab-286">O valor inteiro que especifica o número de PINs anteriores que podem ser associados a uma conta de usuário que não podem ser reutilizados.</span><span class="sxs-lookup"><span data-stu-id="771ab-286">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="771ab-287">O maior número que é possível definir para essa configuração de política é 50.</span><span class="sxs-lookup"><span data-stu-id="771ab-287">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="771ab-288">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="771ab-288">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="771ab-289">Se essa política for definida como 0, o armazenamento de PINs anteriores não será necessário.</span><span class="sxs-lookup"><span data-stu-id="771ab-289">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="771ab-290">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="771ab-290">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="771ab-291">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="771ab-291">Default is 0.</span></span>|
|<span data-ttu-id="771ab-292">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="771ab-292">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="771ab-293">Int32</span><span class="sxs-lookup"><span data-stu-id="771ab-293">Int32</span></span>|<span data-ttu-id="771ab-294">O número de falhas de autenticação permitido antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="771ab-294">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="771ab-295">O valor 0 desabilita a funcionalidade de apagamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="771ab-295">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="771ab-296">O intervalo é um inteiro X, em que 4 <= X <= 16 para desktop e 0 <= X <= 999 para dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="771ab-296">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="771ab-297">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="771ab-297">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="771ab-298">Int32</span><span class="sxs-lookup"><span data-stu-id="771ab-298">Int32</span></span>|<span data-ttu-id="771ab-299">Especifica a quantidade máxima de tempo (em minutos) permitida após o dispositivo ficar ocioso antes que ele seja bloqueado por PIN ou senha.</span><span class="sxs-lookup"><span data-stu-id="771ab-299">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="771ab-300">O intervalo é um inteiro X, em que 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="771ab-300">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="771ab-301">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="771ab-301">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="771ab-302">Int32</span><span class="sxs-lookup"><span data-stu-id="771ab-302">Int32</span></span>|<span data-ttu-id="771ab-303">Intervalo offline antes do apagamento dos dados do aplicativo (dias)</span><span class="sxs-lookup"><span data-stu-id="771ab-303">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="771ab-304">Resposta</span><span class="sxs-lookup"><span data-stu-id="771ab-304">Response</span></span>
<span data-ttu-id="771ab-305">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="771ab-305">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="771ab-306">Exemplo</span><span class="sxs-lookup"><span data-stu-id="771ab-306">Example</span></span>
### <a name="request"></a><span data-ttu-id="771ab-307">Solicitação</span><span class="sxs-lookup"><span data-stu-id="771ab-307">Request</span></span>
<span data-ttu-id="771ab-308">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="771ab-308">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4466

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```

### <a name="response"></a><span data-ttu-id="771ab-309">Resposta</span><span class="sxs-lookup"><span data-stu-id="771ab-309">Response</span></span>
<span data-ttu-id="771ab-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="771ab-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4574

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "6397be61-be61-6397-61be-976361be9763",
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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 0,
  "pinUppercaseLetters": "requireAtLeastOne",
  "pinLowercaseLetters": "requireAtLeastOne",
  "pinSpecialCharacters": "requireAtLeastOne",
  "pinExpirationDays": 1,
  "numberOfPastPinsRemembered": 10,
  "passwordMaximumAttemptCount": 11,
  "minutesOfInactivityBeforeDeviceLock": 3,
  "daysWithoutContactBeforeUnenroll": 0
}
```



