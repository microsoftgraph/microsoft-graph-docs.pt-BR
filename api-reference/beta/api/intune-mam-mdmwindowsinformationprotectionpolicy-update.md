---
title: Atualizar mdmWindowsInformationProtectionPolicy
description: Atualizar as propriedades de um objeto mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fcb71179ccb165d559bcbc7b556eca3fd1bb64d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973493"
---
# <a name="update-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="d8b30-103">Atualizar mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d8b30-103">Update mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="d8b30-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8b30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8b30-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8b30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8b30-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d8b30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8b30-107">Atualizar as propriedades de um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d8b30-107">Update the properties of a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8b30-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8b30-108">Prerequisites</span></span>
<span data-ttu-id="d8b30-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8b30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8b30-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8b30-111">Permission type</span></span>|<span data-ttu-id="d8b30-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8b30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8b30-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8b30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8b30-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b30-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8b30-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8b30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8b30-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8b30-116">Not supported.</span></span>|
|<span data-ttu-id="d8b30-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8b30-117">Application</span></span>|<span data-ttu-id="d8b30-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8b30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8b30-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8b30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="d8b30-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b30-120">Request headers</span></span>
|<span data-ttu-id="d8b30-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8b30-121">Header</span></span>|<span data-ttu-id="d8b30-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8b30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8b30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8b30-123">Authorization</span></span>|<span data-ttu-id="d8b30-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8b30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8b30-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8b30-125">Accept</span></span>|<span data-ttu-id="d8b30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8b30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8b30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b30-127">Request body</span></span>
<span data-ttu-id="d8b30-128">No corpo da solicitação, forneça uma representação JSON do objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d8b30-128">In the request body, supply a JSON representation for the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

<span data-ttu-id="d8b30-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d8b30-129">The following table shows the properties that are required when you create the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

