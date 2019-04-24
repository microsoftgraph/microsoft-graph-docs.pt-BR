---
title: Criar windowsPhoneEASEmailProfileConfiguration
description: Criar um novo objeto windowsPhoneEASEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5cb552095848bb768159160487f178681511187d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32512527"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="25ff6-103">Criar windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="25ff6-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="25ff6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25ff6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25ff6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25ff6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25ff6-106">Criar um novo objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="25ff6-106">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25ff6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25ff6-107">Prerequisites</span></span>
<span data-ttu-id="25ff6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25ff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25ff6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25ff6-110">Permission type</span></span>|<span data-ttu-id="25ff6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25ff6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25ff6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25ff6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25ff6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25ff6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25ff6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25ff6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25ff6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25ff6-115">Not supported.</span></span>|
|<span data-ttu-id="25ff6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25ff6-116">Application</span></span>|<span data-ttu-id="25ff6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25ff6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25ff6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25ff6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="25ff6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25ff6-119">Request headers</span></span>
|<span data-ttu-id="25ff6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25ff6-120">Header</span></span>|<span data-ttu-id="25ff6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="25ff6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25ff6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="25ff6-122">Authorization</span></span>|<span data-ttu-id="25ff6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25ff6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25ff6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25ff6-124">Accept</span></span>|<span data-ttu-id="25ff6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25ff6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25ff6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25ff6-126">Request body</span></span>
<span data-ttu-id="25ff6-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhoneEASEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="25ff6-127">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="25ff6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhoneEASEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="25ff6-128">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="25ff6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25ff6-129">Property</span></span>|<span data-ttu-id="25ff6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="25ff6-130">Type</span></span>|<span data-ttu-id="25ff6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="25ff6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25ff6-132">id</span><span class="sxs-lookup"><span data-stu-id="25ff6-132">id</span></span>|<span data-ttu-id="25ff6-133">String</span><span class="sxs-lookup"><span data-stu-id="25ff6-133">String</span></span>|<span data-ttu-id="25ff6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25ff6-134">Key of the entity.</span></span> <span data-ttu-id="25ff6-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25ff6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25ff6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="25ff6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25ff6-137">DateTimeOffset</span></span>|<span data-ttu-id="25ff6-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="25ff6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="25ff6-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25ff6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="25ff6-140">roleScopeTagIds</span></span>|<span data-ttu-id="25ff6-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="25ff6-141">String collection</span></span>|<span data-ttu-id="25ff6-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="25ff6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="25ff6-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25ff6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="25ff6-144">supportsScopeTags</span></span>|<span data-ttu-id="25ff6-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="25ff6-145">Boolean</span></span>|<span data-ttu-id="25ff6-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="25ff6-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="25ff6-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="25ff6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="25ff6-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25ff6-149">This property is read-only.</span></span> <span data-ttu-id="25ff6-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25ff6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25ff6-151">createdDateTime</span></span>|<span data-ttu-id="25ff6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25ff6-152">DateTimeOffset</span></span>|<span data-ttu-id="25ff6-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="25ff6-153">DateTime the object was created.</span></span> <span data-ttu-id="25ff6-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25ff6-155">description</span><span class="sxs-lookup"><span data-stu-id="25ff6-155">description</span></span>|<span data-ttu-id="25ff6-156">String</span><span class="sxs-lookup"><span data-stu-id="25ff6-156">String</span></span>|<span data-ttu-id="25ff6-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="25ff6-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25ff6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="25ff6-159">displayName</span></span>|<span data-ttu-id="25ff6-160">String</span><span class="sxs-lookup"><span data-stu-id="25ff6-160">String</span></span>|<span data-ttu-id="25ff6-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="25ff6-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25ff6-163">versão</span><span class="sxs-lookup"><span data-stu-id="25ff6-163">version</span></span>|<span data-ttu-id="25ff6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="25ff6-164">Int32</span></span>|<span data-ttu-id="25ff6-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-165">Version of the device configuration.</span></span> <span data-ttu-id="25ff6-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25ff6-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="25ff6-167">usernameSource</span></span>|[<span data-ttu-id="25ff6-168">userEmail</span><span class="sxs-lookup"><span data-stu-id="25ff6-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="25ff6-169">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="25ff6-170">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="25ff6-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="25ff6-171">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="25ff6-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="25ff6-172">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="25ff6-172">usernameAADSource</span></span>|[<span data-ttu-id="25ff6-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="25ff6-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="25ff6-174">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="25ff6-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="25ff6-175">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="25ff6-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="25ff6-176">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="25ff6-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="25ff6-177">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="25ff6-177">userDomainNameSource</span></span>|[<span data-ttu-id="25ff6-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="25ff6-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="25ff6-179">Atributo userDomainname que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="25ff6-180">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="25ff6-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="25ff6-181">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="25ff6-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="25ff6-182">customDomainName</span><span class="sxs-lookup"><span data-stu-id="25ff6-182">customDomainName</span></span>|<span data-ttu-id="25ff6-183">String</span><span class="sxs-lookup"><span data-stu-id="25ff6-183">String</span></span>|<span data-ttu-id="25ff6-184">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="25ff6-185">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="25ff6-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="25ff6-186">accountName</span><span class="sxs-lookup"><span data-stu-id="25ff6-186">accountName</span></span>|<span data-ttu-id="25ff6-187">String</span><span class="sxs-lookup"><span data-stu-id="25ff6-187">String</span></span>|<span data-ttu-id="25ff6-188">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="25ff6-188">Account name.</span></span>|
|<span data-ttu-id="25ff6-189">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="25ff6-189">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="25ff6-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="25ff6-190">Boolean</span></span>|<span data-ttu-id="25ff6-191">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="25ff6-191">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="25ff6-192">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25ff6-192">This property is read-only.</span></span>|
|<span data-ttu-id="25ff6-193">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="25ff6-193">syncCalendar</span></span>|<span data-ttu-id="25ff6-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="25ff6-194">Boolean</span></span>|<span data-ttu-id="25ff6-195">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="25ff6-195">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="25ff6-196">syncContacts</span><span class="sxs-lookup"><span data-stu-id="25ff6-196">syncContacts</span></span>|<span data-ttu-id="25ff6-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="25ff6-197">Boolean</span></span>|<span data-ttu-id="25ff6-198">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="25ff6-198">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="25ff6-199">syncTasks</span><span class="sxs-lookup"><span data-stu-id="25ff6-199">syncTasks</span></span>|<span data-ttu-id="25ff6-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="25ff6-200">Boolean</span></span>|<span data-ttu-id="25ff6-201">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="25ff6-201">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="25ff6-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="25ff6-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="25ff6-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="25ff6-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="25ff6-204">Duração do email a ser sincronizado. Os valores possíveis são `userDefined`: `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`,.</span><span class="sxs-lookup"><span data-stu-id="25ff6-204">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="25ff6-205">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="25ff6-205">emailAddressSource</span></span>|[<span data-ttu-id="25ff6-206">userEmail</span><span class="sxs-lookup"><span data-stu-id="25ff6-206">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="25ff6-207">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25ff6-207">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="25ff6-208">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="25ff6-208">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="25ff6-209">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="25ff6-209">emailSyncSchedule</span></span>|[<span data-ttu-id="25ff6-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="25ff6-210">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="25ff6-211">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="25ff6-211">Email sync schedule.</span></span> <span data-ttu-id="25ff6-212">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="25ff6-212">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="25ff6-213">hostName</span><span class="sxs-lookup"><span data-stu-id="25ff6-213">hostName</span></span>|<span data-ttu-id="25ff6-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25ff6-214">String</span></span>|<span data-ttu-id="25ff6-215">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="25ff6-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="25ff6-216">requireSsl</span><span class="sxs-lookup"><span data-stu-id="25ff6-216">requireSsl</span></span>|<span data-ttu-id="25ff6-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="25ff6-217">Boolean</span></span>|<span data-ttu-id="25ff6-218">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="25ff6-218">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="25ff6-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="25ff6-219">Response</span></span>
<span data-ttu-id="25ff6-220">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25ff6-220">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25ff6-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25ff6-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="25ff6-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25ff6-222">Request</span></span>
<span data-ttu-id="25ff6-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25ff6-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="25ff6-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="25ff6-224">Response</span></span>
<span data-ttu-id="25ff6-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25ff6-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





