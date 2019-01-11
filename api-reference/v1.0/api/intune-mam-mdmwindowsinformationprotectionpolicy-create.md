---
title: Criar mdmWindowsInformationProtectionPolicy
description: Cria um novo objeto mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc1a96f6fb6bf4e8ea2ec20289aa9dfa68ccfa03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826023"
---
# <a name="create-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="41c71-103">Criar mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="41c71-103">Create mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="41c71-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="41c71-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41c71-105">Cria um novo objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="41c71-105">Create a new [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41c71-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41c71-106">Prerequisites</span></span>
<span data-ttu-id="41c71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41c71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c71-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41c71-109">Permission type</span></span>|<span data-ttu-id="41c71-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41c71-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41c71-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41c71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41c71-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41c71-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41c71-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41c71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41c71-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41c71-114">Not supported.</span></span>|
|<span data-ttu-id="41c71-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41c71-115">Application</span></span>|<span data-ttu-id="41c71-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41c71-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41c71-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41c71-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="41c71-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41c71-118">Request headers</span></span>
|<span data-ttu-id="41c71-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41c71-119">Header</span></span>|<span data-ttu-id="41c71-120">Valor</span><span class="sxs-lookup"><span data-stu-id="41c71-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41c71-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="41c71-121">Authorization</span></span>|<span data-ttu-id="41c71-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41c71-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41c71-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41c71-123">Accept</span></span>|<span data-ttu-id="41c71-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41c71-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41c71-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41c71-125">Request body</span></span>
<span data-ttu-id="41c71-126">No corpo da solicitação, forneça uma representação JSON do objeto mdmWindowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="41c71-126">In the request body, supply a JSON representation for the mdmWindowsInformationProtectionPolicy object.</span></span>

<span data-ttu-id="41c71-127">A tabela a seguir mostra as propriedades que são necessárias ao criar mdmWindowsInformationProtectionPolicy.</span><span class="sxs-lookup"><span data-stu-id="41c71-127">The following table shows the properties that are required when you create the mdmWindowsInformationProtectionPolicy.</span></span>

