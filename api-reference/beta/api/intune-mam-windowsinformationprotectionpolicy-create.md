---
title: Criar windowsInformationProtectionPolicy
description: Cria um novo objeto windowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e92d2a90366b265065f2c480b90234e478be05aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462870"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="8c80b-103">Criar windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8c80b-103">Create windowsInformationProtectionPolicy</span></span>

<span data-ttu-id="8c80b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c80b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c80b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c80b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c80b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c80b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c80b-107">Cria um novo objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c80b-107">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c80b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c80b-108">Prerequisites</span></span>
<span data-ttu-id="8c80b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c80b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c80b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c80b-111">Permission type</span></span>|<span data-ttu-id="8c80b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c80b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c80b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c80b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c80b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c80b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c80b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c80b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c80b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c80b-116">Not supported.</span></span>|
|<span data-ttu-id="8c80b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c80b-117">Application</span></span>|<span data-ttu-id="8c80b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c80b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c80b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c80b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8c80b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c80b-120">Request headers</span></span>
|<span data-ttu-id="8c80b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c80b-121">Header</span></span>|<span data-ttu-id="8c80b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c80b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c80b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c80b-123">Authorization</span></span>|<span data-ttu-id="8c80b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c80b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c80b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c80b-125">Accept</span></span>|<span data-ttu-id="8c80b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c80b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c80b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c80b-127">Request body</span></span>
<span data-ttu-id="8c80b-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="8c80b-128">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="8c80b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="8c80b-129">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="8c80b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c80b-130">Property</span></span>|<span data-ttu-id="8c80b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c80b-131">Type</span></span>|<span data-ttu-id="8c80b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c80b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c80b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8c80b-133">displayName</span></span>|<span data-ttu-id="8c80b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c80b-134">String</span></span>|<span data-ttu-id="8c80b-135">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="8c80b-135">Policy display name.</span></span> <span data-ttu-id="8c80b-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c80b-137">description</span><span class="sxs-lookup"><span data-stu-id="8c80b-137">description</span></span>|<span data-ttu-id="8c80b-138">String</span><span class="sxs-lookup"><span data-stu-id="8c80b-138">String</span></span>|<span data-ttu-id="8c80b-139">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="8c80b-139">The policy's description.</span></span> <span data-ttu-id="8c80b-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c80b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c80b-141">createdDateTime</span></span>|<span data-ttu-id="8c80b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c80b-142">DateTimeOffset</span></span>|<span data-ttu-id="8c80b-143">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="8c80b-143">The date and time the policy was created.</span></span> <span data-ttu-id="8c80b-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c80b-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c80b-145">lastModifiedDateTime</span></span>|<span data-ttu-id="8c80b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c80b-146">DateTimeOffset</span></span>|<span data-ttu-id="8c80b-147">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="8c80b-147">Last time the policy was modified.</span></span> <span data-ttu-id="8c80b-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c80b-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8c80b-149">roleScopeTagIds</span></span>|<span data-ttu-id="8c80b-150">String collection</span><span class="sxs-lookup"><span data-stu-id="8c80b-150">String collection</span></span>|<span data-ttu-id="8c80b-151">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8c80b-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8c80b-152">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c80b-153">id</span><span class="sxs-lookup"><span data-stu-id="8c80b-153">id</span></span>|<span data-ttu-id="8c80b-154">String</span><span class="sxs-lookup"><span data-stu-id="8c80b-154">String</span></span>|<span data-ttu-id="8c80b-155">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c80b-155">Key of the entity.</span></span> <span data-ttu-id="8c80b-156">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c80b-157">version</span><span class="sxs-lookup"><span data-stu-id="8c80b-157">version</span></span>|<span data-ttu-id="8c80b-158">String</span><span class="sxs-lookup"><span data-stu-id="8c80b-158">String</span></span>|<span data-ttu-id="8c80b-159">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c80b-159">Version of the entity.</span></span> <span data-ttu-id="8c80b-160">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c80b-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="8c80b-161">enforcementLevel</span></span>|[<span data-ttu-id="8c80b-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="8c80b-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="8c80b-163">Nível de imposição WIP. Confira a definição de enumeração para valores suportados herdados de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8c80b-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="8c80b-164">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="8c80b-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="8c80b-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="8c80b-165">enterpriseDomain</span></span>|<span data-ttu-id="8c80b-166">String</span><span class="sxs-lookup"><span data-stu-id="8c80b-166">String</span></span>|<span data-ttu-id="8c80b-167">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="8c80b-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="8c80b-169">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c80b-170">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="8c80b-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="8c80b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c80b-172">Boolean</span></span>|<span data-ttu-id="8c80b-173">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8c80b-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="8c80b-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8c80b-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="8c80b-176">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="8c80b-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="8c80b-177">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="8c80b-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="8c80b-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c80b-179">Boolean</span></span>|<span data-ttu-id="8c80b-180">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="8c80b-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="8c80b-181">Se definido como 1 (não revogar teclas), as teclas não serão revogadas e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="8c80b-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="8c80b-182">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="8c80b-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="8c80b-183">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="8c80b-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="8c80b-185">Guid</span><span class="sxs-lookup"><span data-stu-id="8c80b-185">Guid</span></span>|<span data-ttu-id="8c80b-186">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="8c80b-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="8c80b-187">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="8c80b-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="8c80b-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c80b-189">Boolean</span></span>|<span data-ttu-id="8c80b-190">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="8c80b-191">iconsVisible</span></span>|<span data-ttu-id="8c80b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c80b-192">Boolean</span></span>|<span data-ttu-id="8c80b-193">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="8c80b-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="8c80b-194">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="8c80b-195">protectedApps</span></span>|<span data-ttu-id="8c80b-196">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="8c80b-197">Os aplicativos protegidos podem acessar dados corporativos e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="8c80b-198">exemptApps</span></span>|<span data-ttu-id="8c80b-199">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="8c80b-200">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="8c80b-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="8c80b-201">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="8c80b-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="8c80b-202">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="8c80b-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="8c80b-204">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c80b-205">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="8c80b-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="8c80b-206">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="8c80b-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="8c80b-208">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="8c80b-209">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="8c80b-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="8c80b-210">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="8c80b-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="8c80b-211">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="8c80b-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="8c80b-212">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="8c80b-213">enterpriseIPRanges</span></span>|<span data-ttu-id="8c80b-214">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="8c80b-215">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="8c80b-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="8c80b-216">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="8c80b-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="8c80b-217">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="8c80b-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="8c80b-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c80b-219">Boolean</span></span>|<span data-ttu-id="8c80b-220">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="8c80b-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="8c80b-221">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="8c80b-222">enterpriseProxyServers</span></span>|<span data-ttu-id="8c80b-223">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c80b-224">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="8c80b-224">This is a list of proxy servers.</span></span> <span data-ttu-id="8c80b-225">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="8c80b-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="8c80b-227">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c80b-228">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="8c80b-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="8c80b-229">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="8c80b-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="8c80b-230">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="8c80b-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="8c80b-231">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="8c80b-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="8c80b-232">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="8c80b-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="8c80b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c80b-234">Boolean</span></span>|<span data-ttu-id="8c80b-235">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8c80b-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="8c80b-236">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="8c80b-237">neutralDomainResources</span></span>|<span data-ttu-id="8c80b-238">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c80b-239">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="8c80b-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="8c80b-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c80b-241">Boolean</span></span>|<span data-ttu-id="8c80b-242">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="8c80b-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="8c80b-244">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="8c80b-245">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8c80b-246">isAssigned</span></span>|<span data-ttu-id="8c80b-247">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c80b-247">Boolean</span></span>|<span data-ttu-id="8c80b-248">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="8c80b-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="8c80b-249">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="8c80b-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="8c80b-250">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="8c80b-250">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="8c80b-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c80b-251">Boolean</span></span>|<span data-ttu-id="8c80b-252">Nova propriedade em RS2, documentação pendente</span><span class="sxs-lookup"><span data-stu-id="8c80b-252">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="8c80b-253">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="8c80b-253">mdmEnrollmentUrl</span></span>|<span data-ttu-id="8c80b-254">String</span><span class="sxs-lookup"><span data-stu-id="8c80b-254">String</span></span>|<span data-ttu-id="8c80b-255">Url do registro do MDM</span><span class="sxs-lookup"><span data-stu-id="8c80b-255">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="8c80b-256">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="8c80b-256">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="8c80b-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c80b-257">Boolean</span></span>|<span data-ttu-id="8c80b-258">Valor booliano que define o Windows Hello para Empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="8c80b-258">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="8c80b-259">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8c80b-259">pinMinimumLength</span></span>|<span data-ttu-id="8c80b-260">Int32</span><span class="sxs-lookup"><span data-stu-id="8c80b-260">Int32</span></span>|<span data-ttu-id="8c80b-261">Valor inteiro que define o número mínimo de caracteres necessários para o PIN.</span><span class="sxs-lookup"><span data-stu-id="8c80b-261">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="8c80b-262">O valor padrão é 4.</span><span class="sxs-lookup"><span data-stu-id="8c80b-262">Default value is 4.</span></span> <span data-ttu-id="8c80b-263">O menor número que é possível definir para essa configuração de política é 4.</span><span class="sxs-lookup"><span data-stu-id="8c80b-263">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="8c80b-264">O maior número que é possível definir deve ser menor que o número configurado na política de comprimento máximo do PIN ou menor que 127, seja qual for o menor.</span><span class="sxs-lookup"><span data-stu-id="8c80b-264">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="8c80b-265">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="8c80b-265">pinUppercaseLetters</span></span>|[<span data-ttu-id="8c80b-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="8c80b-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="8c80b-267">Valor inteiro que configura o uso de letras maiúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="8c80b-267">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="8c80b-268">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="8c80b-268">Default is NotAllow.</span></span> <span data-ttu-id="8c80b-269">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="8c80b-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="8c80b-270">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="8c80b-270">pinLowercaseLetters</span></span>|[<span data-ttu-id="8c80b-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="8c80b-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="8c80b-272">Valor inteiro que configura o uso de letras minúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="8c80b-272">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="8c80b-273">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="8c80b-273">Default is NotAllow.</span></span> <span data-ttu-id="8c80b-274">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="8c80b-274">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="8c80b-275">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="8c80b-275">pinSpecialCharacters</span></span>|[<span data-ttu-id="8c80b-276">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="8c80b-276">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="8c80b-277">Valor inteiro que configura o uso de caracteres especiais no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="8c80b-277">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="8c80b-278">Os caracteres especiais válidos para o PIN do Windows Hello para Empresas incluem: !</span><span class="sxs-lookup"><span data-stu-id="8c80b-278">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="8c80b-279">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="8c80b-279">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="8c80b-280">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="8c80b-280">/ : ; < = > ?</span></span><span data-ttu-id="8c80b-281"> @ \[ \ \]^ _ ` { | } ~. Default is NotAllow. Possible values are: `permitir`, `requireAtLeastOne`, `permitido '.</span><span class="sxs-lookup"><span data-stu-id="8c80b-281"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allo\w`.</span></span>|
|<span data-ttu-id="8c80b-282">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8c80b-282">pinExpirationDays</span></span>|<span data-ttu-id="8c80b-283">Int32</span><span class="sxs-lookup"><span data-stu-id="8c80b-283">Int32</span></span>|<span data-ttu-id="8c80b-284">O valor inteiro especifica o período de tempo (em dias) em que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="8c80b-284">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="8c80b-285">O maior número que é possível definir para essa configuração de política é 730.</span><span class="sxs-lookup"><span data-stu-id="8c80b-285">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="8c80b-286">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="8c80b-286">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="8c80b-287">Se essa política for definida como 0, o PIN do usuário nunca irá expirar.</span><span class="sxs-lookup"><span data-stu-id="8c80b-287">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="8c80b-288">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="8c80b-288">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="8c80b-289">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="8c80b-289">Default is 0.</span></span>|
|<span data-ttu-id="8c80b-290">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="8c80b-290">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="8c80b-291">Int32</span><span class="sxs-lookup"><span data-stu-id="8c80b-291">Int32</span></span>|<span data-ttu-id="8c80b-292">O valor inteiro que especifica o número de PINs anteriores que podem ser associados a uma conta de usuário que não podem ser reutilizados.</span><span class="sxs-lookup"><span data-stu-id="8c80b-292">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="8c80b-293">O maior número que é possível definir para essa configuração de política é 50.</span><span class="sxs-lookup"><span data-stu-id="8c80b-293">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="8c80b-294">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="8c80b-294">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="8c80b-295">Se essa política for definida como 0, o armazenamento de PINs anteriores não será necessário.</span><span class="sxs-lookup"><span data-stu-id="8c80b-295">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="8c80b-296">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="8c80b-296">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="8c80b-297">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="8c80b-297">Default is 0.</span></span>|
|<span data-ttu-id="8c80b-298">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="8c80b-298">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="8c80b-299">Int32</span><span class="sxs-lookup"><span data-stu-id="8c80b-299">Int32</span></span>|<span data-ttu-id="8c80b-300">O número de falhas de autenticação permitido antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="8c80b-300">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="8c80b-301">O valor 0 desabilita a funcionalidade de apagamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c80b-301">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="8c80b-302">O intervalo é um inteiro X, em que 4 <= X <= 16 para desktop e 0 <= X <= 999 para dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="8c80b-302">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="8c80b-303">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="8c80b-303">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="8c80b-304">Int32</span><span class="sxs-lookup"><span data-stu-id="8c80b-304">Int32</span></span>|<span data-ttu-id="8c80b-305">Especifica a quantidade máxima de tempo (em minutos) permitida após o dispositivo ficar ocioso antes que ele seja bloqueado por PIN ou senha.</span><span class="sxs-lookup"><span data-stu-id="8c80b-305">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="8c80b-306">O intervalo é um inteiro X, em que 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="8c80b-306">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="8c80b-307">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="8c80b-307">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="8c80b-308">Int32</span><span class="sxs-lookup"><span data-stu-id="8c80b-308">Int32</span></span>|<span data-ttu-id="8c80b-309">Intervalo offline antes do apagamento dos dados do aplicativo (dias)</span><span class="sxs-lookup"><span data-stu-id="8c80b-309">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="8c80b-310">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c80b-310">Response</span></span>
<span data-ttu-id="8c80b-311">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c80b-311">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c80b-312">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c80b-312">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c80b-313">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c80b-313">Request</span></span>
<span data-ttu-id="8c80b-314">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c80b-314">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4467

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
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

### <a name="response"></a><span data-ttu-id="8c80b-315">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c80b-315">Response</span></span>
<span data-ttu-id="8c80b-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c80b-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4639

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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





