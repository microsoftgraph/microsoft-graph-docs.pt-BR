---
title: Criar windows81GeneralConfiguration
description: Criar um novo objeto windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 062c38d95da5187699fa40278557464562d4ba47
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187216"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="84a41-103">Criar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a41-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="84a41-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84a41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84a41-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84a41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84a41-106">Criar um novo objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84a41-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84a41-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84a41-107">Prerequisites</span></span>
<span data-ttu-id="84a41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84a41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84a41-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84a41-110">Permission type</span></span>|<span data-ttu-id="84a41-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84a41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84a41-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84a41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84a41-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a41-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84a41-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84a41-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84a41-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84a41-115">Not supported.</span></span>|
|<span data-ttu-id="84a41-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84a41-116">Application</span></span>|<span data-ttu-id="84a41-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a41-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84a41-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84a41-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84a41-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84a41-119">Request headers</span></span>
|<span data-ttu-id="84a41-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84a41-120">Header</span></span>|<span data-ttu-id="84a41-121">Valor</span><span class="sxs-lookup"><span data-stu-id="84a41-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84a41-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="84a41-122">Authorization</span></span>|<span data-ttu-id="84a41-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84a41-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84a41-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84a41-124">Accept</span></span>|<span data-ttu-id="84a41-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84a41-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84a41-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84a41-126">Request body</span></span>
<span data-ttu-id="84a41-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84a41-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="84a41-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84a41-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="84a41-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84a41-129">Property</span></span>|<span data-ttu-id="84a41-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="84a41-130">Type</span></span>|<span data-ttu-id="84a41-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="84a41-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84a41-132">id</span><span class="sxs-lookup"><span data-stu-id="84a41-132">id</span></span>|<span data-ttu-id="84a41-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a41-133">String</span></span>|<span data-ttu-id="84a41-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="84a41-134">Key of the entity.</span></span> <span data-ttu-id="84a41-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84a41-136">lastModifiedDateTime</span></span>|<span data-ttu-id="84a41-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84a41-137">DateTimeOffset</span></span>|<span data-ttu-id="84a41-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="84a41-138">DateTime the object was last modified.</span></span> <span data-ttu-id="84a41-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84a41-140">roleScopeTagIds</span></span>|<span data-ttu-id="84a41-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="84a41-141">String collection</span></span>|<span data-ttu-id="84a41-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="84a41-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84a41-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84a41-144">supportsScopeTags</span></span>|<span data-ttu-id="84a41-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-145">Boolean</span></span>|<span data-ttu-id="84a41-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="84a41-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84a41-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="84a41-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84a41-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="84a41-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84a41-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84a41-149">This property is read-only.</span></span> <span data-ttu-id="84a41-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="84a41-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="84a41-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="84a41-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="84a41-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="84a41-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="84a41-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="84a41-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="84a41-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="84a41-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="84a41-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="84a41-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="84a41-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="84a41-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="84a41-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="84a41-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="84a41-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="84a41-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="84a41-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84a41-163">createdDateTime</span></span>|<span data-ttu-id="84a41-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84a41-164">DateTimeOffset</span></span>|<span data-ttu-id="84a41-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="84a41-165">DateTime the object was created.</span></span> <span data-ttu-id="84a41-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-167">descrição</span><span class="sxs-lookup"><span data-stu-id="84a41-167">description</span></span>|<span data-ttu-id="84a41-168">String</span><span class="sxs-lookup"><span data-stu-id="84a41-168">String</span></span>|<span data-ttu-id="84a41-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84a41-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84a41-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-171">displayName</span><span class="sxs-lookup"><span data-stu-id="84a41-171">displayName</span></span>|<span data-ttu-id="84a41-172">String</span><span class="sxs-lookup"><span data-stu-id="84a41-172">String</span></span>|<span data-ttu-id="84a41-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84a41-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84a41-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-175">versão</span><span class="sxs-lookup"><span data-stu-id="84a41-175">version</span></span>|<span data-ttu-id="84a41-176">Int32</span><span class="sxs-lookup"><span data-stu-id="84a41-176">Int32</span></span>|<span data-ttu-id="84a41-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84a41-177">Version of the device configuration.</span></span> <span data-ttu-id="84a41-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84a41-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84a41-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="84a41-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="84a41-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-180">Boolean</span></span>|<span data-ttu-id="84a41-181">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="84a41-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="84a41-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="84a41-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="84a41-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-183">Boolean</span></span>|<span data-ttu-id="84a41-184">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="84a41-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="84a41-185">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84a41-185">This property is read-only.</span></span>|
|<span data-ttu-id="84a41-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="84a41-186">browserBlockAutofill</span></span>|<span data-ttu-id="84a41-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-187">Boolean</span></span>|<span data-ttu-id="84a41-188">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84a41-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="84a41-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="84a41-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="84a41-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-190">Boolean</span></span>|<span data-ttu-id="84a41-191">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="84a41-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="84a41-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="84a41-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="84a41-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-193">Boolean</span></span>|<span data-ttu-id="84a41-194">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84a41-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="84a41-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="84a41-195">browserBlockJavaScript</span></span>|<span data-ttu-id="84a41-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-196">Boolean</span></span>|<span data-ttu-id="84a41-197">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="84a41-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="84a41-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="84a41-198">browserBlockPlugins</span></span>|<span data-ttu-id="84a41-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-199">Boolean</span></span>|<span data-ttu-id="84a41-200">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="84a41-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="84a41-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="84a41-201">browserBlockPopups</span></span>|<span data-ttu-id="84a41-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-202">Boolean</span></span>|<span data-ttu-id="84a41-203">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="84a41-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="84a41-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="84a41-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="84a41-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-205">Boolean</span></span>|<span data-ttu-id="84a41-206">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="84a41-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="84a41-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="84a41-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="84a41-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-208">Boolean</span></span>|<span data-ttu-id="84a41-209">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="84a41-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="84a41-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="84a41-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="84a41-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a41-211">Boolean</span></span>|<span data-ttu-id="84a41-212">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="84a41-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="84a41-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="84a41-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="84a41-214">String</span><span class="sxs-lookup"><span data-stu-id="84a41-214">String</span></span>|<span data-ttu-id="84a41-215">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="84a41-215">The enterprise mode site list location.</span></span> <span data-ttu-id="84a41-216">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="84a41-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="84a41-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="84a41-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="84a41-218">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="84a41-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="84a41-219">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="84a41-219">The internet security level.</span></span> <span data-ttu-id="84a41-220">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="84a41-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="84a41-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="84a41-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="84a41-222">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="84a41-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="84a41-223">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="84a41-223">The Intranet security level.</span></span> <span data-ttu-id="84a41-224">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="84a41-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="84a41-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="84a41-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="84a41-226">String</span><span class="sxs-lookup"><span data-stu-id="84a41-226">String</span></span>|<span data-ttu-id="84a41-227">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="84a41-227">The logging report location.</span></span>|
|<span data-ttu-id="84a41-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="84a41-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="84a41-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-229">Boolean</span></span>|<span data-ttu-id="84a41-230">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="84a41-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="84a41-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="84a41-231">browserRequireFirewall</span></span>|<span data-ttu-id="84a41-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-232">Boolean</span></span>|<span data-ttu-id="84a41-233">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="84a41-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="84a41-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="84a41-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="84a41-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-235">Boolean</span></span>|<span data-ttu-id="84a41-236">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="84a41-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="84a41-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="84a41-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="84a41-238">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="84a41-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="84a41-239">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="84a41-239">The trusted sites security level.</span></span> <span data-ttu-id="84a41-240">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="84a41-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="84a41-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="84a41-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="84a41-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-242">Boolean</span></span>|<span data-ttu-id="84a41-243">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84a41-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="84a41-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="84a41-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="84a41-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-245">Boolean</span></span>|<span data-ttu-id="84a41-246">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84a41-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="84a41-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="84a41-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="84a41-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-248">Boolean</span></span>|<span data-ttu-id="84a41-249">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="84a41-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="84a41-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="84a41-250">passwordExpirationDays</span></span>|<span data-ttu-id="84a41-251">Int32</span><span class="sxs-lookup"><span data-stu-id="84a41-251">Int32</span></span>|<span data-ttu-id="84a41-252">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="84a41-252">Password expiration in days.</span></span>|
|<span data-ttu-id="84a41-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="84a41-253">passwordMinimumLength</span></span>|<span data-ttu-id="84a41-254">Int32</span><span class="sxs-lookup"><span data-stu-id="84a41-254">Int32</span></span>|<span data-ttu-id="84a41-255">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="84a41-255">The minimum password length.</span></span>|
|<span data-ttu-id="84a41-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="84a41-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="84a41-257">Int32</span><span class="sxs-lookup"><span data-stu-id="84a41-257">Int32</span></span>|<span data-ttu-id="84a41-258">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="84a41-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="84a41-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="84a41-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="84a41-260">Int32</span><span class="sxs-lookup"><span data-stu-id="84a41-260">Int32</span></span>|<span data-ttu-id="84a41-261">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="84a41-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="84a41-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="84a41-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="84a41-263">Int32</span><span class="sxs-lookup"><span data-stu-id="84a41-263">Int32</span></span>|<span data-ttu-id="84a41-264">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="84a41-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="84a41-265">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="84a41-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="84a41-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="84a41-266">passwordRequiredType</span></span>|[<span data-ttu-id="84a41-267">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="84a41-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="84a41-268">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="84a41-268">The required password type.</span></span> <span data-ttu-id="84a41-269">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="84a41-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="84a41-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="84a41-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="84a41-271">Int32</span><span class="sxs-lookup"><span data-stu-id="84a41-271">Int32</span></span>|<span data-ttu-id="84a41-272">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="84a41-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="84a41-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="84a41-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="84a41-274">Booliano</span><span class="sxs-lookup"><span data-stu-id="84a41-274">Boolean</span></span>|<span data-ttu-id="84a41-275">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="84a41-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="84a41-276">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="84a41-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="84a41-277">updateClassification</span><span class="sxs-lookup"><span data-stu-id="84a41-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="84a41-278">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="84a41-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="84a41-279">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="84a41-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="84a41-280">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="84a41-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="84a41-281">updateClassification</span><span class="sxs-lookup"><span data-stu-id="84a41-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="84a41-282">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="84a41-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="84a41-283">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="84a41-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="84a41-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="84a41-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="84a41-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="84a41-285">Boolean</span></span>|<span data-ttu-id="84a41-286">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="84a41-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="84a41-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="84a41-287">userAccountControlSettings</span></span>|[<span data-ttu-id="84a41-288">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="84a41-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="84a41-289">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="84a41-289">The user account control settings.</span></span> <span data-ttu-id="84a41-290">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="84a41-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="84a41-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="84a41-291">workFoldersUrl</span></span>|<span data-ttu-id="84a41-292">String</span><span class="sxs-lookup"><span data-stu-id="84a41-292">String</span></span>|<span data-ttu-id="84a41-293">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="84a41-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="84a41-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a41-294">Response</span></span>
<span data-ttu-id="84a41-295">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84a41-295">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84a41-296">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84a41-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="84a41-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84a41-297">Request</span></span>
<span data-ttu-id="84a41-298">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84a41-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="84a41-299">Resposta</span><span class="sxs-lookup"><span data-stu-id="84a41-299">Response</span></span>
<span data-ttu-id="84a41-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84a41-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




