---
title: Atualizar windowsPhoneEASEmailProfileConfiguration
description: Atualize as propriedades de um objeto windowsPhoneEASEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45042dbccbc6ef9d465a554c8de339e9d8b6cc91
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154711"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="ce13f-103">Atualizar windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce13f-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

<span data-ttu-id="ce13f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce13f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce13f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce13f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce13f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce13f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce13f-107">Atualize as propriedades de um [objeto windowsPhoneEASEmailProfileConfiguration.](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-107">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce13f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce13f-108">Prerequisites</span></span>
<span data-ttu-id="ce13f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce13f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce13f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce13f-111">Permission type</span></span>|<span data-ttu-id="ce13f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce13f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce13f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce13f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce13f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce13f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce13f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce13f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce13f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce13f-116">Not supported.</span></span>|
|<span data-ttu-id="ce13f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce13f-117">Application</span></span>|<span data-ttu-id="ce13f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce13f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce13f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce13f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ce13f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce13f-120">Request headers</span></span>
|<span data-ttu-id="ce13f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce13f-121">Header</span></span>|<span data-ttu-id="ce13f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ce13f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce13f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce13f-123">Authorization</span></span>|<span data-ttu-id="ce13f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce13f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce13f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce13f-125">Accept</span></span>|<span data-ttu-id="ce13f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce13f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce13f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce13f-127">Request body</span></span>
<span data-ttu-id="ce13f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsPhoneEASEmailProfileConfiguration.](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-128">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="ce13f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce13f-129">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="ce13f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce13f-130">Property</span></span>|<span data-ttu-id="ce13f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce13f-131">Type</span></span>|<span data-ttu-id="ce13f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce13f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce13f-133">id</span><span class="sxs-lookup"><span data-stu-id="ce13f-133">id</span></span>|<span data-ttu-id="ce13f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce13f-134">String</span></span>|<span data-ttu-id="ce13f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ce13f-135">Key of the entity.</span></span> <span data-ttu-id="ce13f-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce13f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ce13f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce13f-138">DateTimeOffset</span></span>|<span data-ttu-id="ce13f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ce13f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ce13f-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce13f-141">roleScopeTagIds</span></span>|<span data-ttu-id="ce13f-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce13f-142">String collection</span></span>|<span data-ttu-id="ce13f-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="ce13f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce13f-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ce13f-145">supportsScopeTags</span></span>|<span data-ttu-id="ce13f-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="ce13f-146">Boolean</span></span>|<span data-ttu-id="ce13f-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce13f-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce13f-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ce13f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce13f-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce13f-150">This property is read-only.</span></span> <span data-ttu-id="ce13f-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce13f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ce13f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce13f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ce13f-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ce13f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ce13f-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce13f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ce13f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce13f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ce13f-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ce13f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ce13f-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce13f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ce13f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce13f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ce13f-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ce13f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ce13f-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce13f-164">createdDateTime</span></span>|<span data-ttu-id="ce13f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce13f-165">DateTimeOffset</span></span>|<span data-ttu-id="ce13f-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ce13f-166">DateTime the object was created.</span></span> <span data-ttu-id="ce13f-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-168">descrição</span><span class="sxs-lookup"><span data-stu-id="ce13f-168">description</span></span>|<span data-ttu-id="ce13f-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce13f-169">String</span></span>|<span data-ttu-id="ce13f-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce13f-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ce13f-172">displayName</span></span>|<span data-ttu-id="ce13f-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce13f-173">String</span></span>|<span data-ttu-id="ce13f-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce13f-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-176">versão</span><span class="sxs-lookup"><span data-stu-id="ce13f-176">version</span></span>|<span data-ttu-id="ce13f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ce13f-177">Int32</span></span>|<span data-ttu-id="ce13f-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-178">Version of the device configuration.</span></span> <span data-ttu-id="ce13f-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce13f-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ce13f-180">usernameSource</span></span>|[<span data-ttu-id="ce13f-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ce13f-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ce13f-182">Atributo username que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ce13f-183">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ce13f-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ce13f-184">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ce13f-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ce13f-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="ce13f-185">usernameAADSource</span></span>|[<span data-ttu-id="ce13f-186">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ce13f-186">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="ce13f-187">Nome do campo AAD, que será usado para recuperar UserName para perfil de email.</span><span class="sxs-lookup"><span data-stu-id="ce13f-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="ce13f-188">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ce13f-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ce13f-189">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="ce13f-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="ce13f-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="ce13f-190">userDomainNameSource</span></span>|[<span data-ttu-id="ce13f-191">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="ce13f-191">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="ce13f-192">Atributo UserDomainname que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ce13f-193">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ce13f-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ce13f-194">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="ce13f-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="ce13f-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="ce13f-195">customDomainName</span></span>|<span data-ttu-id="ce13f-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce13f-196">String</span></span>|<span data-ttu-id="ce13f-197">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="ce13f-198">Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="ce13f-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="ce13f-199">accountName</span><span class="sxs-lookup"><span data-stu-id="ce13f-199">accountName</span></span>|<span data-ttu-id="ce13f-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce13f-200">String</span></span>|<span data-ttu-id="ce13f-201">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="ce13f-201">Account name.</span></span>|
|<span data-ttu-id="ce13f-202">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="ce13f-202">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="ce13f-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce13f-203">Boolean</span></span>|<span data-ttu-id="ce13f-204">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="ce13f-204">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ce13f-205">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce13f-205">This property is read-only.</span></span>|
|<span data-ttu-id="ce13f-206">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="ce13f-206">syncCalendar</span></span>|<span data-ttu-id="ce13f-207">Booleano</span><span class="sxs-lookup"><span data-stu-id="ce13f-207">Boolean</span></span>|<span data-ttu-id="ce13f-208">Se deve ou não sincronizar o calendário.</span><span class="sxs-lookup"><span data-stu-id="ce13f-208">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="ce13f-209">syncContacts</span><span class="sxs-lookup"><span data-stu-id="ce13f-209">syncContacts</span></span>|<span data-ttu-id="ce13f-210">Booleano</span><span class="sxs-lookup"><span data-stu-id="ce13f-210">Boolean</span></span>|<span data-ttu-id="ce13f-211">Se deve ou não sincronizar contatos.</span><span class="sxs-lookup"><span data-stu-id="ce13f-211">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="ce13f-212">syncTasks</span><span class="sxs-lookup"><span data-stu-id="ce13f-212">syncTasks</span></span>|<span data-ttu-id="ce13f-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="ce13f-213">Boolean</span></span>|<span data-ttu-id="ce13f-214">Se deve ou não sincronizar tarefas.</span><span class="sxs-lookup"><span data-stu-id="ce13f-214">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="ce13f-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="ce13f-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="ce13f-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="ce13f-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="ce13f-217">Duração do email para sincronização. Os valores possíveis `userDefined` são: `oneDay` , , , , , , `threeDays` `oneWeek` `twoWeeks` `oneMonth` `unlimited` .</span><span class="sxs-lookup"><span data-stu-id="ce13f-217">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="ce13f-218">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="ce13f-218">emailAddressSource</span></span>|[<span data-ttu-id="ce13f-219">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ce13f-219">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ce13f-220">Atributo de email que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce13f-220">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ce13f-221">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ce13f-221">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ce13f-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="ce13f-222">emailSyncSchedule</span></span>|[<span data-ttu-id="ce13f-223">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="ce13f-223">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="ce13f-224">Agendamento de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="ce13f-224">Email sync schedule.</span></span> <span data-ttu-id="ce13f-225">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="ce13f-225">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="ce13f-226">hostName</span><span class="sxs-lookup"><span data-stu-id="ce13f-226">hostName</span></span>|<span data-ttu-id="ce13f-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce13f-227">String</span></span>|<span data-ttu-id="ce13f-228">Local do Exchange que (URL) ao que o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="ce13f-228">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="ce13f-229">requireSsl</span><span class="sxs-lookup"><span data-stu-id="ce13f-229">requireSsl</span></span>|<span data-ttu-id="ce13f-230">Booleano</span><span class="sxs-lookup"><span data-stu-id="ce13f-230">Boolean</span></span>|<span data-ttu-id="ce13f-231">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="ce13f-231">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="ce13f-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce13f-232">Response</span></span>
<span data-ttu-id="ce13f-233">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce13f-233">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce13f-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce13f-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce13f-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce13f-235">Request</span></span>
<span data-ttu-id="ce13f-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce13f-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce13f-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce13f-237">Response</span></span>
<span data-ttu-id="ce13f-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce13f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




