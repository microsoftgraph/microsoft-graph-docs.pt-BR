---
title: Atualizar iosEasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e7b1b7e311db6547627f8367bf0a8f9e0bf252f9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265056"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="15379-103">Atualizar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="15379-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="15379-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15379-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15379-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15379-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15379-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15379-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15379-107">Atualiza as propriedades de um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="15379-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15379-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15379-108">Prerequisites</span></span>
<span data-ttu-id="15379-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15379-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15379-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15379-111">Permission type</span></span>|<span data-ttu-id="15379-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15379-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15379-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15379-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15379-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15379-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15379-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15379-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15379-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15379-116">Not supported.</span></span>|
|<span data-ttu-id="15379-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15379-117">Application</span></span>|<span data-ttu-id="15379-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15379-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15379-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15379-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="15379-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15379-120">Request headers</span></span>
|<span data-ttu-id="15379-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15379-121">Header</span></span>|<span data-ttu-id="15379-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15379-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15379-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15379-123">Authorization</span></span>|<span data-ttu-id="15379-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15379-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15379-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15379-125">Accept</span></span>|<span data-ttu-id="15379-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15379-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15379-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15379-127">Request body</span></span>
<span data-ttu-id="15379-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="15379-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="15379-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15379-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="15379-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15379-130">Property</span></span>|<span data-ttu-id="15379-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="15379-131">Type</span></span>|<span data-ttu-id="15379-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="15379-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15379-133">id</span><span class="sxs-lookup"><span data-stu-id="15379-133">id</span></span>|<span data-ttu-id="15379-134">String</span><span class="sxs-lookup"><span data-stu-id="15379-134">String</span></span>|<span data-ttu-id="15379-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="15379-135">Key of the entity.</span></span> <span data-ttu-id="15379-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15379-137">lastModifiedDateTime</span></span>|<span data-ttu-id="15379-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15379-138">DateTimeOffset</span></span>|<span data-ttu-id="15379-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="15379-139">DateTime the object was last modified.</span></span> <span data-ttu-id="15379-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15379-141">roleScopeTagIds</span></span>|<span data-ttu-id="15379-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="15379-142">String collection</span></span>|<span data-ttu-id="15379-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="15379-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15379-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="15379-145">supportsScopeTags</span></span>|<span data-ttu-id="15379-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-146">Boolean</span></span>|<span data-ttu-id="15379-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="15379-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="15379-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="15379-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="15379-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="15379-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="15379-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="15379-150">This property is read-only.</span></span> <span data-ttu-id="15379-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15379-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="15379-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15379-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="15379-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="15379-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="15379-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15379-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="15379-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15379-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="15379-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="15379-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="15379-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15379-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="15379-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15379-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="15379-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="15379-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="15379-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15379-164">createdDateTime</span></span>|<span data-ttu-id="15379-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15379-165">DateTimeOffset</span></span>|<span data-ttu-id="15379-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="15379-166">DateTime the object was created.</span></span> <span data-ttu-id="15379-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-168">description</span><span class="sxs-lookup"><span data-stu-id="15379-168">description</span></span>|<span data-ttu-id="15379-169">String</span><span class="sxs-lookup"><span data-stu-id="15379-169">String</span></span>|<span data-ttu-id="15379-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15379-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15379-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-172">displayName</span><span class="sxs-lookup"><span data-stu-id="15379-172">displayName</span></span>|<span data-ttu-id="15379-173">String</span><span class="sxs-lookup"><span data-stu-id="15379-173">String</span></span>|<span data-ttu-id="15379-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15379-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15379-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-176">versão</span><span class="sxs-lookup"><span data-stu-id="15379-176">version</span></span>|<span data-ttu-id="15379-177">Int32</span><span class="sxs-lookup"><span data-stu-id="15379-177">Int32</span></span>|<span data-ttu-id="15379-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15379-178">Version of the device configuration.</span></span> <span data-ttu-id="15379-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15379-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15379-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="15379-180">usernameSource</span></span>|[<span data-ttu-id="15379-181">UserEmail</span><span class="sxs-lookup"><span data-stu-id="15379-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="15379-182">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15379-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="15379-183">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="15379-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="15379-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="15379-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="15379-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="15379-185">usernameAADSource</span></span>|[<span data-ttu-id="15379-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="15379-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="15379-187">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="15379-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="15379-188">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="15379-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="15379-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="15379-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="15379-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="15379-190">userDomainNameSource</span></span>|[<span data-ttu-id="15379-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="15379-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="15379-192">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15379-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="15379-193">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="15379-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="15379-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="15379-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="15379-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="15379-195">customDomainName</span></span>|<span data-ttu-id="15379-196">String</span><span class="sxs-lookup"><span data-stu-id="15379-196">String</span></span>|<span data-ttu-id="15379-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15379-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="15379-198">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="15379-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="15379-199">accountName</span><span class="sxs-lookup"><span data-stu-id="15379-199">accountName</span></span>|<span data-ttu-id="15379-200">String</span><span class="sxs-lookup"><span data-stu-id="15379-200">String</span></span>|<span data-ttu-id="15379-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="15379-201">Account name.</span></span>|
|<span data-ttu-id="15379-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="15379-202">authenticationMethod</span></span>|[<span data-ttu-id="15379-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="15379-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="15379-204">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="15379-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="15379-205">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="15379-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="15379-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="15379-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="15379-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-207">Boolean</span></span>|<span data-ttu-id="15379-208">Indica se as mensagens de movimentação devem ou não ser bloqueadas para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="15379-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="15379-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="15379-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="15379-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-210">Boolean</span></span>|<span data-ttu-id="15379-211">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="15379-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="15379-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="15379-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="15379-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-213">Boolean</span></span>|<span data-ttu-id="15379-214">Indica se a sincronização de endereços de email usados recentemente deve ou não ser bloqueada, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="15379-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="15379-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="15379-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="15379-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="15379-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="15379-217">Duração de tempo que o email deve ser sincronizado de volta para o.</span><span class="sxs-lookup"><span data-stu-id="15379-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="15379-218">.</span><span class="sxs-lookup"><span data-stu-id="15379-218">.</span></span> <span data-ttu-id="15379-219">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="15379-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="15379-220">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="15379-220">emailAddressSource</span></span>|[<span data-ttu-id="15379-221">UserEmail</span><span class="sxs-lookup"><span data-stu-id="15379-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="15379-222">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15379-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="15379-223">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="15379-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="15379-224">easServices</span><span class="sxs-lookup"><span data-stu-id="15379-224">easServices</span></span>|[<span data-ttu-id="15379-225">easServices</span><span class="sxs-lookup"><span data-stu-id="15379-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="15379-226">Trocar dados a serem sincronizados. Os valores possíveis são: `none` , `calendars` , `contacts` , `email` , `notes` , `reminders` .</span><span class="sxs-lookup"><span data-stu-id="15379-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="15379-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="15379-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="15379-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-228">Boolean</span></span>|<span data-ttu-id="15379-229">Permitir que os usuários alterem as configurações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="15379-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="15379-230">hostName</span><span class="sxs-lookup"><span data-stu-id="15379-230">hostName</span></span>|<span data-ttu-id="15379-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15379-231">String</span></span>|<span data-ttu-id="15379-232">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="15379-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="15379-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="15379-233">requireSmime</span></span>|<span data-ttu-id="15379-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-234">Boolean</span></span>|<span data-ttu-id="15379-235">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="15379-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="15379-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="15379-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="15379-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-237">Boolean</span></span>|<span data-ttu-id="15379-238">Indica se os emails não criptografados devem ou não ser permitidos.</span><span class="sxs-lookup"><span data-stu-id="15379-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="15379-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="15379-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="15379-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-240">Boolean</span></span>|<span data-ttu-id="15379-241">Se definido como true a criptografia S/MIME estiver habilitada por padrão.</span><span class="sxs-lookup"><span data-stu-id="15379-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="15379-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="15379-242">smimeSigningEnabled</span></span>|<span data-ttu-id="15379-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-243">Boolean</span></span>|<span data-ttu-id="15379-244">Se definido como true a assinatura S/MIME estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="15379-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="15379-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="15379-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="15379-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-246">Boolean</span></span>|<span data-ttu-id="15379-247">Se definido como true, o usuário pode ativar ou desativar a assinatura S/MIME.</span><span class="sxs-lookup"><span data-stu-id="15379-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="15379-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="15379-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="15379-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-249">Boolean</span></span>|<span data-ttu-id="15379-250">Se definido como true, o usuário pode ativar a opção criptografia por padrão.</span><span class="sxs-lookup"><span data-stu-id="15379-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="15379-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="15379-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="15379-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-252">Boolean</span></span>|<span data-ttu-id="15379-253">Se definido como true, o usuário pode selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="15379-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="15379-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="15379-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="15379-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-255">Boolean</span></span>|<span data-ttu-id="15379-256">Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="15379-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="15379-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="15379-257">requireSsl</span></span>|<span data-ttu-id="15379-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-258">Boolean</span></span>|<span data-ttu-id="15379-259">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="15379-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="15379-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="15379-260">useOAuth</span></span>|<span data-ttu-id="15379-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="15379-261">Boolean</span></span>|<span data-ttu-id="15379-262">Especifica se a conexão deve usar o OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="15379-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="15379-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="15379-263">signingCertificateType</span></span>|[<span data-ttu-id="15379-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="15379-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="15379-265">Assinatura tipo de certificado para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="15379-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="15379-266">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="15379-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="15379-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="15379-267">encryptionCertificateType</span></span>|[<span data-ttu-id="15379-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="15379-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="15379-269">Tipo de certificado de criptografia para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="15379-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="15379-270">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="15379-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="15379-271">perAppVPNProfileId</span><span class="sxs-lookup"><span data-stu-id="15379-271">perAppVPNProfileId</span></span>|<span data-ttu-id="15379-272">String</span><span class="sxs-lookup"><span data-stu-id="15379-272">String</span></span>|<span data-ttu-id="15379-273">ID de perfil da política de VPN Per-App a ser usada para acessar emails a partir do cliente de email nativo</span><span class="sxs-lookup"><span data-stu-id="15379-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="15379-274">Resposta</span><span class="sxs-lookup"><span data-stu-id="15379-274">Response</span></span>
<span data-ttu-id="15379-275">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15379-275">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15379-276">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15379-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="15379-277">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15379-277">Request</span></span>
<span data-ttu-id="15379-278">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15379-278">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2187

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "easServices": "calendars",
  "easServicesUserOverrideEnabled": true,
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate",
  "perAppVPNProfileId": "Per App VPNProfile Id value"
}
```

### <a name="response"></a><span data-ttu-id="15379-279">Resposta</span><span class="sxs-lookup"><span data-stu-id="15379-279">Response</span></span>
<span data-ttu-id="15379-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15379-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2359

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "easServices": "calendars",
  "easServicesUserOverrideEnabled": true,
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate",
  "perAppVPNProfileId": "Per App VPNProfile Id value"
}
```




