---
title: Atualizar iosEasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6bd71c5db6f634e0ce333818c709c9c55316ba8c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923627"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="c3bd2-103">Atualizar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3bd2-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="c3bd2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3bd2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3bd2-106">Atualiza as propriedades de um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c3bd2-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3bd2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c3bd2-107">Prerequisites</span></span>
<span data-ttu-id="c3bd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3bd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3bd2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3bd2-110">Permission type</span></span>|<span data-ttu-id="c3bd2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3bd2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3bd2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bd2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3bd2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3bd2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-115">Not supported.</span></span>|
|<span data-ttu-id="c3bd2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3bd2-116">Application</span></span>|<span data-ttu-id="c3bd2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3bd2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3bd2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c3bd2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3bd2-119">Request headers</span></span>
|<span data-ttu-id="c3bd2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3bd2-120">Header</span></span>|<span data-ttu-id="c3bd2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c3bd2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3bd2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3bd2-122">Authorization</span></span>|<span data-ttu-id="c3bd2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3bd2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c3bd2-124">Accept</span></span>|<span data-ttu-id="c3bd2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3bd2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3bd2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3bd2-126">Request body</span></span>
<span data-ttu-id="c3bd2-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c3bd2-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="c3bd2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bd2-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="c3bd2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3bd2-129">Property</span></span>|<span data-ttu-id="c3bd2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3bd2-130">Type</span></span>|<span data-ttu-id="c3bd2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3bd2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3bd2-132">id</span><span class="sxs-lookup"><span data-stu-id="c3bd2-132">id</span></span>|<span data-ttu-id="c3bd2-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bd2-133">String</span></span>|<span data-ttu-id="c3bd2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-134">Key of the entity.</span></span> <span data-ttu-id="c3bd2-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bd2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3bd2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c3bd2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3bd2-137">DateTimeOffset</span></span>|<span data-ttu-id="c3bd2-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c3bd2-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bd2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3bd2-140">roleScopeTagIds</span></span>|<span data-ttu-id="c3bd2-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bd2-141">String collection</span></span>|<span data-ttu-id="c3bd2-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c3bd2-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bd2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c3bd2-144">supportsScopeTags</span></span>|<span data-ttu-id="c3bd2-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-145">Boolean</span></span>|<span data-ttu-id="c3bd2-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c3bd2-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c3bd2-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c3bd2-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-149">This property is read-only.</span></span> <span data-ttu-id="c3bd2-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bd2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3bd2-151">createdDateTime</span></span>|<span data-ttu-id="c3bd2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3bd2-152">DateTimeOffset</span></span>|<span data-ttu-id="c3bd2-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-153">DateTime the object was created.</span></span> <span data-ttu-id="c3bd2-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bd2-155">description</span><span class="sxs-lookup"><span data-stu-id="c3bd2-155">description</span></span>|<span data-ttu-id="c3bd2-156">String</span><span class="sxs-lookup"><span data-stu-id="c3bd2-156">String</span></span>|<span data-ttu-id="c3bd2-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3bd2-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bd2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c3bd2-159">displayName</span></span>|<span data-ttu-id="c3bd2-160">String</span><span class="sxs-lookup"><span data-stu-id="c3bd2-160">String</span></span>|<span data-ttu-id="c3bd2-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3bd2-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bd2-163">versão</span><span class="sxs-lookup"><span data-stu-id="c3bd2-163">version</span></span>|<span data-ttu-id="c3bd2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bd2-164">Int32</span></span>|<span data-ttu-id="c3bd2-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-165">Version of the device configuration.</span></span> <span data-ttu-id="c3bd2-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bd2-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c3bd2-167">usernameSource</span></span>|[<span data-ttu-id="c3bd2-168">UserEmail</span><span class="sxs-lookup"><span data-stu-id="c3bd2-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c3bd2-169">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c3bd2-170">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c3bd2-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c3bd2-171">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c3bd2-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="c3bd2-172">usernameAADSource</span></span>|[<span data-ttu-id="c3bd2-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c3bd2-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="c3bd2-174">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="c3bd2-175">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c3bd2-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c3bd2-176">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="c3bd2-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="c3bd2-177">userDomainNameSource</span></span>|[<span data-ttu-id="c3bd2-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="c3bd2-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="c3bd2-179">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c3bd2-180">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c3bd2-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c3bd2-181">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="c3bd2-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="c3bd2-182">customDomainName</span></span>|<span data-ttu-id="c3bd2-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bd2-183">String</span></span>|<span data-ttu-id="c3bd2-184">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="c3bd2-185">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="c3bd2-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="c3bd2-186">accountName</span><span class="sxs-lookup"><span data-stu-id="c3bd2-186">accountName</span></span>|<span data-ttu-id="c3bd2-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bd2-187">String</span></span>|<span data-ttu-id="c3bd2-188">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-188">Account name.</span></span>|
|<span data-ttu-id="c3bd2-189">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c3bd2-189">authenticationMethod</span></span>|[<span data-ttu-id="c3bd2-190">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c3bd2-190">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="c3bd2-191">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-191">Authentication method for this Email profile.</span></span> <span data-ttu-id="c3bd2-192">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-192">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c3bd2-193">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="c3bd2-193">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="c3bd2-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-194">Boolean</span></span>|<span data-ttu-id="c3bd2-195">Indica se as mensagens de movimentação devem ou não ser bloqueadas para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-195">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="c3bd2-196">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="c3bd2-196">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="c3bd2-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-197">Boolean</span></span>|<span data-ttu-id="c3bd2-198">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-198">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="c3bd2-199">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c3bd2-199">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="c3bd2-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-200">Boolean</span></span>|<span data-ttu-id="c3bd2-201">Indica se a sincronização de endereços de email usados recentemente deve ou não ser bloqueada, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-201">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="c3bd2-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c3bd2-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="c3bd2-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="c3bd2-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c3bd2-204">Duração de tempo que o email deve ser sincronizado de volta para o.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-204">Duration of time email should be synced back to.</span></span> <span data-ttu-id="c3bd2-205">.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-205"></span></span> <span data-ttu-id="c3bd2-206">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c3bd2-207">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="c3bd2-207">emailAddressSource</span></span>|[<span data-ttu-id="c3bd2-208">UserEmail</span><span class="sxs-lookup"><span data-stu-id="c3bd2-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c3bd2-209">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c3bd2-210">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c3bd2-211">hostName</span><span class="sxs-lookup"><span data-stu-id="c3bd2-211">hostName</span></span>|<span data-ttu-id="c3bd2-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bd2-212">String</span></span>|<span data-ttu-id="c3bd2-213">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-213">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="c3bd2-214">requireSmime</span><span class="sxs-lookup"><span data-stu-id="c3bd2-214">requireSmime</span></span>|<span data-ttu-id="c3bd2-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-215">Boolean</span></span>|<span data-ttu-id="c3bd2-216">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-216">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="c3bd2-217">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="c3bd2-217">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="c3bd2-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-218">Boolean</span></span>|<span data-ttu-id="c3bd2-219">Indica se os emails não criptografados devem ou não ser permitidos.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-219">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="c3bd2-220">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bd2-220">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="c3bd2-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-221">Boolean</span></span>|<span data-ttu-id="c3bd2-222">Se definido como true a criptografia S/MIME estiver habilitada por padrão.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-222">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="c3bd2-223">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bd2-223">smimeSigningEnabled</span></span>|<span data-ttu-id="c3bd2-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-224">Boolean</span></span>|<span data-ttu-id="c3bd2-225">Se definido como true a assinatura S/MIME estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="c3bd2-225">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="c3bd2-226">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bd2-226">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="c3bd2-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-227">Boolean</span></span>|<span data-ttu-id="c3bd2-228">Se definido como true, o usuário pode ativar ou desativar a assinatura S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-228">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="c3bd2-229">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bd2-229">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="c3bd2-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-230">Boolean</span></span>|<span data-ttu-id="c3bd2-231">Se definido como true, o usuário pode ativar a opção criptografia por padrão.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-231">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="c3bd2-232">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bd2-232">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="c3bd2-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-233">Boolean</span></span>|<span data-ttu-id="c3bd2-234">Se definido como true, o usuário pode selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-234">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="c3bd2-235">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="c3bd2-235">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="c3bd2-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-236">Boolean</span></span>|<span data-ttu-id="c3bd2-237">Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-237">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="c3bd2-238">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c3bd2-238">requireSsl</span></span>|<span data-ttu-id="c3bd2-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-239">Boolean</span></span>|<span data-ttu-id="c3bd2-240">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-240">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="c3bd2-241">useOAuth</span><span class="sxs-lookup"><span data-stu-id="c3bd2-241">useOAuth</span></span>|<span data-ttu-id="c3bd2-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3bd2-242">Boolean</span></span>|<span data-ttu-id="c3bd2-243">Especifica se a conexão deve usar o OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-243">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="c3bd2-244">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="c3bd2-244">signingCertificateType</span></span>|[<span data-ttu-id="c3bd2-245">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="c3bd2-245">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="c3bd2-246">Assinatura tipo de certificado para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-246">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="c3bd2-247">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-247">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c3bd2-248">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="c3bd2-248">encryptionCertificateType</span></span>|[<span data-ttu-id="c3bd2-249">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="c3bd2-249">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="c3bd2-250">Tipo de certificado de criptografia para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-250">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="c3bd2-251">Os valores possíveis são: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-251">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="c3bd2-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3bd2-252">Response</span></span>
<span data-ttu-id="c3bd2-253">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-253">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3bd2-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3bd2-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3bd2-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3bd2-255">Request</span></span>
<span data-ttu-id="c3bd2-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1284

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="c3bd2-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3bd2-257">Response</span></span>
<span data-ttu-id="c3bd2-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3bd2-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1456

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




