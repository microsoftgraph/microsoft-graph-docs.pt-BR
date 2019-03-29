---
title: Criar windows10EasEmailProfileConfiguration
description: Criar um novo objeto windows10EasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6984d381bd3e19a5174db4ebc562bdacf5382aa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984293"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="7dc61-103">Criar windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="7dc61-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="7dc61-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dc61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dc61-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dc61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dc61-106">Criar um novo objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7dc61-106">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dc61-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7dc61-107">Prerequisites</span></span>
<span data-ttu-id="7dc61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dc61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dc61-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dc61-110">Permission type</span></span>|<span data-ttu-id="7dc61-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7dc61-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dc61-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dc61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7dc61-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc61-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7dc61-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dc61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dc61-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dc61-115">Not supported.</span></span>|
|<span data-ttu-id="7dc61-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dc61-116">Application</span></span>|<span data-ttu-id="7dc61-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dc61-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dc61-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7dc61-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc61-119">Request headers</span></span>
|<span data-ttu-id="7dc61-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7dc61-120">Header</span></span>|<span data-ttu-id="7dc61-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7dc61-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dc61-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dc61-122">Authorization</span></span>|<span data-ttu-id="7dc61-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dc61-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dc61-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7dc61-124">Accept</span></span>|<span data-ttu-id="7dc61-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7dc61-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dc61-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc61-126">Request body</span></span>
<span data-ttu-id="7dc61-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7dc61-127">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="7dc61-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7dc61-128">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="7dc61-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dc61-129">Property</span></span>|<span data-ttu-id="7dc61-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dc61-130">Type</span></span>|<span data-ttu-id="7dc61-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dc61-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dc61-132">id</span><span class="sxs-lookup"><span data-stu-id="7dc61-132">id</span></span>|<span data-ttu-id="7dc61-133">String</span><span class="sxs-lookup"><span data-stu-id="7dc61-133">String</span></span>|<span data-ttu-id="7dc61-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7dc61-134">Key of the entity.</span></span> <span data-ttu-id="7dc61-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dc61-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dc61-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7dc61-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dc61-137">DateTimeOffset</span></span>|<span data-ttu-id="7dc61-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7dc61-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7dc61-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dc61-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7dc61-140">roleScopeTagIds</span></span>|<span data-ttu-id="7dc61-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7dc61-141">String collection</span></span>|<span data-ttu-id="7dc61-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7dc61-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7dc61-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dc61-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7dc61-144">supportsScopeTags</span></span>|<span data-ttu-id="7dc61-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc61-145">Boolean</span></span>|<span data-ttu-id="7dc61-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7dc61-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7dc61-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7dc61-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7dc61-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7dc61-149">This property is read-only.</span></span> <span data-ttu-id="7dc61-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dc61-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dc61-151">createdDateTime</span></span>|<span data-ttu-id="7dc61-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dc61-152">DateTimeOffset</span></span>|<span data-ttu-id="7dc61-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7dc61-153">DateTime the object was created.</span></span> <span data-ttu-id="7dc61-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dc61-155">descrição</span><span class="sxs-lookup"><span data-stu-id="7dc61-155">description</span></span>|<span data-ttu-id="7dc61-156">String</span><span class="sxs-lookup"><span data-stu-id="7dc61-156">String</span></span>|<span data-ttu-id="7dc61-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7dc61-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dc61-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7dc61-159">displayName</span></span>|<span data-ttu-id="7dc61-160">String</span><span class="sxs-lookup"><span data-stu-id="7dc61-160">String</span></span>|<span data-ttu-id="7dc61-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7dc61-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dc61-163">versão</span><span class="sxs-lookup"><span data-stu-id="7dc61-163">version</span></span>|<span data-ttu-id="7dc61-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7dc61-164">Int32</span></span>|<span data-ttu-id="7dc61-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-165">Version of the device configuration.</span></span> <span data-ttu-id="7dc61-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dc61-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7dc61-167">usernameSource</span></span>|[<span data-ttu-id="7dc61-168">userEmail</span><span class="sxs-lookup"><span data-stu-id="7dc61-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7dc61-169">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7dc61-170">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7dc61-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7dc61-171">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7dc61-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7dc61-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="7dc61-172">usernameAADSource</span></span>|[<span data-ttu-id="7dc61-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7dc61-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="7dc61-174">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="7dc61-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="7dc61-175">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7dc61-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7dc61-176">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="7dc61-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="7dc61-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="7dc61-177">userDomainNameSource</span></span>|[<span data-ttu-id="7dc61-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="7dc61-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="7dc61-179">Atributo userDomainname que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7dc61-180">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7dc61-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7dc61-181">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="7dc61-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="7dc61-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="7dc61-182">customDomainName</span></span>|<span data-ttu-id="7dc61-183">String</span><span class="sxs-lookup"><span data-stu-id="7dc61-183">String</span></span>|<span data-ttu-id="7dc61-184">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="7dc61-185">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="7dc61-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="7dc61-186">accountName</span><span class="sxs-lookup"><span data-stu-id="7dc61-186">accountName</span></span>|<span data-ttu-id="7dc61-187">String</span><span class="sxs-lookup"><span data-stu-id="7dc61-187">String</span></span>|<span data-ttu-id="7dc61-188">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="7dc61-188">Account name.</span></span>|
|<span data-ttu-id="7dc61-189">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="7dc61-189">syncCalendar</span></span>|<span data-ttu-id="7dc61-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc61-190">Boolean</span></span>|<span data-ttu-id="7dc61-191">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="7dc61-191">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="7dc61-192">syncContacts</span><span class="sxs-lookup"><span data-stu-id="7dc61-192">syncContacts</span></span>|<span data-ttu-id="7dc61-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc61-193">Boolean</span></span>|<span data-ttu-id="7dc61-194">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="7dc61-194">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="7dc61-195">syncTasks</span><span class="sxs-lookup"><span data-stu-id="7dc61-195">syncTasks</span></span>|<span data-ttu-id="7dc61-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc61-196">Boolean</span></span>|<span data-ttu-id="7dc61-197">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="7dc61-197">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="7dc61-198">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7dc61-198">durationOfEmailToSync</span></span>|[<span data-ttu-id="7dc61-199">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7dc61-199">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7dc61-200">Duração do email a ser sincronizado. Os valores possíveis são `userDefined`: `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`,.</span><span class="sxs-lookup"><span data-stu-id="7dc61-200">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7dc61-201">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="7dc61-201">emailAddressSource</span></span>|[<span data-ttu-id="7dc61-202">userEmail</span><span class="sxs-lookup"><span data-stu-id="7dc61-202">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7dc61-203">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7dc61-203">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7dc61-204">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7dc61-204">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7dc61-205">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="7dc61-205">emailSyncSchedule</span></span>|[<span data-ttu-id="7dc61-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="7dc61-206">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="7dc61-207">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="7dc61-207">Email sync schedule.</span></span> <span data-ttu-id="7dc61-208">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="7dc61-208">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="7dc61-209">hostName</span><span class="sxs-lookup"><span data-stu-id="7dc61-209">hostName</span></span>|<span data-ttu-id="7dc61-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7dc61-210">String</span></span>|<span data-ttu-id="7dc61-211">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="7dc61-211">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="7dc61-212">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7dc61-212">requireSsl</span></span>|<span data-ttu-id="7dc61-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc61-213">Boolean</span></span>|<span data-ttu-id="7dc61-214">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="7dc61-214">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="7dc61-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc61-215">Response</span></span>
<span data-ttu-id="7dc61-216">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dc61-216">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dc61-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dc61-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dc61-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc61-218">Request</span></span>
<span data-ttu-id="7dc61-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dc61-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 753

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="7dc61-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc61-220">Response</span></span>
<span data-ttu-id="7dc61-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dc61-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




