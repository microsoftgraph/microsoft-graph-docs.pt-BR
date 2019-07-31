---
title: Atualizar windows81GeneralConfiguration
description: Atualizar as propriedades de um objeto windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26436c15fd71d861d3326447375ac95b2b3c9f08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974966"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="46157-103">Atualizar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="46157-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="46157-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46157-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46157-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46157-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46157-106">Atualizar as propriedades de um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46157-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46157-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46157-107">Prerequisites</span></span>
<span data-ttu-id="46157-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46157-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46157-110">Permission type</span></span>|<span data-ttu-id="46157-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46157-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46157-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46157-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46157-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46157-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46157-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46157-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46157-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46157-115">Not supported.</span></span>|
|<span data-ttu-id="46157-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46157-116">Application</span></span>|<span data-ttu-id="46157-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46157-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46157-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46157-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="46157-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46157-119">Request headers</span></span>
|<span data-ttu-id="46157-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46157-120">Header</span></span>|<span data-ttu-id="46157-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46157-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46157-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46157-122">Authorization</span></span>|<span data-ttu-id="46157-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46157-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46157-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46157-124">Accept</span></span>|<span data-ttu-id="46157-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46157-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46157-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46157-126">Request body</span></span>
<span data-ttu-id="46157-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46157-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="46157-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46157-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="46157-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46157-129">Property</span></span>|<span data-ttu-id="46157-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="46157-130">Type</span></span>|<span data-ttu-id="46157-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="46157-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46157-132">id</span><span class="sxs-lookup"><span data-stu-id="46157-132">id</span></span>|<span data-ttu-id="46157-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46157-133">String</span></span>|<span data-ttu-id="46157-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="46157-134">Key of the entity.</span></span> <span data-ttu-id="46157-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46157-136">lastModifiedDateTime</span></span>|<span data-ttu-id="46157-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46157-137">DateTimeOffset</span></span>|<span data-ttu-id="46157-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="46157-138">DateTime the object was last modified.</span></span> <span data-ttu-id="46157-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="46157-140">roleScopeTagIds</span></span>|<span data-ttu-id="46157-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="46157-141">String collection</span></span>|<span data-ttu-id="46157-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="46157-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="46157-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="46157-144">supportsScopeTags</span></span>|<span data-ttu-id="46157-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-145">Boolean</span></span>|<span data-ttu-id="46157-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="46157-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="46157-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="46157-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="46157-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="46157-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="46157-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46157-149">This property is read-only.</span></span> <span data-ttu-id="46157-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="46157-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="46157-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="46157-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="46157-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="46157-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="46157-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="46157-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="46157-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="46157-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="46157-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="46157-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="46157-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="46157-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="46157-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="46157-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="46157-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="46157-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="46157-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46157-163">createdDateTime</span></span>|<span data-ttu-id="46157-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46157-164">DateTimeOffset</span></span>|<span data-ttu-id="46157-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="46157-165">DateTime the object was created.</span></span> <span data-ttu-id="46157-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-167">descrição</span><span class="sxs-lookup"><span data-stu-id="46157-167">description</span></span>|<span data-ttu-id="46157-168">String</span><span class="sxs-lookup"><span data-stu-id="46157-168">String</span></span>|<span data-ttu-id="46157-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46157-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="46157-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-171">displayName</span><span class="sxs-lookup"><span data-stu-id="46157-171">displayName</span></span>|<span data-ttu-id="46157-172">String</span><span class="sxs-lookup"><span data-stu-id="46157-172">String</span></span>|<span data-ttu-id="46157-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46157-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="46157-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-175">versão</span><span class="sxs-lookup"><span data-stu-id="46157-175">version</span></span>|<span data-ttu-id="46157-176">Int32</span><span class="sxs-lookup"><span data-stu-id="46157-176">Int32</span></span>|<span data-ttu-id="46157-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46157-177">Version of the device configuration.</span></span> <span data-ttu-id="46157-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46157-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46157-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="46157-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="46157-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-180">Boolean</span></span>|<span data-ttu-id="46157-181">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="46157-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="46157-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="46157-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="46157-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-183">Boolean</span></span>|<span data-ttu-id="46157-184">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="46157-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="46157-185">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46157-185">This property is read-only.</span></span>|
|<span data-ttu-id="46157-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="46157-186">browserBlockAutofill</span></span>|<span data-ttu-id="46157-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-187">Boolean</span></span>|<span data-ttu-id="46157-188">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="46157-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="46157-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="46157-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="46157-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-190">Boolean</span></span>|<span data-ttu-id="46157-191">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="46157-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="46157-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="46157-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="46157-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-193">Boolean</span></span>|<span data-ttu-id="46157-194">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="46157-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="46157-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="46157-195">browserBlockJavaScript</span></span>|<span data-ttu-id="46157-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-196">Boolean</span></span>|<span data-ttu-id="46157-197">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="46157-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="46157-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="46157-198">browserBlockPlugins</span></span>|<span data-ttu-id="46157-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-199">Boolean</span></span>|<span data-ttu-id="46157-200">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="46157-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="46157-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="46157-201">browserBlockPopups</span></span>|<span data-ttu-id="46157-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-202">Boolean</span></span>|<span data-ttu-id="46157-203">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="46157-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="46157-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="46157-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="46157-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-205">Boolean</span></span>|<span data-ttu-id="46157-206">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="46157-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="46157-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="46157-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="46157-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-208">Boolean</span></span>|<span data-ttu-id="46157-209">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="46157-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="46157-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="46157-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="46157-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="46157-211">Boolean</span></span>|<span data-ttu-id="46157-212">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="46157-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="46157-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="46157-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="46157-214">String</span><span class="sxs-lookup"><span data-stu-id="46157-214">String</span></span>|<span data-ttu-id="46157-215">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="46157-215">The enterprise mode site list location.</span></span> <span data-ttu-id="46157-216">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="46157-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="46157-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="46157-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="46157-218">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="46157-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="46157-219">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="46157-219">The internet security level.</span></span> <span data-ttu-id="46157-220">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="46157-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="46157-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="46157-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="46157-222">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="46157-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="46157-223">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="46157-223">The Intranet security level.</span></span> <span data-ttu-id="46157-224">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="46157-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="46157-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="46157-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="46157-226">String</span><span class="sxs-lookup"><span data-stu-id="46157-226">String</span></span>|<span data-ttu-id="46157-227">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="46157-227">The logging report location.</span></span>|
|<span data-ttu-id="46157-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="46157-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="46157-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-229">Boolean</span></span>|<span data-ttu-id="46157-230">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="46157-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="46157-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="46157-231">browserRequireFirewall</span></span>|<span data-ttu-id="46157-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-232">Boolean</span></span>|<span data-ttu-id="46157-233">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="46157-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="46157-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="46157-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="46157-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-235">Boolean</span></span>|<span data-ttu-id="46157-236">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="46157-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="46157-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="46157-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="46157-238">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="46157-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="46157-239">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="46157-239">The trusted sites security level.</span></span> <span data-ttu-id="46157-240">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="46157-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="46157-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="46157-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="46157-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-242">Boolean</span></span>|<span data-ttu-id="46157-243">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="46157-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="46157-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="46157-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="46157-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-245">Boolean</span></span>|<span data-ttu-id="46157-246">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="46157-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="46157-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="46157-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="46157-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-248">Boolean</span></span>|<span data-ttu-id="46157-249">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="46157-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="46157-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="46157-250">passwordExpirationDays</span></span>|<span data-ttu-id="46157-251">Int32</span><span class="sxs-lookup"><span data-stu-id="46157-251">Int32</span></span>|<span data-ttu-id="46157-252">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="46157-252">Password expiration in days.</span></span>|
|<span data-ttu-id="46157-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="46157-253">passwordMinimumLength</span></span>|<span data-ttu-id="46157-254">Int32</span><span class="sxs-lookup"><span data-stu-id="46157-254">Int32</span></span>|<span data-ttu-id="46157-255">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="46157-255">The minimum password length.</span></span>|
|<span data-ttu-id="46157-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="46157-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="46157-257">Int32</span><span class="sxs-lookup"><span data-stu-id="46157-257">Int32</span></span>|<span data-ttu-id="46157-258">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="46157-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="46157-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="46157-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="46157-260">Int32</span><span class="sxs-lookup"><span data-stu-id="46157-260">Int32</span></span>|<span data-ttu-id="46157-261">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="46157-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="46157-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="46157-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="46157-263">Int32</span><span class="sxs-lookup"><span data-stu-id="46157-263">Int32</span></span>|<span data-ttu-id="46157-264">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="46157-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="46157-265">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="46157-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="46157-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="46157-266">passwordRequiredType</span></span>|[<span data-ttu-id="46157-267">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="46157-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="46157-268">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="46157-268">The required password type.</span></span> <span data-ttu-id="46157-269">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="46157-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="46157-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="46157-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="46157-271">Int32</span><span class="sxs-lookup"><span data-stu-id="46157-271">Int32</span></span>|<span data-ttu-id="46157-272">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="46157-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="46157-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="46157-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="46157-274">Booliano</span><span class="sxs-lookup"><span data-stu-id="46157-274">Boolean</span></span>|<span data-ttu-id="46157-275">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="46157-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="46157-276">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="46157-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="46157-277">updateClassification</span><span class="sxs-lookup"><span data-stu-id="46157-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="46157-278">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="46157-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="46157-279">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="46157-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="46157-280">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="46157-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="46157-281">updateClassification</span><span class="sxs-lookup"><span data-stu-id="46157-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="46157-282">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="46157-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="46157-283">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="46157-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="46157-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="46157-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="46157-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="46157-285">Boolean</span></span>|<span data-ttu-id="46157-286">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="46157-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="46157-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="46157-287">userAccountControlSettings</span></span>|[<span data-ttu-id="46157-288">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="46157-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="46157-289">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="46157-289">The user account control settings.</span></span> <span data-ttu-id="46157-290">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="46157-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="46157-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="46157-291">workFoldersUrl</span></span>|<span data-ttu-id="46157-292">String</span><span class="sxs-lookup"><span data-stu-id="46157-292">String</span></span>|<span data-ttu-id="46157-293">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="46157-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="46157-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="46157-294">Response</span></span>
<span data-ttu-id="46157-295">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46157-295">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46157-296">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46157-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="46157-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46157-297">Request</span></span>
<span data-ttu-id="46157-298">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46157-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2697

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="46157-299">Resposta</span><span class="sxs-lookup"><span data-stu-id="46157-299">Response</span></span>
<span data-ttu-id="46157-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46157-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2869

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```





