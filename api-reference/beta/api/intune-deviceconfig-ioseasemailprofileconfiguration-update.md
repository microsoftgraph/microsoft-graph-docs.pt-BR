---
title: Atualizar iosEasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto iosEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7470630caf4cedc46a5f51efeed926dfe7502fba
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780473"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="6389d-103">Atualizar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="6389d-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="6389d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6389d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6389d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6389d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6389d-106">Atualiza as propriedades de um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6389d-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6389d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6389d-107">Prerequisites</span></span>
<span data-ttu-id="6389d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6389d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6389d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6389d-110">Permission type</span></span>|<span data-ttu-id="6389d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6389d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6389d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6389d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6389d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6389d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6389d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6389d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6389d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6389d-115">Not supported.</span></span>|
|<span data-ttu-id="6389d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6389d-116">Application</span></span>|<span data-ttu-id="6389d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6389d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6389d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6389d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6389d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6389d-119">Request headers</span></span>
|<span data-ttu-id="6389d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6389d-120">Header</span></span>|<span data-ttu-id="6389d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6389d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6389d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6389d-122">Authorization</span></span>|<span data-ttu-id="6389d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6389d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6389d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6389d-124">Accept</span></span>|<span data-ttu-id="6389d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6389d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6389d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6389d-126">Request body</span></span>
<span data-ttu-id="6389d-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6389d-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="6389d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6389d-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="6389d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6389d-129">Property</span></span>|<span data-ttu-id="6389d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6389d-130">Type</span></span>|<span data-ttu-id="6389d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6389d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6389d-132">id</span><span class="sxs-lookup"><span data-stu-id="6389d-132">id</span></span>|<span data-ttu-id="6389d-133">String</span><span class="sxs-lookup"><span data-stu-id="6389d-133">String</span></span>|<span data-ttu-id="6389d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6389d-134">Key of the entity.</span></span> <span data-ttu-id="6389d-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6389d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6389d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6389d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6389d-137">DateTimeOffset</span></span>|<span data-ttu-id="6389d-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6389d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6389d-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6389d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6389d-140">roleScopeTagIds</span></span>|<span data-ttu-id="6389d-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6389d-141">String collection</span></span>|<span data-ttu-id="6389d-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6389d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6389d-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6389d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6389d-144">supportsScopeTags</span></span>|<span data-ttu-id="6389d-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-145">Boolean</span></span>|<span data-ttu-id="6389d-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6389d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6389d-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6389d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6389d-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6389d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6389d-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6389d-149">This property is read-only.</span></span> <span data-ttu-id="6389d-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6389d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6389d-151">createdDateTime</span></span>|<span data-ttu-id="6389d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6389d-152">DateTimeOffset</span></span>|<span data-ttu-id="6389d-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6389d-153">DateTime the object was created.</span></span> <span data-ttu-id="6389d-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6389d-155">description</span><span class="sxs-lookup"><span data-stu-id="6389d-155">description</span></span>|<span data-ttu-id="6389d-156">String</span><span class="sxs-lookup"><span data-stu-id="6389d-156">String</span></span>|<span data-ttu-id="6389d-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6389d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6389d-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6389d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6389d-159">displayName</span></span>|<span data-ttu-id="6389d-160">String</span><span class="sxs-lookup"><span data-stu-id="6389d-160">String</span></span>|<span data-ttu-id="6389d-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6389d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6389d-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6389d-163">versão</span><span class="sxs-lookup"><span data-stu-id="6389d-163">version</span></span>|<span data-ttu-id="6389d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6389d-164">Int32</span></span>|<span data-ttu-id="6389d-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6389d-165">Version of the device configuration.</span></span> <span data-ttu-id="6389d-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6389d-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6389d-167">usernameSource</span></span>|[<span data-ttu-id="6389d-168">userEmail</span><span class="sxs-lookup"><span data-stu-id="6389d-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6389d-169">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6389d-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6389d-170">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="6389d-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6389d-171">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6389d-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6389d-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="6389d-172">usernameAADSource</span></span>|[<span data-ttu-id="6389d-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6389d-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="6389d-174">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="6389d-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="6389d-175">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="6389d-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6389d-176">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="6389d-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="6389d-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="6389d-177">userDomainNameSource</span></span>|[<span data-ttu-id="6389d-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="6389d-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="6389d-179">Atributo userDomainname que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6389d-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6389d-180">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="6389d-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6389d-181">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="6389d-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="6389d-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="6389d-182">customDomainName</span></span>|<span data-ttu-id="6389d-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6389d-183">String</span></span>|<span data-ttu-id="6389d-184">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6389d-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="6389d-185">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6389d-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="6389d-186">accountName</span><span class="sxs-lookup"><span data-stu-id="6389d-186">accountName</span></span>|<span data-ttu-id="6389d-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6389d-187">String</span></span>|<span data-ttu-id="6389d-188">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="6389d-188">Account name.</span></span>|
|<span data-ttu-id="6389d-189">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6389d-189">authenticationMethod</span></span>|[<span data-ttu-id="6389d-190">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6389d-190">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="6389d-191">Método de autenticação para este perfil de email.</span><span class="sxs-lookup"><span data-stu-id="6389d-191">Authentication method for this Email profile.</span></span> <span data-ttu-id="6389d-192">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="6389d-192">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="6389d-193">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="6389d-193">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="6389d-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-194">Boolean</span></span>|<span data-ttu-id="6389d-195">Indica se as mensagens de movimentação devem ou não ser bloqueadas para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="6389d-195">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="6389d-196">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="6389d-196">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="6389d-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-197">Boolean</span></span>|<span data-ttu-id="6389d-198">Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6389d-198">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="6389d-199">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="6389d-199">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="6389d-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-200">Boolean</span></span>|<span data-ttu-id="6389d-201">Indica se a sincronização de endereços de email usados recentemente deve ou não ser bloqueada, por exemplo, ao compor novos emails.</span><span class="sxs-lookup"><span data-stu-id="6389d-201">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="6389d-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6389d-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="6389d-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="6389d-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6389d-204">Duração de tempo que o email deve ser sincronizado de volta para o.</span><span class="sxs-lookup"><span data-stu-id="6389d-204">Duration of time email should be synced back to.</span></span> <span data-ttu-id="6389d-205">.</span><span class="sxs-lookup"><span data-stu-id="6389d-205"></span></span> <span data-ttu-id="6389d-206">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="6389d-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6389d-207">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="6389d-207">emailAddressSource</span></span>|[<span data-ttu-id="6389d-208">userEmail</span><span class="sxs-lookup"><span data-stu-id="6389d-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6389d-209">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6389d-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6389d-210">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6389d-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6389d-211">hostName</span><span class="sxs-lookup"><span data-stu-id="6389d-211">hostName</span></span>|<span data-ttu-id="6389d-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6389d-212">String</span></span>|<span data-ttu-id="6389d-213">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="6389d-213">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="6389d-214">requireSmime</span><span class="sxs-lookup"><span data-stu-id="6389d-214">requireSmime</span></span>|<span data-ttu-id="6389d-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-215">Boolean</span></span>|<span data-ttu-id="6389d-216">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="6389d-216">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="6389d-217">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="6389d-217">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="6389d-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-218">Boolean</span></span>|<span data-ttu-id="6389d-219">Indica se os emails não criptografados devem ou não ser permitidos.</span><span class="sxs-lookup"><span data-stu-id="6389d-219">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="6389d-220">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="6389d-220">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="6389d-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-221">Boolean</span></span>|<span data-ttu-id="6389d-222">Se definido como true a criptografia S/MIME estiver habilitada por padrão.</span><span class="sxs-lookup"><span data-stu-id="6389d-222">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="6389d-223">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="6389d-223">smimeSigningEnabled</span></span>|<span data-ttu-id="6389d-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-224">Boolean</span></span>|<span data-ttu-id="6389d-225">Se definido como true a assinatura S/MIME estiver habilitada para essa conta</span><span class="sxs-lookup"><span data-stu-id="6389d-225">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="6389d-226">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="6389d-226">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="6389d-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-227">Boolean</span></span>|<span data-ttu-id="6389d-228">Se definido como true, o usuário pode ativar ou desativar a assinatura S/MIME.</span><span class="sxs-lookup"><span data-stu-id="6389d-228">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="6389d-229">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="6389d-229">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="6389d-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-230">Boolean</span></span>|<span data-ttu-id="6389d-231">Se definido como true, o usuário pode ativar a opção criptografia por padrão.</span><span class="sxs-lookup"><span data-stu-id="6389d-231">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="6389d-232">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="6389d-232">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="6389d-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-233">Boolean</span></span>|<span data-ttu-id="6389d-234">Se definido como true, o usuário pode selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="6389d-234">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="6389d-235">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="6389d-235">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="6389d-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-236">Boolean</span></span>|<span data-ttu-id="6389d-237">Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="6389d-237">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="6389d-238">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6389d-238">requireSsl</span></span>|<span data-ttu-id="6389d-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-239">Boolean</span></span>|<span data-ttu-id="6389d-240">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="6389d-240">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="6389d-241">useOAuth</span><span class="sxs-lookup"><span data-stu-id="6389d-241">useOAuth</span></span>|<span data-ttu-id="6389d-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="6389d-242">Boolean</span></span>|<span data-ttu-id="6389d-243">Especifica se a conexão deve usar o OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="6389d-243">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="6389d-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="6389d-244">Response</span></span>
<span data-ttu-id="6389d-245">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6389d-245">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6389d-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6389d-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="6389d-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6389d-247">Request</span></span>
<span data-ttu-id="6389d-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6389d-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1193

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
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="6389d-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="6389d-249">Response</span></span>
<span data-ttu-id="6389d-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6389d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1365

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
  "useOAuth": true
}
```





