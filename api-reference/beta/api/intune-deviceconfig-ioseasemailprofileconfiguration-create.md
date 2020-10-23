---
title: Criar iosEasEmailProfileConfiguration
description: Criar um novo objeto iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b3bceef2f2e9c264cdc02dd5b9363c39306a3d2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735698"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="a1860-103">Criar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1860-103">Create iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="a1860-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1860-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1860-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1860-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1860-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1860-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1860-107">Criar um novo objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a1860-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1860-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1860-108">Prerequisites</span></span>
<span data-ttu-id="a1860-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1860-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1860-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1860-111">Permission type</span></span>|<span data-ttu-id="a1860-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1860-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1860-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1860-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1860-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1860-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1860-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1860-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1860-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1860-116">Not supported.</span></span>|
|<span data-ttu-id="a1860-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1860-117">Application</span></span>|<span data-ttu-id="a1860-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1860-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1860-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1860-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a1860-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1860-120">Request headers</span></span>
|<span data-ttu-id="a1860-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1860-121">Header</span></span>|<span data-ttu-id="a1860-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a1860-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1860-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1860-123">Authorization</span></span>|<span data-ttu-id="a1860-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1860-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1860-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1860-125">Accept</span></span>|<span data-ttu-id="a1860-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1860-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1860-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1860-127">Request body</span></span>
<span data-ttu-id="a1860-128">No corpo da solicitação, forneça uma representação JSON do objeto iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a1860-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="a1860-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a1860-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="a1860-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1860-130">Property</span></span>|<span data-ttu-id="a1860-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1860-131">Type</span></span>|<span data-ttu-id="a1860-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1860-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1860-133">id</span><span class="sxs-lookup"><span data-stu-id="a1860-133">id</span></span>|<span data-ttu-id="a1860-134">String</span><span class="sxs-lookup"><span data-stu-id="a1860-134">String</span></span>|<span data-ttu-id="a1860-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1860-135">Key of the entity.</span></span> <span data-ttu-id="a1860-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1860-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a1860-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1860-138">DateTimeOffset</span></span>|<span data-ttu-id="a1860-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a1860-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a1860-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1860-141">roleScopeTagIds</span></span>|<span data-ttu-id="a1860-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1860-142">String collection</span></span>|<span data-ttu-id="a1860-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a1860-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a1860-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a1860-145">supportsScopeTags</span></span>|<span data-ttu-id="a1860-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-146">Boolean</span></span>|<span data-ttu-id="a1860-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a1860-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a1860-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a1860-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a1860-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a1860-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a1860-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1860-150">This property is read-only.</span></span> <span data-ttu-id="a1860-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1860-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a1860-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1860-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a1860-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a1860-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a1860-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1860-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a1860-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1860-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a1860-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a1860-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a1860-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1860-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a1860-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1860-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a1860-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a1860-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a1860-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1860-164">createdDateTime</span></span>|<span data-ttu-id="a1860-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1860-165">DateTimeOffset</span></span>|<span data-ttu-id="a1860-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a1860-166">DateTime the object was created.</span></span> <span data-ttu-id="a1860-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-168">description</span><span class="sxs-lookup"><span data-stu-id="a1860-168">description</span></span>|<span data-ttu-id="a1860-169">String</span><span class="sxs-lookup"><span data-stu-id="a1860-169">String</span></span>|<span data-ttu-id="a1860-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1860-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1860-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a1860-172">displayName</span></span>|<span data-ttu-id="a1860-173">String</span><span class="sxs-lookup"><span data-stu-id="a1860-173">String</span></span>|<span data-ttu-id="a1860-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1860-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1860-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-176">versão</span><span class="sxs-lookup"><span data-stu-id="a1860-176">version</span></span>|<span data-ttu-id="a1860-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a1860-177">Int32</span></span>|<span data-ttu-id="a1860-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1860-178">Version of the device configuration.</span></span> <span data-ttu-id="a1860-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1860-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a1860-180">usernameSource</span></span>|[<span data-ttu-id="a1860-181">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a1860-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a1860-182">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1860-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a1860-183">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a1860-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a1860-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a1860-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a1860-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="a1860-185">usernameAADSource</span></span>|[<span data-ttu-id="a1860-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a1860-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="a1860-187">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="a1860-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="a1860-188">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a1860-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a1860-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="a1860-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="a1860-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="a1860-190">userDomainNameSource</span></span>|[<span data-ttu-id="a1860-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="a1860-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="a1860-192">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1860-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a1860-193">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a1860-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a1860-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="a1860-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="a1860-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="a1860-195">customDomainName</span></span>|<span data-ttu-id="a1860-196">String</span><span class="sxs-lookup"><span data-stu-id="a1860-196">String</span></span>|<span data-ttu-id="a1860-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1860-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="a1860-198">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="a1860-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="a1860-199">accountName</span><span class="sxs-lookup"><span data-stu-id="a1860-199">accountName</span></span>|<span data-ttu-id="a1860-200">String</span><span class="sxs-lookup"><span data-stu-id="a1860-200">String</span></span>|<span data-ttu-id="a1860-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="a1860-201">Account name.</span></span>|
|<span data-ttu-id="a1860-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a1860-202">authenticationMethod</span></span>|[<span data-ttu-id="a1860-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a1860-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a1860-204">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="a1860-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="a1860-205">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a1860-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a1860-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="a1860-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="a1860-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-207">Boolean</span></span>|<span data-ttu-id="a1860-208">Indica se as mensagens de movimentação devem ou não ser bloqueadas para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="a1860-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="a1860-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="a1860-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="a1860-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-210">Boolean</span></span>|<span data-ttu-id="a1860-211">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="a1860-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="a1860-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a1860-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="a1860-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-213">Boolean</span></span>|<span data-ttu-id="a1860-214">Indica se a sincronização de endereços de email usados recentemente deve ou não ser bloqueada, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="a1860-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="a1860-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a1860-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="a1860-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a1860-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a1860-217">Duração de tempo que o email deve ser sincronizado de volta para o.</span><span class="sxs-lookup"><span data-stu-id="a1860-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="a1860-218">.</span><span class="sxs-lookup"><span data-stu-id="a1860-218">.</span></span> <span data-ttu-id="a1860-219">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="a1860-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a1860-220">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="a1860-220">emailAddressSource</span></span>|[<span data-ttu-id="a1860-221">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a1860-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a1860-222">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1860-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a1860-223">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a1860-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a1860-224">easServices</span><span class="sxs-lookup"><span data-stu-id="a1860-224">easServices</span></span>|[<span data-ttu-id="a1860-225">easServices</span><span class="sxs-lookup"><span data-stu-id="a1860-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="a1860-226">Trocar dados a serem sincronizados. Os valores possíveis são: `none` , `calendars` , `contacts` , `email` , `notes` , `reminders` .</span><span class="sxs-lookup"><span data-stu-id="a1860-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="a1860-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a1860-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="a1860-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-228">Boolean</span></span>|<span data-ttu-id="a1860-229">Permitir que os usuários alterem as configurações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="a1860-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="a1860-230">hostName</span><span class="sxs-lookup"><span data-stu-id="a1860-230">hostName</span></span>|<span data-ttu-id="a1860-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1860-231">String</span></span>|<span data-ttu-id="a1860-232">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="a1860-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="a1860-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="a1860-233">requireSmime</span></span>|<span data-ttu-id="a1860-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-234">Boolean</span></span>|<span data-ttu-id="a1860-235">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="a1860-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="a1860-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="a1860-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="a1860-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-237">Boolean</span></span>|<span data-ttu-id="a1860-238">Indica se os emails não criptografados devem ou não ser permitidos.</span><span class="sxs-lookup"><span data-stu-id="a1860-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="a1860-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="a1860-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="a1860-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-240">Boolean</span></span>|<span data-ttu-id="a1860-241">Se definido como true a criptografia S/MIME estiver habilitada por padrão.</span><span class="sxs-lookup"><span data-stu-id="a1860-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="a1860-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="a1860-242">smimeSigningEnabled</span></span>|<span data-ttu-id="a1860-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-243">Boolean</span></span>|<span data-ttu-id="a1860-244">Se definido como true a assinatura S/MIME estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="a1860-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="a1860-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a1860-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="a1860-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-246">Boolean</span></span>|<span data-ttu-id="a1860-247">Se definido como true, o usuário pode ativar ou desativar a assinatura S/MIME.</span><span class="sxs-lookup"><span data-stu-id="a1860-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="a1860-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a1860-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="a1860-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-249">Boolean</span></span>|<span data-ttu-id="a1860-250">Se definido como true, o usuário pode ativar a opção criptografia por padrão.</span><span class="sxs-lookup"><span data-stu-id="a1860-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="a1860-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a1860-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="a1860-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-252">Boolean</span></span>|<span data-ttu-id="a1860-253">Se definido como true, o usuário pode selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="a1860-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="a1860-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a1860-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="a1860-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-255">Boolean</span></span>|<span data-ttu-id="a1860-256">Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="a1860-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="a1860-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a1860-257">requireSsl</span></span>|<span data-ttu-id="a1860-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-258">Boolean</span></span>|<span data-ttu-id="a1860-259">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="a1860-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="a1860-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="a1860-260">useOAuth</span></span>|<span data-ttu-id="a1860-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1860-261">Boolean</span></span>|<span data-ttu-id="a1860-262">Especifica se a conexão deve usar o OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="a1860-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="a1860-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="a1860-263">signingCertificateType</span></span>|[<span data-ttu-id="a1860-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="a1860-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="a1860-265">Assinatura tipo de certificado para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="a1860-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="a1860-266">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a1860-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a1860-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="a1860-267">encryptionCertificateType</span></span>|[<span data-ttu-id="a1860-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="a1860-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="a1860-269">Tipo de certificado de criptografia para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="a1860-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="a1860-270">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a1860-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a1860-271">perAppVPNProfileId</span><span class="sxs-lookup"><span data-stu-id="a1860-271">perAppVPNProfileId</span></span>|<span data-ttu-id="a1860-272">String</span><span class="sxs-lookup"><span data-stu-id="a1860-272">String</span></span>|<span data-ttu-id="a1860-273">ID de perfil da política de VPN Per-App a ser usada para acessar emails a partir do cliente de email nativo</span><span class="sxs-lookup"><span data-stu-id="a1860-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="a1860-274">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1860-274">Response</span></span>
<span data-ttu-id="a1860-275">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1860-275">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1860-276">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1860-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1860-277">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1860-277">Request</span></span>
<span data-ttu-id="a1860-278">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1860-278">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1860-279">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1860-279">Response</span></span>
<span data-ttu-id="a1860-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1860-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





