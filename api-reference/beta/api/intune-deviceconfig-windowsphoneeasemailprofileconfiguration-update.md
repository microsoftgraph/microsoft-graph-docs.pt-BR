---
title: Atualizar windowsPhoneEASEmailProfileConfiguration
description: Atualiza as propriedades de um objeto windowsPhoneEASEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b236924707f262fc3e728efa9930dfb4f3ee62aa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168100"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="73240-103">Atualizar windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="73240-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="73240-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73240-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73240-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73240-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73240-106">Atualiza as propriedades de um objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="73240-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73240-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73240-107">Prerequisites</span></span>
<span data-ttu-id="73240-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="73240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="73240-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73240-110">Permission type</span></span>|<span data-ttu-id="73240-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73240-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73240-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73240-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73240-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73240-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73240-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73240-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73240-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73240-115">Not supported.</span></span>|
|<span data-ttu-id="73240-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73240-116">Application</span></span>|<span data-ttu-id="73240-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73240-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73240-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73240-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="73240-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73240-119">Request headers</span></span>
|<span data-ttu-id="73240-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73240-120">Header</span></span>|<span data-ttu-id="73240-121">Valor</span><span class="sxs-lookup"><span data-stu-id="73240-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73240-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73240-122">Authorization</span></span>|<span data-ttu-id="73240-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73240-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73240-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73240-124">Accept</span></span>|<span data-ttu-id="73240-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73240-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73240-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73240-126">Request body</span></span>
<span data-ttu-id="73240-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="73240-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="73240-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="73240-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="73240-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73240-129">Property</span></span>|<span data-ttu-id="73240-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="73240-130">Type</span></span>|<span data-ttu-id="73240-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="73240-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73240-132">id</span><span class="sxs-lookup"><span data-stu-id="73240-132">id</span></span>|<span data-ttu-id="73240-133">String</span><span class="sxs-lookup"><span data-stu-id="73240-133">String</span></span>|<span data-ttu-id="73240-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73240-134">Key of the entity.</span></span> <span data-ttu-id="73240-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73240-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73240-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73240-136">lastModifiedDateTime</span></span>|<span data-ttu-id="73240-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73240-137">DateTimeOffset</span></span>|<span data-ttu-id="73240-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="73240-138">DateTime the object was last modified.</span></span> <span data-ttu-id="73240-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73240-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73240-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73240-140">roleScopeTagIds</span></span>|<span data-ttu-id="73240-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73240-141">String collection</span></span>|<span data-ttu-id="73240-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="73240-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73240-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73240-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73240-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73240-144">supportsScopeTags</span></span>|<span data-ttu-id="73240-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="73240-145">Boolean</span></span>|<span data-ttu-id="73240-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="73240-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73240-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="73240-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73240-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="73240-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73240-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73240-149">This property is read-only.</span></span> <span data-ttu-id="73240-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73240-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73240-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73240-151">createdDateTime</span></span>|<span data-ttu-id="73240-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73240-152">DateTimeOffset</span></span>|<span data-ttu-id="73240-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="73240-153">DateTime the object was created.</span></span> <span data-ttu-id="73240-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73240-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73240-155">description</span><span class="sxs-lookup"><span data-stu-id="73240-155">description</span></span>|<span data-ttu-id="73240-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73240-156">String</span></span>|<span data-ttu-id="73240-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73240-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73240-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73240-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73240-159">displayName</span><span class="sxs-lookup"><span data-stu-id="73240-159">displayName</span></span>|<span data-ttu-id="73240-160">String</span><span class="sxs-lookup"><span data-stu-id="73240-160">String</span></span>|<span data-ttu-id="73240-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73240-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73240-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73240-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73240-163">version</span><span class="sxs-lookup"><span data-stu-id="73240-163">version</span></span>|<span data-ttu-id="73240-164">Int32</span><span class="sxs-lookup"><span data-stu-id="73240-164">Int32</span></span>|<span data-ttu-id="73240-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73240-165">Version of the device configuration.</span></span> <span data-ttu-id="73240-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73240-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73240-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="73240-167">usernameSource</span></span>|[<span data-ttu-id="73240-168">userEmail</span><span class="sxs-lookup"><span data-stu-id="73240-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="73240-169">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73240-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="73240-170">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="73240-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="73240-171">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="73240-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="73240-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="73240-172">usernameAADSource</span></span>|[<span data-ttu-id="73240-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="73240-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="73240-174">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="73240-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="73240-175">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="73240-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="73240-176">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="73240-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="73240-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="73240-177">userDomainNameSource</span></span>|[<span data-ttu-id="73240-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="73240-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="73240-179">Atributo userDomainname que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73240-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="73240-180">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="73240-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="73240-181">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="73240-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="73240-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="73240-182">customDomainName</span></span>|<span data-ttu-id="73240-183">String</span><span class="sxs-lookup"><span data-stu-id="73240-183">String</span></span>|<span data-ttu-id="73240-184">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73240-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="73240-185">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="73240-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="73240-186">accountName</span><span class="sxs-lookup"><span data-stu-id="73240-186">accountName</span></span>|<span data-ttu-id="73240-187">String</span><span class="sxs-lookup"><span data-stu-id="73240-187">String</span></span>|<span data-ttu-id="73240-188">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="73240-188">Account name.</span></span>|
|<span data-ttu-id="73240-189">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="73240-189">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="73240-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="73240-190">Boolean</span></span>|<span data-ttu-id="73240-191">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="73240-191">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="73240-192">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73240-192">This property is read-only.</span></span>|
|<span data-ttu-id="73240-193">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="73240-193">syncCalendar</span></span>|<span data-ttu-id="73240-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="73240-194">Boolean</span></span>|<span data-ttu-id="73240-195">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="73240-195">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="73240-196">syncContacts</span><span class="sxs-lookup"><span data-stu-id="73240-196">syncContacts</span></span>|<span data-ttu-id="73240-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="73240-197">Boolean</span></span>|<span data-ttu-id="73240-198">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="73240-198">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="73240-199">syncTasks</span><span class="sxs-lookup"><span data-stu-id="73240-199">syncTasks</span></span>|<span data-ttu-id="73240-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="73240-200">Boolean</span></span>|<span data-ttu-id="73240-201">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="73240-201">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="73240-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="73240-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="73240-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="73240-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="73240-204">Duração do email a ser sincronizado. Os valores possíveis são `userDefined`: `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`,.</span><span class="sxs-lookup"><span data-stu-id="73240-204">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="73240-205">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="73240-205">emailAddressSource</span></span>|[<span data-ttu-id="73240-206">userEmail</span><span class="sxs-lookup"><span data-stu-id="73240-206">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="73240-207">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73240-207">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="73240-208">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="73240-208">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="73240-209">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="73240-209">emailSyncSchedule</span></span>|[<span data-ttu-id="73240-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="73240-210">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="73240-211">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="73240-211">Email sync schedule.</span></span> <span data-ttu-id="73240-212">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="73240-212">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="73240-213">hostName</span><span class="sxs-lookup"><span data-stu-id="73240-213">hostName</span></span>|<span data-ttu-id="73240-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73240-214">String</span></span>|<span data-ttu-id="73240-215">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="73240-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="73240-216">requireSsl</span><span class="sxs-lookup"><span data-stu-id="73240-216">requireSsl</span></span>|<span data-ttu-id="73240-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="73240-217">Boolean</span></span>|<span data-ttu-id="73240-218">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="73240-218">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="73240-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="73240-219">Response</span></span>
<span data-ttu-id="73240-220">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73240-220">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73240-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73240-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="73240-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73240-222">Request</span></span>
<span data-ttu-id="73240-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73240-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 794

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
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

### <a name="response"></a><span data-ttu-id="73240-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="73240-224">Response</span></span>
<span data-ttu-id="73240-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73240-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 966

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
  "applyOnlyToWindowsPhone81": true,
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




