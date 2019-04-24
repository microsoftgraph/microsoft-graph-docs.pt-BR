---
title: Criar windowsInformationProtectionPolicy
description: Cria um novo objeto windowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6595d126447db628b447fd94d5d33260ffd0290
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453557"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="6f1d6-103">Criar windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="6f1d6-103">Create windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="6f1d6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f1d6-105">Cria um novo objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6f1d6-105">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f1d6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f1d6-106">Prerequisites</span></span>
<span data-ttu-id="6f1d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f1d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f1d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f1d6-109">Permission type</span></span>|<span data-ttu-id="6f1d6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f1d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f1d6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f1d6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6f1d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f1d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-114">Not supported.</span></span>|
|<span data-ttu-id="6f1d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f1d6-115">Application</span></span>|<span data-ttu-id="6f1d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f1d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f1d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="6f1d6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f1d6-118">Request headers</span></span>
|<span data-ttu-id="6f1d6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f1d6-119">Header</span></span>|<span data-ttu-id="6f1d6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6f1d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f1d6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f1d6-121">Authorization</span></span>|<span data-ttu-id="6f1d6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f1d6-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f1d6-123">Accept</span></span>|<span data-ttu-id="6f1d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f1d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f1d6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f1d6-125">Request body</span></span>
<span data-ttu-id="6f1d6-126">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-126">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="6f1d6-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-127">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="6f1d6-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f1d6-128">Property</span></span>|<span data-ttu-id="6f1d6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f1d6-129">Type</span></span>|<span data-ttu-id="6f1d6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f1d6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f1d6-131">displayName</span><span class="sxs-lookup"><span data-stu-id="6f1d6-131">displayName</span></span>|<span data-ttu-id="6f1d6-132">String</span><span class="sxs-lookup"><span data-stu-id="6f1d6-132">String</span></span>|<span data-ttu-id="6f1d6-133">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-133">Policy display name.</span></span> <span data-ttu-id="6f1d6-134">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6f1d6-135">description</span><span class="sxs-lookup"><span data-stu-id="6f1d6-135">description</span></span>|<span data-ttu-id="6f1d6-136">String</span><span class="sxs-lookup"><span data-stu-id="6f1d6-136">String</span></span>|<span data-ttu-id="6f1d6-137">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-137">The policy's description.</span></span> <span data-ttu-id="6f1d6-138">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6f1d6-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f1d6-139">createdDateTime</span></span>|<span data-ttu-id="6f1d6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f1d6-140">DateTimeOffset</span></span>|<span data-ttu-id="6f1d6-141">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-141">The date and time the policy was created.</span></span> <span data-ttu-id="6f1d6-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6f1d6-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f1d6-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6f1d6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f1d6-144">DateTimeOffset</span></span>|<span data-ttu-id="6f1d6-145">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-145">Last time the policy was modified.</span></span> <span data-ttu-id="6f1d6-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6f1d6-147">id</span><span class="sxs-lookup"><span data-stu-id="6f1d6-147">id</span></span>|<span data-ttu-id="6f1d6-148">String</span><span class="sxs-lookup"><span data-stu-id="6f1d6-148">String</span></span>|<span data-ttu-id="6f1d6-149">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-149">Key of the entity.</span></span> <span data-ttu-id="6f1d6-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6f1d6-151">version</span><span class="sxs-lookup"><span data-stu-id="6f1d6-151">version</span></span>|<span data-ttu-id="6f1d6-152">String</span><span class="sxs-lookup"><span data-stu-id="6f1d6-152">String</span></span>|<span data-ttu-id="6f1d6-153">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-153">Version of the entity.</span></span> <span data-ttu-id="6f1d6-154">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6f1d6-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="6f1d6-155">enforcementLevel</span></span>|[<span data-ttu-id="6f1d6-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="6f1d6-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="6f1d6-157">Nível de imposição WIP. ConFira a definição de enumeração para valores suportados herdados de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="6f1d6-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="6f1d6-158">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="6f1d6-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="6f1d6-159">enterpriseDomain</span></span>|<span data-ttu-id="6f1d6-160">String</span><span class="sxs-lookup"><span data-stu-id="6f1d6-160">String</span></span>|<span data-ttu-id="6f1d6-161">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="6f1d6-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="6f1d6-163">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6f1d6-164">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="6f1d6-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="6f1d6-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1d6-166">Boolean</span></span>|<span data-ttu-id="6f1d6-167">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="6f1d6-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="6f1d6-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="6f1d6-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="6f1d6-170">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="6f1d6-171">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="6f1d6-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="6f1d6-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1d6-173">Boolean</span></span>|<span data-ttu-id="6f1d6-174">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="6f1d6-175">Se definido como 1 (não revogar teclas), as teclas não serão revogadas e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="6f1d6-176">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="6f1d6-177">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="6f1d6-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="6f1d6-179">Guid</span><span class="sxs-lookup"><span data-stu-id="6f1d6-179">Guid</span></span>|<span data-ttu-id="6f1d6-180">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="6f1d6-181">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="6f1d6-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="6f1d6-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f1d6-183">Boolean</span></span>|<span data-ttu-id="6f1d6-184">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="6f1d6-185">iconsVisible</span></span>|<span data-ttu-id="6f1d6-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1d6-186">Boolean</span></span>|<span data-ttu-id="6f1d6-187">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="6f1d6-188">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="6f1d6-189">protectedApps</span></span>|<span data-ttu-id="6f1d6-190">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="6f1d6-191">Os aplicativos protegidos podem acessar dados corporativos e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="6f1d6-192">exemptApps</span></span>|<span data-ttu-id="6f1d6-193">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="6f1d6-194">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="6f1d6-195">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="6f1d6-196">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="6f1d6-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="6f1d6-198">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6f1d6-199">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="6f1d6-200">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="6f1d6-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="6f1d6-202">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="6f1d6-203">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="6f1d6-204">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="6f1d6-205">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="6f1d6-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="6f1d6-206">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="6f1d6-207">enterpriseIPRanges</span></span>|<span data-ttu-id="6f1d6-208">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="6f1d6-209">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="6f1d6-210">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="6f1d6-211">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="6f1d6-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="6f1d6-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1d6-213">Boolean</span></span>|<span data-ttu-id="6f1d6-214">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="6f1d6-215">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="6f1d6-216">enterpriseProxyServers</span></span>|<span data-ttu-id="6f1d6-217">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6f1d6-218">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-218">This is a list of proxy servers.</span></span> <span data-ttu-id="6f1d6-219">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="6f1d6-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="6f1d6-221">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6f1d6-222">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="6f1d6-223">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="6f1d6-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="6f1d6-224">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="6f1d6-225">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="6f1d6-226">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="6f1d6-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="6f1d6-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1d6-228">Boolean</span></span>|<span data-ttu-id="6f1d6-229">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="6f1d6-230">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="6f1d6-231">neutralDomainResources</span></span>|<span data-ttu-id="6f1d6-232">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6f1d6-233">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="6f1d6-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="6f1d6-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1d6-235">Boolean</span></span>|<span data-ttu-id="6f1d6-236">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="6f1d6-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="6f1d6-238">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="6f1d6-239">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6f1d6-240">isAssigned</span></span>|<span data-ttu-id="6f1d6-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f1d6-241">Boolean</span></span>|<span data-ttu-id="6f1d6-242">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="6f1d6-243">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="6f1d6-244">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="6f1d6-244">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="6f1d6-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1d6-245">Boolean</span></span>|<span data-ttu-id="6f1d6-246">Nova propriedade em RS2, documentação pendente</span><span class="sxs-lookup"><span data-stu-id="6f1d6-246">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="6f1d6-247">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="6f1d6-247">mdmEnrollmentUrl</span></span>|<span data-ttu-id="6f1d6-248">String</span><span class="sxs-lookup"><span data-stu-id="6f1d6-248">String</span></span>|<span data-ttu-id="6f1d6-249">Url do registro do MDM</span><span class="sxs-lookup"><span data-stu-id="6f1d6-249">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="6f1d6-250">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="6f1d6-250">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="6f1d6-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1d6-251">Boolean</span></span>|<span data-ttu-id="6f1d6-252">Valor booliano que define o Windows Hello para Empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-252">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="6f1d6-253">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6f1d6-253">pinMinimumLength</span></span>|<span data-ttu-id="6f1d6-254">Int32</span><span class="sxs-lookup"><span data-stu-id="6f1d6-254">Int32</span></span>|<span data-ttu-id="6f1d6-255">Valor inteiro que define o número mínimo de caracteres necessários para o PIN.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-255">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="6f1d6-256">O valor padrão é 4.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-256">Default value is 4.</span></span> <span data-ttu-id="6f1d6-257">O menor número que é possível definir para essa configuração de política é 4.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-257">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="6f1d6-258">O maior número que é possível definir deve ser menor que o número configurado na política de comprimento máximo do PIN ou menor que 127, seja qual for o menor.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-258">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="6f1d6-259">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="6f1d6-259">pinUppercaseLetters</span></span>|[<span data-ttu-id="6f1d6-260">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="6f1d6-260">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="6f1d6-261">Valor inteiro que configura o uso de letras maiúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-261">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="6f1d6-262">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-262">Default is NotAllow.</span></span> <span data-ttu-id="6f1d6-263">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-263">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="6f1d6-264">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="6f1d6-264">pinLowercaseLetters</span></span>|[<span data-ttu-id="6f1d6-265">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="6f1d6-265">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="6f1d6-266">Valor inteiro que configura o uso de letras minúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-266">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="6f1d6-267">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-267">Default is NotAllow.</span></span> <span data-ttu-id="6f1d6-268">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-268">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="6f1d6-269">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="6f1d6-269">pinSpecialCharacters</span></span>|[<span data-ttu-id="6f1d6-270">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="6f1d6-270">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="6f1d6-271">Valor inteiro que configura o uso de caracteres especiais no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-271">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="6f1d6-272">Os caracteres especiais válidos para o PIN do Windows Hello para Empresas incluem: !</span><span class="sxs-lookup"><span data-stu-id="6f1d6-272">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="6f1d6-273">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="6f1d6-273">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="6f1d6-274">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="6f1d6-274">/ : ; < = > ?</span></span><span data-ttu-id="6f1d6-275"> @ \[ \ \]^ _ ` { | } ~. Default is NotAllow. Possible values are: \`permitir`, \`requireAtLeastOne`, \`permitido '.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-275"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: \`notAllow`, \`requireAtLeastOne`, \`allow\`.</span></span>|
|<span data-ttu-id="6f1d6-276">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6f1d6-276">pinExpirationDays</span></span>|<span data-ttu-id="6f1d6-277">Int32</span><span class="sxs-lookup"><span data-stu-id="6f1d6-277">Int32</span></span>|<span data-ttu-id="6f1d6-278">O valor inteiro especifica o período de tempo (em dias) em que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-278">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="6f1d6-279">O maior número que é possível definir para essa configuração de política é 730.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-279">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="6f1d6-280">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-280">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="6f1d6-281">Se essa política for definida como 0, o PIN do usuário nunca irá expirar.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-281">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="6f1d6-282">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-282">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="6f1d6-283">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-283">Default is 0.</span></span>|
|<span data-ttu-id="6f1d6-284">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="6f1d6-284">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="6f1d6-285">Int32</span><span class="sxs-lookup"><span data-stu-id="6f1d6-285">Int32</span></span>|<span data-ttu-id="6f1d6-286">O valor inteiro que especifica o número de PINs anteriores que podem ser associados a uma conta de usuário que não podem ser reutilizados.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-286">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="6f1d6-287">O maior número que é possível definir para essa configuração de política é 50.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-287">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="6f1d6-288">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-288">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="6f1d6-289">Se essa política for definida como 0, o armazenamento de PINs anteriores não será necessário.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-289">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="6f1d6-290">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-290">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="6f1d6-291">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-291">Default is 0.</span></span>|
|<span data-ttu-id="6f1d6-292">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="6f1d6-292">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="6f1d6-293">Int32</span><span class="sxs-lookup"><span data-stu-id="6f1d6-293">Int32</span></span>|<span data-ttu-id="6f1d6-294">O número de falhas de autenticação permitido antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-294">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="6f1d6-295">O valor 0 desabilita a funcionalidade de apagamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-295">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="6f1d6-296">O intervalo é um inteiro X, em que 4 <= X <= 16 para desktop e 0 <= X <= 999 para dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-296">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="6f1d6-297">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="6f1d6-297">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="6f1d6-298">Int32</span><span class="sxs-lookup"><span data-stu-id="6f1d6-298">Int32</span></span>|<span data-ttu-id="6f1d6-299">Especifica a quantidade máxima de tempo (em minutos) permitida após o dispositivo ficar ocioso antes que ele seja bloqueado por PIN ou senha.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-299">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="6f1d6-300">O intervalo é um inteiro X, em que 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-300">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="6f1d6-301">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="6f1d6-301">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="6f1d6-302">Int32</span><span class="sxs-lookup"><span data-stu-id="6f1d6-302">Int32</span></span>|<span data-ttu-id="6f1d6-303">Intervalo offline antes do apagamento dos dados do aplicativo (dias)</span><span class="sxs-lookup"><span data-stu-id="6f1d6-303">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="6f1d6-304">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f1d6-304">Response</span></span>
<span data-ttu-id="6f1d6-305">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-305">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f1d6-306">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f1d6-306">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f1d6-307">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f1d6-307">Request</span></span>
<span data-ttu-id="6f1d6-308">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-308">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4405

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
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

### <a name="response"></a><span data-ttu-id="6f1d6-309">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f1d6-309">Response</span></span>
<span data-ttu-id="6f1d6-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f1d6-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



