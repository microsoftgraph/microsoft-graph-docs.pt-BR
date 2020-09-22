---
title: Criar windowsInformationProtectionPolicy
description: Cria um novo objeto windowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5378c5ecc083ed484653c9eef5e0fc0f375ed6ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978934"
---
# <a name="create-windowsinformationprotectionpolicy"></a><span data-ttu-id="a26b3-103">Criar windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a26b3-103">Create windowsInformationProtectionPolicy</span></span>

<span data-ttu-id="a26b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a26b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a26b3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a26b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a26b3-106">Cria um novo objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a26b3-106">Create a new [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a26b3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a26b3-107">Prerequisites</span></span>
<span data-ttu-id="a26b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a26b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a26b3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a26b3-110">Permission type</span></span>|<span data-ttu-id="a26b3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a26b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a26b3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a26b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a26b3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a26b3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a26b3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a26b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a26b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a26b3-115">Not supported.</span></span>|
|<span data-ttu-id="a26b3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a26b3-116">Application</span></span>|<span data-ttu-id="a26b3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a26b3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a26b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a26b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a26b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a26b3-119">Request headers</span></span>
|<span data-ttu-id="a26b3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a26b3-120">Header</span></span>|<span data-ttu-id="a26b3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a26b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a26b3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a26b3-122">Authorization</span></span>|<span data-ttu-id="a26b3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a26b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a26b3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a26b3-124">Accept</span></span>|<span data-ttu-id="a26b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a26b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a26b3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a26b3-126">Request body</span></span>
<span data-ttu-id="a26b3-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="a26b3-127">In the request body, supply a JSON representation for the windowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="a26b3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="a26b3-128">The following table shows the properties that are required when you create the windowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="a26b3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a26b3-129">Property</span></span>|<span data-ttu-id="a26b3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a26b3-130">Type</span></span>|<span data-ttu-id="a26b3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a26b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a26b3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a26b3-132">displayName</span></span>|<span data-ttu-id="a26b3-133">String</span><span class="sxs-lookup"><span data-stu-id="a26b3-133">String</span></span>|<span data-ttu-id="a26b3-134">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="a26b3-134">Policy display name.</span></span> <span data-ttu-id="a26b3-135">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a26b3-136">description</span><span class="sxs-lookup"><span data-stu-id="a26b3-136">description</span></span>|<span data-ttu-id="a26b3-137">String</span><span class="sxs-lookup"><span data-stu-id="a26b3-137">String</span></span>|<span data-ttu-id="a26b3-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="a26b3-138">The policy's description.</span></span> <span data-ttu-id="a26b3-139">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a26b3-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a26b3-140">createdDateTime</span></span>|<span data-ttu-id="a26b3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a26b3-141">DateTimeOffset</span></span>|<span data-ttu-id="a26b3-142">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="a26b3-142">The date and time the policy was created.</span></span> <span data-ttu-id="a26b3-143">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a26b3-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a26b3-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a26b3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a26b3-145">DateTimeOffset</span></span>|<span data-ttu-id="a26b3-146">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="a26b3-146">Last time the policy was modified.</span></span> <span data-ttu-id="a26b3-147">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a26b3-148">id</span><span class="sxs-lookup"><span data-stu-id="a26b3-148">id</span></span>|<span data-ttu-id="a26b3-149">String</span><span class="sxs-lookup"><span data-stu-id="a26b3-149">String</span></span>|<span data-ttu-id="a26b3-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a26b3-150">Key of the entity.</span></span> <span data-ttu-id="a26b3-151">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a26b3-152">version</span><span class="sxs-lookup"><span data-stu-id="a26b3-152">version</span></span>|<span data-ttu-id="a26b3-153">String</span><span class="sxs-lookup"><span data-stu-id="a26b3-153">String</span></span>|<span data-ttu-id="a26b3-154">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="a26b3-154">Version of the entity.</span></span> <span data-ttu-id="a26b3-155">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a26b3-156">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a26b3-156">enforcementLevel</span></span>|[<span data-ttu-id="a26b3-157">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="a26b3-157">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="a26b3-158">Nível de imposição WIP. Confira a definição de enumeração para valores suportados herdados de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="a26b3-158">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="a26b3-159">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="a26b3-159">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="a26b3-160">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="a26b3-160">enterpriseDomain</span></span>|<span data-ttu-id="a26b3-161">String</span><span class="sxs-lookup"><span data-stu-id="a26b3-161">String</span></span>|<span data-ttu-id="a26b3-162">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-162">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-163">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="a26b3-163">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="a26b3-164">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-164">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a26b3-165">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-165">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-166">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="a26b3-166">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="a26b3-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-167">Boolean</span></span>|<span data-ttu-id="a26b3-168">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-168">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-169">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a26b3-169">dataRecoveryCertificate</span></span>|[<span data-ttu-id="a26b3-170">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a26b3-170">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="a26b3-171">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="a26b3-171">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="a26b3-172">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-172">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-173">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="a26b3-173">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="a26b3-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-174">Boolean</span></span>|<span data-ttu-id="a26b3-175">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a26b3-175">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="a26b3-176">Se definido como 1 (não revogar teclas), as teclas não serão revogadas e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="a26b3-176">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="a26b3-177">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="a26b3-177">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="a26b3-178">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-178">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-179">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="a26b3-179">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="a26b3-180">Guid</span><span class="sxs-lookup"><span data-stu-id="a26b3-180">Guid</span></span>|<span data-ttu-id="a26b3-181">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="a26b3-181">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="a26b3-182">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-182">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-183">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="a26b3-183">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="a26b3-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-184">Boolean</span></span>|<span data-ttu-id="a26b3-185">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-185">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-186">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="a26b3-186">iconsVisible</span></span>|<span data-ttu-id="a26b3-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-187">Boolean</span></span>|<span data-ttu-id="a26b3-188">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="a26b3-188">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="a26b3-189">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-189">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-190">protectedApps</span><span class="sxs-lookup"><span data-stu-id="a26b3-190">protectedApps</span></span>|<span data-ttu-id="a26b3-191">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-191">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a26b3-192">Os aplicativos protegidos podem acessar dados corporativos e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-192">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-193">exemptApps</span><span class="sxs-lookup"><span data-stu-id="a26b3-193">exemptApps</span></span>|<span data-ttu-id="a26b3-194">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-194">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="a26b3-195">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="a26b3-195">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="a26b3-196">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="a26b3-196">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="a26b3-197">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-197">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-198">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="a26b3-198">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="a26b3-199">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-199">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a26b3-200">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="a26b3-200">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="a26b3-201">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-201">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-202">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="a26b3-202">enterpriseProxiedDomains</span></span>|<span data-ttu-id="a26b3-203">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-203">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="a26b3-204">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="a26b3-204">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="a26b3-205">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="a26b3-205">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="a26b3-206">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="a26b3-206">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="a26b3-207">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-207">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-208">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="a26b3-208">enterpriseIPRanges</span></span>|<span data-ttu-id="a26b3-209">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-209">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="a26b3-210">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="a26b3-210">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="a26b3-211">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="a26b3-211">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="a26b3-212">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-212">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-213">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a26b3-213">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="a26b3-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-214">Boolean</span></span>|<span data-ttu-id="a26b3-215">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="a26b3-215">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="a26b3-216">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-216">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-217">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="a26b3-217">enterpriseProxyServers</span></span>|<span data-ttu-id="a26b3-218">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-218">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a26b3-219">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="a26b3-219">This is a list of proxy servers.</span></span> <span data-ttu-id="a26b3-220">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-220">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-221">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="a26b3-221">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="a26b3-222">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-222">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a26b3-223">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="a26b3-223">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="a26b3-224">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="a26b3-224">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="a26b3-225">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="a26b3-225">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="a26b3-226">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="a26b3-226">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="a26b3-227">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-227">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-228">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="a26b3-228">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="a26b3-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-229">Boolean</span></span>|<span data-ttu-id="a26b3-230">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a26b3-230">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="a26b3-231">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-231">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-232">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="a26b3-232">neutralDomainResources</span></span>|<span data-ttu-id="a26b3-233">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a26b3-234">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-234">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-235">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="a26b3-235">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="a26b3-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-236">Boolean</span></span>|<span data-ttu-id="a26b3-237">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-237">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-238">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="a26b3-238">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="a26b3-239">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-239">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="a26b3-240">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-240">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-241">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a26b3-241">isAssigned</span></span>|<span data-ttu-id="a26b3-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-242">Boolean</span></span>|<span data-ttu-id="a26b3-243">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="a26b3-243">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="a26b3-244">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="a26b3-244">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="a26b3-245">revokeOnMdmHandoffDisabled</span><span class="sxs-lookup"><span data-stu-id="a26b3-245">revokeOnMdmHandoffDisabled</span></span>|<span data-ttu-id="a26b3-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-246">Boolean</span></span>|<span data-ttu-id="a26b3-247">Nova propriedade em RS2, documentação pendente</span><span class="sxs-lookup"><span data-stu-id="a26b3-247">New property in RS2, pending documentation</span></span>|
|<span data-ttu-id="a26b3-248">mdmEnrollmentUrl</span><span class="sxs-lookup"><span data-stu-id="a26b3-248">mdmEnrollmentUrl</span></span>|<span data-ttu-id="a26b3-249">String</span><span class="sxs-lookup"><span data-stu-id="a26b3-249">String</span></span>|<span data-ttu-id="a26b3-250">Url do registro do MDM</span><span class="sxs-lookup"><span data-stu-id="a26b3-250">Enrollment url for the MDM</span></span>|
|<span data-ttu-id="a26b3-251">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="a26b3-251">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="a26b3-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26b3-252">Boolean</span></span>|<span data-ttu-id="a26b3-253">Valor booliano que define o Windows Hello para Empresas como um método para entrar no Windows.</span><span class="sxs-lookup"><span data-stu-id="a26b3-253">Boolean value that sets Windows Hello for Business as a method for signing into Windows.</span></span>|
|<span data-ttu-id="a26b3-254">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a26b3-254">pinMinimumLength</span></span>|<span data-ttu-id="a26b3-255">Int32</span><span class="sxs-lookup"><span data-stu-id="a26b3-255">Int32</span></span>|<span data-ttu-id="a26b3-256">Valor inteiro que define o número mínimo de caracteres necessários para o PIN.</span><span class="sxs-lookup"><span data-stu-id="a26b3-256">Integer value that sets the minimum number of characters required for the PIN.</span></span> <span data-ttu-id="a26b3-257">O valor padrão é 4.</span><span class="sxs-lookup"><span data-stu-id="a26b3-257">Default value is 4.</span></span> <span data-ttu-id="a26b3-258">O menor número que é possível definir para essa configuração de política é 4.</span><span class="sxs-lookup"><span data-stu-id="a26b3-258">The lowest number you can configure for this policy setting is 4.</span></span> <span data-ttu-id="a26b3-259">O maior número que é possível definir deve ser menor que o número configurado na política de comprimento máximo do PIN ou menor que 127, seja qual for o menor.</span><span class="sxs-lookup"><span data-stu-id="a26b3-259">The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.</span></span>|
|<span data-ttu-id="a26b3-260">pinUppercaseLetters</span><span class="sxs-lookup"><span data-stu-id="a26b3-260">pinUppercaseLetters</span></span>|[<span data-ttu-id="a26b3-261">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="a26b3-261">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="a26b3-262">Valor inteiro que configura o uso de letras maiúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="a26b3-262">Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a26b3-263">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="a26b3-263">Default is NotAllow.</span></span> <span data-ttu-id="a26b3-264">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="a26b3-264">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="a26b3-265">pinLowercaseLetters</span><span class="sxs-lookup"><span data-stu-id="a26b3-265">pinLowercaseLetters</span></span>|[<span data-ttu-id="a26b3-266">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="a26b3-266">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="a26b3-267">Valor inteiro que configura o uso de letras minúsculas no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="a26b3-267">Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a26b3-268">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="a26b3-268">Default is NotAllow.</span></span> <span data-ttu-id="a26b3-269">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="a26b3-269">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="a26b3-270">pinSpecialCharacters</span><span class="sxs-lookup"><span data-stu-id="a26b3-270">pinSpecialCharacters</span></span>|[<span data-ttu-id="a26b3-271">windowsInformationProtectionPinCharacterRequirements</span><span class="sxs-lookup"><span data-stu-id="a26b3-271">windowsInformationProtectionPinCharacterRequirements</span></span>](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|<span data-ttu-id="a26b3-272">Valor inteiro que configura o uso de caracteres especiais no PIN do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="a26b3-272">Integer value that configures the use of special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a26b3-273">Os caracteres especiais válidos para o PIN do Windows Hello para Empresas incluem: !</span><span class="sxs-lookup"><span data-stu-id="a26b3-273">Valid special characters for Windows Hello for Business PIN gestures include: !</span></span> <span data-ttu-id="a26b3-274">" # $ % & ' ( ) \* + , - .</span><span class="sxs-lookup"><span data-stu-id="a26b3-274">" # $ % & ' ( ) \* + , - .</span></span> <span data-ttu-id="a26b3-275">/ : ; < = > ?</span><span class="sxs-lookup"><span data-stu-id="a26b3-275">/ : ; < = > ?</span></span><span data-ttu-id="a26b3-276"> @ \[ \ \] ^ _ \` { | } ~.</span><span class="sxs-lookup"><span data-stu-id="a26b3-276"> @ \[ \ \] ^ _ \` { | } ~.</span></span> <span data-ttu-id="a26b3-277">O padrão é NotAllow.</span><span class="sxs-lookup"><span data-stu-id="a26b3-277">Default is NotAllow.</span></span> <span data-ttu-id="a26b3-278">Os valores possíveis são: `notAllow`, `requireAtLeastOne`, `allow`.</span><span class="sxs-lookup"><span data-stu-id="a26b3-278">Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.</span></span>|
|<span data-ttu-id="a26b3-279">pinExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a26b3-279">pinExpirationDays</span></span>|<span data-ttu-id="a26b3-280">Int32</span><span class="sxs-lookup"><span data-stu-id="a26b3-280">Int32</span></span>|<span data-ttu-id="a26b3-281">O valor inteiro especifica o período de tempo (em dias) em que um PIN pode ser usado antes que o sistema exija que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="a26b3-281">Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="a26b3-282">O maior número que é possível definir para essa configuração de política é 730.</span><span class="sxs-lookup"><span data-stu-id="a26b3-282">The largest number you can configure for this policy setting is 730.</span></span> <span data-ttu-id="a26b3-283">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="a26b3-283">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="a26b3-284">Se essa política for definida como 0, o PIN do usuário nunca irá expirar.</span><span class="sxs-lookup"><span data-stu-id="a26b3-284">If this policy is set to 0, then the user's PIN will never expire.</span></span> <span data-ttu-id="a26b3-285">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="a26b3-285">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="a26b3-286">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="a26b3-286">Default is 0.</span></span>|
|<span data-ttu-id="a26b3-287">numberOfPastPinsRemembered</span><span class="sxs-lookup"><span data-stu-id="a26b3-287">numberOfPastPinsRemembered</span></span>|<span data-ttu-id="a26b3-288">Int32</span><span class="sxs-lookup"><span data-stu-id="a26b3-288">Int32</span></span>|<span data-ttu-id="a26b3-289">O valor inteiro que especifica o número de PINs anteriores que podem ser associados a uma conta de usuário que não podem ser reutilizados.</span><span class="sxs-lookup"><span data-stu-id="a26b3-289">Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.</span></span> <span data-ttu-id="a26b3-290">O maior número que é possível definir para essa configuração de política é 50.</span><span class="sxs-lookup"><span data-stu-id="a26b3-290">The largest number you can configure for this policy setting is 50.</span></span> <span data-ttu-id="a26b3-291">O menor número que é possível definir para essa configuração de política é 0.</span><span class="sxs-lookup"><span data-stu-id="a26b3-291">The lowest number you can configure for this policy setting is 0.</span></span> <span data-ttu-id="a26b3-292">Se essa política for definida como 0, o armazenamento de PINs anteriores não será necessário.</span><span class="sxs-lookup"><span data-stu-id="a26b3-292">If this policy is set to 0, then storage of previous PINs is not required.</span></span> <span data-ttu-id="a26b3-293">Este nó foi adicionado no Windows 10, versão 1511.</span><span class="sxs-lookup"><span data-stu-id="a26b3-293">This node was added in Windows 10, version 1511.</span></span> <span data-ttu-id="a26b3-294">O padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="a26b3-294">Default is 0.</span></span>|
|<span data-ttu-id="a26b3-295">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="a26b3-295">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="a26b3-296">Int32</span><span class="sxs-lookup"><span data-stu-id="a26b3-296">Int32</span></span>|<span data-ttu-id="a26b3-297">O número de falhas de autenticação permitido antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="a26b3-297">The number of authentication failures allowed before the device will be wiped.</span></span> <span data-ttu-id="a26b3-298">O valor 0 desabilita a funcionalidade de apagamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a26b3-298">A value of 0 disables device wipe functionality.</span></span> <span data-ttu-id="a26b3-299">O intervalo é um inteiro X, em que 4 <= X <= 16 para desktop e 0 <= X <= 999 para dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="a26b3-299">Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.</span></span>|
|<span data-ttu-id="a26b3-300">minutesOfInactivityBeforeDeviceLock</span><span class="sxs-lookup"><span data-stu-id="a26b3-300">minutesOfInactivityBeforeDeviceLock</span></span>|<span data-ttu-id="a26b3-301">Int32</span><span class="sxs-lookup"><span data-stu-id="a26b3-301">Int32</span></span>|<span data-ttu-id="a26b3-302">Especifica a quantidade máxima de tempo (em minutos) permitida após o dispositivo ficar ocioso antes que ele seja bloqueado por PIN ou senha.</span><span class="sxs-lookup"><span data-stu-id="a26b3-302">Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.</span></span>   <span data-ttu-id="a26b3-303">O intervalo é um inteiro X, em que 0 <= X <= 999.</span><span class="sxs-lookup"><span data-stu-id="a26b3-303">Range is an integer X where 0 <= X <= 999.</span></span>|
|<span data-ttu-id="a26b3-304">daysWithoutContactBeforeUnenroll</span><span class="sxs-lookup"><span data-stu-id="a26b3-304">daysWithoutContactBeforeUnenroll</span></span>|<span data-ttu-id="a26b3-305">Int32</span><span class="sxs-lookup"><span data-stu-id="a26b3-305">Int32</span></span>|<span data-ttu-id="a26b3-306">Intervalo offline antes do apagamento dos dados do aplicativo (dias)</span><span class="sxs-lookup"><span data-stu-id="a26b3-306">Offline interval before app data is wiped (days)</span></span> |



## <a name="response"></a><span data-ttu-id="a26b3-307">Resposta</span><span class="sxs-lookup"><span data-stu-id="a26b3-307">Response</span></span>
<span data-ttu-id="a26b3-308">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a26b3-308">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a26b3-309">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a26b3-309">Example</span></span>

### <a name="request"></a><span data-ttu-id="a26b3-310">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a26b3-310">Request</span></span>
<span data-ttu-id="a26b3-311">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a26b3-311">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a26b3-312">Resposta</span><span class="sxs-lookup"><span data-stu-id="a26b3-312">Response</span></span>
<span data-ttu-id="a26b3-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a26b3-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