|<span data-ttu-id="41c71-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41c71-128">Property</span></span>|<span data-ttu-id="41c71-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="41c71-129">Type</span></span>|<span data-ttu-id="41c71-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="41c71-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41c71-131">displayName</span><span class="sxs-lookup"><span data-stu-id="41c71-131">displayName</span></span>|<span data-ttu-id="41c71-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41c71-132">String</span></span>|<span data-ttu-id="41c71-133">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="41c71-133">Policy display name.</span></span> <span data-ttu-id="41c71-134">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41c71-135">description</span><span class="sxs-lookup"><span data-stu-id="41c71-135">description</span></span>|<span data-ttu-id="41c71-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41c71-136">String</span></span>|<span data-ttu-id="41c71-137">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="41c71-137">The policy's description.</span></span> <span data-ttu-id="41c71-138">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41c71-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41c71-139">createdDateTime</span></span>|<span data-ttu-id="41c71-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41c71-140">DateTimeOffset</span></span>|<span data-ttu-id="41c71-141">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="41c71-141">The date and time the policy was created.</span></span> <span data-ttu-id="41c71-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41c71-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41c71-143">lastModifiedDateTime</span></span>|<span data-ttu-id="41c71-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41c71-144">DateTimeOffset</span></span>|<span data-ttu-id="41c71-145">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="41c71-145">Last time the policy was modified.</span></span> <span data-ttu-id="41c71-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41c71-147">id</span><span class="sxs-lookup"><span data-stu-id="41c71-147">id</span></span>|<span data-ttu-id="41c71-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41c71-148">String</span></span>|<span data-ttu-id="41c71-149">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="41c71-149">Key of the entity.</span></span> <span data-ttu-id="41c71-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41c71-151">version</span><span class="sxs-lookup"><span data-stu-id="41c71-151">version</span></span>|<span data-ttu-id="41c71-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41c71-152">String</span></span>|<span data-ttu-id="41c71-153">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="41c71-153">Version of the entity.</span></span> <span data-ttu-id="41c71-154">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="41c71-155">enforcementLevel</span><span class="sxs-lookup"><span data-stu-id="41c71-155">enforcementLevel</span></span>|[<span data-ttu-id="41c71-156">windowsInformationProtectionEnforcementLevel</span><span class="sxs-lookup"><span data-stu-id="41c71-156">windowsInformationProtectionEnforcementLevel</span></span>](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|<span data-ttu-id="41c71-157">Nível da imposição de WIP. Consulte a definição de Enum de valores suportados Inherited de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="41c71-157">WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span></span> <span data-ttu-id="41c71-158">Os valores possíveis são: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span><span class="sxs-lookup"><span data-stu-id="41c71-158">Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.</span></span>|
|<span data-ttu-id="41c71-159">enterpriseDomain</span><span class="sxs-lookup"><span data-stu-id="41c71-159">enterpriseDomain</span></span>|<span data-ttu-id="41c71-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41c71-160">String</span></span>|<span data-ttu-id="41c71-161">Domínio primário da empresa Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-161">Primary enterprise domain Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-162">enterpriseProtectedDomainNames</span><span class="sxs-lookup"><span data-stu-id="41c71-162">enterpriseProtectedDomainNames</span></span>|<span data-ttu-id="41c71-163">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-163">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41c71-164">Lista de domínios primários da empresa a serem protegidos Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-164">List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-165">protectionUnderLockConfigRequired</span><span class="sxs-lookup"><span data-stu-id="41c71-165">protectionUnderLockConfigRequired</span></span>|<span data-ttu-id="41c71-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="41c71-166">Boolean</span></span>|<span data-ttu-id="41c71-167">Especifica se a proteção no recurso de bloqueio (também conhecido como criptografar com pin) deve ser configurada Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-167">Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-168">dataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="41c71-168">dataRecoveryCertificate</span></span>|[<span data-ttu-id="41c71-169">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="41c71-169">windowsInformationProtectionDataRecoveryCertificate</span></span>](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|<span data-ttu-id="41c71-170">Especifica um certificado de recuperação que pode ser usado para recuperação de dados de arquivos criptografados.</span><span class="sxs-lookup"><span data-stu-id="41c71-170">Specifies a recovery certificate that can be used for data recovery of encrypted files.</span></span> <span data-ttu-id="41c71-171">Isso é o mesmo que o certificado do Agente de recuperação de dados (DRA) para sistema de arquivos com criptografia (EFS) Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-171">This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-172">revokeOnUnenrollDisabled</span><span class="sxs-lookup"><span data-stu-id="41c71-172">revokeOnUnenrollDisabled</span></span>|<span data-ttu-id="41c71-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="41c71-173">Boolean</span></span>|<span data-ttu-id="41c71-174">Essa política controla se as teclas WIP serão revogadas quando for cancelado o registro de um dispositivo no serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="41c71-174">This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.</span></span> <span data-ttu-id="41c71-175">Se definido como 1 (não revogar teclas), as teclas não serão revogadas, e o usuário continuará a ter acesso a arquivos protegidos após o cancelamento de registro.</span><span class="sxs-lookup"><span data-stu-id="41c71-175">If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.</span></span> <span data-ttu-id="41c71-176">Se as teclas não forem revogadas, não haverá limpeza de arquivos revogados posteriormente.</span><span class="sxs-lookup"><span data-stu-id="41c71-176">If the keys are not revoked, there will be no revoked file cleanup subsequently.</span></span> <span data-ttu-id="41c71-177">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-177">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-178">rightsManagementServicesTemplateId</span><span class="sxs-lookup"><span data-stu-id="41c71-178">rightsManagementServicesTemplateId</span></span>|<span data-ttu-id="41c71-179">Guid</span><span class="sxs-lookup"><span data-stu-id="41c71-179">Guid</span></span>|<span data-ttu-id="41c71-180">GUID de TemplateID para uso em criptografia RMS.</span><span class="sxs-lookup"><span data-stu-id="41c71-180">TemplateID GUID to use for RMS encryption.</span></span> <span data-ttu-id="41c71-181">O modelo do RMS permite ao administrador de TI configurar os detalhes sobre quem tem acesso a arquivos protegidos por RMS e por quanto tempo tem esse acesso Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-181">The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-182">azureRightsManagementServicesAllowed</span><span class="sxs-lookup"><span data-stu-id="41c71-182">azureRightsManagementServicesAllowed</span></span>|<span data-ttu-id="41c71-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="41c71-183">Boolean</span></span>|<span data-ttu-id="41c71-184">Especifica se a criptografia do Azure RMS para WIP será permitida Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-184">Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-185">iconsVisible</span><span class="sxs-lookup"><span data-stu-id="41c71-185">iconsVisible</span></span>|<span data-ttu-id="41c71-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="41c71-186">Boolean</span></span>|<span data-ttu-id="41c71-187">Determina se sobreposições são adicionadas a ícones em arquivos protegido por WIP no Explorador e em blocos de aplicativos somente para empresas no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="41c71-187">Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.</span></span> <span data-ttu-id="41c71-188">A partir do Windows 10, versão 1703, essa configuração também define a visibilidade do ícone WIP na barra de título de um aplicativo protegido por WIP Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-188">Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-189">protectedApps</span><span class="sxs-lookup"><span data-stu-id="41c71-189">protectedApps</span></span>|<span data-ttu-id="41c71-190">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-190">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="41c71-191">Aplicativos protegidos podem acessar dados corporativos, e os dados manipulados por esses aplicativos são protegidos com criptografia Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-191">Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-192">exemptApps</span><span class="sxs-lookup"><span data-stu-id="41c71-192">exemptApps</span></span>|<span data-ttu-id="41c71-193">Coleção [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-193">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) collection</span></span>|<span data-ttu-id="41c71-194">Os aplicativos isentos também podem acessar dados corporativos, mas os dados manipulados por esses aplicativos não são protegidos.</span><span class="sxs-lookup"><span data-stu-id="41c71-194">Exempt applications can also access enterprise data, but the data handled by those applications are not protected.</span></span> <span data-ttu-id="41c71-195">Isso ocorre porque alguns aplicativos corporativos essenciais podem ter problemas de compatibilidade com dados criptografados.</span><span class="sxs-lookup"><span data-stu-id="41c71-195">This is because some critical enterprise applications may have compatibility problems with encrypted data.</span></span> <span data-ttu-id="41c71-196">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-196">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-197">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="41c71-197">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="41c71-198">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-198">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41c71-199">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="41c71-199">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="41c71-200">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e serão protegidos Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-200">Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-201">enterpriseProxiedDomains</span><span class="sxs-lookup"><span data-stu-id="41c71-201">enterpriseProxiedDomains</span></span>|<span data-ttu-id="41c71-202">Coleção [windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-202">[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) collection</span></span>|<span data-ttu-id="41c71-203">Contém uma lista de domínios de recursos da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="41c71-203">Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="41c71-204">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="41c71-204">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="41c71-205">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="41c71-205">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="41c71-206">Um servidor proxy usado com essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-206">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-207">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="41c71-207">enterpriseIPRanges</span></span>|<span data-ttu-id="41c71-208">Coleção [windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-208">[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) collection</span></span>|<span data-ttu-id="41c71-209">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="41c71-209">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="41c71-210">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="41c71-210">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="41c71-211">Esses locais serão considerados um destino seguro para que dados corporativos sejam compartilhados Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-211">These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-212">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="41c71-212">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="41c71-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="41c71-213">Boolean</span></span>|<span data-ttu-id="41c71-214">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="41c71-214">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="41c71-215">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-215">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-216">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="41c71-216">enterpriseProxyServers</span></span>|<span data-ttu-id="41c71-217">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-217">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41c71-218">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="41c71-218">This is a list of proxy servers.</span></span> <span data-ttu-id="41c71-219">Qualquer servidor que não esteja na lista é considerado não corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-219">Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-220">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="41c71-220">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="41c71-221">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-221">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41c71-222">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="41c71-222">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="41c71-223">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="41c71-223">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="41c71-224">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="41c71-224">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="41c71-225">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="41c71-225">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="41c71-226">Os proxies são utilizados somente na configuração da política EnterpriseProxiedDomains para forçar o tráfego para os domínios correspondentes por meio desses proxies Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-226">The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-227">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="41c71-227">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="41c71-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="41c71-228">Boolean</span></span>|<span data-ttu-id="41c71-229">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="41c71-229">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="41c71-230">A padrão é false Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-230">Default is false Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-231">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="41c71-231">neutralDomainResources</span></span>|<span data-ttu-id="41c71-232">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-232">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41c71-233">Lista de nomes de domínio que podem ser usados para recurso de trabalho ou pessoal Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-233">List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-234">indexingEncryptedStoresOrItemsBlocked</span><span class="sxs-lookup"><span data-stu-id="41c71-234">indexingEncryptedStoresOrItemsBlocked</span></span>|<span data-ttu-id="41c71-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="41c71-235">Boolean</span></span>|<span data-ttu-id="41c71-236">Esta opção é para o indexador do Windows Search para permitir ou não a indexação de itens Herdado do [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-236">This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-237">smbAutoEncryptedFileExtensions</span><span class="sxs-lookup"><span data-stu-id="41c71-237">smbAutoEncryptedFileExtensions</span></span>|<span data-ttu-id="41c71-238">Coleção [windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-238">[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) collection</span></span>|<span data-ttu-id="41c71-239">Especifica uma lista de extensões de arquivo para que os arquivos com essas extensões sejam criptografados quando copiados de um compartilhamento SMB dentro do limite corporativo Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-239">Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|
|<span data-ttu-id="41c71-240">isAssigned</span><span class="sxs-lookup"><span data-stu-id="41c71-240">isAssigned</span></span>|<span data-ttu-id="41c71-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="41c71-241">Boolean</span></span>|<span data-ttu-id="41c71-242">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="41c71-242">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="41c71-243">Herdado de [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span><span class="sxs-lookup"><span data-stu-id="41c71-243">Inherited from [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)</span></span>|



## <a name="response"></a><span data-ttu-id="41c71-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="41c71-244">Response</span></span>
<span data-ttu-id="41c71-245">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41c71-245">If successful, this method returns a `201 Created` response code and a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41c71-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41c71-246">Example</span></span>
### <a name="request"></a><span data-ttu-id="41c71-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41c71-247">Request</span></span>
<span data-ttu-id="41c71-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41c71-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
Content-type: application/json
Content-length: 3905

{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="41c71-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="41c71-249">Response</span></span>
<span data-ttu-id="41c71-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41c71-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