|<span data-ttu-id="d8b30-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8b30-130">Property</span></span>|<span data-ttu-id="d8b30-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8b30-131">Type</span></span>|<span data-ttu-id="d8b30-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8b30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8b30-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d8b30-133">displayName</span></span>|<span data-ttu-id="d8b30-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b30-134">String</span></span>|<span data-ttu-id="d8b30-135">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="d8b30-135">Policy display name.</span></span> <span data-ttu-id="d8b30-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8b30-137">description</span><span class="sxs-lookup"><span data-stu-id="d8b30-137">description</span></span>|<span data-ttu-id="d8b30-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b30-138">String</span></span>|<span data-ttu-id="d8b30-139">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="d8b30-139">The policy's description.</span></span> <span data-ttu-id="d8b30-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8b30-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8b30-141">createdDateTime</span></span>|<span data-ttu-id="d8b30-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8b30-142">DateTimeOffset</span></span>|<span data-ttu-id="d8b30-143">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="d8b30-143">The date and time the policy was created.</span></span> <span data-ttu-id="d8b30-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8b30-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8b30-145">lastModifiedDateTime</span></span>|<span data-ttu-id="d8b30-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8b30-146">DateTimeOffset</span></span>|<span data-ttu-id="d8b30-147">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="d8b30-147">Last time the policy was modified.</span></span> <span data-ttu-id="d8b30-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8b30-149">id</span><span class="sxs-lookup"><span data-stu-id="d8b30-149">id</span></span>|<span data-ttu-id="d8b30-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b30-150">String</span></span>|<span data-ttu-id="d8b30-151">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8b30-151">Key of the entity.</span></span> <span data-ttu-id="d8b30-152">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8b30-153">version</span><span class="sxs-lookup"><span data-stu-id="d8b30-153">version</span></span>|<span data-ttu-id="d8b30-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b30-154">String</span></span>|<span data-ttu-id="d8b30-155">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8b30-155">Version of the entity.</span></span> <span data-ttu-id="d8b30-156">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="d8b30-157">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d8b30-157">enforcementLevel</span></span>|[<span data-ttu-id="d8b30-158">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="d8b30-158">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="d8b30-159">Nível da imposição de WIP. Consulte a definição de Enum de valores suportados Inherited de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="d8b30-159">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="d8b30-160">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="d8b30-160">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="d8b30-161">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="d8b30-161">enterpriseDomain</span></span>|<span data-ttu-id="d8b30-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b30-162">String</span></span>|<span data-ttu-id="d8b30-163">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-163">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-164">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="d8b30-164">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="d8b30-165">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-165">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d8b30-166">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-166">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-167">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="d8b30-167">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="d8b30-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8b30-168">Boolean</span></span>|<span data-ttu-id="d8b30-169">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-169">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-170">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d8b30-170">dataRecoveryCertificate</span></span>|[<span data-ttu-id="d8b30-171">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d8b30-171">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="d8b30-172">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="d8b30-172">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="d8b30-173">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-173">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-174">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="d8b30-174">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="d8b30-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8b30-175">Boolean</span></span>|<span data-ttu-id="d8b30-176">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d8b30-176">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="d8b30-177">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="d8b30-177">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="d8b30-178">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="d8b30-178">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="d8b30-179">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-179">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-180">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="d8b30-180">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="d8b30-181">Guid</span><span class="sxs-lookup"><span data-stu-id="d8b30-181">Guid</span></span>|<span data-ttu-id="d8b30-182">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="d8b30-182">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="d8b30-183">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-183">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-184">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="d8b30-184">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="d8b30-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8b30-185">Boolean</span></span>|<span data-ttu-id="d8b30-186">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-186">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-187">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="d8b30-187">iconsVisible</span></span>|<span data-ttu-id="d8b30-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8b30-188">Boolean</span></span>|<span data-ttu-id="d8b30-189">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="d8b30-189">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="d8b30-190">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-190">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-191">protectedApps</span><span class="sxs-lookup"><span data-stu-id="d8b30-191">protectedApps</span></span>|<span data-ttu-id="d8b30-192">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-192">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d8b30-193">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-193">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-194">exemptApps</span><span class="sxs-lookup"><span data-stu-id="d8b30-194">exemptApps</span></span>|<span data-ttu-id="d8b30-195">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-195">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="d8b30-196">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="d8b30-196">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="d8b30-197">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="d8b30-197">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="d8b30-198">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-198">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-199">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="d8b30-199">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="d8b30-200">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-200">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d8b30-201">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="d8b30-201">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="d8b30-202">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-202">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-203">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="d8b30-203">enterpriseProxiedDomains</span></span>|<span data-ttu-id="d8b30-204">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-204">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="d8b30-205">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="d8b30-205">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="d8b30-206">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="d8b30-206">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="d8b30-207">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="d8b30-207">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="d8b30-208">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-208">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-209">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="d8b30-209">enterpriseIPRanges</span></span>|<span data-ttu-id="d8b30-210">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-210">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="d8b30-211">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="d8b30-211">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="d8b30-212">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="d8b30-212">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="d8b30-213">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-213">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-214">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d8b30-214">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="d8b30-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8b30-215">Boolean</span></span>|<span data-ttu-id="d8b30-216">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="d8b30-216">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="d8b30-217">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-217">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-218">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="d8b30-218">enterpriseProxyServers</span></span>|<span data-ttu-id="d8b30-219">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-219">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d8b30-220">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="d8b30-220">This is a list of proxy servers.</span></span> <span data-ttu-id="d8b30-221">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-221">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-222">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="d8b30-222">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="d8b30-223">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-223">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d8b30-224">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="d8b30-224">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="d8b30-225">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="d8b30-225">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="d8b30-226">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="d8b30-226">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="d8b30-227">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="d8b30-227">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="d8b30-228">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-228">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-229">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="d8b30-229">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="d8b30-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8b30-230">Boolean</span></span>|<span data-ttu-id="d8b30-231">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d8b30-231">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="d8b30-232">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-232">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-233">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="d8b30-233">neutralDomainResources</span></span>|<span data-ttu-id="d8b30-234">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-234">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d8b30-235">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-235">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-236">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="d8b30-236">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="d8b30-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8b30-237">Boolean</span></span>|<span data-ttu-id="d8b30-238">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-238">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-239">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="d8b30-239">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="d8b30-240">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-240">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="d8b30-241">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-241">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="d8b30-242">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d8b30-242">isAssigned</span></span>|<span data-ttu-id="d8b30-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8b30-243">Boolean</span></span>|<span data-ttu-id="d8b30-244">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="d8b30-244">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="d8b30-245">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="d8b30-245">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d8b30-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8b30-246">Response</span></span>
<span data-ttu-id="d8b30-247">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8b30-247">If successful, this method returns a `200 OK` response code and an updated [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8b30-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8b30-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8b30-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b30-249">Request</span></span>
<span data-ttu-id="d8b30-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8b30-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
Content-type: application/json
Content-length: 3893

{
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="d8b30-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8b30-251">Response</span></span>
<span data-ttu-id="d8b30-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8b30-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4077

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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





