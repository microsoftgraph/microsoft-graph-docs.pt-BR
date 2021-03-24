---
title: Atualizar iosEasEmailProfileConfiguration
description: Atualize as propriedades de um objeto iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a965fa5e70c2182c54a9c67ba4aa9144e56ea4e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129990"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="0ae02-103">Atualizar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ae02-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="0ae02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ae02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ae02-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ae02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ae02-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ae02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ae02-107">Atualize as propriedades de [um objeto iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ae02-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ae02-108">Prerequisites</span></span>
<span data-ttu-id="0ae02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ae02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ae02-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ae02-111">Permission type</span></span>|<span data-ttu-id="0ae02-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ae02-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ae02-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ae02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ae02-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ae02-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ae02-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ae02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ae02-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ae02-116">Not supported.</span></span>|
|<span data-ttu-id="0ae02-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ae02-117">Application</span></span>|<span data-ttu-id="0ae02-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ae02-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ae02-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ae02-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0ae02-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae02-120">Request headers</span></span>
|<span data-ttu-id="0ae02-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ae02-121">Header</span></span>|<span data-ttu-id="0ae02-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0ae02-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ae02-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ae02-123">Authorization</span></span>|<span data-ttu-id="0ae02-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ae02-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ae02-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ae02-125">Accept</span></span>|<span data-ttu-id="0ae02-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ae02-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ae02-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae02-127">Request body</span></span>
<span data-ttu-id="0ae02-128">No corpo da solicitação, fornece uma representação JSON para o [objeto iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="0ae02-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ae02-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="0ae02-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ae02-130">Property</span></span>|<span data-ttu-id="0ae02-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ae02-131">Type</span></span>|<span data-ttu-id="0ae02-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ae02-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ae02-133">id</span><span class="sxs-lookup"><span data-stu-id="0ae02-133">id</span></span>|<span data-ttu-id="0ae02-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae02-134">String</span></span>|<span data-ttu-id="0ae02-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ae02-135">Key of the entity.</span></span> <span data-ttu-id="0ae02-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ae02-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0ae02-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ae02-138">DateTimeOffset</span></span>|<span data-ttu-id="0ae02-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0ae02-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0ae02-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ae02-141">roleScopeTagIds</span></span>|<span data-ttu-id="0ae02-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae02-142">String collection</span></span>|<span data-ttu-id="0ae02-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="0ae02-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ae02-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ae02-145">supportsScopeTags</span></span>|<span data-ttu-id="0ae02-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-146">Boolean</span></span>|<span data-ttu-id="0ae02-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ae02-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ae02-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ae02-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ae02-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ae02-150">This property is read-only.</span></span> <span data-ttu-id="0ae02-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ae02-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0ae02-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ae02-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0ae02-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0ae02-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0ae02-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ae02-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0ae02-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ae02-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0ae02-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0ae02-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0ae02-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ae02-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0ae02-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ae02-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0ae02-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0ae02-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0ae02-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ae02-164">createdDateTime</span></span>|<span data-ttu-id="0ae02-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ae02-165">DateTimeOffset</span></span>|<span data-ttu-id="0ae02-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0ae02-166">DateTime the object was created.</span></span> <span data-ttu-id="0ae02-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-168">descrição</span><span class="sxs-lookup"><span data-stu-id="0ae02-168">description</span></span>|<span data-ttu-id="0ae02-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae02-169">String</span></span>|<span data-ttu-id="0ae02-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ae02-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0ae02-172">displayName</span></span>|<span data-ttu-id="0ae02-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae02-173">String</span></span>|<span data-ttu-id="0ae02-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ae02-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-176">versão</span><span class="sxs-lookup"><span data-stu-id="0ae02-176">version</span></span>|<span data-ttu-id="0ae02-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae02-177">Int32</span></span>|<span data-ttu-id="0ae02-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-178">Version of the device configuration.</span></span> <span data-ttu-id="0ae02-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ae02-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0ae02-180">usernameSource</span></span>|[<span data-ttu-id="0ae02-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="0ae02-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0ae02-182">Atributo username que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0ae02-183">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="0ae02-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0ae02-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0ae02-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0ae02-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="0ae02-185">usernameAADSource</span></span>|[<span data-ttu-id="0ae02-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0ae02-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="0ae02-187">Nome do campo AAD, que será usado para recuperar UserName para perfil de email.</span><span class="sxs-lookup"><span data-stu-id="0ae02-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="0ae02-188">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="0ae02-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0ae02-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="0ae02-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="0ae02-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="0ae02-190">userDomainNameSource</span></span>|[<span data-ttu-id="0ae02-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="0ae02-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="0ae02-192">Atributo UserDomainname que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0ae02-193">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="0ae02-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0ae02-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="0ae02-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="0ae02-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="0ae02-195">customDomainName</span></span>|<span data-ttu-id="0ae02-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae02-196">String</span></span>|<span data-ttu-id="0ae02-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="0ae02-198">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="0ae02-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="0ae02-199">accountName</span><span class="sxs-lookup"><span data-stu-id="0ae02-199">accountName</span></span>|<span data-ttu-id="0ae02-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae02-200">String</span></span>|<span data-ttu-id="0ae02-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="0ae02-201">Account name.</span></span>|
|<span data-ttu-id="0ae02-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ae02-202">authenticationMethod</span></span>|[<span data-ttu-id="0ae02-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0ae02-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0ae02-204">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="0ae02-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="0ae02-205">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0ae02-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0ae02-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="0ae02-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="0ae02-207">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-207">Boolean</span></span>|<span data-ttu-id="0ae02-208">Indica se deve ou não bloquear a movimentação de mensagens para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="0ae02-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="0ae02-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="0ae02-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="0ae02-210">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-210">Boolean</span></span>|<span data-ttu-id="0ae02-211">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0ae02-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="0ae02-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="0ae02-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="0ae02-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-213">Boolean</span></span>|<span data-ttu-id="0ae02-214">Indica se deve ou não bloquear a sincronização de endereços de email usados recentemente, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="0ae02-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="0ae02-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="0ae02-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="0ae02-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="0ae02-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0ae02-217">A duração do tempo em que o email deve ser sincronizado novamente.</span><span class="sxs-lookup"><span data-stu-id="0ae02-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="0ae02-218">.</span><span class="sxs-lookup"><span data-stu-id="0ae02-218">.</span></span> <span data-ttu-id="0ae02-219">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="0ae02-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0ae02-220">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="0ae02-220">emailAddressSource</span></span>|[<span data-ttu-id="0ae02-221">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="0ae02-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0ae02-222">Atributo de email que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ae02-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0ae02-223">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0ae02-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0ae02-224">easServices</span><span class="sxs-lookup"><span data-stu-id="0ae02-224">easServices</span></span>|[<span data-ttu-id="0ae02-225">easServices</span><span class="sxs-lookup"><span data-stu-id="0ae02-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="0ae02-226">Dados do Exchange para sincronização. Os valores possíveis `none` são: `calendars` , , , , , `contacts` `email` `notes` `reminders` .</span><span class="sxs-lookup"><span data-stu-id="0ae02-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="0ae02-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0ae02-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="0ae02-228">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-228">Boolean</span></span>|<span data-ttu-id="0ae02-229">Permitir que os usuários alterem as configurações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0ae02-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="0ae02-230">hostName</span><span class="sxs-lookup"><span data-stu-id="0ae02-230">hostName</span></span>|<span data-ttu-id="0ae02-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae02-231">String</span></span>|<span data-ttu-id="0ae02-232">Local do Exchange que (URL) ao que o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="0ae02-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="0ae02-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="0ae02-233">requireSmime</span></span>|<span data-ttu-id="0ae02-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-234">Boolean</span></span>|<span data-ttu-id="0ae02-235">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="0ae02-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="0ae02-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="0ae02-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="0ae02-237">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-237">Boolean</span></span>|<span data-ttu-id="0ae02-238">Indica se os emails não criptografados permitirão ou não.</span><span class="sxs-lookup"><span data-stu-id="0ae02-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="0ae02-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="0ae02-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="0ae02-240">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-240">Boolean</span></span>|<span data-ttu-id="0ae02-241">Se definido como criptografia S/MIME verdadeiro estiver habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="0ae02-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="0ae02-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="0ae02-242">smimeSigningEnabled</span></span>|<span data-ttu-id="0ae02-243">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-243">Boolean</span></span>|<span data-ttu-id="0ae02-244">Se definido como a assinatura S/MIME verdadeira estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="0ae02-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="0ae02-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0ae02-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="0ae02-246">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-246">Boolean</span></span>|<span data-ttu-id="0ae02-247">Se for definido como true, o usuário poderá alternar a sessão S/MIME para 1 ou 2016.</span><span class="sxs-lookup"><span data-stu-id="0ae02-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="0ae02-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0ae02-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="0ae02-249">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-249">Boolean</span></span>|<span data-ttu-id="0ae02-250">Se definido como true, o usuário pode alternar a criptografia por configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="0ae02-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="0ae02-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0ae02-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="0ae02-252">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-252">Boolean</span></span>|<span data-ttu-id="0ae02-253">Se for definido como true, o usuário poderá selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="0ae02-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="0ae02-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="0ae02-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="0ae02-255">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-255">Boolean</span></span>|<span data-ttu-id="0ae02-256">Se definido como true, o usuário poderá selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="0ae02-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="0ae02-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="0ae02-257">requireSsl</span></span>|<span data-ttu-id="0ae02-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-258">Boolean</span></span>|<span data-ttu-id="0ae02-259">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="0ae02-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="0ae02-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="0ae02-260">useOAuth</span></span>|<span data-ttu-id="0ae02-261">Booleano</span><span class="sxs-lookup"><span data-stu-id="0ae02-261">Boolean</span></span>|<span data-ttu-id="0ae02-262">Especifica se a conexão deve usar OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="0ae02-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="0ae02-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="0ae02-263">signingCertificateType</span></span>|[<span data-ttu-id="0ae02-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="0ae02-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="0ae02-265">Tipo de certificado de assinatura para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="0ae02-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="0ae02-266">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0ae02-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0ae02-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="0ae02-267">encryptionCertificateType</span></span>|[<span data-ttu-id="0ae02-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="0ae02-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="0ae02-269">Tipo de certificado de criptografia para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="0ae02-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="0ae02-270">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0ae02-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0ae02-271">perAppVPNProfileId</span><span class="sxs-lookup"><span data-stu-id="0ae02-271">perAppVPNProfileId</span></span>|<span data-ttu-id="0ae02-272">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ae02-272">String</span></span>|<span data-ttu-id="0ae02-273">ID de perfil da política Per-App VPN a ser usada para acessar emails do cliente de Email nativo</span><span class="sxs-lookup"><span data-stu-id="0ae02-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="0ae02-274">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ae02-274">Response</span></span>
<span data-ttu-id="0ae02-275">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ae02-275">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ae02-276">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ae02-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ae02-277">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae02-277">Request</span></span>
<span data-ttu-id="0ae02-278">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ae02-278">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ae02-279">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ae02-279">Response</span></span>
<span data-ttu-id="0ae02-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ae02-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




