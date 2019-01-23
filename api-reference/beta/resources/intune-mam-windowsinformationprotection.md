---
title: Tipo de recurso windowsInformationProtection
description: Política para proteção de informações do Windows para definir configurações de gerenciamento detalhadas
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41f288e360aaf7a086541fb483c93af5dc451942
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403158"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="043dc-103">Tipo de recurso windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="043dc-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="043dc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="043dc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="043dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="043dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="043dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="043dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="043dc-107">Política para proteção de informações do Windows para definir configurações de gerenciamento detalhadas</span><span class="sxs-lookup"><span data-stu-id="043dc-107">Policy for Windows information protection to configure detailed management settings</span></span>


<span data-ttu-id="043dc-108">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="043dc-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="043dc-109">Methods</span></span>
|<span data-ttu-id="043dc-110">Método</span><span class="sxs-lookup"><span data-stu-id="043dc-110">Method</span></span>|<span data-ttu-id="043dc-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="043dc-111">Return Type</span></span>|<span data-ttu-id="043dc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="043dc-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="043dc-113">Listar windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="043dc-113">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="043dc-114">Coleção [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-114">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="043dc-115">Listar propriedades e relações dos objetos [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="043dc-115">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="043dc-116">Obter windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="043dc-116">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="043dc-117">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="043dc-117">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="043dc-118">Ler propriedades e relações do objeto [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="043dc-118">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="043dc-119">Ação assign</span><span class="sxs-lookup"><span data-stu-id="043dc-119">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="043dc-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="043dc-120">None</span></span>|<span data-ttu-id="043dc-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="043dc-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="043dc-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="043dc-122">Properties</span></span>
|<span data-ttu-id="043dc-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="043dc-123">Property</span></span>|<span data-ttu-id="043dc-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="043dc-124">Type</span></span>|<span data-ttu-id="043dc-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="043dc-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="043dc-126">displayName</span><span class="sxs-lookup"><span data-stu-id="043dc-126">displayName</span></span>|<span data-ttu-id="043dc-127">String</span><span class="sxs-lookup"><span data-stu-id="043dc-127">String</span></span>|<span data-ttu-id="043dc-128">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="043dc-128">Policy display name.</span></span> <span data-ttu-id="043dc-129">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="043dc-130">description</span><span class="sxs-lookup"><span data-stu-id="043dc-130">description</span></span>|<span data-ttu-id="043dc-131">String</span><span class="sxs-lookup"><span data-stu-id="043dc-131">String</span></span>|<span data-ttu-id="043dc-132">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="043dc-132">The policy's description.</span></span> <span data-ttu-id="043dc-133">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="043dc-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="043dc-134">createdDateTime</span></span>|<span data-ttu-id="043dc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="043dc-135">DateTimeOffset</span></span>|<span data-ttu-id="043dc-136">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="043dc-136">The date and time the policy was created.</span></span> <span data-ttu-id="043dc-137">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="043dc-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="043dc-138">lastModifiedDateTime</span></span>|<span data-ttu-id="043dc-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="043dc-139">DateTimeOffset</span></span>|<span data-ttu-id="043dc-140">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="043dc-140">Last time the policy was modified.</span></span> <span data-ttu-id="043dc-141">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="043dc-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="043dc-142">roleScopeTagIds</span></span>|<span data-ttu-id="043dc-143">String collection</span><span class="sxs-lookup"><span data-stu-id="043dc-143">String collection</span></span>|<span data-ttu-id="043dc-144">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="043dc-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="043dc-145">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="043dc-146">id</span><span class="sxs-lookup"><span data-stu-id="043dc-146">id</span></span>|<span data-ttu-id="043dc-147">String</span><span class="sxs-lookup"><span data-stu-id="043dc-147">String</span></span>|<span data-ttu-id="043dc-148">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="043dc-148">Key of the entity.</span></span> <span data-ttu-id="043dc-149">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="043dc-150">version</span><span class="sxs-lookup"><span data-stu-id="043dc-150">version</span></span>|<span data-ttu-id="043dc-151">String</span><span class="sxs-lookup"><span data-stu-id="043dc-151">String</span></span>|<span data-ttu-id="043dc-152">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="043dc-152">Version of the entity.</span></span> <span data-ttu-id="043dc-153">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="043dc-154">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="043dc-154">enforcementLevel</span></span>|[<span data-ttu-id="043dc-155">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="043dc-155">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="043dc-156">Nível da imposição de WIP. Consulte a definição de Enum de valores suportados.</span><span class="sxs-lookup"><span data-stu-id="043dc-156">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="043dc-157">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="043dc-157">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="043dc-158">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="043dc-158">enterpriseDomain</span></span>|<span data-ttu-id="043dc-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="043dc-159">String</span></span>|<span data-ttu-id="043dc-160">Domínio primário da empresa</span><span class="sxs-lookup"><span data-stu-id="043dc-160">Primary enterprise domain</span></span>|
|<span data-ttu-id="043dc-161">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="043dc-161">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="043dc-162">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-162">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="043dc-163">Lista de domínios da empresa a serem protegidos</span><span class="sxs-lookup"><span data-stu-id="043dc-163">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="043dc-164">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="043dc-164">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="043dc-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="043dc-165">Boolean</span></span>|<span data-ttu-id="043dc-166">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada</span><span class="sxs-lookup"><span data-stu-id="043dc-166">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="043dc-167">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="043dc-167">dataRecoveryCertificate</span></span>|[<span data-ttu-id="043dc-168">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="043dc-168">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="043dc-169">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="043dc-169">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="043dc-170">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS)</span><span class="sxs-lookup"><span data-stu-id="043dc-170">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="043dc-171">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="043dc-171">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="043dc-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="043dc-172">Boolean</span></span>|<span data-ttu-id="043dc-173">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="043dc-173">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="043dc-174">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="043dc-174">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="043dc-175">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="043dc-175">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="043dc-176">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="043dc-176">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="043dc-177">Guid</span><span class="sxs-lookup"><span data-stu-id="043dc-177">Guid</span></span>|<span data-ttu-id="043dc-178">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="043dc-178">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="043dc-179">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso</span><span class="sxs-lookup"><span data-stu-id="043dc-179">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="043dc-180">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="043dc-180">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="043dc-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="043dc-181">Boolean</span></span>|<span data-ttu-id="043dc-182">Especifica se a criptografia do Azure RMS para WIP será permitida</span><span class="sxs-lookup"><span data-stu-id="043dc-182">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="043dc-183">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="043dc-183">iconsVisible</span></span>|<span data-ttu-id="043dc-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="043dc-184">Boolean</span></span>|<span data-ttu-id="043dc-185">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="043dc-185">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="043dc-186">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP</span><span class="sxs-lookup"><span data-stu-id="043dc-186">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="043dc-187">protectedApps</span><span class="sxs-lookup"><span data-stu-id="043dc-187">protectedApps</span></span>|<span data-ttu-id="043dc-188">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-188">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="043dc-189">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia</span><span class="sxs-lookup"><span data-stu-id="043dc-189">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="043dc-190">exemptApps</span><span class="sxs-lookup"><span data-stu-id="043dc-190">exemptApps</span></span>|<span data-ttu-id="043dc-191">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="043dc-192">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="043dc-192">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="043dc-193">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="043dc-193">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="043dc-194">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="043dc-194">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="043dc-195">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-195">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="043dc-196">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="043dc-196">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="043dc-197">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="043dc-197">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="043dc-198">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="043dc-198">enterpriseProxiedDomains</span></span>|<span data-ttu-id="043dc-199">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-199">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="043dc-200">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="043dc-200">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="043dc-201">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="043dc-201">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="043dc-202">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="043dc-202">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="043dc-203">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="043dc-203">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="043dc-204">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="043dc-204">enterpriseIPRanges</span></span>|<span data-ttu-id="043dc-205">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-205">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="043dc-206">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="043dc-206">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="043dc-207">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="043dc-207">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="043dc-208">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="043dc-208">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="043dc-209">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="043dc-209">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="043dc-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="043dc-210">Boolean</span></span>|<span data-ttu-id="043dc-211">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="043dc-211">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="043dc-212">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="043dc-212">Default is false</span></span>|
|<span data-ttu-id="043dc-213">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="043dc-213">enterpriseProxyServers</span></span>|<span data-ttu-id="043dc-214">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-214">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="043dc-215">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="043dc-215">This is a list of proxy servers.</span></span> <span data-ttu-id="043dc-216">Qualquer servidor que não esteja na lista é considerado não corporativo</span><span class="sxs-lookup"><span data-stu-id="043dc-216">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="043dc-217">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="043dc-217">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="043dc-218">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="043dc-219">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="043dc-219">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="043dc-220">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="043dc-220">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="043dc-221">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="043dc-221">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="043dc-222">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="043dc-222">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="043dc-223">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies</span><span class="sxs-lookup"><span data-stu-id="043dc-223">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="043dc-224">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="043dc-224">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="043dc-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="043dc-225">Boolean</span></span>|<span data-ttu-id="043dc-226">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="043dc-226">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="043dc-227">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="043dc-227">Default is false</span></span>|
|<span data-ttu-id="043dc-228">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="043dc-228">neutralDomainResources</span></span>|<span data-ttu-id="043dc-229">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="043dc-230">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal</span><span class="sxs-lookup"><span data-stu-id="043dc-230">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="043dc-231">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="043dc-231">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="043dc-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="043dc-232">Boolean</span></span>|<span data-ttu-id="043dc-233">Esta opção é para o indexador do Windows Search, para permitir ou não a indexação de itens</span><span class="sxs-lookup"><span data-stu-id="043dc-233">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="043dc-234">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="043dc-234">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="043dc-235">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-235">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="043dc-236">Especifica uma lista de extensões de arquivo, para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo</span><span class="sxs-lookup"><span data-stu-id="043dc-236">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="043dc-237">isAssigned</span><span class="sxs-lookup"><span data-stu-id="043dc-237">isAssigned</span></span>|<span data-ttu-id="043dc-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="043dc-238">Boolean</span></span>|<span data-ttu-id="043dc-239">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="043dc-239">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="043dc-240">Relações</span><span class="sxs-lookup"><span data-stu-id="043dc-240">Relationships</span></span>
|<span data-ttu-id="043dc-241">Relação</span><span class="sxs-lookup"><span data-stu-id="043dc-241">Relationship</span></span>|<span data-ttu-id="043dc-242">Tipo</span><span class="sxs-lookup"><span data-stu-id="043dc-242">Type</span></span>|<span data-ttu-id="043dc-243">Descrição</span><span class="sxs-lookup"><span data-stu-id="043dc-243">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="043dc-244">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="043dc-244">protectedAppLockerFiles</span></span>|<span data-ttu-id="043dc-245">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-245">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="043dc-246">Outra maneira de inserir aplicativos protegidos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="043dc-246">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="043dc-247">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="043dc-247">exemptAppLockerFiles</span></span>|<span data-ttu-id="043dc-248">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-248">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="043dc-249">Outra maneira de inserir aplicativos isentos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="043dc-249">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="043dc-250">assignments</span><span class="sxs-lookup"><span data-stu-id="043dc-250">assignments</span></span>|<span data-ttu-id="043dc-251">Coleção [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="043dc-251">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="043dc-252">Propriedade de navegação para lista de grupos de segurança direcionados para política.</span><span class="sxs-lookup"><span data-stu-id="043dc-252">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="043dc-253">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="043dc-253">JSON Representation</span></span>
<span data-ttu-id="043dc-254">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="043dc-254">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
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
  "rightsManagementServicesTemplateId": "Guid",
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




