---
title: Criar windows81GeneralConfiguration
description: Criar um novo objeto windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be8f9d72a6ce7b2e3a43c5f8cffe697c58866e07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975012"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="8aef7-103">Criar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="8aef7-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="8aef7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8aef7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8aef7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8aef7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8aef7-106">Criar um novo objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8aef7-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8aef7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8aef7-107">Prerequisites</span></span>
<span data-ttu-id="8aef7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aef7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8aef7-110">Permission type</span></span>|<span data-ttu-id="8aef7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8aef7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aef7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8aef7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8aef7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aef7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8aef7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8aef7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aef7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aef7-115">Not supported.</span></span>|
|<span data-ttu-id="8aef7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aef7-116">Application</span></span>|<span data-ttu-id="8aef7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aef7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aef7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8aef7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8aef7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8aef7-119">Request headers</span></span>
|<span data-ttu-id="8aef7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8aef7-120">Header</span></span>|<span data-ttu-id="8aef7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8aef7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8aef7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8aef7-122">Authorization</span></span>|<span data-ttu-id="8aef7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8aef7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8aef7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8aef7-124">Accept</span></span>|<span data-ttu-id="8aef7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8aef7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aef7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8aef7-126">Request body</span></span>
<span data-ttu-id="8aef7-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8aef7-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="8aef7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8aef7-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="8aef7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aef7-129">Property</span></span>|<span data-ttu-id="8aef7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aef7-130">Type</span></span>|<span data-ttu-id="8aef7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aef7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aef7-132">id</span><span class="sxs-lookup"><span data-stu-id="8aef7-132">id</span></span>|<span data-ttu-id="8aef7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aef7-133">String</span></span>|<span data-ttu-id="8aef7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8aef7-134">Key of the entity.</span></span> <span data-ttu-id="8aef7-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8aef7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8aef7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aef7-137">DateTimeOffset</span></span>|<span data-ttu-id="8aef7-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8aef7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8aef7-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8aef7-140">roleScopeTagIds</span></span>|<span data-ttu-id="8aef7-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aef7-141">String collection</span></span>|<span data-ttu-id="8aef7-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8aef7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8aef7-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8aef7-144">supportsScopeTags</span></span>|<span data-ttu-id="8aef7-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-145">Boolean</span></span>|<span data-ttu-id="8aef7-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8aef7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8aef7-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8aef7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8aef7-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8aef7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8aef7-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8aef7-149">This property is read-only.</span></span> <span data-ttu-id="8aef7-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8aef7-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8aef7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8aef7-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8aef7-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="8aef7-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8aef7-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8aef7-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8aef7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8aef7-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8aef7-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="8aef7-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8aef7-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8aef7-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8aef7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8aef7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8aef7-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="8aef7-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8aef7-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8aef7-163">createdDateTime</span></span>|<span data-ttu-id="8aef7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aef7-164">DateTimeOffset</span></span>|<span data-ttu-id="8aef7-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8aef7-165">DateTime the object was created.</span></span> <span data-ttu-id="8aef7-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-167">descrição</span><span class="sxs-lookup"><span data-stu-id="8aef7-167">description</span></span>|<span data-ttu-id="8aef7-168">String</span><span class="sxs-lookup"><span data-stu-id="8aef7-168">String</span></span>|<span data-ttu-id="8aef7-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8aef7-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8aef7-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8aef7-171">displayName</span></span>|<span data-ttu-id="8aef7-172">String</span><span class="sxs-lookup"><span data-stu-id="8aef7-172">String</span></span>|<span data-ttu-id="8aef7-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8aef7-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8aef7-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-175">versão</span><span class="sxs-lookup"><span data-stu-id="8aef7-175">version</span></span>|<span data-ttu-id="8aef7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8aef7-176">Int32</span></span>|<span data-ttu-id="8aef7-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8aef7-177">Version of the device configuration.</span></span> <span data-ttu-id="8aef7-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8aef7-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8aef7-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="8aef7-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="8aef7-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-180">Boolean</span></span>|<span data-ttu-id="8aef7-181">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8aef7-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="8aef7-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="8aef7-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="8aef7-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-183">Boolean</span></span>|<span data-ttu-id="8aef7-184">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="8aef7-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="8aef7-185">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8aef7-185">This property is read-only.</span></span>|
|<span data-ttu-id="8aef7-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="8aef7-186">browserBlockAutofill</span></span>|<span data-ttu-id="8aef7-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-187">Boolean</span></span>|<span data-ttu-id="8aef7-188">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8aef7-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="8aef7-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="8aef7-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="8aef7-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-190">Boolean</span></span>|<span data-ttu-id="8aef7-191">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8aef7-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="8aef7-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="8aef7-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="8aef7-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-193">Boolean</span></span>|<span data-ttu-id="8aef7-194">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8aef7-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="8aef7-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="8aef7-195">browserBlockJavaScript</span></span>|<span data-ttu-id="8aef7-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-196">Boolean</span></span>|<span data-ttu-id="8aef7-197">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8aef7-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="8aef7-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="8aef7-198">browserBlockPlugins</span></span>|<span data-ttu-id="8aef7-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-199">Boolean</span></span>|<span data-ttu-id="8aef7-200">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="8aef7-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="8aef7-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="8aef7-201">browserBlockPopups</span></span>|<span data-ttu-id="8aef7-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-202">Boolean</span></span>|<span data-ttu-id="8aef7-203">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="8aef7-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="8aef7-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="8aef7-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="8aef7-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-205">Boolean</span></span>|<span data-ttu-id="8aef7-206">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="8aef7-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="8aef7-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="8aef7-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="8aef7-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-208">Boolean</span></span>|<span data-ttu-id="8aef7-209">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8aef7-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="8aef7-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="8aef7-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="8aef7-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aef7-211">Boolean</span></span>|<span data-ttu-id="8aef7-212">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="8aef7-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="8aef7-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="8aef7-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="8aef7-214">String</span><span class="sxs-lookup"><span data-stu-id="8aef7-214">String</span></span>|<span data-ttu-id="8aef7-215">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="8aef7-215">The enterprise mode site list location.</span></span> <span data-ttu-id="8aef7-216">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="8aef7-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="8aef7-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8aef7-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="8aef7-218">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8aef7-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="8aef7-219">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="8aef7-219">The internet security level.</span></span> <span data-ttu-id="8aef7-220">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8aef7-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8aef7-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8aef7-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="8aef7-222">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8aef7-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="8aef7-223">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="8aef7-223">The Intranet security level.</span></span> <span data-ttu-id="8aef7-224">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8aef7-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8aef7-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="8aef7-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="8aef7-226">String</span><span class="sxs-lookup"><span data-stu-id="8aef7-226">String</span></span>|<span data-ttu-id="8aef7-227">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="8aef7-227">The logging report location.</span></span>|
|<span data-ttu-id="8aef7-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="8aef7-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="8aef7-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-229">Boolean</span></span>|<span data-ttu-id="8aef7-230">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="8aef7-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="8aef7-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="8aef7-231">browserRequireFirewall</span></span>|<span data-ttu-id="8aef7-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-232">Boolean</span></span>|<span data-ttu-id="8aef7-233">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="8aef7-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="8aef7-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="8aef7-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="8aef7-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-235">Boolean</span></span>|<span data-ttu-id="8aef7-236">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="8aef7-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="8aef7-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8aef7-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="8aef7-238">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8aef7-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="8aef7-239">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="8aef7-239">The trusted sites security level.</span></span> <span data-ttu-id="8aef7-240">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8aef7-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8aef7-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="8aef7-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="8aef7-242">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-242">Boolean</span></span>|<span data-ttu-id="8aef7-243">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8aef7-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="8aef7-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="8aef7-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="8aef7-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-245">Boolean</span></span>|<span data-ttu-id="8aef7-246">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8aef7-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="8aef7-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="8aef7-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="8aef7-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-248">Boolean</span></span>|<span data-ttu-id="8aef7-249">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="8aef7-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="8aef7-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8aef7-250">passwordExpirationDays</span></span>|<span data-ttu-id="8aef7-251">Int32</span><span class="sxs-lookup"><span data-stu-id="8aef7-251">Int32</span></span>|<span data-ttu-id="8aef7-252">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="8aef7-252">Password expiration in days.</span></span>|
|<span data-ttu-id="8aef7-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8aef7-253">passwordMinimumLength</span></span>|<span data-ttu-id="8aef7-254">Int32</span><span class="sxs-lookup"><span data-stu-id="8aef7-254">Int32</span></span>|<span data-ttu-id="8aef7-255">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="8aef7-255">The minimum password length.</span></span>|
|<span data-ttu-id="8aef7-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8aef7-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8aef7-257">Int32</span><span class="sxs-lookup"><span data-stu-id="8aef7-257">Int32</span></span>|<span data-ttu-id="8aef7-258">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="8aef7-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8aef7-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8aef7-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8aef7-260">Int32</span><span class="sxs-lookup"><span data-stu-id="8aef7-260">Int32</span></span>|<span data-ttu-id="8aef7-261">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="8aef7-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8aef7-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8aef7-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8aef7-263">Int32</span><span class="sxs-lookup"><span data-stu-id="8aef7-263">Int32</span></span>|<span data-ttu-id="8aef7-264">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="8aef7-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="8aef7-265">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="8aef7-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8aef7-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8aef7-266">passwordRequiredType</span></span>|[<span data-ttu-id="8aef7-267">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8aef7-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8aef7-268">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="8aef7-268">The required password type.</span></span> <span data-ttu-id="8aef7-269">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8aef7-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8aef7-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8aef7-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8aef7-271">Int32</span><span class="sxs-lookup"><span data-stu-id="8aef7-271">Int32</span></span>|<span data-ttu-id="8aef7-272">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="8aef7-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="8aef7-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="8aef7-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="8aef7-274">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aef7-274">Boolean</span></span>|<span data-ttu-id="8aef7-275">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="8aef7-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="8aef7-276">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="8aef7-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="8aef7-277">updateClassification</span><span class="sxs-lookup"><span data-stu-id="8aef7-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="8aef7-278">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="8aef7-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="8aef7-279">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8aef7-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="8aef7-280">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="8aef7-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="8aef7-281">updateClassification</span><span class="sxs-lookup"><span data-stu-id="8aef7-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="8aef7-282">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="8aef7-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="8aef7-283">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8aef7-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="8aef7-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="8aef7-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="8aef7-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aef7-285">Boolean</span></span>|<span data-ttu-id="8aef7-286">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="8aef7-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="8aef7-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8aef7-287">userAccountControlSettings</span></span>|[<span data-ttu-id="8aef7-288">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8aef7-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="8aef7-289">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="8aef7-289">The user account control settings.</span></span> <span data-ttu-id="8aef7-290">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="8aef7-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="8aef7-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="8aef7-291">workFoldersUrl</span></span>|<span data-ttu-id="8aef7-292">String</span><span class="sxs-lookup"><span data-stu-id="8aef7-292">String</span></span>|<span data-ttu-id="8aef7-293">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="8aef7-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="8aef7-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aef7-294">Response</span></span>
<span data-ttu-id="8aef7-295">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aef7-295">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8aef7-296">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8aef7-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="8aef7-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8aef7-297">Request</span></span>
<span data-ttu-id="8aef7-298">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8aef7-298">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8aef7-299">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aef7-299">Response</span></span>
<span data-ttu-id="8aef7-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8aef7-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





