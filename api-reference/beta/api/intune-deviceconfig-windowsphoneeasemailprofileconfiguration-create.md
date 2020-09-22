---
title: Criar windowsPhoneEASEmailProfileConfiguration
description: Criar um novo objeto windowsPhoneEASEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 361b9157f4b88644979068424b14b7eca7557180
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972361"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="05810-103">Criar windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="05810-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

<span data-ttu-id="05810-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05810-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05810-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05810-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05810-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05810-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05810-107">Criar um novo objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="05810-107">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05810-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05810-108">Prerequisites</span></span>
<span data-ttu-id="05810-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05810-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05810-111">Permission type</span></span>|<span data-ttu-id="05810-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05810-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05810-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05810-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05810-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05810-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05810-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05810-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05810-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05810-116">Not supported.</span></span>|
|<span data-ttu-id="05810-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05810-117">Application</span></span>|<span data-ttu-id="05810-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05810-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05810-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05810-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="05810-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05810-120">Request headers</span></span>
|<span data-ttu-id="05810-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05810-121">Header</span></span>|<span data-ttu-id="05810-122">Valor</span><span class="sxs-lookup"><span data-stu-id="05810-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05810-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05810-123">Authorization</span></span>|<span data-ttu-id="05810-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05810-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05810-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05810-125">Accept</span></span>|<span data-ttu-id="05810-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05810-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05810-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05810-127">Request body</span></span>
<span data-ttu-id="05810-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhoneEASEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05810-128">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="05810-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhoneEASEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05810-129">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="05810-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05810-130">Property</span></span>|<span data-ttu-id="05810-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="05810-131">Type</span></span>|<span data-ttu-id="05810-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="05810-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05810-133">id</span><span class="sxs-lookup"><span data-stu-id="05810-133">id</span></span>|<span data-ttu-id="05810-134">String</span><span class="sxs-lookup"><span data-stu-id="05810-134">String</span></span>|<span data-ttu-id="05810-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05810-135">Key of the entity.</span></span> <span data-ttu-id="05810-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05810-137">lastModifiedDateTime</span></span>|<span data-ttu-id="05810-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05810-138">DateTimeOffset</span></span>|<span data-ttu-id="05810-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="05810-139">DateTime the object was last modified.</span></span> <span data-ttu-id="05810-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="05810-141">roleScopeTagIds</span></span>|<span data-ttu-id="05810-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05810-142">String collection</span></span>|<span data-ttu-id="05810-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="05810-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="05810-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="05810-145">supportsScopeTags</span></span>|<span data-ttu-id="05810-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="05810-146">Boolean</span></span>|<span data-ttu-id="05810-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="05810-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="05810-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="05810-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="05810-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="05810-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="05810-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05810-150">This property is read-only.</span></span> <span data-ttu-id="05810-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="05810-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="05810-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="05810-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="05810-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="05810-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="05810-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="05810-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="05810-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="05810-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="05810-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="05810-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="05810-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="05810-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="05810-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="05810-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="05810-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="05810-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="05810-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05810-164">createdDateTime</span></span>|<span data-ttu-id="05810-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05810-165">DateTimeOffset</span></span>|<span data-ttu-id="05810-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="05810-166">DateTime the object was created.</span></span> <span data-ttu-id="05810-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-168">description</span><span class="sxs-lookup"><span data-stu-id="05810-168">description</span></span>|<span data-ttu-id="05810-169">String</span><span class="sxs-lookup"><span data-stu-id="05810-169">String</span></span>|<span data-ttu-id="05810-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05810-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="05810-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-172">displayName</span><span class="sxs-lookup"><span data-stu-id="05810-172">displayName</span></span>|<span data-ttu-id="05810-173">String</span><span class="sxs-lookup"><span data-stu-id="05810-173">String</span></span>|<span data-ttu-id="05810-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05810-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="05810-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-176">versão</span><span class="sxs-lookup"><span data-stu-id="05810-176">version</span></span>|<span data-ttu-id="05810-177">Int32</span><span class="sxs-lookup"><span data-stu-id="05810-177">Int32</span></span>|<span data-ttu-id="05810-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05810-178">Version of the device configuration.</span></span> <span data-ttu-id="05810-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05810-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05810-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="05810-180">usernameSource</span></span>|[<span data-ttu-id="05810-181">UserEmail</span><span class="sxs-lookup"><span data-stu-id="05810-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="05810-182">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05810-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="05810-183">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="05810-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="05810-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="05810-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="05810-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="05810-185">usernameAADSource</span></span>|[<span data-ttu-id="05810-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="05810-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="05810-187">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="05810-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="05810-188">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="05810-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="05810-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="05810-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="05810-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="05810-190">userDomainNameSource</span></span>|[<span data-ttu-id="05810-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="05810-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="05810-192">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05810-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="05810-193">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="05810-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="05810-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="05810-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="05810-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="05810-195">customDomainName</span></span>|<span data-ttu-id="05810-196">String</span><span class="sxs-lookup"><span data-stu-id="05810-196">String</span></span>|<span data-ttu-id="05810-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05810-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="05810-198">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="05810-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="05810-199">accountName</span><span class="sxs-lookup"><span data-stu-id="05810-199">accountName</span></span>|<span data-ttu-id="05810-200">String</span><span class="sxs-lookup"><span data-stu-id="05810-200">String</span></span>|<span data-ttu-id="05810-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="05810-201">Account name.</span></span>|
|<span data-ttu-id="05810-202">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="05810-202">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="05810-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="05810-203">Boolean</span></span>|<span data-ttu-id="05810-204">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="05810-204">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="05810-205">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05810-205">This property is read-only.</span></span>|
|<span data-ttu-id="05810-206">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="05810-206">syncCalendar</span></span>|<span data-ttu-id="05810-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="05810-207">Boolean</span></span>|<span data-ttu-id="05810-208">Se o calendário deve ou não ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="05810-208">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="05810-209">syncContacts</span><span class="sxs-lookup"><span data-stu-id="05810-209">syncContacts</span></span>|<span data-ttu-id="05810-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="05810-210">Boolean</span></span>|<span data-ttu-id="05810-211">Se os contatos devem ou não ser sincronizados.</span><span class="sxs-lookup"><span data-stu-id="05810-211">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="05810-212">syncTasks</span><span class="sxs-lookup"><span data-stu-id="05810-212">syncTasks</span></span>|<span data-ttu-id="05810-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="05810-213">Boolean</span></span>|<span data-ttu-id="05810-214">Se as tarefas devem ou não ser sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="05810-214">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="05810-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="05810-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="05810-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="05810-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="05810-217">Duração do email a ser sincronizado. Os valores possíveis são: `userDefined` , `oneDay` , `threeDays` , `oneWeek` , `twoWeeks` , `oneMonth` , `unlimited` .</span><span class="sxs-lookup"><span data-stu-id="05810-217">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="05810-218">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="05810-218">emailAddressSource</span></span>|[<span data-ttu-id="05810-219">UserEmail</span><span class="sxs-lookup"><span data-stu-id="05810-219">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="05810-220">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05810-220">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="05810-221">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="05810-221">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="05810-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="05810-222">emailSyncSchedule</span></span>|[<span data-ttu-id="05810-223">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="05810-223">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="05810-224">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="05810-224">Email sync schedule.</span></span> <span data-ttu-id="05810-225">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="05810-225">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="05810-226">hostName</span><span class="sxs-lookup"><span data-stu-id="05810-226">hostName</span></span>|<span data-ttu-id="05810-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05810-227">String</span></span>|<span data-ttu-id="05810-228">Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="05810-228">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="05810-229">requireSsl</span><span class="sxs-lookup"><span data-stu-id="05810-229">requireSsl</span></span>|<span data-ttu-id="05810-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="05810-230">Boolean</span></span>|<span data-ttu-id="05810-231">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="05810-231">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="05810-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="05810-232">Response</span></span>
<span data-ttu-id="05810-233">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05810-233">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05810-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05810-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="05810-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05810-235">Request</span></span>
<span data-ttu-id="05810-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05810-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="05810-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="05810-237">Response</span></span>
<span data-ttu-id="05810-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05810-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






