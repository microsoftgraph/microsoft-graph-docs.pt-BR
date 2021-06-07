---
title: Criar windowsInformationProtectionPolicy
description: Cria um novo objeto windowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32a6841ae42b038885e58005f3646d898219df3a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756916"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="c55f0-103">Criar windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c55f0-103">Create windowsInformationProtectionPolicy</span></span>

<span data-ttu-id="c55f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c55f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c55f0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c55f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c55f0-106">Cria um novo objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c55f0-106">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c55f0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c55f0-107">Prerequisites</span></span>
<span data-ttu-id="c55f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c55f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c55f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c55f0-110">Permission type</span></span>|<span data-ttu-id="c55f0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c55f0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c55f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c55f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c55f0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c55f0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c55f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c55f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c55f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c55f0-115">Not supported.</span></span>|
|<span data-ttu-id="c55f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c55f0-116">Application</span></span>|<span data-ttu-id="c55f0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c55f0-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c55f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c55f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c55f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c55f0-119">Request headers</span></span>
|<span data-ttu-id="c55f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c55f0-120">Header</span></span>|<span data-ttu-id="c55f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c55f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c55f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c55f0-122">Authorization</span></span>|<span data-ttu-id="c55f0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c55f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c55f0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c55f0-124">Accept</span></span>|<span data-ttu-id="c55f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c55f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c55f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c55f0-126">Request body</span></span>
<span data-ttu-id="c55f0-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="c55f0-127">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="c55f0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="c55f0-128">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="c55f0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c55f0-129">Property</span></span>|<span data-ttu-id="c55f0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c55f0-130">Type</span></span>|<span data-ttu-id="c55f0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c55f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c55f0-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c55f0-132">displayName</span></span>|<span data-ttu-id="c55f0-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c55f0-133">String</span></span>|<span data-ttu-id="c55f0-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="c55f0-134">Policy display name.</span></span> <span data-ttu-id="c55f0-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c55f0-136">descrição</span><span class="sxs-lookup"><span data-stu-id="c55f0-136">description</span></span>|<span data-ttu-id="c55f0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c55f0-137">String</span></span>|<span data-ttu-id="c55f0-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="c55f0-138">The policy's description.</span></span> <span data-ttu-id="c55f0-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c55f0-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c55f0-140">createdDateTime</span></span>|<span data-ttu-id="c55f0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c55f0-141">DateTimeOffset</span></span>|<span data-ttu-id="c55f0-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="c55f0-142">The date and time the policy was created.</span></span> <span data-ttu-id="c55f0-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c55f0-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c55f0-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c55f0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c55f0-145">DateTimeOffset</span></span>|<span data-ttu-id="c55f0-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="c55f0-146">Last time the policy was modified.</span></span> <span data-ttu-id="c55f0-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c55f0-148">id</span><span class="sxs-lookup"><span data-stu-id="c55f0-148">id</span></span>|<span data-ttu-id="c55f0-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c55f0-149">String</span></span>|<span data-ttu-id="c55f0-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c55f0-150">Key of the entity.</span></span> <span data-ttu-id="c55f0-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c55f0-152">version</span><span class="sxs-lookup"><span data-stu-id="c55f0-152">version</span></span>|<span data-ttu-id="c55f0-153">String</span><span class="sxs-lookup"><span data-stu-id="c55f0-153">String</span></span>|<span data-ttu-id="c55f0-154">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="c55f0-154">Version of the entity.</span></span> <span data-ttu-id="c55f0-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c55f0-156">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="c55f0-156">enforcementLevel</span></span>|[<span data-ttu-id="c55f0-157">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="c55f0-157">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="c55f0-158">Nível de aplicação da WIP. Consulte a definição Enum para valores com suporte Herdados de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="c55f0-158">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="c55f0-159">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="c55f0-159">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="c55f0-160">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="c55f0-160">enterpriseDomain</span></span>|<span data-ttu-id="c55f0-161">String</span><span class="sxs-lookup"><span data-stu-id="c55f0-161">String</span></span>|<span data-ttu-id="c55f0-162">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-162">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-163">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="c55f0-163">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="c55f0-164">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-164">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c55f0-165">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-165">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-166">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="c55f0-166">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="c55f0-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-167">Boolean</span></span>|<span data-ttu-id="c55f0-168">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-168">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-169">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="c55f0-169">dataRecoveryCertificate</span></span>|[<span data-ttu-id="c55f0-170">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="c55f0-170">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="c55f0-171">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="c55f0-171">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="c55f0-172">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-172">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-173">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="c55f0-173">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="c55f0-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-174">Boolean</span></span>|<span data-ttu-id="c55f0-175">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c55f0-175">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="c55f0-176">Se definido como 1 (não revogar teclas), as teclas não serão revogadas e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="c55f0-176">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="c55f0-177">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="c55f0-177">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="c55f0-178">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-178">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-179">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="c55f0-179">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="c55f0-180">Guid</span><span class="sxs-lookup"><span data-stu-id="c55f0-180">Guid</span></span>|<span data-ttu-id="c55f0-181">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="c55f0-181">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="c55f0-182">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-182">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-183">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="c55f0-183">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="c55f0-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-184">Boolean</span></span>|<span data-ttu-id="c55f0-185">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-185">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-186">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="c55f0-186">iconsVisible</span></span>|<span data-ttu-id="c55f0-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-187">Boolean</span></span>|<span data-ttu-id="c55f0-188">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="c55f0-188">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="c55f0-189">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-189">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-190">protectedApps</span><span class="sxs-lookup"><span data-stu-id="c55f0-190">protectedApps</span></span>|<span data-ttu-id="c55f0-191">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="c55f0-192">Os aplicativos protegidos podem acessar dados corporativos e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-192">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-193">exemptApps</span><span class="sxs-lookup"><span data-stu-id="c55f0-193">exemptApps</span></span>|<span data-ttu-id="c55f0-194">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="c55f0-195">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="c55f0-195">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="c55f0-196">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="c55f0-196">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="c55f0-197">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-197">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-198">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="c55f0-198">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="c55f0-199">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-199">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c55f0-200">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="c55f0-200">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="c55f0-201">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-201">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-202">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="c55f0-202">enterpriseProxiedDomains</span></span>|<span data-ttu-id="c55f0-203">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-203">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="c55f0-204">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="c55f0-204">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="c55f0-205">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="c55f0-205">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="c55f0-206">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="c55f0-206">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="c55f0-207">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-207">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-208">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="c55f0-208">enterpriseIPRanges</span></span>|<span data-ttu-id="c55f0-209">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-209">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="c55f0-210">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="c55f0-210">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="c55f0-211">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="c55f0-211">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="c55f0-212">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-212">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-213">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="c55f0-213">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="c55f0-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-214">Boolean</span></span>|<span data-ttu-id="c55f0-215">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="c55f0-215">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="c55f0-216">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-216">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-217">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="c55f0-217">enterpriseProxyServers</span></span>|<span data-ttu-id="c55f0-218">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c55f0-219">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="c55f0-219">This is a list of proxy servers.</span></span> <span data-ttu-id="c55f0-220">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-220">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-221">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="c55f0-221">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="c55f0-222">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c55f0-223">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="c55f0-223">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="c55f0-224">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="c55f0-224">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="c55f0-225">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="c55f0-225">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="c55f0-226">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="c55f0-226">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="c55f0-227">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-227">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-228">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="c55f0-228">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="c55f0-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-229">Boolean</span></span>|<span data-ttu-id="c55f0-230">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c55f0-230">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="c55f0-231">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-231">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-232">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="c55f0-232">neutralDomainResources</span></span>|<span data-ttu-id="c55f0-233">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c55f0-234">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-234">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-235">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="c55f0-235">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="c55f0-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-236">Boolean</span></span>|<span data-ttu-id="c55f0-237">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-237">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-238">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="c55f0-238">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="c55f0-239">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-239">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="c55f0-240">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-240">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-241">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c55f0-241">isAssigned</span></span>|<span data-ttu-id="c55f0-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-242">Boolean</span></span>|<span data-ttu-id="c55f0-243">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="c55f0-243">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="c55f0-244">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="c55f0-244">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="c55f0-245">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="c55f0-245">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="c55f0-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-246">Boolean</span></span>|<span data-ttu-id="c55f0-247">Nova propriedade em RS2, documentação pendente</span><span class="sxs-lookup"><span data-stu-id="c55f0-247">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="c55f0-248">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="c55f0-248">mdmEnrollmentUrl</span></span>|<span data-ttu-id="c55f0-249">String</span><span class="sxs-lookup"><span data-stu-id="c55f0-249">String</span></span>|<span data-ttu-id="c55f0-250">Url do registro do MDM</span><span class="sxs-lookup"><span data-stu-id="c55f0-250">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="c55f0-251">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="c55f0-251">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="c55f0-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55f0-252">Boolean</span></span>|<span data-ttu-id="c55f0-253">Valor booliano que define o Windows Hello para Empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="c55f0-253">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="c55f0-254">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c55f0-254">pinMinimumLength</span></span>|<span data-ttu-id="c55f0-255">Int32</span><span class="sxs-lookup"><span data-stu-id="c55f0-255">Int32</span></span>|<span data-ttu-id="c55f0-256">Valor inteiro que define o número mínimo de caracteres necessários para o PIN.</span><span class="sxs-lookup"><span data-stu-id="c55f0-256">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="c55f0-257">O valor padrão é 4.</span><span class="sxs-lookup"><span data-stu-id="c55f0-257">Default value is 4.</span></span> <span data-ttu-id="c55f0-258">O menor número que é possível definir para essa configuração de política é 4.</span><span class="sxs-lookup"><span data-stu-id="c55f0-258">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="c55f0-259">O maior número que é possível definir deve ser menor que o número configurado na política de comprimento máximo do PIN ou menor que 127, seja qual for o menor.</span><span class="sxs-lookup"><span data-stu-id="c55f0-259">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="c55f0-260">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="c55f0-260">pinUppercaseLetters</span></span>|[<span data-ttu-id="c55f0-261">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="c55f0-261">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="c55f0-262">Valor inteiro que configura o uso de letras maiúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="c55f0-262">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="c55f0-263">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="c55f0-263">Default is NotAllow.</span></span> <span data-ttu-id="c55f0-264">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="c55f0-264">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="c55f0-265">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="c55f0-265">pinLowercaseLetters</span></span>|[<span data-ttu-id="c55f0-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="c55f0-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="c55f0-267">Valor inteiro que configura o uso de letras minúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="c55f0-267">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="c55f0-268">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="c55f0-268">Default is NotAllow.</span></span> <span data-ttu-id="c55f0-269">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="c55f0-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="c55f0-270">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="c55f0-270">pinSpecialCharacters</span></span>|[<span data-ttu-id="c55f0-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="c55f0-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="c55f0-272">Valor inteiro que configura o uso de caracteres especiais no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="c55f0-272">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="c55f0-273">Os caracteres especiais válidos para o PIN do Windows Hello para Empresas incluem: !</span><span class="sxs-lookup"><span data-stu-id="c55f0-273">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="c55f0-274">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="c55f0-274">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="c55f0-275">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="c55f0-275">/ : ; < = > ?</span></span><span data-ttu-id="c55f0-276"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: ` notAllow `, ` requireAtLeastOne `, ` allow'.</span><span class="sxs-lookup"><span data-stu-id="c55f0-276"> @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allo\w`.</span></span>|
|<span data-ttu-id="c55f0-277">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c55f0-277">pinExpirationDays</span></span>|<span data-ttu-id="c55f0-278">Int32</span><span class="sxs-lookup"><span data-stu-id="c55f0-278">Int32</span></span>|<span data-ttu-id="c55f0-279">O valor inteiro especifica o período de tempo (em dias) em que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="c55f0-279">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="c55f0-280">O maior número que é possível definir para essa configuração de política é 730.</span><span class="sxs-lookup"><span data-stu-id="c55f0-280">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="c55f0-281">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="c55f0-281">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="c55f0-282">Se essa política for definida como 0, o PIN do usuário nunca irá expirar.</span><span class="sxs-lookup"><span data-stu-id="c55f0-282">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="c55f0-283">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="c55f0-283">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="c55f0-284">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="c55f0-284">Default is 0.</span></span>|
|<span data-ttu-id="c55f0-285">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="c55f0-285">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="c55f0-286">Int32</span><span class="sxs-lookup"><span data-stu-id="c55f0-286">Int32</span></span>|<span data-ttu-id="c55f0-287">O valor inteiro que especifica o número de PINs anteriores que podem ser associados a uma conta de usuário que não podem ser reutilizados.</span><span class="sxs-lookup"><span data-stu-id="c55f0-287">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="c55f0-288">O maior número que é possível definir para essa configuração de política é 50.</span><span class="sxs-lookup"><span data-stu-id="c55f0-288">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="c55f0-289">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="c55f0-289">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="c55f0-290">Se essa política for definida como 0, o armazenamento de PINs anteriores não será necessário.</span><span class="sxs-lookup"><span data-stu-id="c55f0-290">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="c55f0-291">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="c55f0-291">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="c55f0-292">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="c55f0-292">Default is 0.</span></span>|
|<span data-ttu-id="c55f0-293">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="c55f0-293">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="c55f0-294">Int32</span><span class="sxs-lookup"><span data-stu-id="c55f0-294">Int32</span></span>|<span data-ttu-id="c55f0-295">O número de falhas de autenticação permitido antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="c55f0-295">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="c55f0-296">O valor 0 desabilita a funcionalidade de apagamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c55f0-296">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="c55f0-297">O intervalo é um inteiro X, em que 4 <= X <= 16 para desktop e 0 <= X <= 999 para dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="c55f0-297">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="c55f0-298">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="c55f0-298">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="c55f0-299">Int32</span><span class="sxs-lookup"><span data-stu-id="c55f0-299">Int32</span></span>|<span data-ttu-id="c55f0-300">Especifica a quantidade máxima de tempo (em minutos) permitida após o dispositivo ficar ocioso antes que ele seja bloqueado por PIN ou senha.</span><span class="sxs-lookup"><span data-stu-id="c55f0-300">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="c55f0-301">O intervalo é um inteiro X, em que 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="c55f0-301">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="c55f0-302">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="c55f0-302">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="c55f0-303">Int32</span><span class="sxs-lookup"><span data-stu-id="c55f0-303">Int32</span></span>|<span data-ttu-id="c55f0-304">Intervalo offline antes do apagamento dos dados do aplicativo (dias)</span><span class="sxs-lookup"><span data-stu-id="c55f0-304">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="c55f0-305">Resposta</span><span class="sxs-lookup"><span data-stu-id="c55f0-305">Response</span></span>
<span data-ttu-id="c55f0-306">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c55f0-306">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c55f0-307">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c55f0-307">Example</span></span>

### <a name="request"></a><span data-ttu-id="c55f0-308">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c55f0-308">Request</span></span>
<span data-ttu-id="c55f0-309">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c55f0-309">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
Content-type: application/json
Content-length: 4303

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
          "@odata.type": "microsoft.graph.ipRange"
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

### <a name="response"></a><span data-ttu-id="c55f0-310">Resposta</span><span class="sxs-lookup"><span data-stu-id="c55f0-310">Response</span></span>
<span data-ttu-id="c55f0-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c55f0-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4475

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
          "@odata.type": "microsoft.graph.ipRange"
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




