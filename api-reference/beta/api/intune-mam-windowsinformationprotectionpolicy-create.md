---
title: Criar windowsInformationProtectionPolicy
description: Cria um novo objeto windowsInformationProtectionPolicy.
author: tfitzmac
ms.openlocfilehash: 80615563dcc85b74a7f8d40f9c6752d4c16fdae8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323776"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="9e32d-103">Criar windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9e32d-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="9e32d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e32d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e32d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e32d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e32d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9e32d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e32d-107">Cria um novo objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e32d-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e32d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e32d-108">Prerequisites</span></span>
<span data-ttu-id="9e32d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e32d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e32d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e32d-111">Permission type</span></span>|<span data-ttu-id="9e32d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e32d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e32d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e32d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e32d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e32d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9e32d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e32d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e32d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e32d-116">Not supported.</span></span>|
|<span data-ttu-id="9e32d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e32d-117">Application</span></span>|<span data-ttu-id="9e32d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e32d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e32d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e32d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="9e32d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e32d-120">Request headers</span></span>
|<span data-ttu-id="9e32d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e32d-121">Header</span></span>|<span data-ttu-id="9e32d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9e32d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e32d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e32d-123">Authorization</span></span>|<span data-ttu-id="9e32d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e32d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e32d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e32d-125">Accept</span></span>|<span data-ttu-id="9e32d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e32d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e32d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e32d-127">Request body</span></span>
<span data-ttu-id="9e32d-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="9e32d-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="9e32d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="9e32d-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="9e32d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e32d-130">Property</span></span>|<span data-ttu-id="9e32d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e32d-131">Type</span></span>|<span data-ttu-id="9e32d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e32d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e32d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9e32d-133">displayName</span></span>|<span data-ttu-id="9e32d-134">String</span><span class="sxs-lookup"><span data-stu-id="9e32d-134">String</span></span>|<span data-ttu-id="9e32d-135">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="9e32d-135">Policy display name.</span></span> <span data-ttu-id="9e32d-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e32d-137">description</span><span class="sxs-lookup"><span data-stu-id="9e32d-137">description</span></span>|<span data-ttu-id="9e32d-138">String</span><span class="sxs-lookup"><span data-stu-id="9e32d-138">String</span></span>|<span data-ttu-id="9e32d-139">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="9e32d-139">The policy's description.</span></span> <span data-ttu-id="9e32d-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e32d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e32d-141">createdDateTime</span></span>|<span data-ttu-id="9e32d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e32d-142">DateTimeOffset</span></span>|<span data-ttu-id="9e32d-143">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="9e32d-143">The date and time the policy was created.</span></span> <span data-ttu-id="9e32d-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e32d-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e32d-145">lastModifiedDateTime</span></span>|<span data-ttu-id="9e32d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e32d-146">DateTimeOffset</span></span>|<span data-ttu-id="9e32d-147">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="9e32d-147">Last time the policy was modified.</span></span> <span data-ttu-id="9e32d-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e32d-149">id</span><span class="sxs-lookup"><span data-stu-id="9e32d-149">id</span></span>|<span data-ttu-id="9e32d-150">String</span><span class="sxs-lookup"><span data-stu-id="9e32d-150">String</span></span>|<span data-ttu-id="9e32d-151">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e32d-151">Key of the entity.</span></span> <span data-ttu-id="9e32d-152">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e32d-153">version</span><span class="sxs-lookup"><span data-stu-id="9e32d-153">version</span></span>|<span data-ttu-id="9e32d-154">String</span><span class="sxs-lookup"><span data-stu-id="9e32d-154">String</span></span>|<span data-ttu-id="9e32d-155">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e32d-155">Version of the entity.</span></span> <span data-ttu-id="9e32d-156">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="9e32d-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="9e32d-157">enforcementLevel</span></span>|[<span data-ttu-id="9e32d-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="9e32d-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="9e32d-159">Nível da imposição de WIP. Consulte a definição de Enum de valores suportados Inherited de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9e32d-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="9e32d-160">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="9e32d-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="9e32d-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="9e32d-161">enterpriseDomain</span></span>|<span data-ttu-id="9e32d-162">String</span><span class="sxs-lookup"><span data-stu-id="9e32d-162">String</span></span>|<span data-ttu-id="9e32d-163">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="9e32d-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="9e32d-165">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9e32d-166">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="9e32d-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="9e32d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-168">Boolean</span></span>|<span data-ttu-id="9e32d-169">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9e32d-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="9e32d-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9e32d-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="9e32d-172">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="9e32d-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="9e32d-173">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="9e32d-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="9e32d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-175">Boolean</span></span>|<span data-ttu-id="9e32d-176">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9e32d-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="9e32d-177">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="9e32d-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="9e32d-178">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="9e32d-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="9e32d-179">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="9e32d-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="9e32d-181">Guid</span><span class="sxs-lookup"><span data-stu-id="9e32d-181">Guid</span></span>|<span data-ttu-id="9e32d-182">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="9e32d-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="9e32d-183">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="9e32d-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="9e32d-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-185">Boolean</span></span>|<span data-ttu-id="9e32d-186">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="9e32d-187">iconsVisible</span></span>|<span data-ttu-id="9e32d-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-188">Boolean</span></span>|<span data-ttu-id="9e32d-189">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="9e32d-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="9e32d-190">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="9e32d-191">protectedApps</span></span>|<span data-ttu-id="9e32d-192">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="9e32d-193">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="9e32d-194">exemptApps</span></span>|<span data-ttu-id="9e32d-195">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="9e32d-196">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="9e32d-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="9e32d-197">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="9e32d-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="9e32d-198">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="9e32d-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="9e32d-200">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9e32d-201">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="9e32d-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="9e32d-202">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="9e32d-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="9e32d-204">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="9e32d-205">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="9e32d-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="9e32d-206">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="9e32d-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="9e32d-207">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="9e32d-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="9e32d-208">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="9e32d-209">enterpriseIPRanges</span></span>|<span data-ttu-id="9e32d-210">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="9e32d-211">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="9e32d-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="9e32d-212">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="9e32d-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="9e32d-213">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9e32d-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="9e32d-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-215">Boolean</span></span>|<span data-ttu-id="9e32d-216">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="9e32d-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="9e32d-217">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="9e32d-218">enterpriseProxyServers</span></span>|<span data-ttu-id="9e32d-219">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9e32d-220">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="9e32d-220">This is a list of proxy servers.</span></span> <span data-ttu-id="9e32d-221">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="9e32d-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="9e32d-223">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9e32d-224">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="9e32d-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="9e32d-225">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="9e32d-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="9e32d-226">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="9e32d-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="9e32d-227">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="9e32d-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="9e32d-228">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9e32d-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="9e32d-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-230">Boolean</span></span>|<span data-ttu-id="9e32d-231">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9e32d-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="9e32d-232">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="9e32d-233">neutralDomainResources</span></span>|<span data-ttu-id="9e32d-234">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9e32d-235">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="9e32d-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="9e32d-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-237">Boolean</span></span>|<span data-ttu-id="9e32d-238">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="9e32d-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="9e32d-240">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="9e32d-241">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9e32d-242">isAssigned</span></span>|<span data-ttu-id="9e32d-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-243">Boolean</span></span>|<span data-ttu-id="9e32d-244">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="9e32d-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="9e32d-245">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="9e32d-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="9e32d-246">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="9e32d-246">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="9e32d-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-247">Boolean</span></span>|<span data-ttu-id="9e32d-248">Nova propriedade em RS2, documentação pendente</span><span class="sxs-lookup"><span data-stu-id="9e32d-248">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="9e32d-249">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="9e32d-249">mdmEnrollmentUrl</span></span>|<span data-ttu-id="9e32d-250">String</span><span class="sxs-lookup"><span data-stu-id="9e32d-250">String</span></span>|<span data-ttu-id="9e32d-251">Url do registro do MDM</span><span class="sxs-lookup"><span data-stu-id="9e32d-251">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="9e32d-252">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="9e32d-252">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="9e32d-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e32d-253">Boolean</span></span>|<span data-ttu-id="9e32d-254">Valor booliano que define o Windows Hello para Empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="9e32d-254">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="9e32d-255">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9e32d-255">pinMinimumLength</span></span>|<span data-ttu-id="9e32d-256">Int32</span><span class="sxs-lookup"><span data-stu-id="9e32d-256">Int32</span></span>|<span data-ttu-id="9e32d-257">Valor inteiro que define o número mínimo de caracteres necessários para o PIN.</span><span class="sxs-lookup"><span data-stu-id="9e32d-257">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="9e32d-258">O valor padrão é 4.</span><span class="sxs-lookup"><span data-stu-id="9e32d-258">Default value is 4.</span></span> <span data-ttu-id="9e32d-259">O menor número que é possível definir para essa configuração de política é 4.</span><span class="sxs-lookup"><span data-stu-id="9e32d-259">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="9e32d-260">O maior número que é possível definir deve ser menor que o número configurado na política de comprimento máximo do PIN ou menor que 127, seja qual for o menor.</span><span class="sxs-lookup"><span data-stu-id="9e32d-260">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="9e32d-261">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="9e32d-261">pinUppercaseLetters</span></span>|[<span data-ttu-id="9e32d-262">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="9e32d-262">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="9e32d-263">Valor inteiro que configura o uso de letras maiúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="9e32d-263">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9e32d-264">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="9e32d-264">Default is NotAllow.</span></span> <span data-ttu-id="9e32d-265">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="9e32d-265">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="9e32d-266">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="9e32d-266">pinLowercaseLetters</span></span>|[<span data-ttu-id="9e32d-267">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="9e32d-267">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="9e32d-268">Valor inteiro que configura o uso de letras minúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="9e32d-268">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9e32d-269">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="9e32d-269">Default is NotAllow.</span></span> <span data-ttu-id="9e32d-270">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="9e32d-270">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="9e32d-271">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="9e32d-271">pinSpecialCharacters</span></span>|[<span data-ttu-id="9e32d-272">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="9e32d-272">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="9e32d-273">Valor inteiro que configura o uso de caracteres especiais no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="9e32d-273">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9e32d-274">Os caracteres especiais válidos para o PIN do Windows Hello para Empresas incluem: !</span><span class="sxs-lookup"><span data-stu-id="9e32d-274">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="9e32d-275">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="9e32d-275">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="9e32d-276">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="9e32d-276">/ : ; < = > ?</span></span><span data-ttu-id="9e32d-277"> @ \[ \ \] ^ _ \` {</span><span class="sxs-lookup"><span data-stu-id="9e32d-277"> @ \[ \ \] ^ _ \` {</span></span> | <span data-ttu-id="9e32d-278">} ~.</span><span class="sxs-lookup"><span data-stu-id="9e32d-278">} ~.</span></span> <span data-ttu-id="9e32d-279">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="9e32d-279">Default is NotAllow.</span></span> <span data-ttu-id="9e32d-280">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="9e32d-280">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="9e32d-281">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9e32d-281">pinExpirationDays</span></span>|<span data-ttu-id="9e32d-282">Int32</span><span class="sxs-lookup"><span data-stu-id="9e32d-282">Int32</span></span>|<span data-ttu-id="9e32d-283">O valor inteiro especifica o período de tempo (em dias) em que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="9e32d-283">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="9e32d-284">O maior número que é possível definir para essa configuração de política é 730.</span><span class="sxs-lookup"><span data-stu-id="9e32d-284">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="9e32d-285">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="9e32d-285">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="9e32d-286">Se essa política for definida como 0, o PIN do usuário nunca irá expirar.</span><span class="sxs-lookup"><span data-stu-id="9e32d-286">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="9e32d-287">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="9e32d-287">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="9e32d-288">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="9e32d-288">Default is 0.</span></span>|
|<span data-ttu-id="9e32d-289">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="9e32d-289">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="9e32d-290">Int32</span><span class="sxs-lookup"><span data-stu-id="9e32d-290">Int32</span></span>|<span data-ttu-id="9e32d-291">O valor inteiro que especifica o número de PINs anteriores que podem ser associados a uma conta de usuário que não podem ser reutilizados.</span><span class="sxs-lookup"><span data-stu-id="9e32d-291">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="9e32d-292">O maior número que é possível definir para essa configuração de política é 50.</span><span class="sxs-lookup"><span data-stu-id="9e32d-292">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="9e32d-293">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="9e32d-293">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="9e32d-294">Se essa política for definida como 0, o armazenamento de PINs anteriores não será necessário.</span><span class="sxs-lookup"><span data-stu-id="9e32d-294">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="9e32d-295">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="9e32d-295">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="9e32d-296">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="9e32d-296">Default is 0.</span></span>|
|<span data-ttu-id="9e32d-297">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="9e32d-297">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="9e32d-298">Int32</span><span class="sxs-lookup"><span data-stu-id="9e32d-298">Int32</span></span>|<span data-ttu-id="9e32d-299">O número de falhas de autenticação permitido antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="9e32d-299">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="9e32d-300">O valor 0 desabilita a funcionalidade de apagamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e32d-300">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="9e32d-301">O intervalo é um inteiro X, em que 4 <= X <= 16 para desktop e 0 <= X <= 999 para dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="9e32d-301">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="9e32d-302">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="9e32d-302">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="9e32d-303">Int32</span><span class="sxs-lookup"><span data-stu-id="9e32d-303">Int32</span></span>|<span data-ttu-id="9e32d-304">Especifica a quantidade máxima de tempo (em minutos) permitida após o dispositivo ficar ocioso antes que ele seja bloqueado por PIN ou senha.</span><span class="sxs-lookup"><span data-stu-id="9e32d-304">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="9e32d-305">O intervalo é um inteiro X, em que 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="9e32d-305">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="9e32d-306">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="9e32d-306">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="9e32d-307">Int32</span><span class="sxs-lookup"><span data-stu-id="9e32d-307">Int32</span></span>|<span data-ttu-id="9e32d-308">Intervalo offline antes do apagamento dos dados do aplicativo (dias)</span><span class="sxs-lookup"><span data-stu-id="9e32d-308">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="9e32d-309">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e32d-309">Response</span></span>
<span data-ttu-id="9e32d-310">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e32d-310">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e32d-311">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e32d-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e32d-312">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e32d-312">Request</span></span>
<span data-ttu-id="9e32d-313">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e32d-313">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4469

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

### <a name="response"></a><span data-ttu-id="9e32d-314">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e32d-314">Response</span></span>
<span data-ttu-id="9e32d-p132">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e32d-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4577

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





