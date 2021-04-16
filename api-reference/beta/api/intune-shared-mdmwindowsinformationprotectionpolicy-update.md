---
title: Atualizar mdmWindowsInformationProtectionPolicy
description: Atualizar as propriedades de um objeto mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82fddd86ba1ec2ed971041b8c14c9580881b9cb5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865121"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="fca88-103">Atualizar mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fca88-103">Update mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="fca88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fca88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fca88-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fca88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fca88-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fca88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fca88-107">Atualizar as propriedades de um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fca88-107">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fca88-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fca88-108">Prerequisites</span></span>
<span data-ttu-id="fca88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fca88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fca88-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fca88-111">Permission type</span></span>|<span data-ttu-id="fca88-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fca88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fca88-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fca88-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fca88-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="fca88-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="fca88-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca88-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="fca88-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="fca88-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="fca88-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca88-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fca88-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fca88-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fca88-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fca88-119">Not supported.</span></span>|
|<span data-ttu-id="fca88-120">Application</span><span class="sxs-lookup"><span data-stu-id="fca88-120">Application</span></span>||
| <span data-ttu-id="fca88-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="fca88-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="fca88-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca88-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="fca88-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="fca88-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="fca88-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca88-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fca88-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fca88-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fca88-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fca88-126">Request headers</span></span>
|<span data-ttu-id="fca88-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fca88-127">Header</span></span>|<span data-ttu-id="fca88-128">Valor</span><span class="sxs-lookup"><span data-stu-id="fca88-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fca88-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="fca88-129">Authorization</span></span>|<span data-ttu-id="fca88-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fca88-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fca88-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fca88-131">Accept</span></span>|<span data-ttu-id="fca88-132">application/json</span><span class="sxs-lookup"><span data-stu-id="fca88-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fca88-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fca88-133">Request body</span></span>
<span data-ttu-id="fca88-134">No corpo da solicitação, forneça uma representação JSON do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fca88-134">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="fca88-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fca88-135">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="fca88-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fca88-136">Property</span></span>|<span data-ttu-id="fca88-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="fca88-137">Type</span></span>|<span data-ttu-id="fca88-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="fca88-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fca88-139">displayName</span><span class="sxs-lookup"><span data-stu-id="fca88-139">displayName</span></span>|<span data-ttu-id="fca88-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fca88-140">String</span></span>|<span data-ttu-id="fca88-141">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="fca88-141">Policy display name.</span></span> <span data-ttu-id="fca88-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fca88-143">description</span><span class="sxs-lookup"><span data-stu-id="fca88-143">description</span></span>|<span data-ttu-id="fca88-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fca88-144">String</span></span>|<span data-ttu-id="fca88-145">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="fca88-145">The policy's description.</span></span> <span data-ttu-id="fca88-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fca88-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fca88-147">createdDateTime</span></span>|<span data-ttu-id="fca88-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fca88-148">DateTimeOffset</span></span>|<span data-ttu-id="fca88-149">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="fca88-149">The date and time the policy was created.</span></span> <span data-ttu-id="fca88-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fca88-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fca88-151">lastModifiedDateTime</span></span>|<span data-ttu-id="fca88-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fca88-152">DateTimeOffset</span></span>|<span data-ttu-id="fca88-153">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="fca88-153">Last time the policy was modified.</span></span> <span data-ttu-id="fca88-154">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fca88-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fca88-155">roleScopeTagIds</span></span>|<span data-ttu-id="fca88-156">Coleção String</span><span class="sxs-lookup"><span data-stu-id="fca88-156">String collection</span></span>|<span data-ttu-id="fca88-157">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="fca88-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fca88-158">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fca88-159">id</span><span class="sxs-lookup"><span data-stu-id="fca88-159">id</span></span>|<span data-ttu-id="fca88-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fca88-160">String</span></span>|<span data-ttu-id="fca88-161">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fca88-161">Key of the entity.</span></span> <span data-ttu-id="fca88-162">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fca88-163">version</span><span class="sxs-lookup"><span data-stu-id="fca88-163">version</span></span>|<span data-ttu-id="fca88-164">String</span><span class="sxs-lookup"><span data-stu-id="fca88-164">String</span></span>|<span data-ttu-id="fca88-165">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="fca88-165">Version of the entity.</span></span> <span data-ttu-id="fca88-166">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fca88-167">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fca88-167">enforcementLevel</span></span>|[<span data-ttu-id="fca88-168">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="fca88-168">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="fca88-169">Nível de aplicação da WIP. Consulte a definição Enum para valores com suporte Herdados de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fca88-169">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="fca88-170">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="fca88-170">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="fca88-171">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="fca88-171">enterpriseDomain</span></span>|<span data-ttu-id="fca88-172">String</span><span class="sxs-lookup"><span data-stu-id="fca88-172">String</span></span>|<span data-ttu-id="fca88-173">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-173">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-174">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="fca88-174">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="fca88-175">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-175">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fca88-176">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-176">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-177">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="fca88-177">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="fca88-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="fca88-178">Boolean</span></span>|<span data-ttu-id="fca88-179">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-179">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-180">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fca88-180">dataRecoveryCertificate</span></span>|[<span data-ttu-id="fca88-181">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fca88-181">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="fca88-182">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="fca88-182">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="fca88-183">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-183">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-184">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="fca88-184">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="fca88-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="fca88-185">Boolean</span></span>|<span data-ttu-id="fca88-186">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fca88-186">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="fca88-187">Se definido como 1 (não revogar teclas), as teclas não serão revogadas e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="fca88-187">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="fca88-188">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="fca88-188">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="fca88-189">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-189">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-190">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="fca88-190">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="fca88-191">Guid</span><span class="sxs-lookup"><span data-stu-id="fca88-191">Guid</span></span>|<span data-ttu-id="fca88-192">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="fca88-192">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="fca88-193">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-193">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-194">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="fca88-194">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="fca88-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="fca88-195">Boolean</span></span>|<span data-ttu-id="fca88-196">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-196">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-197">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="fca88-197">iconsVisible</span></span>|<span data-ttu-id="fca88-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="fca88-198">Boolean</span></span>|<span data-ttu-id="fca88-199">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="fca88-199">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="fca88-200">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-200">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-201">protectedApps</span><span class="sxs-lookup"><span data-stu-id="fca88-201">protectedApps</span></span>|<span data-ttu-id="fca88-202">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-202">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fca88-203">Os aplicativos protegidos podem acessar dados corporativos e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-203">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-204">exemptApps</span><span class="sxs-lookup"><span data-stu-id="fca88-204">exemptApps</span></span>|<span data-ttu-id="fca88-205">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-205">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="fca88-206">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="fca88-206">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="fca88-207">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="fca88-207">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="fca88-208">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-208">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-209">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="fca88-209">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="fca88-210">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-210">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fca88-211">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="fca88-211">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="fca88-212">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-212">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-213">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="fca88-213">enterpriseProxiedDomains</span></span>|<span data-ttu-id="fca88-214">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-214">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="fca88-215">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="fca88-215">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="fca88-216">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="fca88-216">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="fca88-217">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="fca88-217">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="fca88-218">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-218">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-219">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="fca88-219">enterpriseIPRanges</span></span>|<span data-ttu-id="fca88-220">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-220">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="fca88-221">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="fca88-221">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="fca88-222">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="fca88-222">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="fca88-223">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-223">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-224">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fca88-224">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="fca88-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="fca88-225">Boolean</span></span>|<span data-ttu-id="fca88-226">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="fca88-226">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="fca88-227">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-227">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-228">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="fca88-228">enterpriseProxyServers</span></span>|<span data-ttu-id="fca88-229">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-229">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fca88-230">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="fca88-230">This is a list of proxy servers.</span></span> <span data-ttu-id="fca88-231">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-231">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-232">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="fca88-232">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="fca88-233">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-233">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fca88-234">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="fca88-234">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="fca88-235">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="fca88-235">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="fca88-236">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="fca88-236">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="fca88-237">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="fca88-237">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="fca88-238">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-238">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-239">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="fca88-239">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="fca88-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="fca88-240">Boolean</span></span>|<span data-ttu-id="fca88-241">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="fca88-241">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="fca88-242">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-242">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-243">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="fca88-243">neutralDomainResources</span></span>|<span data-ttu-id="fca88-244">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fca88-245">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-245">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-246">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="fca88-246">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="fca88-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="fca88-247">Boolean</span></span>|<span data-ttu-id="fca88-248">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-248">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-249">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="fca88-249">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="fca88-250">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-250">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="fca88-251">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-251">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="fca88-252">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fca88-252">isAssigned</span></span>|<span data-ttu-id="fca88-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="fca88-253">Boolean</span></span>|<span data-ttu-id="fca88-254">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="fca88-254">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="fca88-255">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="fca88-255">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fca88-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="fca88-256">Response</span></span>
<span data-ttu-id="fca88-257">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fca88-257">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fca88-258">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fca88-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="fca88-259">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fca88-259">Request</span></span>
<span data-ttu-id="fca88-260">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fca88-260">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fca88-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="fca88-261">Response</span></span>
<span data-ttu-id="fca88-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fca88-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







