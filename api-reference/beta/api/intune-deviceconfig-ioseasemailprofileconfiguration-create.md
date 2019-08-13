---
title: Criar iosEasEmailProfileConfiguration
description: Criar um novo objeto iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a09aa3f2680599869b1762c7d8712e40f7f9ae31
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339411"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="7edd7-103">Criar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="7edd7-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="7edd7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7edd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7edd7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7edd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7edd7-106">Criar um novo objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7edd7-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7edd7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7edd7-107">Prerequisites</span></span>
<span data-ttu-id="7edd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7edd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7edd7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7edd7-110">Permission type</span></span>|<span data-ttu-id="7edd7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7edd7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7edd7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7edd7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7edd7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7edd7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7edd7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7edd7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7edd7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7edd7-115">Not supported.</span></span>|
|<span data-ttu-id="7edd7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7edd7-116">Application</span></span>|<span data-ttu-id="7edd7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7edd7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7edd7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7edd7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7edd7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7edd7-119">Request headers</span></span>
|<span data-ttu-id="7edd7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7edd7-120">Header</span></span>|<span data-ttu-id="7edd7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7edd7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7edd7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7edd7-122">Authorization</span></span>|<span data-ttu-id="7edd7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7edd7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7edd7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7edd7-124">Accept</span></span>|<span data-ttu-id="7edd7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7edd7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7edd7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7edd7-126">Request body</span></span>
<span data-ttu-id="7edd7-127">No corpo da solicitação, forneça uma representação JSON do objeto iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7edd7-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="7edd7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7edd7-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="7edd7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7edd7-129">Property</span></span>|<span data-ttu-id="7edd7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7edd7-130">Type</span></span>|<span data-ttu-id="7edd7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7edd7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7edd7-132">id</span><span class="sxs-lookup"><span data-stu-id="7edd7-132">id</span></span>|<span data-ttu-id="7edd7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7edd7-133">String</span></span>|<span data-ttu-id="7edd7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7edd7-134">Key of the entity.</span></span> <span data-ttu-id="7edd7-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7edd7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7edd7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7edd7-137">DateTimeOffset</span></span>|<span data-ttu-id="7edd7-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7edd7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7edd7-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7edd7-140">roleScopeTagIds</span></span>|<span data-ttu-id="7edd7-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7edd7-141">String collection</span></span>|<span data-ttu-id="7edd7-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7edd7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7edd7-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7edd7-144">supportsScopeTags</span></span>|<span data-ttu-id="7edd7-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-145">Boolean</span></span>|<span data-ttu-id="7edd7-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7edd7-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7edd7-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7edd7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7edd7-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7edd7-149">This property is read-only.</span></span> <span data-ttu-id="7edd7-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7edd7-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7edd7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7edd7-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7edd7-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="7edd7-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7edd7-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7edd7-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7edd7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7edd7-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7edd7-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="7edd7-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7edd7-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7edd7-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7edd7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7edd7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7edd7-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="7edd7-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7edd7-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7edd7-163">createdDateTime</span></span>|<span data-ttu-id="7edd7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7edd7-164">DateTimeOffset</span></span>|<span data-ttu-id="7edd7-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7edd7-165">DateTime the object was created.</span></span> <span data-ttu-id="7edd7-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-167">descrição</span><span class="sxs-lookup"><span data-stu-id="7edd7-167">description</span></span>|<span data-ttu-id="7edd7-168">String</span><span class="sxs-lookup"><span data-stu-id="7edd7-168">String</span></span>|<span data-ttu-id="7edd7-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7edd7-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7edd7-171">displayName</span></span>|<span data-ttu-id="7edd7-172">String</span><span class="sxs-lookup"><span data-stu-id="7edd7-172">String</span></span>|<span data-ttu-id="7edd7-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7edd7-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-175">versão</span><span class="sxs-lookup"><span data-stu-id="7edd7-175">version</span></span>|<span data-ttu-id="7edd7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7edd7-176">Int32</span></span>|<span data-ttu-id="7edd7-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-177">Version of the device configuration.</span></span> <span data-ttu-id="7edd7-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7edd7-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7edd7-179">usernameSource</span></span>|[<span data-ttu-id="7edd7-180">UserEmail</span><span class="sxs-lookup"><span data-stu-id="7edd7-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7edd7-181">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7edd7-182">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7edd7-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7edd7-183">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7edd7-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7edd7-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="7edd7-184">usernameAADSource</span></span>|[<span data-ttu-id="7edd7-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7edd7-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="7edd7-186">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="7edd7-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="7edd7-187">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7edd7-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7edd7-188">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="7edd7-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="7edd7-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="7edd7-189">userDomainNameSource</span></span>|[<span data-ttu-id="7edd7-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="7edd7-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="7edd7-191">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7edd7-192">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7edd7-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7edd7-193">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="7edd7-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="7edd7-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="7edd7-194">customDomainName</span></span>|<span data-ttu-id="7edd7-195">String</span><span class="sxs-lookup"><span data-stu-id="7edd7-195">String</span></span>|<span data-ttu-id="7edd7-196">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="7edd7-197">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="7edd7-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="7edd7-198">accountName</span><span class="sxs-lookup"><span data-stu-id="7edd7-198">accountName</span></span>|<span data-ttu-id="7edd7-199">String</span><span class="sxs-lookup"><span data-stu-id="7edd7-199">String</span></span>|<span data-ttu-id="7edd7-200">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="7edd7-200">Account name.</span></span>|
|<span data-ttu-id="7edd7-201">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7edd7-201">authenticationMethod</span></span>|[<span data-ttu-id="7edd7-202">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7edd7-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="7edd7-203">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="7edd7-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="7edd7-204">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7edd7-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7edd7-205">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="7edd7-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="7edd7-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-206">Boolean</span></span>|<span data-ttu-id="7edd7-207">Indica se as mensagens de movimentação devem ou não ser bloqueadas para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="7edd7-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="7edd7-208">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="7edd7-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="7edd7-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-209">Boolean</span></span>|<span data-ttu-id="7edd7-210">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7edd7-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="7edd7-211">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="7edd7-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="7edd7-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-212">Boolean</span></span>|<span data-ttu-id="7edd7-213">Indica se a sincronização de endereços de email usados recentemente deve ou não ser bloqueada, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="7edd7-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="7edd7-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7edd7-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="7edd7-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7edd7-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7edd7-216">Duração de tempo que o email deve ser sincronizado de volta para o.</span><span class="sxs-lookup"><span data-stu-id="7edd7-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="7edd7-217">.</span><span class="sxs-lookup"><span data-stu-id="7edd7-217"></span></span> <span data-ttu-id="7edd7-218">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="7edd7-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7edd7-219">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="7edd7-219">emailAddressSource</span></span>|[<span data-ttu-id="7edd7-220">UserEmail</span><span class="sxs-lookup"><span data-stu-id="7edd7-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7edd7-221">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7edd7-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7edd7-222">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7edd7-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7edd7-223">hostName</span><span class="sxs-lookup"><span data-stu-id="7edd7-223">hostName</span></span>|<span data-ttu-id="7edd7-224">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7edd7-224">String</span></span>|<span data-ttu-id="7edd7-225">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="7edd7-225">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="7edd7-226">requireSmime</span><span class="sxs-lookup"><span data-stu-id="7edd7-226">requireSmime</span></span>|<span data-ttu-id="7edd7-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-227">Boolean</span></span>|<span data-ttu-id="7edd7-228">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="7edd7-228">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="7edd7-229">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="7edd7-229">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="7edd7-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-230">Boolean</span></span>|<span data-ttu-id="7edd7-231">Indica se os emails não criptografados devem ou não ser permitidos.</span><span class="sxs-lookup"><span data-stu-id="7edd7-231">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="7edd7-232">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="7edd7-232">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="7edd7-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-233">Boolean</span></span>|<span data-ttu-id="7edd7-234">Se definido como true a criptografia S/MIME estiver habilitada por padrão.</span><span class="sxs-lookup"><span data-stu-id="7edd7-234">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="7edd7-235">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="7edd7-235">smimeSigningEnabled</span></span>|<span data-ttu-id="7edd7-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-236">Boolean</span></span>|<span data-ttu-id="7edd7-237">Se definido como true a assinatura S/MIME estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="7edd7-237">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="7edd7-238">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="7edd7-238">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="7edd7-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-239">Boolean</span></span>|<span data-ttu-id="7edd7-240">Se definido como true, o usuário pode ativar ou desativar a assinatura S/MIME.</span><span class="sxs-lookup"><span data-stu-id="7edd7-240">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="7edd7-241">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="7edd7-241">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="7edd7-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-242">Boolean</span></span>|<span data-ttu-id="7edd7-243">Se definido como true, o usuário pode ativar a opção criptografia por padrão.</span><span class="sxs-lookup"><span data-stu-id="7edd7-243">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="7edd7-244">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="7edd7-244">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="7edd7-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-245">Boolean</span></span>|<span data-ttu-id="7edd7-246">Se definido como true, o usuário pode selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="7edd7-246">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="7edd7-247">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="7edd7-247">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="7edd7-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-248">Boolean</span></span>|<span data-ttu-id="7edd7-249">Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="7edd7-249">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="7edd7-250">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7edd7-250">requireSsl</span></span>|<span data-ttu-id="7edd7-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-251">Boolean</span></span>|<span data-ttu-id="7edd7-252">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="7edd7-252">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="7edd7-253">useOAuth</span><span class="sxs-lookup"><span data-stu-id="7edd7-253">useOAuth</span></span>|<span data-ttu-id="7edd7-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="7edd7-254">Boolean</span></span>|<span data-ttu-id="7edd7-255">Especifica se a conexão deve usar o OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="7edd7-255">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="7edd7-256">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="7edd7-256">signingCertificateType</span></span>|[<span data-ttu-id="7edd7-257">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="7edd7-257">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="7edd7-258">Assinatura tipo de certificado para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="7edd7-258">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="7edd7-259">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7edd7-259">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7edd7-260">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="7edd7-260">encryptionCertificateType</span></span>|[<span data-ttu-id="7edd7-261">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="7edd7-261">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="7edd7-262">Tipo de certificado de criptografia para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="7edd7-262">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="7edd7-263">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7edd7-263">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="7edd7-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="7edd7-264">Response</span></span>
<span data-ttu-id="7edd7-265">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7edd7-265">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7edd7-266">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7edd7-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="7edd7-267">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7edd7-267">Request</span></span>
<span data-ttu-id="7edd7-268">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7edd7-268">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2057

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

### <a name="response"></a><span data-ttu-id="7edd7-269">Resposta</span><span class="sxs-lookup"><span data-stu-id="7edd7-269">Response</span></span>
<span data-ttu-id="7edd7-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7edd7-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2229

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






