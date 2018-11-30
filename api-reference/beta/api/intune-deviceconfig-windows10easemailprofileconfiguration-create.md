---
title: Criar windows10EasEmailProfileConfiguration
description: Crie um novo objeto de windows10EasEmailProfileConfiguration.
ms.openlocfilehash: 8c3eed8547de75538cfce2a7260deaa0a67fa407
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036103"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="95e24-103">Criar windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="95e24-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="95e24-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="95e24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95e24-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95e24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95e24-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="95e24-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95e24-107">Crie um novo objeto de [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="95e24-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95e24-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95e24-108">Prerequisites</span></span>
<span data-ttu-id="95e24-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95e24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95e24-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95e24-111">Permission type</span></span>|<span data-ttu-id="95e24-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95e24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95e24-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95e24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95e24-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e24-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95e24-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95e24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95e24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95e24-116">Not supported.</span></span>|
|<span data-ttu-id="95e24-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95e24-117">Application</span></span>|<span data-ttu-id="95e24-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95e24-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95e24-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95e24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="95e24-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95e24-120">Request headers</span></span>
|<span data-ttu-id="95e24-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95e24-121">Header</span></span>|<span data-ttu-id="95e24-122">Valor</span><span class="sxs-lookup"><span data-stu-id="95e24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95e24-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95e24-123">Authorization</span></span>|<span data-ttu-id="95e24-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95e24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95e24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95e24-125">Accept</span></span>|<span data-ttu-id="95e24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95e24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95e24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95e24-127">Request body</span></span>
<span data-ttu-id="95e24-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="95e24-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="95e24-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="95e24-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="95e24-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95e24-130">Property</span></span>|<span data-ttu-id="95e24-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="95e24-131">Type</span></span>|<span data-ttu-id="95e24-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="95e24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95e24-133">id</span><span class="sxs-lookup"><span data-stu-id="95e24-133">id</span></span>|<span data-ttu-id="95e24-134">String</span><span class="sxs-lookup"><span data-stu-id="95e24-134">String</span></span>|<span data-ttu-id="95e24-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="95e24-135">Key of the entity.</span></span> <span data-ttu-id="95e24-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95e24-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95e24-137">lastModifiedDateTime</span></span>|<span data-ttu-id="95e24-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95e24-138">DateTimeOffset</span></span>|<span data-ttu-id="95e24-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="95e24-139">DateTime the object was last modified.</span></span> <span data-ttu-id="95e24-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95e24-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95e24-141">roleScopeTagIds</span></span>|<span data-ttu-id="95e24-142">String collection</span><span class="sxs-lookup"><span data-stu-id="95e24-142">String collection</span></span>|<span data-ttu-id="95e24-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="95e24-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95e24-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95e24-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95e24-145">supportsScopeTags</span></span>|<span data-ttu-id="95e24-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="95e24-146">Boolean</span></span>|<span data-ttu-id="95e24-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="95e24-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95e24-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="95e24-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95e24-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="95e24-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95e24-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95e24-150">This property is read-only.</span></span> <span data-ttu-id="95e24-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95e24-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95e24-152">createdDateTime</span></span>|<span data-ttu-id="95e24-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95e24-153">DateTimeOffset</span></span>|<span data-ttu-id="95e24-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="95e24-154">DateTime the object was created.</span></span> <span data-ttu-id="95e24-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95e24-156">description</span><span class="sxs-lookup"><span data-stu-id="95e24-156">description</span></span>|<span data-ttu-id="95e24-157">String</span><span class="sxs-lookup"><span data-stu-id="95e24-157">String</span></span>|<span data-ttu-id="95e24-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95e24-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95e24-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95e24-160">displayName</span><span class="sxs-lookup"><span data-stu-id="95e24-160">displayName</span></span>|<span data-ttu-id="95e24-161">String</span><span class="sxs-lookup"><span data-stu-id="95e24-161">String</span></span>|<span data-ttu-id="95e24-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95e24-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95e24-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95e24-164">version</span><span class="sxs-lookup"><span data-stu-id="95e24-164">version</span></span>|<span data-ttu-id="95e24-165">Int32</span><span class="sxs-lookup"><span data-stu-id="95e24-165">Int32</span></span>|<span data-ttu-id="95e24-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95e24-166">Version of the device configuration.</span></span> <span data-ttu-id="95e24-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95e24-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="95e24-168">usernameSource</span></span>|[<span data-ttu-id="95e24-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="95e24-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="95e24-170">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95e24-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="95e24-171">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="95e24-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="95e24-172">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="95e24-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="95e24-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="95e24-173">usernameAADSource</span></span>|[<span data-ttu-id="95e24-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="95e24-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="95e24-175">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="95e24-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="95e24-176">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="95e24-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="95e24-177">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="95e24-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="95e24-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="95e24-178">userDomainNameSource</span></span>|[<span data-ttu-id="95e24-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="95e24-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="95e24-180">Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95e24-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="95e24-181">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="95e24-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="95e24-182">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="95e24-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="95e24-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="95e24-183">customDomainName</span></span>|<span data-ttu-id="95e24-184">String</span><span class="sxs-lookup"><span data-stu-id="95e24-184">String</span></span>|<span data-ttu-id="95e24-185">Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95e24-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="95e24-186">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="95e24-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="95e24-187">accountName</span><span class="sxs-lookup"><span data-stu-id="95e24-187">accountName</span></span>|<span data-ttu-id="95e24-188">String</span><span class="sxs-lookup"><span data-stu-id="95e24-188">String</span></span>|<span data-ttu-id="95e24-189">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="95e24-189">Account name.</span></span>|
|<span data-ttu-id="95e24-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="95e24-190">syncCalendar</span></span>|<span data-ttu-id="95e24-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="95e24-191">Boolean</span></span>|<span data-ttu-id="95e24-192">Se deseja ou não sincronizar o calendário.</span><span class="sxs-lookup"><span data-stu-id="95e24-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="95e24-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="95e24-193">syncContacts</span></span>|<span data-ttu-id="95e24-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="95e24-194">Boolean</span></span>|<span data-ttu-id="95e24-195">Se deseja ou não sincronizar contatos.</span><span class="sxs-lookup"><span data-stu-id="95e24-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="95e24-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="95e24-196">syncTasks</span></span>|<span data-ttu-id="95e24-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="95e24-197">Boolean</span></span>|<span data-ttu-id="95e24-198">Se deseja ou não sincronizar tarefas.</span><span class="sxs-lookup"><span data-stu-id="95e24-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="95e24-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="95e24-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="95e24-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="95e24-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="95e24-201">Duração de email para sincronizar. Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="95e24-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="95e24-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="95e24-202">emailAddressSource</span></span>|[<span data-ttu-id="95e24-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="95e24-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="95e24-204">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95e24-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="95e24-205">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="95e24-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="95e24-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="95e24-206">emailSyncSchedule</span></span>|[<span data-ttu-id="95e24-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="95e24-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="95e24-208">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="95e24-208">Email sync schedule.</span></span> <span data-ttu-id="95e24-209">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="95e24-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="95e24-210">hostName</span><span class="sxs-lookup"><span data-stu-id="95e24-210">hostName</span></span>|<span data-ttu-id="95e24-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95e24-211">String</span></span>|<span data-ttu-id="95e24-212">Local do Exchange que (URL) que o aplicativo de email nativo se conecta ao.</span><span class="sxs-lookup"><span data-stu-id="95e24-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="95e24-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="95e24-213">requireSsl</span></span>|<span data-ttu-id="95e24-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="95e24-214">Boolean</span></span>|<span data-ttu-id="95e24-215">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="95e24-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="95e24-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="95e24-216">Response</span></span>
<span data-ttu-id="95e24-217">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95e24-217">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95e24-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95e24-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="95e24-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95e24-219">Request</span></span>
<span data-ttu-id="95e24-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95e24-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 817

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="95e24-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="95e24-221">Response</span></span>
<span data-ttu-id="95e24-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95e24-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 925

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```





