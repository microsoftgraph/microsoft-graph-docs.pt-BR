---
title: Tipo de recurso windowsInformationProtection
description: Política para proteção de informações do Windows para definir configurações de gerenciamento detalhadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d0e4a18282265b0f6c7a03ba6d395198175366e5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760199"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="9560c-103">Tipo de recurso windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="9560c-103">windowsInformationProtection resource type</span></span>

<span data-ttu-id="9560c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9560c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9560c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9560c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9560c-106">Política para proteção de informações do Windows para definir configurações de gerenciamento detalhadas</span><span class="sxs-lookup"><span data-stu-id="9560c-106">Policy for Windows information protection to configure detailed management settings</span></span>


<span data-ttu-id="9560c-107">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9560c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9560c-108">Methods</span></span>
|<span data-ttu-id="9560c-109">Método</span><span class="sxs-lookup"><span data-stu-id="9560c-109">Method</span></span>|<span data-ttu-id="9560c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9560c-110">Return Type</span></span>|<span data-ttu-id="9560c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9560c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9560c-112">Listar windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="9560c-112">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="9560c-113">Coleção [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-113">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="9560c-114">Listar propriedades e relações dos objetos [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9560c-114">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="9560c-115">Obter windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="9560c-115">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="9560c-116">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="9560c-116">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="9560c-117">Ler propriedades e relações do objeto [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9560c-117">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="9560c-118">Ação assign</span><span class="sxs-lookup"><span data-stu-id="9560c-118">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="9560c-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9560c-119">None</span></span>|<span data-ttu-id="9560c-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9560c-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9560c-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9560c-121">Properties</span></span>
|<span data-ttu-id="9560c-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9560c-122">Property</span></span>|<span data-ttu-id="9560c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9560c-123">Type</span></span>|<span data-ttu-id="9560c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9560c-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9560c-125">displayName</span><span class="sxs-lookup"><span data-stu-id="9560c-125">displayName</span></span>|<span data-ttu-id="9560c-126">String</span><span class="sxs-lookup"><span data-stu-id="9560c-126">String</span></span>|<span data-ttu-id="9560c-127">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="9560c-127">Policy display name.</span></span> <span data-ttu-id="9560c-128">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9560c-129">description</span><span class="sxs-lookup"><span data-stu-id="9560c-129">description</span></span>|<span data-ttu-id="9560c-130">String</span><span class="sxs-lookup"><span data-stu-id="9560c-130">String</span></span>|<span data-ttu-id="9560c-131">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="9560c-131">The policy's description.</span></span> <span data-ttu-id="9560c-132">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9560c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9560c-133">createdDateTime</span></span>|<span data-ttu-id="9560c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9560c-134">DateTimeOffset</span></span>|<span data-ttu-id="9560c-135">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="9560c-135">The date and time the policy was created.</span></span> <span data-ttu-id="9560c-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9560c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9560c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9560c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9560c-138">DateTimeOffset</span></span>|<span data-ttu-id="9560c-139">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="9560c-139">Last time the policy was modified.</span></span> <span data-ttu-id="9560c-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9560c-141">id</span><span class="sxs-lookup"><span data-stu-id="9560c-141">id</span></span>|<span data-ttu-id="9560c-142">String</span><span class="sxs-lookup"><span data-stu-id="9560c-142">String</span></span>|<span data-ttu-id="9560c-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9560c-143">Key of the entity.</span></span> <span data-ttu-id="9560c-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9560c-145">version</span><span class="sxs-lookup"><span data-stu-id="9560c-145">version</span></span>|<span data-ttu-id="9560c-146">String</span><span class="sxs-lookup"><span data-stu-id="9560c-146">String</span></span>|<span data-ttu-id="9560c-147">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="9560c-147">Version of the entity.</span></span> <span data-ttu-id="9560c-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9560c-149">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="9560c-149">enforcementLevel</span></span>|[<span data-ttu-id="9560c-150">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="9560c-150">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="9560c-151">Nível de aplicação da WIP. Consulte a definição Enum para valores com suporte.</span><span class="sxs-lookup"><span data-stu-id="9560c-151">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="9560c-152">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="9560c-152">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="9560c-153">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="9560c-153">enterpriseDomain</span></span>|<span data-ttu-id="9560c-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9560c-154">String</span></span>|<span data-ttu-id="9560c-155">Domínio primário da empresa</span><span class="sxs-lookup"><span data-stu-id="9560c-155">Primary enterprise domain</span></span>|
|<span data-ttu-id="9560c-156">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="9560c-156">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="9560c-157">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-157">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9560c-158">Lista de domínios da empresa a serem protegidos</span><span class="sxs-lookup"><span data-stu-id="9560c-158">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="9560c-159">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="9560c-159">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="9560c-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="9560c-160">Boolean</span></span>|<span data-ttu-id="9560c-161">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada</span><span class="sxs-lookup"><span data-stu-id="9560c-161">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="9560c-162">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9560c-162">dataRecoveryCertificate</span></span>|[<span data-ttu-id="9560c-163">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9560c-163">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="9560c-164">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="9560c-164">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="9560c-165">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS)</span><span class="sxs-lookup"><span data-stu-id="9560c-165">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="9560c-166">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="9560c-166">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="9560c-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="9560c-167">Boolean</span></span>|<span data-ttu-id="9560c-168">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9560c-168">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="9560c-169">Se definido como 1 (não revogar teclas), as teclas não serão revogadas e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="9560c-169">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="9560c-170">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="9560c-170">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="9560c-171">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="9560c-171">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="9560c-172">Guid</span><span class="sxs-lookup"><span data-stu-id="9560c-172">Guid</span></span>|<span data-ttu-id="9560c-173">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="9560c-173">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="9560c-174">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso</span><span class="sxs-lookup"><span data-stu-id="9560c-174">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="9560c-175">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="9560c-175">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="9560c-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="9560c-176">Boolean</span></span>|<span data-ttu-id="9560c-177">Especifica se a criptografia do Azure RMS para WIP será permitida</span><span class="sxs-lookup"><span data-stu-id="9560c-177">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="9560c-178">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="9560c-178">iconsVisible</span></span>|<span data-ttu-id="9560c-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="9560c-179">Boolean</span></span>|<span data-ttu-id="9560c-180">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="9560c-180">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="9560c-181">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP</span><span class="sxs-lookup"><span data-stu-id="9560c-181">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="9560c-182">protectedApps</span><span class="sxs-lookup"><span data-stu-id="9560c-182">protectedApps</span></span>|<span data-ttu-id="9560c-183">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-183">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="9560c-184">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia</span><span class="sxs-lookup"><span data-stu-id="9560c-184">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="9560c-185">exemptApps</span><span class="sxs-lookup"><span data-stu-id="9560c-185">exemptApps</span></span>|<span data-ttu-id="9560c-186">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-186">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="9560c-187">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="9560c-187">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="9560c-188">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="9560c-188">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="9560c-189">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="9560c-189">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="9560c-190">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-190">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9560c-191">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="9560c-191">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="9560c-192">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="9560c-192">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="9560c-193">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="9560c-193">enterpriseProxiedDomains</span></span>|<span data-ttu-id="9560c-194">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-194">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="9560c-195">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="9560c-195">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="9560c-196">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="9560c-196">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="9560c-197">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="9560c-197">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="9560c-198">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="9560c-198">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="9560c-199">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="9560c-199">enterpriseIPRanges</span></span>|<span data-ttu-id="9560c-200">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-200">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="9560c-201">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="9560c-201">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="9560c-202">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="9560c-202">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="9560c-203">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="9560c-203">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="9560c-204">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9560c-204">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="9560c-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9560c-205">Boolean</span></span>|<span data-ttu-id="9560c-206">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="9560c-206">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="9560c-207">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="9560c-207">Default is false</span></span>|
|<span data-ttu-id="9560c-208">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="9560c-208">enterpriseProxyServers</span></span>|<span data-ttu-id="9560c-209">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-209">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9560c-210">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="9560c-210">This is a list of proxy servers.</span></span> <span data-ttu-id="9560c-211">Qualquer servidor que não esteja na lista é considerado não corporativo</span><span class="sxs-lookup"><span data-stu-id="9560c-211">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="9560c-212">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="9560c-212">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="9560c-213">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-213">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9560c-214">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="9560c-214">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="9560c-215">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="9560c-215">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="9560c-216">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="9560c-216">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="9560c-217">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="9560c-217">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="9560c-218">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies</span><span class="sxs-lookup"><span data-stu-id="9560c-218">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="9560c-219">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9560c-219">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="9560c-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="9560c-220">Boolean</span></span>|<span data-ttu-id="9560c-221">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9560c-221">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="9560c-222">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="9560c-222">Default is false</span></span>|
|<span data-ttu-id="9560c-223">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="9560c-223">neutralDomainResources</span></span>|<span data-ttu-id="9560c-224">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-224">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9560c-225">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal</span><span class="sxs-lookup"><span data-stu-id="9560c-225">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="9560c-226">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="9560c-226">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="9560c-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="9560c-227">Boolean</span></span>|<span data-ttu-id="9560c-228">Esta opção é para o indexador do Windows Search, para permitir ou não a indexação de itens</span><span class="sxs-lookup"><span data-stu-id="9560c-228">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="9560c-229">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="9560c-229">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="9560c-230">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-230">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9560c-231">Especifica uma lista de extensões de arquivo, para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo</span><span class="sxs-lookup"><span data-stu-id="9560c-231">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="9560c-232">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9560c-232">isAssigned</span></span>|<span data-ttu-id="9560c-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="9560c-233">Boolean</span></span>|<span data-ttu-id="9560c-234">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="9560c-234">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9560c-235">Relações</span><span class="sxs-lookup"><span data-stu-id="9560c-235">Relationships</span></span>
|<span data-ttu-id="9560c-236">Relação</span><span class="sxs-lookup"><span data-stu-id="9560c-236">Relationship</span></span>|<span data-ttu-id="9560c-237">Tipo</span><span class="sxs-lookup"><span data-stu-id="9560c-237">Type</span></span>|<span data-ttu-id="9560c-238">Descrição</span><span class="sxs-lookup"><span data-stu-id="9560c-238">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9560c-239">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="9560c-239">protectedAppLockerFiles</span></span>|<span data-ttu-id="9560c-240">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-240">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="9560c-241">Outra maneira de inserir aplicativos protegidos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="9560c-241">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="9560c-242">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="9560c-242">exemptAppLockerFiles</span></span>|<span data-ttu-id="9560c-243">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-243">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="9560c-244">Outra maneira de inserir aplicativos isentos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="9560c-244">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="9560c-245">assignments</span><span class="sxs-lookup"><span data-stu-id="9560c-245">assignments</span></span>|<span data-ttu-id="9560c-246">Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9560c-246">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="9560c-247">Propriedade de navegação para lista de grupos de segurança direcionados para política.</span><span class="sxs-lookup"><span data-stu-id="9560c-247">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9560c-248">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9560c-248">JSON Representation</span></span>
<span data-ttu-id="9560c-249">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9560c-249">Here is a JSON representation of the resource.</span></span>
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
          "@odata.type": "microsoft.graph.ipRange"
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




