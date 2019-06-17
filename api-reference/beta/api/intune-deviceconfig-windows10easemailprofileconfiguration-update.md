---
title: Atualizar windows10EasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto windows10EasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c50ec850aa99770b4a7d036bdf9f5bf7092548f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962705"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="25977-103">Atualizar windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="25977-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="25977-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25977-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25977-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25977-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25977-106">Atualiza as propriedades de um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="25977-106">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25977-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25977-107">Prerequisites</span></span>
<span data-ttu-id="25977-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25977-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25977-110">Permission type</span></span>|<span data-ttu-id="25977-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25977-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25977-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25977-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25977-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25977-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25977-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25977-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25977-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25977-115">Not supported.</span></span>|
|<span data-ttu-id="25977-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25977-116">Application</span></span>|<span data-ttu-id="25977-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25977-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25977-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25977-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="25977-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25977-119">Request headers</span></span>
|<span data-ttu-id="25977-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25977-120">Header</span></span>|<span data-ttu-id="25977-121">Valor</span><span class="sxs-lookup"><span data-stu-id="25977-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25977-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="25977-122">Authorization</span></span>|<span data-ttu-id="25977-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25977-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25977-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25977-124">Accept</span></span>|<span data-ttu-id="25977-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25977-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25977-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25977-126">Request body</span></span>
<span data-ttu-id="25977-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="25977-127">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="25977-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25977-128">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="25977-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25977-129">Property</span></span>|<span data-ttu-id="25977-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="25977-130">Type</span></span>|<span data-ttu-id="25977-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="25977-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25977-132">id</span><span class="sxs-lookup"><span data-stu-id="25977-132">id</span></span>|<span data-ttu-id="25977-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25977-133">String</span></span>|<span data-ttu-id="25977-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25977-134">Key of the entity.</span></span> <span data-ttu-id="25977-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25977-136">lastModifiedDateTime</span></span>|<span data-ttu-id="25977-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25977-137">DateTimeOffset</span></span>|<span data-ttu-id="25977-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="25977-138">DateTime the object was last modified.</span></span> <span data-ttu-id="25977-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="25977-140">roleScopeTagIds</span></span>|<span data-ttu-id="25977-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="25977-141">String collection</span></span>|<span data-ttu-id="25977-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="25977-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="25977-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="25977-144">supportsScopeTags</span></span>|<span data-ttu-id="25977-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="25977-145">Boolean</span></span>|<span data-ttu-id="25977-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="25977-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="25977-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="25977-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="25977-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="25977-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="25977-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25977-149">This property is read-only.</span></span> <span data-ttu-id="25977-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="25977-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="25977-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="25977-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="25977-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="25977-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="25977-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="25977-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="25977-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="25977-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="25977-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="25977-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="25977-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="25977-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="25977-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="25977-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="25977-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="25977-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="25977-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25977-163">createdDateTime</span></span>|<span data-ttu-id="25977-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25977-164">DateTimeOffset</span></span>|<span data-ttu-id="25977-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="25977-165">DateTime the object was created.</span></span> <span data-ttu-id="25977-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-167">descrição</span><span class="sxs-lookup"><span data-stu-id="25977-167">description</span></span>|<span data-ttu-id="25977-168">String</span><span class="sxs-lookup"><span data-stu-id="25977-168">String</span></span>|<span data-ttu-id="25977-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25977-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="25977-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-171">displayName</span><span class="sxs-lookup"><span data-stu-id="25977-171">displayName</span></span>|<span data-ttu-id="25977-172">String</span><span class="sxs-lookup"><span data-stu-id="25977-172">String</span></span>|<span data-ttu-id="25977-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25977-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="25977-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-175">versão</span><span class="sxs-lookup"><span data-stu-id="25977-175">version</span></span>|<span data-ttu-id="25977-176">Int32</span><span class="sxs-lookup"><span data-stu-id="25977-176">Int32</span></span>|<span data-ttu-id="25977-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25977-177">Version of the device configuration.</span></span> <span data-ttu-id="25977-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25977-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25977-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="25977-179">usernameSource</span></span>|[<span data-ttu-id="25977-180">UserEmail</span><span class="sxs-lookup"><span data-stu-id="25977-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="25977-181">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25977-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="25977-182">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="25977-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="25977-183">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="25977-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="25977-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="25977-184">usernameAADSource</span></span>|[<span data-ttu-id="25977-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="25977-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="25977-186">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="25977-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="25977-187">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="25977-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="25977-188">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="25977-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="25977-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="25977-189">userDomainNameSource</span></span>|[<span data-ttu-id="25977-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="25977-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="25977-191">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25977-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="25977-192">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="25977-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="25977-193">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="25977-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="25977-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="25977-194">customDomainName</span></span>|<span data-ttu-id="25977-195">String</span><span class="sxs-lookup"><span data-stu-id="25977-195">String</span></span>|<span data-ttu-id="25977-196">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25977-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="25977-197">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="25977-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="25977-198">accountName</span><span class="sxs-lookup"><span data-stu-id="25977-198">accountName</span></span>|<span data-ttu-id="25977-199">String</span><span class="sxs-lookup"><span data-stu-id="25977-199">String</span></span>|<span data-ttu-id="25977-200">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="25977-200">Account name.</span></span>|
|<span data-ttu-id="25977-201">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="25977-201">syncCalendar</span></span>|<span data-ttu-id="25977-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="25977-202">Boolean</span></span>|<span data-ttu-id="25977-203">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="25977-203">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="25977-204">syncContacts</span><span class="sxs-lookup"><span data-stu-id="25977-204">syncContacts</span></span>|<span data-ttu-id="25977-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="25977-205">Boolean</span></span>|<span data-ttu-id="25977-206">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="25977-206">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="25977-207">syncTasks</span><span class="sxs-lookup"><span data-stu-id="25977-207">syncTasks</span></span>|<span data-ttu-id="25977-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="25977-208">Boolean</span></span>|<span data-ttu-id="25977-209">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="25977-209">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="25977-210">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="25977-210">durationOfEmailToSync</span></span>|[<span data-ttu-id="25977-211">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="25977-211">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="25977-212">Duração do email a ser sincronizado. Os valores possíveis são `userDefined`: `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`,.</span><span class="sxs-lookup"><span data-stu-id="25977-212">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="25977-213">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="25977-213">emailAddressSource</span></span>|[<span data-ttu-id="25977-214">UserEmail</span><span class="sxs-lookup"><span data-stu-id="25977-214">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="25977-215">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25977-215">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="25977-216">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="25977-216">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="25977-217">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="25977-217">emailSyncSchedule</span></span>|[<span data-ttu-id="25977-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="25977-218">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="25977-219">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="25977-219">Email sync schedule.</span></span> <span data-ttu-id="25977-220">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="25977-220">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="25977-221">hostName</span><span class="sxs-lookup"><span data-stu-id="25977-221">hostName</span></span>|<span data-ttu-id="25977-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25977-222">String</span></span>|<span data-ttu-id="25977-223">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="25977-223">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="25977-224">requireSsl</span><span class="sxs-lookup"><span data-stu-id="25977-224">requireSsl</span></span>|<span data-ttu-id="25977-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="25977-225">Boolean</span></span>|<span data-ttu-id="25977-226">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="25977-226">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="25977-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="25977-227">Response</span></span>
<span data-ttu-id="25977-228">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25977-228">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25977-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25977-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="25977-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25977-230">Request</span></span>
<span data-ttu-id="25977-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25977-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="25977-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="25977-232">Response</span></span>
<span data-ttu-id="25977-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25977-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





