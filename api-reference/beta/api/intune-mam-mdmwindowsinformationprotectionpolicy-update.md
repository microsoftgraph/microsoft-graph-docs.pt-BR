---
title: Atualizar mdmWindowsInformationProtectionPolicy
description: Atualizar as propriedades de um objeto mdmWindowsInformationProtectionPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 900a2eaf57b6b6ba33d0f6071aaa9fc875e81762
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400246"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="457a8-103">Atualizar mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="457a8-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="457a8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="457a8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="457a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="457a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="457a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="457a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="457a8-107">Atualizar as propriedades de um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="457a8-107">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="457a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="457a8-108">Prerequisites</span></span>
<span data-ttu-id="457a8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="457a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="457a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="457a8-111">Permission type</span></span>|<span data-ttu-id="457a8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="457a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="457a8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="457a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="457a8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457a8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="457a8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="457a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="457a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="457a8-116">Not supported.</span></span>|
|<span data-ttu-id="457a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="457a8-117">Application</span></span>|<span data-ttu-id="457a8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="457a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="457a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="457a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="457a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="457a8-120">Request headers</span></span>
|<span data-ttu-id="457a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="457a8-121">Header</span></span>|<span data-ttu-id="457a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="457a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="457a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="457a8-123">Authorization</span></span>|<span data-ttu-id="457a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="457a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="457a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="457a8-125">Accept</span></span>|<span data-ttu-id="457a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="457a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="457a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="457a8-127">Request body</span></span>
<span data-ttu-id="457a8-128">No corpo da solicitação, forneça uma representação JSON do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="457a8-128">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="457a8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="457a8-129">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="457a8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="457a8-130">Property</span></span>|<span data-ttu-id="457a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="457a8-131">Type</span></span>|<span data-ttu-id="457a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="457a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="457a8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="457a8-133">displayName</span></span>|<span data-ttu-id="457a8-134">String</span><span class="sxs-lookup"><span data-stu-id="457a8-134">String</span></span>|<span data-ttu-id="457a8-135">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="457a8-135">Policy display name.</span></span> <span data-ttu-id="457a8-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="457a8-137">description</span><span class="sxs-lookup"><span data-stu-id="457a8-137">description</span></span>|<span data-ttu-id="457a8-138">String</span><span class="sxs-lookup"><span data-stu-id="457a8-138">String</span></span>|<span data-ttu-id="457a8-139">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="457a8-139">The policy's description.</span></span> <span data-ttu-id="457a8-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="457a8-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="457a8-141">createdDateTime</span></span>|<span data-ttu-id="457a8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457a8-142">DateTimeOffset</span></span>|<span data-ttu-id="457a8-143">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="457a8-143">The date and time the policy was created.</span></span> <span data-ttu-id="457a8-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="457a8-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="457a8-145">lastModifiedDateTime</span></span>|<span data-ttu-id="457a8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="457a8-146">DateTimeOffset</span></span>|<span data-ttu-id="457a8-147">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="457a8-147">Last time the policy was modified.</span></span> <span data-ttu-id="457a8-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="457a8-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="457a8-149">roleScopeTagIds</span></span>|<span data-ttu-id="457a8-150">String collection</span><span class="sxs-lookup"><span data-stu-id="457a8-150">String collection</span></span>|<span data-ttu-id="457a8-151">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="457a8-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="457a8-152">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="457a8-153">id</span><span class="sxs-lookup"><span data-stu-id="457a8-153">id</span></span>|<span data-ttu-id="457a8-154">String</span><span class="sxs-lookup"><span data-stu-id="457a8-154">String</span></span>|<span data-ttu-id="457a8-155">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="457a8-155">Key of the entity.</span></span> <span data-ttu-id="457a8-156">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="457a8-157">version</span><span class="sxs-lookup"><span data-stu-id="457a8-157">version</span></span>|<span data-ttu-id="457a8-158">String</span><span class="sxs-lookup"><span data-stu-id="457a8-158">String</span></span>|<span data-ttu-id="457a8-159">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="457a8-159">Version of the entity.</span></span> <span data-ttu-id="457a8-160">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="457a8-161">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="457a8-161">enforcementLevel</span></span>|[<span data-ttu-id="457a8-162">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="457a8-162">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="457a8-163">Nível da imposição de WIP. Consulte a definição de Enum de valores suportados Inherited de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="457a8-163">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="457a8-164">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="457a8-164">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="457a8-165">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="457a8-165">enterpriseDomain</span></span>|<span data-ttu-id="457a8-166">String</span><span class="sxs-lookup"><span data-stu-id="457a8-166">String</span></span>|<span data-ttu-id="457a8-167">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-167">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-168">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="457a8-168">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="457a8-169">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-169">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="457a8-170">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-170">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-171">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="457a8-171">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="457a8-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="457a8-172">Boolean</span></span>|<span data-ttu-id="457a8-173">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-173">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-174">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="457a8-174">dataRecoveryCertificate</span></span>|[<span data-ttu-id="457a8-175">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="457a8-175">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="457a8-176">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="457a8-176">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="457a8-177">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-177">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-178">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="457a8-178">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="457a8-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="457a8-179">Boolean</span></span>|<span data-ttu-id="457a8-180">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="457a8-180">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="457a8-181">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="457a8-181">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="457a8-182">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="457a8-182">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="457a8-183">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-183">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-184">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="457a8-184">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="457a8-185">Guid</span><span class="sxs-lookup"><span data-stu-id="457a8-185">Guid</span></span>|<span data-ttu-id="457a8-186">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="457a8-186">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="457a8-187">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-187">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-188">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="457a8-188">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="457a8-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="457a8-189">Boolean</span></span>|<span data-ttu-id="457a8-190">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-190">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-191">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="457a8-191">iconsVisible</span></span>|<span data-ttu-id="457a8-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="457a8-192">Boolean</span></span>|<span data-ttu-id="457a8-193">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="457a8-193">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="457a8-194">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-194">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-195">protectedApps</span><span class="sxs-lookup"><span data-stu-id="457a8-195">protectedApps</span></span>|<span data-ttu-id="457a8-196">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-196">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="457a8-197">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-197">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-198">exemptApps</span><span class="sxs-lookup"><span data-stu-id="457a8-198">exemptApps</span></span>|<span data-ttu-id="457a8-199">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-199">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="457a8-200">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="457a8-200">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="457a8-201">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="457a8-201">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="457a8-202">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-202">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-203">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="457a8-203">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="457a8-204">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-204">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="457a8-205">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="457a8-205">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="457a8-206">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-206">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-207">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="457a8-207">enterpriseProxiedDomains</span></span>|<span data-ttu-id="457a8-208">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-208">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="457a8-209">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="457a8-209">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="457a8-210">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="457a8-210">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="457a8-211">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="457a8-211">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="457a8-212">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-212">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-213">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="457a8-213">enterpriseIPRanges</span></span>|<span data-ttu-id="457a8-214">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-214">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="457a8-215">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="457a8-215">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="457a8-216">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="457a8-216">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="457a8-217">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-217">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-218">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="457a8-218">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="457a8-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="457a8-219">Boolean</span></span>|<span data-ttu-id="457a8-220">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="457a8-220">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="457a8-221">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-221">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-222">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="457a8-222">enterpriseProxyServers</span></span>|<span data-ttu-id="457a8-223">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="457a8-224">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="457a8-224">This is a list of proxy servers.</span></span> <span data-ttu-id="457a8-225">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-225">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-226">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="457a8-226">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="457a8-227">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-227">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="457a8-228">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="457a8-228">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="457a8-229">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="457a8-229">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="457a8-230">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="457a8-230">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="457a8-231">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="457a8-231">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="457a8-232">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-232">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-233">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="457a8-233">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="457a8-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="457a8-234">Boolean</span></span>|<span data-ttu-id="457a8-235">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="457a8-235">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="457a8-236">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-236">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-237">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="457a8-237">neutralDomainResources</span></span>|<span data-ttu-id="457a8-238">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="457a8-239">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-239">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-240">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="457a8-240">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="457a8-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="457a8-241">Boolean</span></span>|<span data-ttu-id="457a8-242">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-242">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-243">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="457a8-243">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="457a8-244">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-244">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="457a8-245">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-245">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="457a8-246">isAssigned</span><span class="sxs-lookup"><span data-stu-id="457a8-246">isAssigned</span></span>|<span data-ttu-id="457a8-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="457a8-247">Boolean</span></span>|<span data-ttu-id="457a8-248">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="457a8-248">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="457a8-249">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="457a8-249">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="457a8-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="457a8-250">Response</span></span>
<span data-ttu-id="457a8-251">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="457a8-251">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="457a8-252">Exemplo</span><span class="sxs-lookup"><span data-stu-id="457a8-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="457a8-253">Solicitação</span><span class="sxs-lookup"><span data-stu-id="457a8-253">Request</span></span>
<span data-ttu-id="457a8-254">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="457a8-254">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="457a8-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="457a8-255">Response</span></span>
<span data-ttu-id="457a8-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="457a8-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




