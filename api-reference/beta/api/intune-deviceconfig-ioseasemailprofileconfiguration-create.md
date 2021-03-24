---
title: Criar iosEasEmailProfileConfiguration
description: Crie um novo objeto iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eb8a26779255430cf000e7047ef871d8da96b1a4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130011"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="4ed54-103">Criar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ed54-103">Create iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="4ed54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ed54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ed54-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ed54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ed54-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ed54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed54-107">Crie um novo [objeto iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ed54-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ed54-108">Prerequisites</span></span>
<span data-ttu-id="4ed54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ed54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ed54-111">Permission type</span></span>|<span data-ttu-id="4ed54-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ed54-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ed54-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ed54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ed54-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ed54-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ed54-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ed54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ed54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ed54-116">Not supported.</span></span>|
|<span data-ttu-id="4ed54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ed54-117">Application</span></span>|<span data-ttu-id="4ed54-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ed54-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ed54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ed54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ed54-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed54-120">Request headers</span></span>
|<span data-ttu-id="4ed54-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ed54-121">Header</span></span>|<span data-ttu-id="4ed54-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4ed54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ed54-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ed54-123">Authorization</span></span>|<span data-ttu-id="4ed54-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ed54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ed54-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ed54-125">Accept</span></span>|<span data-ttu-id="4ed54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ed54-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed54-127">Request body</span></span>
<span data-ttu-id="4ed54-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ed54-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="4ed54-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ed54-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="4ed54-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ed54-130">Property</span></span>|<span data-ttu-id="4ed54-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ed54-131">Type</span></span>|<span data-ttu-id="4ed54-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ed54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed54-133">id</span><span class="sxs-lookup"><span data-stu-id="4ed54-133">id</span></span>|<span data-ttu-id="4ed54-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed54-134">String</span></span>|<span data-ttu-id="4ed54-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ed54-135">Key of the entity.</span></span> <span data-ttu-id="4ed54-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ed54-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4ed54-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ed54-138">DateTimeOffset</span></span>|<span data-ttu-id="4ed54-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4ed54-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4ed54-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ed54-141">roleScopeTagIds</span></span>|<span data-ttu-id="4ed54-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed54-142">String collection</span></span>|<span data-ttu-id="4ed54-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="4ed54-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ed54-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ed54-145">supportsScopeTags</span></span>|<span data-ttu-id="4ed54-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-146">Boolean</span></span>|<span data-ttu-id="4ed54-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ed54-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ed54-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4ed54-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ed54-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4ed54-150">This property is read-only.</span></span> <span data-ttu-id="4ed54-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ed54-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4ed54-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ed54-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4ed54-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4ed54-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4ed54-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ed54-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4ed54-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ed54-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4ed54-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4ed54-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4ed54-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ed54-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4ed54-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ed54-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4ed54-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4ed54-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4ed54-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ed54-164">createdDateTime</span></span>|<span data-ttu-id="4ed54-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ed54-165">DateTimeOffset</span></span>|<span data-ttu-id="4ed54-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4ed54-166">DateTime the object was created.</span></span> <span data-ttu-id="4ed54-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-168">descrição</span><span class="sxs-lookup"><span data-stu-id="4ed54-168">description</span></span>|<span data-ttu-id="4ed54-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed54-169">String</span></span>|<span data-ttu-id="4ed54-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ed54-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4ed54-172">displayName</span></span>|<span data-ttu-id="4ed54-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed54-173">String</span></span>|<span data-ttu-id="4ed54-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ed54-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-176">versão</span><span class="sxs-lookup"><span data-stu-id="4ed54-176">version</span></span>|<span data-ttu-id="4ed54-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4ed54-177">Int32</span></span>|<span data-ttu-id="4ed54-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-178">Version of the device configuration.</span></span> <span data-ttu-id="4ed54-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed54-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4ed54-180">usernameSource</span></span>|[<span data-ttu-id="4ed54-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4ed54-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4ed54-182">Atributo username que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4ed54-183">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4ed54-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4ed54-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="4ed54-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4ed54-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="4ed54-185">usernameAADSource</span></span>|[<span data-ttu-id="4ed54-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4ed54-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="4ed54-187">Nome do campo AAD, que será usado para recuperar UserName para perfil de email.</span><span class="sxs-lookup"><span data-stu-id="4ed54-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="4ed54-188">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4ed54-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4ed54-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="4ed54-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="4ed54-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="4ed54-190">userDomainNameSource</span></span>|[<span data-ttu-id="4ed54-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="4ed54-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="4ed54-192">Atributo UserDomainname que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4ed54-193">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4ed54-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4ed54-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="4ed54-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="4ed54-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="4ed54-195">customDomainName</span></span>|<span data-ttu-id="4ed54-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed54-196">String</span></span>|<span data-ttu-id="4ed54-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="4ed54-198">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="4ed54-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="4ed54-199">accountName</span><span class="sxs-lookup"><span data-stu-id="4ed54-199">accountName</span></span>|<span data-ttu-id="4ed54-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed54-200">String</span></span>|<span data-ttu-id="4ed54-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="4ed54-201">Account name.</span></span>|
|<span data-ttu-id="4ed54-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ed54-202">authenticationMethod</span></span>|[<span data-ttu-id="4ed54-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ed54-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="4ed54-204">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="4ed54-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="4ed54-205">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="4ed54-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4ed54-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="4ed54-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="4ed54-207">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-207">Boolean</span></span>|<span data-ttu-id="4ed54-208">Indica se deve ou não bloquear a movimentação de mensagens para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="4ed54-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="4ed54-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="4ed54-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="4ed54-210">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-210">Boolean</span></span>|<span data-ttu-id="4ed54-211">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4ed54-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="4ed54-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="4ed54-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="4ed54-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-213">Boolean</span></span>|<span data-ttu-id="4ed54-214">Indica se deve ou não bloquear a sincronização de endereços de email usados recentemente, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="4ed54-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="4ed54-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="4ed54-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="4ed54-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="4ed54-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4ed54-217">A duração do tempo em que o email deve ser sincronizado novamente.</span><span class="sxs-lookup"><span data-stu-id="4ed54-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="4ed54-218">.</span><span class="sxs-lookup"><span data-stu-id="4ed54-218">.</span></span> <span data-ttu-id="4ed54-219">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="4ed54-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4ed54-220">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="4ed54-220">emailAddressSource</span></span>|[<span data-ttu-id="4ed54-221">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4ed54-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4ed54-222">Atributo de email que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ed54-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4ed54-223">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="4ed54-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4ed54-224">easServices</span><span class="sxs-lookup"><span data-stu-id="4ed54-224">easServices</span></span>|[<span data-ttu-id="4ed54-225">easServices</span><span class="sxs-lookup"><span data-stu-id="4ed54-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="4ed54-226">Dados do Exchange para sincronização. Os valores possíveis `none` são: `calendars` , , , , , `contacts` `email` `notes` `reminders` .</span><span class="sxs-lookup"><span data-stu-id="4ed54-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="4ed54-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4ed54-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="4ed54-228">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-228">Boolean</span></span>|<span data-ttu-id="4ed54-229">Permitir que os usuários alterem as configurações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4ed54-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="4ed54-230">hostName</span><span class="sxs-lookup"><span data-stu-id="4ed54-230">hostName</span></span>|<span data-ttu-id="4ed54-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed54-231">String</span></span>|<span data-ttu-id="4ed54-232">Local do Exchange que (URL) ao que o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="4ed54-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="4ed54-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="4ed54-233">requireSmime</span></span>|<span data-ttu-id="4ed54-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-234">Boolean</span></span>|<span data-ttu-id="4ed54-235">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="4ed54-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="4ed54-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="4ed54-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="4ed54-237">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-237">Boolean</span></span>|<span data-ttu-id="4ed54-238">Indica se os emails não criptografados permitirão ou não.</span><span class="sxs-lookup"><span data-stu-id="4ed54-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="4ed54-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="4ed54-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="4ed54-240">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-240">Boolean</span></span>|<span data-ttu-id="4ed54-241">Se definido como criptografia S/MIME verdadeiro estiver habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="4ed54-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="4ed54-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="4ed54-242">smimeSigningEnabled</span></span>|<span data-ttu-id="4ed54-243">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-243">Boolean</span></span>|<span data-ttu-id="4ed54-244">Se definido como a assinatura S/MIME verdadeira estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="4ed54-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="4ed54-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4ed54-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="4ed54-246">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-246">Boolean</span></span>|<span data-ttu-id="4ed54-247">Se for definido como true, o usuário poderá alternar a sessão S/MIME para 1 ou 2016.</span><span class="sxs-lookup"><span data-stu-id="4ed54-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="4ed54-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4ed54-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="4ed54-249">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-249">Boolean</span></span>|<span data-ttu-id="4ed54-250">Se definido como true, o usuário pode alternar a criptografia por configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="4ed54-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="4ed54-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4ed54-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="4ed54-252">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-252">Boolean</span></span>|<span data-ttu-id="4ed54-253">Se for definido como true, o usuário poderá selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="4ed54-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="4ed54-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="4ed54-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="4ed54-255">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-255">Boolean</span></span>|<span data-ttu-id="4ed54-256">Se definido como true, o usuário poderá selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="4ed54-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="4ed54-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="4ed54-257">requireSsl</span></span>|<span data-ttu-id="4ed54-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-258">Boolean</span></span>|<span data-ttu-id="4ed54-259">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="4ed54-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="4ed54-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="4ed54-260">useOAuth</span></span>|<span data-ttu-id="4ed54-261">Booleano</span><span class="sxs-lookup"><span data-stu-id="4ed54-261">Boolean</span></span>|<span data-ttu-id="4ed54-262">Especifica se a conexão deve usar OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="4ed54-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="4ed54-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="4ed54-263">signingCertificateType</span></span>|[<span data-ttu-id="4ed54-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="4ed54-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="4ed54-265">Tipo de certificado de assinatura para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="4ed54-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="4ed54-266">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="4ed54-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4ed54-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="4ed54-267">encryptionCertificateType</span></span>|[<span data-ttu-id="4ed54-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="4ed54-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="4ed54-269">Tipo de certificado de criptografia para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="4ed54-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="4ed54-270">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="4ed54-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4ed54-271">perAppVPNProfileId</span><span class="sxs-lookup"><span data-stu-id="4ed54-271">perAppVPNProfileId</span></span>|<span data-ttu-id="4ed54-272">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed54-272">String</span></span>|<span data-ttu-id="4ed54-273">ID de perfil da política Per-App VPN a ser usada para acessar emails do cliente de Email nativo</span><span class="sxs-lookup"><span data-stu-id="4ed54-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="4ed54-274">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ed54-274">Response</span></span>
<span data-ttu-id="4ed54-275">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ed54-275">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed54-276">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ed54-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ed54-277">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ed54-277">Request</span></span>
<span data-ttu-id="4ed54-278">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ed54-278">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4ed54-279">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ed54-279">Response</span></span>
<span data-ttu-id="4ed54-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ed54-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




