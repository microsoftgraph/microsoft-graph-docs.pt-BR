---
title: Atualizar mdmWindowsInformationProtectionPolicy
description: Atualizar as propriedades de um objeto mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9602d21cf0f9fe79902d1f47f36baa551f955e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353894"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="453cb-103">Atualizar mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="453cb-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="453cb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="453cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="453cb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="453cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="453cb-106">Atualizar as propriedades de um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="453cb-106">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="453cb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="453cb-107">Prerequisites</span></span>
<span data-ttu-id="453cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="453cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="453cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="453cb-110">Permission type</span></span>|<span data-ttu-id="453cb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="453cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="453cb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="453cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="453cb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="453cb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="453cb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="453cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="453cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="453cb-115">Not supported.</span></span>|
|<span data-ttu-id="453cb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="453cb-116">Application</span></span>|<span data-ttu-id="453cb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="453cb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="453cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="453cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="453cb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="453cb-119">Request headers</span></span>
|<span data-ttu-id="453cb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="453cb-120">Header</span></span>|<span data-ttu-id="453cb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="453cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="453cb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="453cb-122">Authorization</span></span>|<span data-ttu-id="453cb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="453cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="453cb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="453cb-124">Accept</span></span>|<span data-ttu-id="453cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="453cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="453cb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="453cb-126">Request body</span></span>
<span data-ttu-id="453cb-127">No corpo da solicitação, forneça uma representação JSON do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="453cb-127">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="453cb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="453cb-128">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="453cb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="453cb-129">Property</span></span>|<span data-ttu-id="453cb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="453cb-130">Type</span></span>|<span data-ttu-id="453cb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="453cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="453cb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="453cb-132">displayName</span></span>|<span data-ttu-id="453cb-133">String</span><span class="sxs-lookup"><span data-stu-id="453cb-133">String</span></span>|<span data-ttu-id="453cb-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="453cb-134">Policy display name.</span></span> <span data-ttu-id="453cb-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="453cb-136">descrição</span><span class="sxs-lookup"><span data-stu-id="453cb-136">description</span></span>|<span data-ttu-id="453cb-137">String</span><span class="sxs-lookup"><span data-stu-id="453cb-137">String</span></span>|<span data-ttu-id="453cb-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="453cb-138">The policy's description.</span></span> <span data-ttu-id="453cb-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="453cb-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="453cb-140">createdDateTime</span></span>|<span data-ttu-id="453cb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="453cb-141">DateTimeOffset</span></span>|<span data-ttu-id="453cb-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="453cb-142">The date and time the policy was created.</span></span> <span data-ttu-id="453cb-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="453cb-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="453cb-144">lastModifiedDateTime</span></span>|<span data-ttu-id="453cb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="453cb-145">DateTimeOffset</span></span>|<span data-ttu-id="453cb-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="453cb-146">Last time the policy was modified.</span></span> <span data-ttu-id="453cb-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="453cb-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="453cb-148">roleScopeTagIds</span></span>|<span data-ttu-id="453cb-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="453cb-149">String collection</span></span>|<span data-ttu-id="453cb-150">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="453cb-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="453cb-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="453cb-152">id</span><span class="sxs-lookup"><span data-stu-id="453cb-152">id</span></span>|<span data-ttu-id="453cb-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="453cb-153">String</span></span>|<span data-ttu-id="453cb-154">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="453cb-154">Key of the entity.</span></span> <span data-ttu-id="453cb-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="453cb-156">version</span><span class="sxs-lookup"><span data-stu-id="453cb-156">version</span></span>|<span data-ttu-id="453cb-157">String</span><span class="sxs-lookup"><span data-stu-id="453cb-157">String</span></span>|<span data-ttu-id="453cb-158">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="453cb-158">Version of the entity.</span></span> <span data-ttu-id="453cb-159">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="453cb-160">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="453cb-160">enforcementLevel</span></span>|[<span data-ttu-id="453cb-161">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="453cb-161">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="453cb-162">Nível de imposição WIP. Confira a definição de enumeração para valores suportados herdados de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="453cb-162">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="453cb-163">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="453cb-163">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="453cb-164">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="453cb-164">enterpriseDomain</span></span>|<span data-ttu-id="453cb-165">String</span><span class="sxs-lookup"><span data-stu-id="453cb-165">String</span></span>|<span data-ttu-id="453cb-166">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-166">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-167">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="453cb-167">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="453cb-168">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-168">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="453cb-169">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-169">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-170">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="453cb-170">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="453cb-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="453cb-171">Boolean</span></span>|<span data-ttu-id="453cb-172">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-172">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-173">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="453cb-173">dataRecoveryCertificate</span></span>|[<span data-ttu-id="453cb-174">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="453cb-174">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="453cb-175">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="453cb-175">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="453cb-176">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-176">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-177">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="453cb-177">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="453cb-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="453cb-178">Boolean</span></span>|<span data-ttu-id="453cb-179">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="453cb-179">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="453cb-180">Se definido como 1 (não revogar teclas), as teclas não serão revogadas e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="453cb-180">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="453cb-181">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="453cb-181">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="453cb-182">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-182">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-183">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="453cb-183">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="453cb-184">Guid</span><span class="sxs-lookup"><span data-stu-id="453cb-184">Guid</span></span>|<span data-ttu-id="453cb-185">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="453cb-185">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="453cb-186">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-186">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-187">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="453cb-187">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="453cb-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="453cb-188">Boolean</span></span>|<span data-ttu-id="453cb-189">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-189">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-190">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="453cb-190">iconsVisible</span></span>|<span data-ttu-id="453cb-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="453cb-191">Boolean</span></span>|<span data-ttu-id="453cb-192">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="453cb-192">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="453cb-193">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-193">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-194">protectedApps</span><span class="sxs-lookup"><span data-stu-id="453cb-194">protectedApps</span></span>|<span data-ttu-id="453cb-195">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="453cb-196">Os aplicativos protegidos podem acessar dados corporativos e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-196">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-197">exemptApps</span><span class="sxs-lookup"><span data-stu-id="453cb-197">exemptApps</span></span>|<span data-ttu-id="453cb-198">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-198">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="453cb-199">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="453cb-199">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="453cb-200">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="453cb-200">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="453cb-201">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-201">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-202">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="453cb-202">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="453cb-203">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-203">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="453cb-204">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="453cb-204">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="453cb-205">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-205">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-206">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="453cb-206">enterpriseProxiedDomains</span></span>|<span data-ttu-id="453cb-207">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-207">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="453cb-208">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="453cb-208">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="453cb-209">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="453cb-209">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="453cb-210">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="453cb-210">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="453cb-211">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-211">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-212">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="453cb-212">enterpriseIPRanges</span></span>|<span data-ttu-id="453cb-213">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-213">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="453cb-214">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="453cb-214">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="453cb-215">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="453cb-215">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="453cb-216">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-216">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-217">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="453cb-217">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="453cb-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="453cb-218">Boolean</span></span>|<span data-ttu-id="453cb-219">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="453cb-219">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="453cb-220">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-220">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-221">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="453cb-221">enterpriseProxyServers</span></span>|<span data-ttu-id="453cb-222">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="453cb-223">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="453cb-223">This is a list of proxy servers.</span></span> <span data-ttu-id="453cb-224">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-224">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-225">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="453cb-225">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="453cb-226">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-226">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="453cb-227">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="453cb-227">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="453cb-228">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="453cb-228">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="453cb-229">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="453cb-229">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="453cb-230">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="453cb-230">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="453cb-231">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-231">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-232">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="453cb-232">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="453cb-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="453cb-233">Boolean</span></span>|<span data-ttu-id="453cb-234">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="453cb-234">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="453cb-235">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-235">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-236">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="453cb-236">neutralDomainResources</span></span>|<span data-ttu-id="453cb-237">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-237">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="453cb-238">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-238">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-239">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="453cb-239">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="453cb-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="453cb-240">Boolean</span></span>|<span data-ttu-id="453cb-241">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-241">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-242">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="453cb-242">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="453cb-243">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-243">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="453cb-244">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-244">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="453cb-245">isAssigned</span><span class="sxs-lookup"><span data-stu-id="453cb-245">isAssigned</span></span>|<span data-ttu-id="453cb-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="453cb-246">Boolean</span></span>|<span data-ttu-id="453cb-247">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="453cb-247">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="453cb-248">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="453cb-248">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="453cb-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="453cb-249">Response</span></span>
<span data-ttu-id="453cb-250">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="453cb-250">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="453cb-251">Exemplo</span><span class="sxs-lookup"><span data-stu-id="453cb-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="453cb-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="453cb-252">Request</span></span>
<span data-ttu-id="453cb-253">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="453cb-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 3967

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="453cb-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="453cb-254">Response</span></span>
<span data-ttu-id="453cb-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="453cb-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4139

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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






