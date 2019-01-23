---
title: Criar iosEasEmailProfileConfiguration
description: Crie um novo objeto de iosEasEmailProfileConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c7de248c21b0efebdcff07ebac804656dc8ebfde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404446"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="f77cd-103">Criar iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="f77cd-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="f77cd-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f77cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f77cd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f77cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f77cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f77cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77cd-107">Crie um novo objeto de [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f77cd-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f77cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f77cd-108">Prerequisites</span></span>
<span data-ttu-id="f77cd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f77cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f77cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f77cd-111">Permission type</span></span>|<span data-ttu-id="f77cd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f77cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f77cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f77cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f77cd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f77cd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f77cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f77cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f77cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f77cd-116">Not supported.</span></span>|
|<span data-ttu-id="f77cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f77cd-117">Application</span></span>|<span data-ttu-id="f77cd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f77cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f77cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f77cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f77cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f77cd-120">Request headers</span></span>
|<span data-ttu-id="f77cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f77cd-121">Header</span></span>|<span data-ttu-id="f77cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f77cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f77cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f77cd-123">Authorization</span></span>|<span data-ttu-id="f77cd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f77cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f77cd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f77cd-125">Accept</span></span>|<span data-ttu-id="f77cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f77cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f77cd-127">Request body</span></span>
<span data-ttu-id="f77cd-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f77cd-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="f77cd-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f77cd-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="f77cd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f77cd-130">Property</span></span>|<span data-ttu-id="f77cd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f77cd-131">Type</span></span>|<span data-ttu-id="f77cd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f77cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f77cd-133">id</span><span class="sxs-lookup"><span data-stu-id="f77cd-133">id</span></span>|<span data-ttu-id="f77cd-134">String</span><span class="sxs-lookup"><span data-stu-id="f77cd-134">String</span></span>|<span data-ttu-id="f77cd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f77cd-135">Key of the entity.</span></span> <span data-ttu-id="f77cd-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f77cd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f77cd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f77cd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77cd-138">DateTimeOffset</span></span>|<span data-ttu-id="f77cd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f77cd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f77cd-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f77cd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f77cd-141">roleScopeTagIds</span></span>|<span data-ttu-id="f77cd-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f77cd-142">String collection</span></span>|<span data-ttu-id="f77cd-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f77cd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f77cd-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f77cd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f77cd-145">supportsScopeTags</span></span>|<span data-ttu-id="f77cd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-146">Boolean</span></span>|<span data-ttu-id="f77cd-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f77cd-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f77cd-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f77cd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f77cd-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f77cd-150">This property is read-only.</span></span> <span data-ttu-id="f77cd-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f77cd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f77cd-152">createdDateTime</span></span>|<span data-ttu-id="f77cd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77cd-153">DateTimeOffset</span></span>|<span data-ttu-id="f77cd-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f77cd-154">DateTime the object was created.</span></span> <span data-ttu-id="f77cd-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f77cd-156">description</span><span class="sxs-lookup"><span data-stu-id="f77cd-156">description</span></span>|<span data-ttu-id="f77cd-157">String</span><span class="sxs-lookup"><span data-stu-id="f77cd-157">String</span></span>|<span data-ttu-id="f77cd-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f77cd-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f77cd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f77cd-160">displayName</span></span>|<span data-ttu-id="f77cd-161">String</span><span class="sxs-lookup"><span data-stu-id="f77cd-161">String</span></span>|<span data-ttu-id="f77cd-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f77cd-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f77cd-164">version</span><span class="sxs-lookup"><span data-stu-id="f77cd-164">version</span></span>|<span data-ttu-id="f77cd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f77cd-165">Int32</span></span>|<span data-ttu-id="f77cd-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-166">Version of the device configuration.</span></span> <span data-ttu-id="f77cd-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f77cd-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="f77cd-168">usernameSource</span></span>|[<span data-ttu-id="f77cd-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="f77cd-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="f77cd-170">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f77cd-171">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="f77cd-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="f77cd-172">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="f77cd-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f77cd-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="f77cd-173">usernameAADSource</span></span>|[<span data-ttu-id="f77cd-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="f77cd-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="f77cd-175">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="f77cd-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="f77cd-176">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="f77cd-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="f77cd-177">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="f77cd-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="f77cd-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="f77cd-178">userDomainNameSource</span></span>|[<span data-ttu-id="f77cd-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="f77cd-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="f77cd-180">Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f77cd-181">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="f77cd-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="f77cd-182">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="f77cd-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="f77cd-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="f77cd-183">customDomainName</span></span>|<span data-ttu-id="f77cd-184">String</span><span class="sxs-lookup"><span data-stu-id="f77cd-184">String</span></span>|<span data-ttu-id="f77cd-185">Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="f77cd-186">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="f77cd-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="f77cd-187">accountName</span><span class="sxs-lookup"><span data-stu-id="f77cd-187">accountName</span></span>|<span data-ttu-id="f77cd-188">String</span><span class="sxs-lookup"><span data-stu-id="f77cd-188">String</span></span>|<span data-ttu-id="f77cd-189">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="f77cd-189">Account name.</span></span>|
|<span data-ttu-id="f77cd-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f77cd-190">authenticationMethod</span></span>|[<span data-ttu-id="f77cd-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f77cd-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="f77cd-192">Método de autenticação para esse perfil de Email.</span><span class="sxs-lookup"><span data-stu-id="f77cd-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="f77cd-193">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="f77cd-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="f77cd-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="f77cd-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="f77cd-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-195">Boolean</span></span>|<span data-ttu-id="f77cd-196">Indica se deve ou não bloquear mover mensagens para outras contas de email.</span><span class="sxs-lookup"><span data-stu-id="f77cd-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="f77cd-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="f77cd-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="f77cd-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-198">Boolean</span></span>|<span data-ttu-id="f77cd-199">Indica se ou não bloquear o envio de email a partir de aplicativos de terceiros.</span><span class="sxs-lookup"><span data-stu-id="f77cd-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="f77cd-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="f77cd-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="f77cd-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-201">Boolean</span></span>|<span data-ttu-id="f77cd-202">Indica se deve ou não bloquear sincronizando endereços de email usados recentemente, por exemplo - ao redigir novo email.</span><span class="sxs-lookup"><span data-stu-id="f77cd-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="f77cd-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="f77cd-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="f77cd-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="f77cd-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="f77cd-205">Duração de email de tempo deve ser sincronizada com.</span><span class="sxs-lookup"><span data-stu-id="f77cd-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="f77cd-206">.</span><span class="sxs-lookup"><span data-stu-id="f77cd-206"></span></span> <span data-ttu-id="f77cd-207">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="f77cd-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="f77cd-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="f77cd-208">emailAddressSource</span></span>|[<span data-ttu-id="f77cd-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="f77cd-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="f77cd-210">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f77cd-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f77cd-211">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="f77cd-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f77cd-212">hostName</span><span class="sxs-lookup"><span data-stu-id="f77cd-212">hostName</span></span>|<span data-ttu-id="f77cd-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f77cd-213">String</span></span>|<span data-ttu-id="f77cd-214">Local do Exchange que (URL) que o aplicativo de email nativo se conecta ao.</span><span class="sxs-lookup"><span data-stu-id="f77cd-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="f77cd-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="f77cd-215">requireSmime</span></span>|<span data-ttu-id="f77cd-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-216">Boolean</span></span>|<span data-ttu-id="f77cd-217">Indica se deve ou não usar certificados S/MIME.</span><span class="sxs-lookup"><span data-stu-id="f77cd-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="f77cd-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="f77cd-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="f77cd-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-219">Boolean</span></span>|<span data-ttu-id="f77cd-220">Indica se deve ou não permitir que os e-mails descriptografados.</span><span class="sxs-lookup"><span data-stu-id="f77cd-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="f77cd-221">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="f77cd-221">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="f77cd-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-222">Boolean</span></span>|<span data-ttu-id="f77cd-223">Se definido como true criptografia de S/MIME é habilitado por padrão.</span><span class="sxs-lookup"><span data-stu-id="f77cd-223">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="f77cd-224">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="f77cd-224">smimeSigningEnabled</span></span>|<span data-ttu-id="f77cd-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-225">Boolean</span></span>|<span data-ttu-id="f77cd-226">Se definido como true de assinatura de S/MIME estiver habilitado para esta conta</span><span class="sxs-lookup"><span data-stu-id="f77cd-226">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="f77cd-227">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="f77cd-227">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="f77cd-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-228">Boolean</span></span>|<span data-ttu-id="f77cd-229">Se definido como true, o usuário pode alternar assinatura S/MIME ativado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="f77cd-229">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="f77cd-230">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="f77cd-230">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="f77cd-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-231">Boolean</span></span>|<span data-ttu-id="f77cd-232">Se definido como true, o usuário pode alternar a criptografia pela configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="f77cd-232">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="f77cd-233">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="f77cd-233">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="f77cd-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-234">Boolean</span></span>|<span data-ttu-id="f77cd-235">Se definido como true, o usuário pode selecionar a identidade de assinatura.</span><span class="sxs-lookup"><span data-stu-id="f77cd-235">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="f77cd-236">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="f77cd-236">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="f77cd-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-237">Boolean</span></span>|<span data-ttu-id="f77cd-238">Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME.</span><span class="sxs-lookup"><span data-stu-id="f77cd-238">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="f77cd-239">requireSsl</span><span class="sxs-lookup"><span data-stu-id="f77cd-239">requireSsl</span></span>|<span data-ttu-id="f77cd-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-240">Boolean</span></span>|<span data-ttu-id="f77cd-241">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="f77cd-241">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="f77cd-242">useOAuth</span><span class="sxs-lookup"><span data-stu-id="f77cd-242">useOAuth</span></span>|<span data-ttu-id="f77cd-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77cd-243">Boolean</span></span>|<span data-ttu-id="f77cd-244">Especifica se a conexão deve usar OAuth para autenticação.</span><span class="sxs-lookup"><span data-stu-id="f77cd-244">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="f77cd-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="f77cd-245">Response</span></span>
<span data-ttu-id="f77cd-246">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f77cd-246">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f77cd-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f77cd-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="f77cd-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f77cd-248">Request</span></span>
<span data-ttu-id="f77cd-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f77cd-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f77cd-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="f77cd-250">Response</span></span>
<span data-ttu-id="f77cd-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f77cd-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




