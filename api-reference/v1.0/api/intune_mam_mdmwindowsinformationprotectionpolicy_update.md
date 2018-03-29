# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="98b44-101">Atualizar mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="98b44-101">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="98b44-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="98b44-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98b44-103">Atualizar as propriedades de um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98b44-103">Update the properties of a [calendar](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98b44-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98b44-104">Prerequisites</span></span>
<span data-ttu-id="98b44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="98b44-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98b44-107">Permission type</span></span>|<span data-ttu-id="98b44-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98b44-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98b44-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98b44-109">Delegated (work or school account)</span></span>|<span data-ttu-id="98b44-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98b44-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98b44-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98b44-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98b44-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98b44-112">Not supported.</span></span>|
|<span data-ttu-id="98b44-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98b44-113">Application</span></span>|<span data-ttu-id="98b44-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98b44-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98b44-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98b44-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="98b44-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98b44-116">Request headers</span></span>
|<span data-ttu-id="98b44-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98b44-117">Header</span></span>|<span data-ttu-id="98b44-118">Valor</span><span class="sxs-lookup"><span data-stu-id="98b44-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98b44-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="98b44-119">Authorization</span></span>|<span data-ttu-id="98b44-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98b44-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="98b44-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98b44-121">Accept</span></span>|<span data-ttu-id="98b44-122">application/json</span><span class="sxs-lookup"><span data-stu-id="98b44-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98b44-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98b44-123">Request body</span></span>
<span data-ttu-id="98b44-124">No corpo da solicitação, forneça uma representação JSON do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98b44-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="98b44-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="98b44-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="98b44-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98b44-126">Property</span></span>|<span data-ttu-id="98b44-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="98b44-127">Type</span></span>|<span data-ttu-id="98b44-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="98b44-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b44-129">displayName</span><span class="sxs-lookup"><span data-stu-id="98b44-129">displayName</span></span>|<span data-ttu-id="98b44-130">String</span><span class="sxs-lookup"><span data-stu-id="98b44-130">String</span></span>|<span data-ttu-id="98b44-131">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="98b44-131">Policy display name.</span></span> <span data-ttu-id="98b44-132">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="98b44-133">descrição</span><span class="sxs-lookup"><span data-stu-id="98b44-133">description</span></span>|<span data-ttu-id="98b44-134">String</span><span class="sxs-lookup"><span data-stu-id="98b44-134">String</span></span>|<span data-ttu-id="98b44-135">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="98b44-135">The policy's description.</span></span> <span data-ttu-id="98b44-136">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="98b44-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98b44-137">createdDateTime</span></span>|<span data-ttu-id="98b44-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98b44-138">DateTimeOffset</span></span>|<span data-ttu-id="98b44-139">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="98b44-139">The date and time the group was created.</span></span> <span data-ttu-id="98b44-140">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="98b44-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98b44-141">lastModifiedDateTime</span></span>|<span data-ttu-id="98b44-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98b44-142">DateTimeOffset</span></span>|<span data-ttu-id="98b44-143">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="98b44-143">Last time the policy was modified.</span></span> <span data-ttu-id="98b44-144">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="98b44-145">id</span><span class="sxs-lookup"><span data-stu-id="98b44-145">id</span></span>|<span data-ttu-id="98b44-146">String</span><span class="sxs-lookup"><span data-stu-id="98b44-146">String</span></span>|<span data-ttu-id="98b44-147">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98b44-147">Key of the setting.</span></span> <span data-ttu-id="98b44-148">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="98b44-149">version</span><span class="sxs-lookup"><span data-stu-id="98b44-149">version</span></span>|<span data-ttu-id="98b44-150">String</span><span class="sxs-lookup"><span data-stu-id="98b44-150">String</span></span>|<span data-ttu-id="98b44-151">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="98b44-151">Version of the entity.</span></span> <span data-ttu-id="98b44-152">Herdado de [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="98b44-153">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="98b44-153">enforcementLevel</span></span>|<span data-ttu-id="98b44-154">String</span><span class="sxs-lookup"><span data-stu-id="98b44-154">String</span></span>|<span data-ttu-id="98b44-155">Nível de imposição WIP. Confira a definição de enumeração para valores compatíveis Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="98b44-155">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="98b44-156">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="98b44-156">enterpriseDomain</span></span>|<span data-ttu-id="98b44-157">String</span><span class="sxs-lookup"><span data-stu-id="98b44-157">String</span></span>|<span data-ttu-id="98b44-158">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-158">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-159">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="98b44-159">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="98b44-160">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-160">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="98b44-161">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-161">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-162">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="98b44-162">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="98b44-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="98b44-163">Boolean</span></span>|<span data-ttu-id="98b44-164">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-164">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-165">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="98b44-165">dataRecoveryCertificate</span></span>|[<span data-ttu-id="98b44-166">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="98b44-166">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="98b44-167">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="98b44-167">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="98b44-168">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-168">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-169">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="98b44-169">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="98b44-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="98b44-170">Boolean</span></span>|<span data-ttu-id="98b44-171">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="98b44-171">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="98b44-172">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="98b44-172">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="98b44-173">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="98b44-173">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="98b44-174">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-174">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-175">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="98b44-175">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="98b44-176">Guid</span><span class="sxs-lookup"><span data-stu-id="98b44-176">Guid</span></span>|<span data-ttu-id="98b44-177">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="98b44-177">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="98b44-178">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-178">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-179">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="98b44-179">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="98b44-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="98b44-180">Boolean</span></span>|<span data-ttu-id="98b44-181">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-181">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-182">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="98b44-182">iconsVisible</span></span>|<span data-ttu-id="98b44-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="98b44-183">Boolean</span></span>|<span data-ttu-id="98b44-184">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="98b44-184">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="98b44-185">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-185">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-186">protectedApps</span><span class="sxs-lookup"><span data-stu-id="98b44-186">protectedApps</span></span>|<span data-ttu-id="98b44-187">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-187">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="98b44-188">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-188">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-189">exemptApps</span><span class="sxs-lookup"><span data-stu-id="98b44-189">exemptApps</span></span>|<span data-ttu-id="98b44-190">Coleção [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-190">[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="98b44-191">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="98b44-191">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="98b44-192">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="98b44-192">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="98b44-193">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-193">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="98b44-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="98b44-195">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-195">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="98b44-196">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="98b44-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="98b44-197">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="98b44-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="98b44-199">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="98b44-200">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="98b44-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="98b44-201">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="98b44-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="98b44-202">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="98b44-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="98b44-203">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="98b44-204">enterpriseIPRanges</span></span>|<span data-ttu-id="98b44-205">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-205">[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="98b44-206">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="98b44-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="98b44-207">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="98b44-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="98b44-208">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-208">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="98b44-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="98b44-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="98b44-210">Boolean</span></span>|<span data-ttu-id="98b44-211">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="98b44-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="98b44-212">A padrão é false Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-212">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="98b44-213">enterpriseProxyServers</span></span>|<span data-ttu-id="98b44-214">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-214">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="98b44-215">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="98b44-215">This is a list of proxy servers.</span></span> <span data-ttu-id="98b44-216">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-216">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="98b44-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="98b44-218">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-218">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="98b44-219">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="98b44-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="98b44-220">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="98b44-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="98b44-221">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="98b44-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="98b44-222">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="98b44-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="98b44-223">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="98b44-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="98b44-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="98b44-225">Boolean</span></span>|<span data-ttu-id="98b44-226">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="98b44-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="98b44-227">A padrão é false Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-227">Default is false Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="98b44-228">neutralDomainResources</span></span>|<span data-ttu-id="98b44-229">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-229">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="98b44-230">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-230">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="98b44-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="98b44-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="98b44-232">Boolean</span></span>|<span data-ttu-id="98b44-233">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="98b44-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="98b44-235">Coleção [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-235">[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="98b44-236">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="98b44-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="98b44-237">isAssigned</span></span>|<span data-ttu-id="98b44-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="98b44-238">Boolean</span></span>|<span data-ttu-id="98b44-239">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="98b44-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="98b44-240">Herdado de [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="98b44-240">Inherited from [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="98b44-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="98b44-241">Response</span></span>
<span data-ttu-id="98b44-242">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98b44-242">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98b44-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98b44-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="98b44-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98b44-244">Request</span></span>
<span data-ttu-id="98b44-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98b44-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 3890

{
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="98b44-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="98b44-246">Response</span></span>
<span data-ttu-id="98b44-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98b44-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4074

{
  "@odata.type": "#microsoft.intune_mam_graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```



