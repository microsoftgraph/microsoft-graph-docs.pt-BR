---
title: Atualizar windowsPhoneEASEmailProfileConfiguration
description: Atualiza as propriedades de um objeto windowsPhoneEASEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4822f8594c6f5100d57b5ae80d8f5822c459361
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338277"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="dd532-103">Atualizar windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd532-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="dd532-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd532-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd532-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd532-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd532-106">Atualiza as propriedades de um objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dd532-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd532-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd532-107">Prerequisites</span></span>
<span data-ttu-id="dd532-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd532-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd532-110">Permission type</span></span>|<span data-ttu-id="dd532-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd532-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd532-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd532-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd532-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd532-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd532-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd532-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd532-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd532-115">Not supported.</span></span>|
|<span data-ttu-id="dd532-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd532-116">Application</span></span>|<span data-ttu-id="dd532-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd532-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd532-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd532-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dd532-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd532-119">Request headers</span></span>
|<span data-ttu-id="dd532-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd532-120">Header</span></span>|<span data-ttu-id="dd532-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dd532-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd532-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd532-122">Authorization</span></span>|<span data-ttu-id="dd532-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd532-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd532-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd532-124">Accept</span></span>|<span data-ttu-id="dd532-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd532-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd532-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd532-126">Request body</span></span>
<span data-ttu-id="dd532-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dd532-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="dd532-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd532-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="dd532-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd532-129">Property</span></span>|<span data-ttu-id="dd532-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd532-130">Type</span></span>|<span data-ttu-id="dd532-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd532-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd532-132">id</span><span class="sxs-lookup"><span data-stu-id="dd532-132">id</span></span>|<span data-ttu-id="dd532-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd532-133">String</span></span>|<span data-ttu-id="dd532-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dd532-134">Key of the entity.</span></span> <span data-ttu-id="dd532-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd532-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dd532-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd532-137">DateTimeOffset</span></span>|<span data-ttu-id="dd532-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="dd532-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dd532-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd532-140">roleScopeTagIds</span></span>|<span data-ttu-id="dd532-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd532-141">String collection</span></span>|<span data-ttu-id="dd532-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="dd532-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dd532-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dd532-144">supportsScopeTags</span></span>|<span data-ttu-id="dd532-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd532-145">Boolean</span></span>|<span data-ttu-id="dd532-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="dd532-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dd532-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="dd532-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dd532-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="dd532-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dd532-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd532-149">This property is read-only.</span></span> <span data-ttu-id="dd532-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dd532-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="dd532-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dd532-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="dd532-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="dd532-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="dd532-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dd532-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="dd532-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dd532-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="dd532-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="dd532-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="dd532-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dd532-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="dd532-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dd532-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="dd532-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="dd532-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="dd532-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd532-163">createdDateTime</span></span>|<span data-ttu-id="dd532-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd532-164">DateTimeOffset</span></span>|<span data-ttu-id="dd532-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="dd532-165">DateTime the object was created.</span></span> <span data-ttu-id="dd532-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-167">descrição</span><span class="sxs-lookup"><span data-stu-id="dd532-167">description</span></span>|<span data-ttu-id="dd532-168">String</span><span class="sxs-lookup"><span data-stu-id="dd532-168">String</span></span>|<span data-ttu-id="dd532-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dd532-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd532-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-171">displayName</span><span class="sxs-lookup"><span data-stu-id="dd532-171">displayName</span></span>|<span data-ttu-id="dd532-172">String</span><span class="sxs-lookup"><span data-stu-id="dd532-172">String</span></span>|<span data-ttu-id="dd532-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dd532-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd532-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-175">versão</span><span class="sxs-lookup"><span data-stu-id="dd532-175">version</span></span>|<span data-ttu-id="dd532-176">Int32</span><span class="sxs-lookup"><span data-stu-id="dd532-176">Int32</span></span>|<span data-ttu-id="dd532-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dd532-177">Version of the device configuration.</span></span> <span data-ttu-id="dd532-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd532-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="dd532-179">usernameSource</span></span>|[<span data-ttu-id="dd532-180">UserEmail</span><span class="sxs-lookup"><span data-stu-id="dd532-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="dd532-181">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dd532-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="dd532-182">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="dd532-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="dd532-183">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="dd532-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="dd532-184">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="dd532-184">usernameAADSource</span></span>|[<span data-ttu-id="dd532-185">usernameSource</span><span class="sxs-lookup"><span data-stu-id="dd532-185">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="dd532-186">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="dd532-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="dd532-187">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="dd532-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="dd532-188">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="dd532-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="dd532-189">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="dd532-189">userDomainNameSource</span></span>|[<span data-ttu-id="dd532-190">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="dd532-190">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="dd532-191">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dd532-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="dd532-192">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="dd532-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="dd532-193">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="dd532-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="dd532-194">customDomainName</span><span class="sxs-lookup"><span data-stu-id="dd532-194">customDomainName</span></span>|<span data-ttu-id="dd532-195">String</span><span class="sxs-lookup"><span data-stu-id="dd532-195">String</span></span>|<span data-ttu-id="dd532-196">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dd532-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="dd532-197">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="dd532-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="dd532-198">accountName</span><span class="sxs-lookup"><span data-stu-id="dd532-198">accountName</span></span>|<span data-ttu-id="dd532-199">String</span><span class="sxs-lookup"><span data-stu-id="dd532-199">String</span></span>|<span data-ttu-id="dd532-200">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="dd532-200">Account name.</span></span>|
|<span data-ttu-id="dd532-201">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="dd532-201">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="dd532-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd532-202">Boolean</span></span>|<span data-ttu-id="dd532-203">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="dd532-203">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="dd532-204">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd532-204">This property is read-only.</span></span>|
|<span data-ttu-id="dd532-205">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="dd532-205">syncCalendar</span></span>|<span data-ttu-id="dd532-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd532-206">Boolean</span></span>|<span data-ttu-id="dd532-207">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="dd532-207">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="dd532-208">syncContacts</span><span class="sxs-lookup"><span data-stu-id="dd532-208">syncContacts</span></span>|<span data-ttu-id="dd532-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd532-209">Boolean</span></span>|<span data-ttu-id="dd532-210">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="dd532-210">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="dd532-211">syncTasks</span><span class="sxs-lookup"><span data-stu-id="dd532-211">syncTasks</span></span>|<span data-ttu-id="dd532-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd532-212">Boolean</span></span>|<span data-ttu-id="dd532-213">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="dd532-213">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="dd532-214">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="dd532-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="dd532-215">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="dd532-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="dd532-216">Duração do email a ser sincronizado. Os valores possíveis são `userDefined`: `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`,.</span><span class="sxs-lookup"><span data-stu-id="dd532-216">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="dd532-217">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="dd532-217">emailAddressSource</span></span>|[<span data-ttu-id="dd532-218">UserEmail</span><span class="sxs-lookup"><span data-stu-id="dd532-218">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="dd532-219">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dd532-219">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="dd532-220">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="dd532-220">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="dd532-221">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="dd532-221">emailSyncSchedule</span></span>|[<span data-ttu-id="dd532-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="dd532-222">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="dd532-223">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="dd532-223">Email sync schedule.</span></span> <span data-ttu-id="dd532-224">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="dd532-224">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="dd532-225">hostName</span><span class="sxs-lookup"><span data-stu-id="dd532-225">hostName</span></span>|<span data-ttu-id="dd532-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd532-226">String</span></span>|<span data-ttu-id="dd532-227">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="dd532-227">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="dd532-228">requireSsl</span><span class="sxs-lookup"><span data-stu-id="dd532-228">requireSsl</span></span>|<span data-ttu-id="dd532-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd532-229">Boolean</span></span>|<span data-ttu-id="dd532-230">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="dd532-230">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="dd532-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd532-231">Response</span></span>
<span data-ttu-id="dd532-232">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd532-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd532-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd532-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd532-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd532-234">Request</span></span>
<span data-ttu-id="dd532-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd532-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1567

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="dd532-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd532-236">Response</span></span>
<span data-ttu-id="dd532-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd532-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1739

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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






