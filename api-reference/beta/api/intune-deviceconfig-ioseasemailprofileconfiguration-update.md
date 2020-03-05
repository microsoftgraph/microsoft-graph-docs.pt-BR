---
title: Atualizar iosEasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab410bc3fc5df4bd595287e35c633458617eab30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448967"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="d3de7-103">Atualizar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3de7-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="d3de7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3de7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3de7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3de7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3de7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3de7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3de7-107">Atualiza as propriedades de um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d3de7-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3de7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3de7-108">Prerequisites</span></span>
<span data-ttu-id="d3de7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3de7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3de7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3de7-111">Permission type</span></span>|<span data-ttu-id="d3de7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3de7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3de7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3de7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3de7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3de7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3de7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3de7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3de7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3de7-116">Not supported.</span></span>|
|<span data-ttu-id="d3de7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3de7-117">Application</span></span>|<span data-ttu-id="d3de7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3de7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3de7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3de7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d3de7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3de7-120">Request headers</span></span>
|<span data-ttu-id="d3de7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3de7-121">Header</span></span>|<span data-ttu-id="d3de7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3de7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3de7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3de7-123">Authorization</span></span>|<span data-ttu-id="d3de7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3de7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3de7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3de7-125">Accept</span></span>|<span data-ttu-id="d3de7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3de7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3de7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3de7-127">Request body</span></span>
<span data-ttu-id="d3de7-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d3de7-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="d3de7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3de7-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="d3de7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3de7-130">Property</span></span>|<span data-ttu-id="d3de7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3de7-131">Type</span></span>|<span data-ttu-id="d3de7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3de7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3de7-133">id</span><span class="sxs-lookup"><span data-stu-id="d3de7-133">id</span></span>|<span data-ttu-id="d3de7-134">String</span><span class="sxs-lookup"><span data-stu-id="d3de7-134">String</span></span>|<span data-ttu-id="d3de7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d3de7-135">Key of the entity.</span></span> <span data-ttu-id="d3de7-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3de7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d3de7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3de7-138">DateTimeOffset</span></span>|<span data-ttu-id="d3de7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d3de7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d3de7-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d3de7-141">roleScopeTagIds</span></span>|<span data-ttu-id="d3de7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="d3de7-142">String collection</span></span>|<span data-ttu-id="d3de7-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d3de7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d3de7-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d3de7-145">supportsScopeTags</span></span>|<span data-ttu-id="d3de7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-146">Boolean</span></span>|<span data-ttu-id="d3de7-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d3de7-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d3de7-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d3de7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d3de7-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3de7-150">This property is read-only.</span></span> <span data-ttu-id="d3de7-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d3de7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d3de7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d3de7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d3de7-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d3de7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d3de7-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d3de7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d3de7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d3de7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d3de7-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d3de7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d3de7-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d3de7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d3de7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d3de7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d3de7-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d3de7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d3de7-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3de7-164">createdDateTime</span></span>|<span data-ttu-id="d3de7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3de7-165">DateTimeOffset</span></span>|<span data-ttu-id="d3de7-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d3de7-166">DateTime the object was created.</span></span> <span data-ttu-id="d3de7-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-168">description</span><span class="sxs-lookup"><span data-stu-id="d3de7-168">description</span></span>|<span data-ttu-id="d3de7-169">String</span><span class="sxs-lookup"><span data-stu-id="d3de7-169">String</span></span>|<span data-ttu-id="d3de7-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d3de7-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d3de7-172">displayName</span></span>|<span data-ttu-id="d3de7-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3de7-173">String</span></span>|<span data-ttu-id="d3de7-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d3de7-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-176">versão</span><span class="sxs-lookup"><span data-stu-id="d3de7-176">version</span></span>|<span data-ttu-id="d3de7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d3de7-177">Int32</span></span>|<span data-ttu-id="d3de7-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-178">Version of the device configuration.</span></span> <span data-ttu-id="d3de7-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3de7-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d3de7-180">usernameSource</span></span>|[<span data-ttu-id="d3de7-181">UserEmail</span><span class="sxs-lookup"><span data-stu-id="d3de7-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d3de7-182">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d3de7-183">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d3de7-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d3de7-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d3de7-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d3de7-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="d3de7-185">usernameAADSource</span></span>|[<span data-ttu-id="d3de7-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d3de7-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="d3de7-187">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="d3de7-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="d3de7-188">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d3de7-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d3de7-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="d3de7-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="d3de7-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="d3de7-190">userDomainNameSource</span></span>|[<span data-ttu-id="d3de7-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="d3de7-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="d3de7-192">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d3de7-193">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d3de7-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d3de7-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="d3de7-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="d3de7-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="d3de7-195">customDomainName</span></span>|<span data-ttu-id="d3de7-196">String</span><span class="sxs-lookup"><span data-stu-id="d3de7-196">String</span></span>|<span data-ttu-id="d3de7-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="d3de7-198">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="d3de7-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="d3de7-199">accountName</span><span class="sxs-lookup"><span data-stu-id="d3de7-199">accountName</span></span>|<span data-ttu-id="d3de7-200">String</span><span class="sxs-lookup"><span data-stu-id="d3de7-200">String</span></span>|<span data-ttu-id="d3de7-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="d3de7-201">Account name.</span></span>|
|<span data-ttu-id="d3de7-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d3de7-202">authenticationMethod</span></span>|[<span data-ttu-id="d3de7-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d3de7-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="d3de7-204">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="d3de7-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="d3de7-205">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d3de7-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d3de7-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="d3de7-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="d3de7-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-207">Boolean</span></span>|<span data-ttu-id="d3de7-208">Indica se as mensagens de movimentação devem ou não ser bloqueadas para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="d3de7-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="d3de7-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="d3de7-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="d3de7-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-210">Boolean</span></span>|<span data-ttu-id="d3de7-211">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d3de7-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="d3de7-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="d3de7-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="d3de7-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-213">Boolean</span></span>|<span data-ttu-id="d3de7-214">Indica se a sincronização de endereços de email usados recentemente deve ou não ser bloqueada, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="d3de7-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="d3de7-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d3de7-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="d3de7-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d3de7-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d3de7-217">Duração de tempo que o email deve ser sincronizado de volta para o.</span><span class="sxs-lookup"><span data-stu-id="d3de7-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="d3de7-218">.</span><span class="sxs-lookup"><span data-stu-id="d3de7-218">.</span></span> <span data-ttu-id="d3de7-219">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="d3de7-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d3de7-220">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="d3de7-220">emailAddressSource</span></span>|[<span data-ttu-id="d3de7-221">UserEmail</span><span class="sxs-lookup"><span data-stu-id="d3de7-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d3de7-222">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3de7-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d3de7-223">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d3de7-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d3de7-224">easServices</span><span class="sxs-lookup"><span data-stu-id="d3de7-224">easServices</span></span>|[<span data-ttu-id="d3de7-225">easServices</span><span class="sxs-lookup"><span data-stu-id="d3de7-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="d3de7-226">Trocar dados a serem sincronizados. Os valores possíveis são `none`: `calendars`, `contacts`, `email`, `notes`, `reminders`,.</span><span class="sxs-lookup"><span data-stu-id="d3de7-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="d3de7-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="d3de7-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="d3de7-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-228">Boolean</span></span>|<span data-ttu-id="d3de7-229">Permitir que os usuários alterem as configurações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="d3de7-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="d3de7-230">hostName</span><span class="sxs-lookup"><span data-stu-id="d3de7-230">hostName</span></span>|<span data-ttu-id="d3de7-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3de7-231">String</span></span>|<span data-ttu-id="d3de7-232">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="d3de7-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="d3de7-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="d3de7-233">requireSmime</span></span>|<span data-ttu-id="d3de7-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-234">Boolean</span></span>|<span data-ttu-id="d3de7-235">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="d3de7-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="d3de7-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="d3de7-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="d3de7-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-237">Boolean</span></span>|<span data-ttu-id="d3de7-238">Indica se os emails não criptografados devem ou não ser permitidos.</span><span class="sxs-lookup"><span data-stu-id="d3de7-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="d3de7-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="d3de7-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="d3de7-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-240">Boolean</span></span>|<span data-ttu-id="d3de7-241">Se definido como true a criptografia S/MIME estiver habilitada por padrão.</span><span class="sxs-lookup"><span data-stu-id="d3de7-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="d3de7-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="d3de7-242">smimeSigningEnabled</span></span>|<span data-ttu-id="d3de7-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-243">Boolean</span></span>|<span data-ttu-id="d3de7-244">Se definido como true a assinatura S/MIME estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="d3de7-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="d3de7-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="d3de7-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="d3de7-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-246">Boolean</span></span>|<span data-ttu-id="d3de7-247">Se definido como true, o usuário pode ativar ou desativar a assinatura S/MIME.</span><span class="sxs-lookup"><span data-stu-id="d3de7-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="d3de7-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="d3de7-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="d3de7-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-249">Boolean</span></span>|<span data-ttu-id="d3de7-250">Se definido como true, o usuário pode ativar a opção criptografia por padrão.</span><span class="sxs-lookup"><span data-stu-id="d3de7-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="d3de7-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="d3de7-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="d3de7-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-252">Boolean</span></span>|<span data-ttu-id="d3de7-253">Se definido como true, o usuário pode selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="d3de7-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="d3de7-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="d3de7-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="d3de7-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-255">Boolean</span></span>|<span data-ttu-id="d3de7-256">Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="d3de7-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="d3de7-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d3de7-257">requireSsl</span></span>|<span data-ttu-id="d3de7-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-258">Boolean</span></span>|<span data-ttu-id="d3de7-259">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="d3de7-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="d3de7-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="d3de7-260">useOAuth</span></span>|<span data-ttu-id="d3de7-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3de7-261">Boolean</span></span>|<span data-ttu-id="d3de7-262">Especifica se a conexão deve usar o OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="d3de7-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="d3de7-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="d3de7-263">signingCertificateType</span></span>|[<span data-ttu-id="d3de7-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="d3de7-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="d3de7-265">Assinatura tipo de certificado para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="d3de7-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="d3de7-266">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d3de7-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d3de7-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="d3de7-267">encryptionCertificateType</span></span>|[<span data-ttu-id="d3de7-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="d3de7-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="d3de7-269">Tipo de certificado de criptografia para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="d3de7-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="d3de7-270">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d3de7-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="d3de7-271">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3de7-271">Response</span></span>
<span data-ttu-id="d3de7-272">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3de7-272">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3de7-273">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3de7-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3de7-274">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3de7-274">Request</span></span>
<span data-ttu-id="d3de7-275">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3de7-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="d3de7-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3de7-276">Response</span></span>
<span data-ttu-id="d3de7-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3de7-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





