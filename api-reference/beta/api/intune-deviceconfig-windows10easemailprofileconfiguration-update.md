---
title: Atualizar windows10EasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto windows10EasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05d2d8451e7c635ed14dcd327223b11e05172de1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230321"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="00809-103">Atualizar windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="00809-103">Update windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="00809-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00809-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00809-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00809-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00809-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00809-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00809-107">Atualiza as propriedades de um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="00809-107">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00809-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00809-108">Prerequisites</span></span>
<span data-ttu-id="00809-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00809-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00809-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00809-111">Permission type</span></span>|<span data-ttu-id="00809-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00809-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00809-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00809-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00809-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00809-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00809-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00809-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00809-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00809-116">Not supported.</span></span>|
|<span data-ttu-id="00809-117">Application</span><span class="sxs-lookup"><span data-stu-id="00809-117">Application</span></span>|<span data-ttu-id="00809-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00809-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00809-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00809-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="00809-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00809-120">Request headers</span></span>
|<span data-ttu-id="00809-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00809-121">Header</span></span>|<span data-ttu-id="00809-122">Valor</span><span class="sxs-lookup"><span data-stu-id="00809-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00809-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="00809-123">Authorization</span></span>|<span data-ttu-id="00809-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00809-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00809-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00809-125">Accept</span></span>|<span data-ttu-id="00809-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00809-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00809-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00809-127">Request body</span></span>
<span data-ttu-id="00809-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="00809-128">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="00809-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00809-129">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="00809-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00809-130">Property</span></span>|<span data-ttu-id="00809-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="00809-131">Type</span></span>|<span data-ttu-id="00809-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="00809-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00809-133">id</span><span class="sxs-lookup"><span data-stu-id="00809-133">id</span></span>|<span data-ttu-id="00809-134">String</span><span class="sxs-lookup"><span data-stu-id="00809-134">String</span></span>|<span data-ttu-id="00809-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="00809-135">Key of the entity.</span></span> <span data-ttu-id="00809-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00809-137">lastModifiedDateTime</span></span>|<span data-ttu-id="00809-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00809-138">DateTimeOffset</span></span>|<span data-ttu-id="00809-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="00809-139">DateTime the object was last modified.</span></span> <span data-ttu-id="00809-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00809-141">roleScopeTagIds</span></span>|<span data-ttu-id="00809-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="00809-142">String collection</span></span>|<span data-ttu-id="00809-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="00809-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="00809-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="00809-145">supportsScopeTags</span></span>|<span data-ttu-id="00809-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="00809-146">Boolean</span></span>|<span data-ttu-id="00809-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="00809-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="00809-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="00809-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="00809-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="00809-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="00809-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00809-150">This property is read-only.</span></span> <span data-ttu-id="00809-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="00809-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="00809-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="00809-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="00809-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="00809-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="00809-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="00809-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="00809-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="00809-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="00809-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="00809-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="00809-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="00809-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="00809-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="00809-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="00809-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="00809-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="00809-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00809-164">createdDateTime</span></span>|<span data-ttu-id="00809-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00809-165">DateTimeOffset</span></span>|<span data-ttu-id="00809-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="00809-166">DateTime the object was created.</span></span> <span data-ttu-id="00809-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-168">description</span><span class="sxs-lookup"><span data-stu-id="00809-168">description</span></span>|<span data-ttu-id="00809-169">String</span><span class="sxs-lookup"><span data-stu-id="00809-169">String</span></span>|<span data-ttu-id="00809-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00809-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00809-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-172">displayName</span><span class="sxs-lookup"><span data-stu-id="00809-172">displayName</span></span>|<span data-ttu-id="00809-173">String</span><span class="sxs-lookup"><span data-stu-id="00809-173">String</span></span>|<span data-ttu-id="00809-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00809-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00809-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-176">versão</span><span class="sxs-lookup"><span data-stu-id="00809-176">version</span></span>|<span data-ttu-id="00809-177">Int32</span><span class="sxs-lookup"><span data-stu-id="00809-177">Int32</span></span>|<span data-ttu-id="00809-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00809-178">Version of the device configuration.</span></span> <span data-ttu-id="00809-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00809-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00809-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="00809-180">usernameSource</span></span>|[<span data-ttu-id="00809-181">UserEmail</span><span class="sxs-lookup"><span data-stu-id="00809-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="00809-182">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00809-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00809-183">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00809-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00809-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="00809-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="00809-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="00809-185">usernameAADSource</span></span>|[<span data-ttu-id="00809-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="00809-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="00809-187">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="00809-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="00809-188">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00809-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00809-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="00809-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="00809-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="00809-190">userDomainNameSource</span></span>|[<span data-ttu-id="00809-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="00809-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="00809-192">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00809-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00809-193">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00809-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00809-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="00809-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="00809-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="00809-195">customDomainName</span></span>|<span data-ttu-id="00809-196">String</span><span class="sxs-lookup"><span data-stu-id="00809-196">String</span></span>|<span data-ttu-id="00809-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00809-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="00809-198">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="00809-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="00809-199">accountName</span><span class="sxs-lookup"><span data-stu-id="00809-199">accountName</span></span>|<span data-ttu-id="00809-200">String</span><span class="sxs-lookup"><span data-stu-id="00809-200">String</span></span>|<span data-ttu-id="00809-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="00809-201">Account name.</span></span>|
|<span data-ttu-id="00809-202">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="00809-202">syncCalendar</span></span>|<span data-ttu-id="00809-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="00809-203">Boolean</span></span>|<span data-ttu-id="00809-204">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="00809-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="00809-205">syncContacts</span><span class="sxs-lookup"><span data-stu-id="00809-205">syncContacts</span></span>|<span data-ttu-id="00809-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="00809-206">Boolean</span></span>|<span data-ttu-id="00809-207">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="00809-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="00809-208">syncTasks</span><span class="sxs-lookup"><span data-stu-id="00809-208">syncTasks</span></span>|<span data-ttu-id="00809-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="00809-209">Boolean</span></span>|<span data-ttu-id="00809-210">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="00809-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="00809-211">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="00809-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="00809-212">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="00809-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="00809-213">Duração do email a ser sincronizado. Os valores possíveis são: `userDefined` , `oneDay` , `threeDays` , `oneWeek` , `twoWeeks` , `oneMonth` , `unlimited` .</span><span class="sxs-lookup"><span data-stu-id="00809-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="00809-214">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="00809-214">emailAddressSource</span></span>|[<span data-ttu-id="00809-215">UserEmail</span><span class="sxs-lookup"><span data-stu-id="00809-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="00809-216">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00809-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00809-217">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="00809-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="00809-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="00809-218">emailSyncSchedule</span></span>|[<span data-ttu-id="00809-219">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="00809-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="00809-220">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="00809-220">Email sync schedule.</span></span> <span data-ttu-id="00809-221">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="00809-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="00809-222">hostName</span><span class="sxs-lookup"><span data-stu-id="00809-222">hostName</span></span>|<span data-ttu-id="00809-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00809-223">String</span></span>|<span data-ttu-id="00809-224">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="00809-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="00809-225">requireSsl</span><span class="sxs-lookup"><span data-stu-id="00809-225">requireSsl</span></span>|<span data-ttu-id="00809-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="00809-226">Boolean</span></span>|<span data-ttu-id="00809-227">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="00809-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="00809-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="00809-228">Response</span></span>
<span data-ttu-id="00809-229">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00809-229">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00809-230">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00809-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="00809-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00809-231">Request</span></span>
<span data-ttu-id="00809-232">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00809-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00809-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="00809-233">Response</span></span>
<span data-ttu-id="00809-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00809-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




