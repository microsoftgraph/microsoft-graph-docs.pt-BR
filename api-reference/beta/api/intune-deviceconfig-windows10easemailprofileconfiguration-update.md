---
title: Atualizar windows10EasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto windows10EasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba65936e593b46ea990d34a02e189eaec96cb527
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689724"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="4acbc-103">Atualizar windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="4acbc-103">Update windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="4acbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4acbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4acbc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4acbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4acbc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4acbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4acbc-107">Atualiza as propriedades de um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4acbc-107">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4acbc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4acbc-108">Prerequisites</span></span>
<span data-ttu-id="4acbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4acbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4acbc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4acbc-111">Permission type</span></span>|<span data-ttu-id="4acbc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4acbc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4acbc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4acbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4acbc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4acbc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4acbc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4acbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4acbc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4acbc-116">Not supported.</span></span>|
|<span data-ttu-id="4acbc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4acbc-117">Application</span></span>|<span data-ttu-id="4acbc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4acbc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4acbc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4acbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4acbc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4acbc-120">Request headers</span></span>
|<span data-ttu-id="4acbc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4acbc-121">Header</span></span>|<span data-ttu-id="4acbc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4acbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4acbc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4acbc-123">Authorization</span></span>|<span data-ttu-id="4acbc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4acbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4acbc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4acbc-125">Accept</span></span>|<span data-ttu-id="4acbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4acbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4acbc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4acbc-127">Request body</span></span>
<span data-ttu-id="4acbc-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4acbc-128">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="4acbc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4acbc-129">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="4acbc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4acbc-130">Property</span></span>|<span data-ttu-id="4acbc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4acbc-131">Type</span></span>|<span data-ttu-id="4acbc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4acbc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4acbc-133">id</span><span class="sxs-lookup"><span data-stu-id="4acbc-133">id</span></span>|<span data-ttu-id="4acbc-134">String</span><span class="sxs-lookup"><span data-stu-id="4acbc-134">String</span></span>|<span data-ttu-id="4acbc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4acbc-135">Key of the entity.</span></span> <span data-ttu-id="4acbc-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4acbc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4acbc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4acbc-138">DateTimeOffset</span></span>|<span data-ttu-id="4acbc-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4acbc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4acbc-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4acbc-141">roleScopeTagIds</span></span>|<span data-ttu-id="4acbc-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4acbc-142">String collection</span></span>|<span data-ttu-id="4acbc-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4acbc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4acbc-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4acbc-145">supportsScopeTags</span></span>|<span data-ttu-id="4acbc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4acbc-146">Boolean</span></span>|<span data-ttu-id="4acbc-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4acbc-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4acbc-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4acbc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4acbc-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4acbc-150">This property is read-only.</span></span> <span data-ttu-id="4acbc-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4acbc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4acbc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4acbc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4acbc-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="4acbc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4acbc-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4acbc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4acbc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4acbc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4acbc-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="4acbc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4acbc-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4acbc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4acbc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4acbc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4acbc-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="4acbc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4acbc-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4acbc-164">createdDateTime</span></span>|<span data-ttu-id="4acbc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4acbc-165">DateTimeOffset</span></span>|<span data-ttu-id="4acbc-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4acbc-166">DateTime the object was created.</span></span> <span data-ttu-id="4acbc-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-168">description</span><span class="sxs-lookup"><span data-stu-id="4acbc-168">description</span></span>|<span data-ttu-id="4acbc-169">String</span><span class="sxs-lookup"><span data-stu-id="4acbc-169">String</span></span>|<span data-ttu-id="4acbc-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4acbc-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4acbc-172">displayName</span></span>|<span data-ttu-id="4acbc-173">String</span><span class="sxs-lookup"><span data-stu-id="4acbc-173">String</span></span>|<span data-ttu-id="4acbc-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4acbc-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-176">versão</span><span class="sxs-lookup"><span data-stu-id="4acbc-176">version</span></span>|<span data-ttu-id="4acbc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4acbc-177">Int32</span></span>|<span data-ttu-id="4acbc-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-178">Version of the device configuration.</span></span> <span data-ttu-id="4acbc-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4acbc-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4acbc-180">usernameSource</span></span>|[<span data-ttu-id="4acbc-181">UserEmail</span><span class="sxs-lookup"><span data-stu-id="4acbc-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4acbc-182">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4acbc-183">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4acbc-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4acbc-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="4acbc-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4acbc-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="4acbc-185">usernameAADSource</span></span>|[<span data-ttu-id="4acbc-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4acbc-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="4acbc-187">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="4acbc-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="4acbc-188">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4acbc-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4acbc-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="4acbc-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="4acbc-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="4acbc-190">userDomainNameSource</span></span>|[<span data-ttu-id="4acbc-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="4acbc-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="4acbc-192">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4acbc-193">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4acbc-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4acbc-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="4acbc-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="4acbc-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="4acbc-195">customDomainName</span></span>|<span data-ttu-id="4acbc-196">String</span><span class="sxs-lookup"><span data-stu-id="4acbc-196">String</span></span>|<span data-ttu-id="4acbc-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="4acbc-198">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="4acbc-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="4acbc-199">accountName</span><span class="sxs-lookup"><span data-stu-id="4acbc-199">accountName</span></span>|<span data-ttu-id="4acbc-200">String</span><span class="sxs-lookup"><span data-stu-id="4acbc-200">String</span></span>|<span data-ttu-id="4acbc-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="4acbc-201">Account name.</span></span>|
|<span data-ttu-id="4acbc-202">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="4acbc-202">syncCalendar</span></span>|<span data-ttu-id="4acbc-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="4acbc-203">Boolean</span></span>|<span data-ttu-id="4acbc-204">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="4acbc-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="4acbc-205">syncContacts</span><span class="sxs-lookup"><span data-stu-id="4acbc-205">syncContacts</span></span>|<span data-ttu-id="4acbc-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4acbc-206">Boolean</span></span>|<span data-ttu-id="4acbc-207">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="4acbc-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="4acbc-208">syncTasks</span><span class="sxs-lookup"><span data-stu-id="4acbc-208">syncTasks</span></span>|<span data-ttu-id="4acbc-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4acbc-209">Boolean</span></span>|<span data-ttu-id="4acbc-210">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="4acbc-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="4acbc-211">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="4acbc-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="4acbc-212">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="4acbc-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4acbc-213">Duração do email a ser sincronizado. Os valores possíveis são: `userDefined` , `oneDay` , `threeDays` , `oneWeek` , `twoWeeks` , `oneMonth` , `unlimited` .</span><span class="sxs-lookup"><span data-stu-id="4acbc-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4acbc-214">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="4acbc-214">emailAddressSource</span></span>|[<span data-ttu-id="4acbc-215">UserEmail</span><span class="sxs-lookup"><span data-stu-id="4acbc-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4acbc-216">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4acbc-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4acbc-217">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="4acbc-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4acbc-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4acbc-218">emailSyncSchedule</span></span>|[<span data-ttu-id="4acbc-219">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4acbc-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="4acbc-220">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="4acbc-220">Email sync schedule.</span></span> <span data-ttu-id="4acbc-221">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="4acbc-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="4acbc-222">hostName</span><span class="sxs-lookup"><span data-stu-id="4acbc-222">hostName</span></span>|<span data-ttu-id="4acbc-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4acbc-223">String</span></span>|<span data-ttu-id="4acbc-224">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="4acbc-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="4acbc-225">requireSsl</span><span class="sxs-lookup"><span data-stu-id="4acbc-225">requireSsl</span></span>|<span data-ttu-id="4acbc-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="4acbc-226">Boolean</span></span>|<span data-ttu-id="4acbc-227">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="4acbc-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="4acbc-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="4acbc-228">Response</span></span>
<span data-ttu-id="4acbc-229">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4acbc-229">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4acbc-230">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4acbc-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="4acbc-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4acbc-231">Request</span></span>
<span data-ttu-id="4acbc-232">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4acbc-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4acbc-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="4acbc-233">Response</span></span>
<span data-ttu-id="4acbc-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4acbc-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





