---
title: Criar iosEasEmailProfileConfiguration
description: Criar um novo objeto iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26d62ae6ee81b69121dd0cd5d76b110a26347cd3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949030"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="874b8-103">Criar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="874b8-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="874b8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="874b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="874b8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="874b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="874b8-106">Criar um novo objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="874b8-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="874b8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="874b8-107">Prerequisites</span></span>
<span data-ttu-id="874b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="874b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="874b8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="874b8-110">Permission type</span></span>|<span data-ttu-id="874b8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="874b8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="874b8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="874b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="874b8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="874b8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="874b8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="874b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="874b8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="874b8-115">Not supported.</span></span>|
|<span data-ttu-id="874b8-116">Application</span><span class="sxs-lookup"><span data-stu-id="874b8-116">Application</span></span>|<span data-ttu-id="874b8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="874b8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="874b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="874b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="874b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="874b8-119">Request headers</span></span>
|<span data-ttu-id="874b8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="874b8-120">Header</span></span>|<span data-ttu-id="874b8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="874b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="874b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="874b8-122">Authorization</span></span>|<span data-ttu-id="874b8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="874b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="874b8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="874b8-124">Accept</span></span>|<span data-ttu-id="874b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="874b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="874b8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="874b8-126">Request body</span></span>
<span data-ttu-id="874b8-127">No corpo da solicitação, forneça uma representação JSON do objeto iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="874b8-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="874b8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="874b8-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="874b8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="874b8-129">Property</span></span>|<span data-ttu-id="874b8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="874b8-130">Type</span></span>|<span data-ttu-id="874b8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="874b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="874b8-132">id</span><span class="sxs-lookup"><span data-stu-id="874b8-132">id</span></span>|<span data-ttu-id="874b8-133">String</span><span class="sxs-lookup"><span data-stu-id="874b8-133">String</span></span>|<span data-ttu-id="874b8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="874b8-134">Key of the entity.</span></span> <span data-ttu-id="874b8-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="874b8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="874b8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="874b8-137">DateTimeOffset</span></span>|<span data-ttu-id="874b8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="874b8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="874b8-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="874b8-140">roleScopeTagIds</span></span>|<span data-ttu-id="874b8-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="874b8-141">String collection</span></span>|<span data-ttu-id="874b8-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="874b8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="874b8-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="874b8-144">supportsScopeTags</span></span>|<span data-ttu-id="874b8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-145">Boolean</span></span>|<span data-ttu-id="874b8-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="874b8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="874b8-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="874b8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="874b8-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="874b8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="874b8-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="874b8-149">This property is read-only.</span></span> <span data-ttu-id="874b8-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="874b8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="874b8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="874b8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="874b8-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="874b8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="874b8-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="874b8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="874b8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="874b8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="874b8-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="874b8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="874b8-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="874b8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="874b8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="874b8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="874b8-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="874b8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="874b8-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="874b8-163">createdDateTime</span></span>|<span data-ttu-id="874b8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="874b8-164">DateTimeOffset</span></span>|<span data-ttu-id="874b8-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="874b8-165">DateTime the object was created.</span></span> <span data-ttu-id="874b8-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-167">description</span><span class="sxs-lookup"><span data-stu-id="874b8-167">description</span></span>|<span data-ttu-id="874b8-168">String</span><span class="sxs-lookup"><span data-stu-id="874b8-168">String</span></span>|<span data-ttu-id="874b8-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="874b8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="874b8-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="874b8-171">displayName</span></span>|<span data-ttu-id="874b8-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="874b8-172">String</span></span>|<span data-ttu-id="874b8-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="874b8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="874b8-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-175">versão</span><span class="sxs-lookup"><span data-stu-id="874b8-175">version</span></span>|<span data-ttu-id="874b8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="874b8-176">Int32</span></span>|<span data-ttu-id="874b8-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="874b8-177">Version of the device configuration.</span></span> <span data-ttu-id="874b8-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="874b8-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="874b8-179">usernameSource</span></span>|[<span data-ttu-id="874b8-180">UserEmail</span><span class="sxs-lookup"><span data-stu-id="874b8-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="874b8-181">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="874b8-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="874b8-182">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="874b8-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="874b8-183">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="874b8-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="874b8-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="874b8-184">usernameAADSource</span></span>|[<span data-ttu-id="874b8-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="874b8-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="874b8-186">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="874b8-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="874b8-187">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="874b8-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="874b8-188">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="874b8-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="874b8-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="874b8-189">userDomainNameSource</span></span>|[<span data-ttu-id="874b8-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="874b8-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="874b8-191">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="874b8-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="874b8-192">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="874b8-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="874b8-193">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="874b8-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="874b8-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="874b8-194">customDomainName</span></span>|<span data-ttu-id="874b8-195">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="874b8-195">String</span></span>|<span data-ttu-id="874b8-196">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="874b8-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="874b8-197">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="874b8-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="874b8-198">accountName</span><span class="sxs-lookup"><span data-stu-id="874b8-198">accountName</span></span>|<span data-ttu-id="874b8-199">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="874b8-199">String</span></span>|<span data-ttu-id="874b8-200">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="874b8-200">Account name.</span></span>|
|<span data-ttu-id="874b8-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="874b8-201">authenticationMethod</span></span>|[<span data-ttu-id="874b8-202">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="874b8-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="874b8-203">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="874b8-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="874b8-204">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="874b8-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="874b8-205">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="874b8-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="874b8-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-206">Boolean</span></span>|<span data-ttu-id="874b8-207">Indica se as mensagens de movimentação devem ou não ser bloqueadas para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="874b8-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="874b8-208">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="874b8-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="874b8-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-209">Boolean</span></span>|<span data-ttu-id="874b8-210">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="874b8-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="874b8-211">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="874b8-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="874b8-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-212">Boolean</span></span>|<span data-ttu-id="874b8-213">Indica se a sincronização de endereços de email usados recentemente deve ou não ser bloqueada, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="874b8-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="874b8-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="874b8-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="874b8-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="874b8-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="874b8-216">Duração de tempo que o email deve ser sincronizado de volta para o.</span><span class="sxs-lookup"><span data-stu-id="874b8-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="874b8-217">.</span><span class="sxs-lookup"><span data-stu-id="874b8-217"></span></span> <span data-ttu-id="874b8-218">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="874b8-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="874b8-219">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="874b8-219">emailAddressSource</span></span>|[<span data-ttu-id="874b8-220">UserEmail</span><span class="sxs-lookup"><span data-stu-id="874b8-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="874b8-221">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="874b8-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="874b8-222">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="874b8-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="874b8-223">easServices</span><span class="sxs-lookup"><span data-stu-id="874b8-223">easServices</span></span>|[<span data-ttu-id="874b8-224">easServices</span><span class="sxs-lookup"><span data-stu-id="874b8-224">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="874b8-225">Trocar dados a serem sincronizados. Os valores possíveis são `none`: `calendars`, `contacts`, `email`, `notes`, `reminders`,.</span><span class="sxs-lookup"><span data-stu-id="874b8-225">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="874b8-226">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="874b8-226">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="874b8-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-227">Boolean</span></span>|<span data-ttu-id="874b8-228">Permitir que os usuários alterem as configurações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="874b8-228">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="874b8-229">hostName</span><span class="sxs-lookup"><span data-stu-id="874b8-229">hostName</span></span>|<span data-ttu-id="874b8-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="874b8-230">String</span></span>|<span data-ttu-id="874b8-231">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="874b8-231">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="874b8-232">requireSmime</span><span class="sxs-lookup"><span data-stu-id="874b8-232">requireSmime</span></span>|<span data-ttu-id="874b8-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-233">Boolean</span></span>|<span data-ttu-id="874b8-234">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="874b8-234">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="874b8-235">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="874b8-235">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="874b8-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-236">Boolean</span></span>|<span data-ttu-id="874b8-237">Indica se os emails não criptografados devem ou não ser permitidos.</span><span class="sxs-lookup"><span data-stu-id="874b8-237">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="874b8-238">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="874b8-238">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="874b8-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-239">Boolean</span></span>|<span data-ttu-id="874b8-240">Se definido como true a criptografia S/MIME estiver habilitada por padrão.</span><span class="sxs-lookup"><span data-stu-id="874b8-240">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="874b8-241">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="874b8-241">smimeSigningEnabled</span></span>|<span data-ttu-id="874b8-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-242">Boolean</span></span>|<span data-ttu-id="874b8-243">Se definido como true a assinatura S/MIME estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="874b8-243">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="874b8-244">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="874b8-244">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="874b8-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-245">Boolean</span></span>|<span data-ttu-id="874b8-246">Se definido como true, o usuário pode ativar ou desativar a assinatura S/MIME.</span><span class="sxs-lookup"><span data-stu-id="874b8-246">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="874b8-247">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="874b8-247">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="874b8-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-248">Boolean</span></span>|<span data-ttu-id="874b8-249">Se definido como true, o usuário pode ativar a opção criptografia por padrão.</span><span class="sxs-lookup"><span data-stu-id="874b8-249">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="874b8-250">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="874b8-250">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="874b8-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-251">Boolean</span></span>|<span data-ttu-id="874b8-252">Se definido como true, o usuário pode selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="874b8-252">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="874b8-253">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="874b8-253">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="874b8-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-254">Boolean</span></span>|<span data-ttu-id="874b8-255">Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="874b8-255">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="874b8-256">requireSsl</span><span class="sxs-lookup"><span data-stu-id="874b8-256">requireSsl</span></span>|<span data-ttu-id="874b8-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-257">Boolean</span></span>|<span data-ttu-id="874b8-258">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="874b8-258">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="874b8-259">useOAuth</span><span class="sxs-lookup"><span data-stu-id="874b8-259">useOAuth</span></span>|<span data-ttu-id="874b8-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="874b8-260">Boolean</span></span>|<span data-ttu-id="874b8-261">Especifica se a conexão deve usar o OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="874b8-261">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="874b8-262">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="874b8-262">signingCertificateType</span></span>|[<span data-ttu-id="874b8-263">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="874b8-263">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="874b8-264">Assinatura tipo de certificado para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="874b8-264">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="874b8-265">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="874b8-265">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="874b8-266">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="874b8-266">encryptionCertificateType</span></span>|[<span data-ttu-id="874b8-267">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="874b8-267">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="874b8-268">Tipo de certificado de criptografia para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="874b8-268">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="874b8-269">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="874b8-269">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="874b8-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="874b8-270">Response</span></span>
<span data-ttu-id="874b8-271">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="874b8-271">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="874b8-272">Exemplo</span><span class="sxs-lookup"><span data-stu-id="874b8-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="874b8-273">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874b8-273">Request</span></span>
<span data-ttu-id="874b8-274">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="874b8-274">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2131

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
  "encryptionCertificateType": "certificate"
}
```

### <a name="response"></a><span data-ttu-id="874b8-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="874b8-275">Response</span></span>
<span data-ttu-id="874b8-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="874b8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2303

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
  "encryptionCertificateType": "certificate"
}
```





