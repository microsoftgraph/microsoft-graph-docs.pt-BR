---
title: Tipo de recurso windowsInformationProtection
description: Política para proteção de informações do Windows para definir configurações de gerenciamento detalhadas
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e768047c1807c804deebcea566a7d45265d6c498
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962657"
---
# <a name="windowsinformationprotection-resource-type"></a><span data-ttu-id="a6b53-103">Tipo de recurso windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="a6b53-103">windowsInformationProtection resource type</span></span>

> <span data-ttu-id="a6b53-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6b53-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6b53-105">Política para proteção de informações do Windows para definir configurações de gerenciamento detalhadas</span><span class="sxs-lookup"><span data-stu-id="a6b53-105">Policy for Windows information protection to configure detailed management settings</span></span>

<span data-ttu-id="a6b53-106">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a6b53-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a6b53-107">Methods</span></span>
|<span data-ttu-id="a6b53-108">Método</span><span class="sxs-lookup"><span data-stu-id="a6b53-108">Method</span></span>|<span data-ttu-id="a6b53-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a6b53-109">Return Type</span></span>|<span data-ttu-id="a6b53-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6b53-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6b53-111">Listar windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="a6b53-111">List windowsInformationProtections</span></span>](../api/intune-mam-windowsinformationprotection-list.md)|<span data-ttu-id="a6b53-112">Coleção [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-112">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) collection</span></span>|<span data-ttu-id="a6b53-113">Listar propriedades e relações dos objetos [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="a6b53-113">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>|
|[<span data-ttu-id="a6b53-114">Obter windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="a6b53-114">Get windowsInformationProtection</span></span>](../api/intune-mam-windowsinformationprotection-get.md)|[<span data-ttu-id="a6b53-115">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="a6b53-115">windowsInformationProtection</span></span>](../resources/intune-mam-windowsinformationprotection.md)|<span data-ttu-id="a6b53-116">Ler propriedades e relações do objeto [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="a6b53-116">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>|
|[<span data-ttu-id="a6b53-117">Ação assign</span><span class="sxs-lookup"><span data-stu-id="a6b53-117">assign action</span></span>](../api/intune-mam-windowsinformationprotection-assign.md)|<span data-ttu-id="a6b53-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6b53-118">None</span></span>|<span data-ttu-id="a6b53-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a6b53-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a6b53-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6b53-120">Properties</span></span>
|<span data-ttu-id="a6b53-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6b53-121">Property</span></span>|<span data-ttu-id="a6b53-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6b53-122">Type</span></span>|<span data-ttu-id="a6b53-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6b53-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b53-124">displayName</span><span class="sxs-lookup"><span data-stu-id="a6b53-124">displayName</span></span>|<span data-ttu-id="a6b53-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b53-125">String</span></span>|<span data-ttu-id="a6b53-126">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="a6b53-126">Policy display name.</span></span> <span data-ttu-id="a6b53-127">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6b53-128">description</span><span class="sxs-lookup"><span data-stu-id="a6b53-128">description</span></span>|<span data-ttu-id="a6b53-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b53-129">String</span></span>|<span data-ttu-id="a6b53-130">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="a6b53-130">The policy's description.</span></span> <span data-ttu-id="a6b53-131">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6b53-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6b53-132">createdDateTime</span></span>|<span data-ttu-id="a6b53-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6b53-133">DateTimeOffset</span></span>|<span data-ttu-id="a6b53-134">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="a6b53-134">The date and time the policy was created.</span></span> <span data-ttu-id="a6b53-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6b53-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6b53-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a6b53-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6b53-137">DateTimeOffset</span></span>|<span data-ttu-id="a6b53-138">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="a6b53-138">Last time the policy was modified.</span></span> <span data-ttu-id="a6b53-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6b53-140">id</span><span class="sxs-lookup"><span data-stu-id="a6b53-140">id</span></span>|<span data-ttu-id="a6b53-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b53-141">String</span></span>|<span data-ttu-id="a6b53-142">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a6b53-142">Key of the entity.</span></span> <span data-ttu-id="a6b53-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6b53-144">version</span><span class="sxs-lookup"><span data-stu-id="a6b53-144">version</span></span>|<span data-ttu-id="a6b53-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b53-145">String</span></span>|<span data-ttu-id="a6b53-146">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="a6b53-146">Version of the entity.</span></span> <span data-ttu-id="a6b53-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a6b53-148">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a6b53-148">enforcementLevel</span></span>|[<span data-ttu-id="a6b53-149">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a6b53-149">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="a6b53-150">Nível da imposição de WIP. Consulte a definição de Enum de valores suportados.</span><span class="sxs-lookup"><span data-stu-id="a6b53-150">WIP enforcement level.See the Enum definition for supported values.</span></span> <span data-ttu-id="a6b53-151">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="a6b53-151">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="a6b53-152">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="a6b53-152">enterpriseDomain</span></span>|<span data-ttu-id="a6b53-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6b53-153">String</span></span>|<span data-ttu-id="a6b53-154">Domínio primário da empresa</span><span class="sxs-lookup"><span data-stu-id="a6b53-154">Primary enterprise domain</span></span>|
|<span data-ttu-id="a6b53-155">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="a6b53-155">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="a6b53-156">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-156">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6b53-157">Lista de domínios da empresa a serem protegidos</span><span class="sxs-lookup"><span data-stu-id="a6b53-157">List of enterprise domains to be protected</span></span>|
|<span data-ttu-id="a6b53-158">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="a6b53-158">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="a6b53-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b53-159">Boolean</span></span>|<span data-ttu-id="a6b53-160">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada</span><span class="sxs-lookup"><span data-stu-id="a6b53-160">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured</span></span>|
|<span data-ttu-id="a6b53-161">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a6b53-161">dataRecoveryCertificate</span></span>|[<span data-ttu-id="a6b53-162">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a6b53-162">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="a6b53-163">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="a6b53-163">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="a6b53-164">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS)</span><span class="sxs-lookup"><span data-stu-id="a6b53-164">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS)</span></span>|
|<span data-ttu-id="a6b53-165">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="a6b53-165">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="a6b53-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b53-166">Boolean</span></span>|<span data-ttu-id="a6b53-167">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a6b53-167">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="a6b53-168">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="a6b53-168">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="a6b53-169">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="a6b53-169">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span>|
|<span data-ttu-id="a6b53-170">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="a6b53-170">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="a6b53-171">Guid</span><span class="sxs-lookup"><span data-stu-id="a6b53-171">Guid</span></span>|<span data-ttu-id="a6b53-172">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="a6b53-172">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="a6b53-173">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso</span><span class="sxs-lookup"><span data-stu-id="a6b53-173">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access</span></span>|
|<span data-ttu-id="a6b53-174">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="a6b53-174">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="a6b53-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b53-175">Boolean</span></span>|<span data-ttu-id="a6b53-176">Especifica se a criptografia do Azure RMS para WIP será permitida</span><span class="sxs-lookup"><span data-stu-id="a6b53-176">Specifies whether to allow Azure RMS encryption for WIP</span></span>|
|<span data-ttu-id="a6b53-177">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="a6b53-177">iconsVisible</span></span>|<span data-ttu-id="a6b53-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b53-178">Boolean</span></span>|<span data-ttu-id="a6b53-179">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="a6b53-179">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="a6b53-180">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP</span><span class="sxs-lookup"><span data-stu-id="a6b53-180">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app</span></span>|
|<span data-ttu-id="a6b53-181">protectedApps</span><span class="sxs-lookup"><span data-stu-id="a6b53-181">protectedApps</span></span>|<span data-ttu-id="a6b53-182">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-182">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a6b53-183">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia</span><span class="sxs-lookup"><span data-stu-id="a6b53-183">Protected applications can access enterprise data and the data handled by those applications are protected with encryption</span></span>|
|<span data-ttu-id="a6b53-184">exemptApps</span><span class="sxs-lookup"><span data-stu-id="a6b53-184">exemptApps</span></span>|<span data-ttu-id="a6b53-185">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-185">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a6b53-186">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="a6b53-186">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="a6b53-187">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="a6b53-187">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span>|
|<span data-ttu-id="a6b53-188">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="a6b53-188">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="a6b53-189">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-189">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6b53-190">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="a6b53-190">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="a6b53-191">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="a6b53-191">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="a6b53-192">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="a6b53-192">enterpriseProxiedDomains</span></span>|<span data-ttu-id="a6b53-193">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-193">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="a6b53-194">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="a6b53-194">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="a6b53-195">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="a6b53-195">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="a6b53-196">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="a6b53-196">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="a6b53-197">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="a6b53-197">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy</span></span>|
|<span data-ttu-id="a6b53-198">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="a6b53-198">enterpriseIPRanges</span></span>|<span data-ttu-id="a6b53-199">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-199">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="a6b53-200">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="a6b53-200">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="a6b53-201">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="a6b53-201">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="a6b53-202">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados</span><span class="sxs-lookup"><span data-stu-id="a6b53-202">These locations will be considered a safe destination for enterprise data to be shared to</span></span>|
|<span data-ttu-id="a6b53-203">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a6b53-203">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="a6b53-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b53-204">Boolean</span></span>|<span data-ttu-id="a6b53-205">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="a6b53-205">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="a6b53-206">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="a6b53-206">Default is false</span></span>|
|<span data-ttu-id="a6b53-207">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="a6b53-207">enterpriseProxyServers</span></span>|<span data-ttu-id="a6b53-208">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-208">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6b53-209">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="a6b53-209">This is a list of proxy servers.</span></span> <span data-ttu-id="a6b53-210">Qualquer servidor que não esteja na lista é considerado não corporativo</span><span class="sxs-lookup"><span data-stu-id="a6b53-210">Any server not on this list is considered non-enterprise</span></span>|
|<span data-ttu-id="a6b53-211">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="a6b53-211">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="a6b53-212">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-212">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6b53-213">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="a6b53-213">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="a6b53-214">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="a6b53-214">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="a6b53-215">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="a6b53-215">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="a6b53-216">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="a6b53-216">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="a6b53-217">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies</span><span class="sxs-lookup"><span data-stu-id="a6b53-217">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies</span></span>|
|<span data-ttu-id="a6b53-218">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a6b53-218">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="a6b53-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b53-219">Boolean</span></span>|<span data-ttu-id="a6b53-220">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a6b53-220">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="a6b53-221">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="a6b53-221">Default is false</span></span>|
|<span data-ttu-id="a6b53-222">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="a6b53-222">neutralDomainResources</span></span>|<span data-ttu-id="a6b53-223">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6b53-224">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal</span><span class="sxs-lookup"><span data-stu-id="a6b53-224">List of domain names that can used for work or personal resource</span></span>|
|<span data-ttu-id="a6b53-225">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="a6b53-225">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="a6b53-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b53-226">Boolean</span></span>|<span data-ttu-id="a6b53-227">Esta opção é para o indexador do Windows Search, para permitir ou não a indexação de itens</span><span class="sxs-lookup"><span data-stu-id="a6b53-227">This switch is for the Windows Search Indexer, to allow or disallow indexing of items</span></span>|
|<span data-ttu-id="a6b53-228">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="a6b53-228">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="a6b53-229">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a6b53-230">Especifica uma lista de extensões de arquivo, para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo</span><span class="sxs-lookup"><span data-stu-id="a6b53-230">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary</span></span>|
|<span data-ttu-id="a6b53-231">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a6b53-231">isAssigned</span></span>|<span data-ttu-id="a6b53-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b53-232">Boolean</span></span>|<span data-ttu-id="a6b53-233">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="a6b53-233">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6b53-234">Relações</span><span class="sxs-lookup"><span data-stu-id="a6b53-234">Relationships</span></span>
|<span data-ttu-id="a6b53-235">Relação</span><span class="sxs-lookup"><span data-stu-id="a6b53-235">Relationship</span></span>|<span data-ttu-id="a6b53-236">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6b53-236">Type</span></span>|<span data-ttu-id="a6b53-237">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6b53-237">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b53-238">protectedAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="a6b53-238">protectedAppLockerFiles</span></span>|<span data-ttu-id="a6b53-239">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-239">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="a6b53-240">Outra maneira de inserir aplicativos protegidos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="a6b53-240">Another way to input protected apps through xml files</span></span>|
|<span data-ttu-id="a6b53-241">exemptAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="a6b53-241">exemptAppLockerFiles</span></span>|<span data-ttu-id="a6b53-242">Coleção [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-242">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) collection</span></span>|<span data-ttu-id="a6b53-243">Outra maneira de inserir aplicativos isentos por meio de arquivos xml</span><span class="sxs-lookup"><span data-stu-id="a6b53-243">Another way to input exempt apps through xml files</span></span>|
|<span data-ttu-id="a6b53-244">assignments</span><span class="sxs-lookup"><span data-stu-id="a6b53-244">assignments</span></span>|<span data-ttu-id="a6b53-245">Coleção [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a6b53-245">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="a6b53-246">Propriedade de navegação para lista de grupos de segurança direcionados para política.</span><span class="sxs-lookup"><span data-stu-id="a6b53-246">Navigation property to list of security groups targeted for policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6b53-247">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6b53-247">JSON Representation</span></span>
<span data-ttu-id="a6b53-248">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6b53-248">Here is a JSON representation of the resource.</span></span>
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



