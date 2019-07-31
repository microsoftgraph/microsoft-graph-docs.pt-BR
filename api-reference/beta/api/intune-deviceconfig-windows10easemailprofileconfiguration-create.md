---
title: Criar windows10EasEmailProfileConfiguration
description: Criar um novo objeto windows10EasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f550e12f258f33724e1366bfd667d2688ac3e2ce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975596"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="54f94-103">Criar windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="54f94-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="54f94-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54f94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54f94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54f94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54f94-106">Criar um novo objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="54f94-106">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54f94-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54f94-107">Prerequisites</span></span>
<span data-ttu-id="54f94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54f94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54f94-110">Permission type</span></span>|<span data-ttu-id="54f94-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54f94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54f94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54f94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54f94-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54f94-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54f94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54f94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54f94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54f94-115">Not supported.</span></span>|
|<span data-ttu-id="54f94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54f94-116">Application</span></span>|<span data-ttu-id="54f94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54f94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54f94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54f94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54f94-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54f94-119">Request headers</span></span>
|<span data-ttu-id="54f94-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54f94-120">Header</span></span>|<span data-ttu-id="54f94-121">Valor</span><span class="sxs-lookup"><span data-stu-id="54f94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54f94-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="54f94-122">Authorization</span></span>|<span data-ttu-id="54f94-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54f94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54f94-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54f94-124">Accept</span></span>|<span data-ttu-id="54f94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54f94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54f94-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54f94-126">Request body</span></span>
<span data-ttu-id="54f94-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54f94-127">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="54f94-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54f94-128">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="54f94-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54f94-129">Property</span></span>|<span data-ttu-id="54f94-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="54f94-130">Type</span></span>|<span data-ttu-id="54f94-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="54f94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54f94-132">id</span><span class="sxs-lookup"><span data-stu-id="54f94-132">id</span></span>|<span data-ttu-id="54f94-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54f94-133">String</span></span>|<span data-ttu-id="54f94-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54f94-134">Key of the entity.</span></span> <span data-ttu-id="54f94-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54f94-136">lastModifiedDateTime</span></span>|<span data-ttu-id="54f94-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54f94-137">DateTimeOffset</span></span>|<span data-ttu-id="54f94-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="54f94-138">DateTime the object was last modified.</span></span> <span data-ttu-id="54f94-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54f94-140">roleScopeTagIds</span></span>|<span data-ttu-id="54f94-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="54f94-141">String collection</span></span>|<span data-ttu-id="54f94-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="54f94-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54f94-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="54f94-144">supportsScopeTags</span></span>|<span data-ttu-id="54f94-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="54f94-145">Boolean</span></span>|<span data-ttu-id="54f94-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="54f94-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54f94-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="54f94-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54f94-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="54f94-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54f94-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54f94-149">This property is read-only.</span></span> <span data-ttu-id="54f94-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54f94-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="54f94-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54f94-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="54f94-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="54f94-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="54f94-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54f94-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="54f94-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54f94-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="54f94-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="54f94-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="54f94-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54f94-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="54f94-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54f94-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="54f94-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="54f94-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="54f94-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54f94-163">createdDateTime</span></span>|<span data-ttu-id="54f94-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54f94-164">DateTimeOffset</span></span>|<span data-ttu-id="54f94-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="54f94-165">DateTime the object was created.</span></span> <span data-ttu-id="54f94-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-167">descrição</span><span class="sxs-lookup"><span data-stu-id="54f94-167">description</span></span>|<span data-ttu-id="54f94-168">String</span><span class="sxs-lookup"><span data-stu-id="54f94-168">String</span></span>|<span data-ttu-id="54f94-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54f94-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54f94-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-171">displayName</span><span class="sxs-lookup"><span data-stu-id="54f94-171">displayName</span></span>|<span data-ttu-id="54f94-172">String</span><span class="sxs-lookup"><span data-stu-id="54f94-172">String</span></span>|<span data-ttu-id="54f94-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54f94-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54f94-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-175">versão</span><span class="sxs-lookup"><span data-stu-id="54f94-175">version</span></span>|<span data-ttu-id="54f94-176">Int32</span><span class="sxs-lookup"><span data-stu-id="54f94-176">Int32</span></span>|<span data-ttu-id="54f94-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54f94-177">Version of the device configuration.</span></span> <span data-ttu-id="54f94-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54f94-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="54f94-179">usernameSource</span></span>|[<span data-ttu-id="54f94-180">UserEmail</span><span class="sxs-lookup"><span data-stu-id="54f94-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="54f94-181">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54f94-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="54f94-182">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="54f94-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="54f94-183">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="54f94-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="54f94-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="54f94-184">usernameAADSource</span></span>|[<span data-ttu-id="54f94-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="54f94-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="54f94-186">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="54f94-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="54f94-187">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="54f94-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="54f94-188">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="54f94-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="54f94-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="54f94-189">userDomainNameSource</span></span>|[<span data-ttu-id="54f94-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="54f94-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="54f94-191">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54f94-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="54f94-192">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="54f94-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="54f94-193">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="54f94-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="54f94-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="54f94-194">customDomainName</span></span>|<span data-ttu-id="54f94-195">String</span><span class="sxs-lookup"><span data-stu-id="54f94-195">String</span></span>|<span data-ttu-id="54f94-196">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54f94-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="54f94-197">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="54f94-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="54f94-198">accountName</span><span class="sxs-lookup"><span data-stu-id="54f94-198">accountName</span></span>|<span data-ttu-id="54f94-199">String</span><span class="sxs-lookup"><span data-stu-id="54f94-199">String</span></span>|<span data-ttu-id="54f94-200">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="54f94-200">Account name.</span></span>|
|<span data-ttu-id="54f94-201">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="54f94-201">syncCalendar</span></span>|<span data-ttu-id="54f94-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="54f94-202">Boolean</span></span>|<span data-ttu-id="54f94-203">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="54f94-203">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="54f94-204">syncContacts</span><span class="sxs-lookup"><span data-stu-id="54f94-204">syncContacts</span></span>|<span data-ttu-id="54f94-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="54f94-205">Boolean</span></span>|<span data-ttu-id="54f94-206">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="54f94-206">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="54f94-207">syncTasks</span><span class="sxs-lookup"><span data-stu-id="54f94-207">syncTasks</span></span>|<span data-ttu-id="54f94-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="54f94-208">Boolean</span></span>|<span data-ttu-id="54f94-209">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="54f94-209">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="54f94-210">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="54f94-210">durationOfEmailToSync</span></span>|[<span data-ttu-id="54f94-211">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="54f94-211">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="54f94-212">Duração do email a ser sincronizado. Os valores possíveis são `userDefined`: `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`,.</span><span class="sxs-lookup"><span data-stu-id="54f94-212">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="54f94-213">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="54f94-213">emailAddressSource</span></span>|[<span data-ttu-id="54f94-214">UserEmail</span><span class="sxs-lookup"><span data-stu-id="54f94-214">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="54f94-215">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54f94-215">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="54f94-216">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="54f94-216">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="54f94-217">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="54f94-217">emailSyncSchedule</span></span>|[<span data-ttu-id="54f94-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="54f94-218">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="54f94-219">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="54f94-219">Email sync schedule.</span></span> <span data-ttu-id="54f94-220">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="54f94-220">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="54f94-221">hostName</span><span class="sxs-lookup"><span data-stu-id="54f94-221">hostName</span></span>|<span data-ttu-id="54f94-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54f94-222">String</span></span>|<span data-ttu-id="54f94-223">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="54f94-223">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="54f94-224">requireSsl</span><span class="sxs-lookup"><span data-stu-id="54f94-224">requireSsl</span></span>|<span data-ttu-id="54f94-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="54f94-225">Boolean</span></span>|<span data-ttu-id="54f94-226">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="54f94-226">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="54f94-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="54f94-227">Response</span></span>
<span data-ttu-id="54f94-228">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54f94-228">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54f94-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54f94-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="54f94-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54f94-230">Request</span></span>
<span data-ttu-id="54f94-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54f94-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1526

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="54f94-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="54f94-232">Response</span></span>
<span data-ttu-id="54f94-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54f94-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1698

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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





