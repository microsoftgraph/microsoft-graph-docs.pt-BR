---
title: Atualizar iosEasEmailProfileConfiguration
description: Atualize as propriedades de um objeto iosEasEmailProfileConfiguration.
author: tfitzmac
ms.openlocfilehash: a330d3c56386da5c440bbe58573f977c876d8481
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343285"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="c365f-103">Atualizar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="c365f-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="c365f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c365f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c365f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c365f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c365f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c365f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c365f-107">Atualize as propriedades de um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c365f-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c365f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c365f-108">Prerequisites</span></span>
<span data-ttu-id="c365f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c365f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c365f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c365f-111">Permission type</span></span>|<span data-ttu-id="c365f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c365f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c365f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c365f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c365f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c365f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c365f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c365f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c365f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c365f-116">Not supported.</span></span>|
|<span data-ttu-id="c365f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c365f-117">Application</span></span>|<span data-ttu-id="c365f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c365f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c365f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c365f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c365f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c365f-120">Request headers</span></span>
|<span data-ttu-id="c365f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c365f-121">Header</span></span>|<span data-ttu-id="c365f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c365f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c365f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c365f-123">Authorization</span></span>|<span data-ttu-id="c365f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c365f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c365f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c365f-125">Accept</span></span>|<span data-ttu-id="c365f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c365f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c365f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c365f-127">Request body</span></span>
<span data-ttu-id="c365f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c365f-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="c365f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c365f-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="c365f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c365f-130">Property</span></span>|<span data-ttu-id="c365f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c365f-131">Type</span></span>|<span data-ttu-id="c365f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c365f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c365f-133">id</span><span class="sxs-lookup"><span data-stu-id="c365f-133">id</span></span>|<span data-ttu-id="c365f-134">String</span><span class="sxs-lookup"><span data-stu-id="c365f-134">String</span></span>|<span data-ttu-id="c365f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c365f-135">Key of the entity.</span></span> <span data-ttu-id="c365f-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c365f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c365f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c365f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c365f-138">DateTimeOffset</span></span>|<span data-ttu-id="c365f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c365f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c365f-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c365f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c365f-141">roleScopeTagIds</span></span>|<span data-ttu-id="c365f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c365f-142">String collection</span></span>|<span data-ttu-id="c365f-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="c365f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c365f-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c365f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c365f-145">supportsScopeTags</span></span>|<span data-ttu-id="c365f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c365f-146">Boolean</span></span>|<span data-ttu-id="c365f-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c365f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c365f-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c365f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c365f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="c365f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c365f-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c365f-150">This property is read-only.</span></span> <span data-ttu-id="c365f-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c365f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c365f-152">createdDateTime</span></span>|<span data-ttu-id="c365f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c365f-153">DateTimeOffset</span></span>|<span data-ttu-id="c365f-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c365f-154">DateTime the object was created.</span></span> <span data-ttu-id="c365f-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c365f-156">description</span><span class="sxs-lookup"><span data-stu-id="c365f-156">description</span></span>|<span data-ttu-id="c365f-157">String</span><span class="sxs-lookup"><span data-stu-id="c365f-157">String</span></span>|<span data-ttu-id="c365f-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c365f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c365f-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c365f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c365f-160">displayName</span></span>|<span data-ttu-id="c365f-161">String</span><span class="sxs-lookup"><span data-stu-id="c365f-161">String</span></span>|<span data-ttu-id="c365f-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c365f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c365f-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c365f-164">version</span><span class="sxs-lookup"><span data-stu-id="c365f-164">version</span></span>|<span data-ttu-id="c365f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c365f-165">Int32</span></span>|<span data-ttu-id="c365f-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c365f-166">Version of the device configuration.</span></span> <span data-ttu-id="c365f-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c365f-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c365f-168">usernameSource</span></span>|[<span data-ttu-id="c365f-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c365f-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c365f-170">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c365f-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c365f-171">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c365f-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c365f-172">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c365f-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c365f-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="c365f-173">usernameAADSource</span></span>|[<span data-ttu-id="c365f-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c365f-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="c365f-175">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="c365f-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="c365f-176">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c365f-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c365f-177">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="c365f-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="c365f-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="c365f-178">userDomainNameSource</span></span>|[<span data-ttu-id="c365f-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="c365f-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="c365f-180">Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c365f-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c365f-181">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c365f-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c365f-182">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="c365f-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="c365f-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="c365f-183">customDomainName</span></span>|<span data-ttu-id="c365f-184">String</span><span class="sxs-lookup"><span data-stu-id="c365f-184">String</span></span>|<span data-ttu-id="c365f-185">Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c365f-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="c365f-186">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="c365f-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="c365f-187">accountName</span><span class="sxs-lookup"><span data-stu-id="c365f-187">accountName</span></span>|<span data-ttu-id="c365f-188">String</span><span class="sxs-lookup"><span data-stu-id="c365f-188">String</span></span>|<span data-ttu-id="c365f-189">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="c365f-189">Account name.</span></span>|
|<span data-ttu-id="c365f-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c365f-190">authenticationMethod</span></span>|[<span data-ttu-id="c365f-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c365f-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="c365f-192">Método de autenticação para esse perfil de Email.</span><span class="sxs-lookup"><span data-stu-id="c365f-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="c365f-193">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="c365f-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="c365f-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="c365f-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="c365f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c365f-195">Boolean</span></span>|<span data-ttu-id="c365f-196">Indica se deve ou não bloquear mover mensagens para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="c365f-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="c365f-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="c365f-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="c365f-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c365f-198">Boolean</span></span>|<span data-ttu-id="c365f-199">Indica se ou não bloquear o envio de email a partir de aplicativos de terceiros.</span><span class="sxs-lookup"><span data-stu-id="c365f-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="c365f-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c365f-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="c365f-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c365f-201">Boolean</span></span>|<span data-ttu-id="c365f-202">Indica se deve ou não bloquear sincronizando endereços de email usados recentemente, por exemplo - ao redigir novo email.</span><span class="sxs-lookup"><span data-stu-id="c365f-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="c365f-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="c365f-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="c365f-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="c365f-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c365f-205">Duração de email de tempo deve ser sincronizada com.</span><span class="sxs-lookup"><span data-stu-id="c365f-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="c365f-206">.</span><span class="sxs-lookup"><span data-stu-id="c365f-206"></span></span> <span data-ttu-id="c365f-207">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="c365f-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c365f-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="c365f-208">emailAddressSource</span></span>|[<span data-ttu-id="c365f-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="c365f-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c365f-210">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c365f-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c365f-211">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c365f-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c365f-212">hostName</span><span class="sxs-lookup"><span data-stu-id="c365f-212">hostName</span></span>|<span data-ttu-id="c365f-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c365f-213">String</span></span>|<span data-ttu-id="c365f-214">Local do Exchange que (URL) que o aplicativo de email nativo se conecta ao.</span><span class="sxs-lookup"><span data-stu-id="c365f-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="c365f-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="c365f-215">requireSmime</span></span>|<span data-ttu-id="c365f-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="c365f-216">Boolean</span></span>|<span data-ttu-id="c365f-217">Indica se deve ou não usar certificados S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c365f-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="c365f-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="c365f-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="c365f-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="c365f-219">Boolean</span></span>|<span data-ttu-id="c365f-220">Indica se deve ou não permitir que os e-mails descriptografados.</span><span class="sxs-lookup"><span data-stu-id="c365f-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="c365f-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="c365f-221">requireSsl</span></span>|<span data-ttu-id="c365f-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c365f-222">Boolean</span></span>|<span data-ttu-id="c365f-223">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="c365f-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="c365f-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="c365f-224">useOAuth</span></span>|<span data-ttu-id="c365f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c365f-225">Boolean</span></span>|<span data-ttu-id="c365f-226">Especifica se a conexão deve usar OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="c365f-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="c365f-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="c365f-227">Response</span></span>
<span data-ttu-id="c365f-228">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c365f-228">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c365f-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c365f-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="c365f-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c365f-230">Request</span></span>
<span data-ttu-id="c365f-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c365f-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 904

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "requireSsl": true,
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="c365f-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="c365f-232">Response</span></span>
<span data-ttu-id="c365f-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c365f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1082

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
  "requireSsl": true,
  "useOAuth": true
}
```





