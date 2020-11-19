---
title: Atualizar windows81GeneralConfiguration
description: Atualizar as propriedades de um objeto windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ad46f5912e473d3f4507adc755cb07b0b268529
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286805"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="ac98b-103">Atualizar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac98b-103">Update windows81GeneralConfiguration</span></span>

<span data-ttu-id="ac98b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac98b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac98b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac98b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac98b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac98b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac98b-107">Atualizar as propriedades de um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac98b-107">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac98b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac98b-108">Prerequisites</span></span>
<span data-ttu-id="ac98b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac98b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac98b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac98b-111">Permission type</span></span>|<span data-ttu-id="ac98b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac98b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac98b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac98b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac98b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac98b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac98b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac98b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac98b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac98b-116">Not supported.</span></span>|
|<span data-ttu-id="ac98b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac98b-117">Application</span></span>|<span data-ttu-id="ac98b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac98b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac98b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac98b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ac98b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac98b-120">Request headers</span></span>
|<span data-ttu-id="ac98b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac98b-121">Header</span></span>|<span data-ttu-id="ac98b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ac98b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac98b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac98b-123">Authorization</span></span>|<span data-ttu-id="ac98b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac98b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac98b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac98b-125">Accept</span></span>|<span data-ttu-id="ac98b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac98b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac98b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac98b-127">Request body</span></span>
<span data-ttu-id="ac98b-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac98b-128">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="ac98b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac98b-129">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="ac98b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac98b-130">Property</span></span>|<span data-ttu-id="ac98b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac98b-131">Type</span></span>|<span data-ttu-id="ac98b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac98b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac98b-133">id</span><span class="sxs-lookup"><span data-stu-id="ac98b-133">id</span></span>|<span data-ttu-id="ac98b-134">String</span><span class="sxs-lookup"><span data-stu-id="ac98b-134">String</span></span>|<span data-ttu-id="ac98b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ac98b-135">Key of the entity.</span></span> <span data-ttu-id="ac98b-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac98b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ac98b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac98b-138">DateTimeOffset</span></span>|<span data-ttu-id="ac98b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ac98b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ac98b-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac98b-141">roleScopeTagIds</span></span>|<span data-ttu-id="ac98b-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac98b-142">String collection</span></span>|<span data-ttu-id="ac98b-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ac98b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ac98b-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ac98b-145">supportsScopeTags</span></span>|<span data-ttu-id="ac98b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac98b-146">Boolean</span></span>|<span data-ttu-id="ac98b-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ac98b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ac98b-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ac98b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ac98b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ac98b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ac98b-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac98b-150">This property is read-only.</span></span> <span data-ttu-id="ac98b-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ac98b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ac98b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ac98b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ac98b-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="ac98b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ac98b-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ac98b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ac98b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ac98b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ac98b-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="ac98b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ac98b-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ac98b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ac98b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ac98b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ac98b-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="ac98b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ac98b-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac98b-164">createdDateTime</span></span>|<span data-ttu-id="ac98b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac98b-165">DateTimeOffset</span></span>|<span data-ttu-id="ac98b-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ac98b-166">DateTime the object was created.</span></span> <span data-ttu-id="ac98b-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-168">description</span><span class="sxs-lookup"><span data-stu-id="ac98b-168">description</span></span>|<span data-ttu-id="ac98b-169">String</span><span class="sxs-lookup"><span data-stu-id="ac98b-169">String</span></span>|<span data-ttu-id="ac98b-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac98b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ac98b-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ac98b-172">displayName</span></span>|<span data-ttu-id="ac98b-173">String</span><span class="sxs-lookup"><span data-stu-id="ac98b-173">String</span></span>|<span data-ttu-id="ac98b-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac98b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ac98b-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-176">versão</span><span class="sxs-lookup"><span data-stu-id="ac98b-176">version</span></span>|<span data-ttu-id="ac98b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ac98b-177">Int32</span></span>|<span data-ttu-id="ac98b-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac98b-178">Version of the device configuration.</span></span> <span data-ttu-id="ac98b-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac98b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac98b-180">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="ac98b-180">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="ac98b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-181">Boolean</span></span>|<span data-ttu-id="ac98b-182">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ac98b-182">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="ac98b-183">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="ac98b-183">applyOnlyToWindows81</span></span>|<span data-ttu-id="ac98b-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-184">Boolean</span></span>|<span data-ttu-id="ac98b-185">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="ac98b-185">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ac98b-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac98b-186">This property is read-only.</span></span>|
|<span data-ttu-id="ac98b-187">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ac98b-187">browserBlockAutofill</span></span>|<span data-ttu-id="ac98b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-188">Boolean</span></span>|<span data-ttu-id="ac98b-189">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ac98b-189">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="ac98b-190">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="ac98b-190">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="ac98b-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-191">Boolean</span></span>|<span data-ttu-id="ac98b-192">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ac98b-192">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="ac98b-193">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="ac98b-193">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="ac98b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-194">Boolean</span></span>|<span data-ttu-id="ac98b-195">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ac98b-195">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="ac98b-196">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ac98b-196">browserBlockJavaScript</span></span>|<span data-ttu-id="ac98b-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-197">Boolean</span></span>|<span data-ttu-id="ac98b-198">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ac98b-198">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="ac98b-199">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="ac98b-199">browserBlockPlugins</span></span>|<span data-ttu-id="ac98b-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-200">Boolean</span></span>|<span data-ttu-id="ac98b-201">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="ac98b-201">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="ac98b-202">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ac98b-202">browserBlockPopups</span></span>|<span data-ttu-id="ac98b-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-203">Boolean</span></span>|<span data-ttu-id="ac98b-204">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="ac98b-204">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="ac98b-205">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="ac98b-205">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="ac98b-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-206">Boolean</span></span>|<span data-ttu-id="ac98b-207">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="ac98b-207">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="ac98b-208">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="ac98b-208">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="ac98b-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-209">Boolean</span></span>|<span data-ttu-id="ac98b-210">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ac98b-210">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="ac98b-211">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="ac98b-211">browserRequireSmartScreen</span></span>|<span data-ttu-id="ac98b-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-212">Boolean</span></span>|<span data-ttu-id="ac98b-213">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="ac98b-213">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="ac98b-214">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="ac98b-214">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="ac98b-215">String</span><span class="sxs-lookup"><span data-stu-id="ac98b-215">String</span></span>|<span data-ttu-id="ac98b-216">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="ac98b-216">The enterprise mode site list location.</span></span> <span data-ttu-id="ac98b-217">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="ac98b-217">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="ac98b-218">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ac98b-218">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="ac98b-219">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ac98b-219">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="ac98b-220">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="ac98b-220">The internet security level.</span></span> <span data-ttu-id="ac98b-221">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ac98b-221">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ac98b-222">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ac98b-222">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="ac98b-223">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ac98b-223">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="ac98b-224">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="ac98b-224">The Intranet security level.</span></span> <span data-ttu-id="ac98b-225">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ac98b-225">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ac98b-226">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="ac98b-226">browserLoggingReportLocation</span></span>|<span data-ttu-id="ac98b-227">String</span><span class="sxs-lookup"><span data-stu-id="ac98b-227">String</span></span>|<span data-ttu-id="ac98b-228">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="ac98b-228">The logging report location.</span></span>|
|<span data-ttu-id="ac98b-229">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="ac98b-229">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="ac98b-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-230">Boolean</span></span>|<span data-ttu-id="ac98b-231">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="ac98b-231">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="ac98b-232">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="ac98b-232">browserRequireFirewall</span></span>|<span data-ttu-id="ac98b-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-233">Boolean</span></span>|<span data-ttu-id="ac98b-234">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="ac98b-234">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="ac98b-235">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ac98b-235">browserRequireFraudWarning</span></span>|<span data-ttu-id="ac98b-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-236">Boolean</span></span>|<span data-ttu-id="ac98b-237">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="ac98b-237">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="ac98b-238">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ac98b-238">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="ac98b-239">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ac98b-239">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="ac98b-240">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="ac98b-240">The trusted sites security level.</span></span> <span data-ttu-id="ac98b-241">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ac98b-241">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ac98b-242">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ac98b-242">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ac98b-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-243">Boolean</span></span>|<span data-ttu-id="ac98b-244">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ac98b-244">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ac98b-245">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="ac98b-245">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="ac98b-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-246">Boolean</span></span>|<span data-ttu-id="ac98b-247">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ac98b-247">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ac98b-248">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="ac98b-248">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="ac98b-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-249">Boolean</span></span>|<span data-ttu-id="ac98b-250">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="ac98b-250">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="ac98b-251">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ac98b-251">passwordExpirationDays</span></span>|<span data-ttu-id="ac98b-252">Int32</span><span class="sxs-lookup"><span data-stu-id="ac98b-252">Int32</span></span>|<span data-ttu-id="ac98b-253">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="ac98b-253">Password expiration in days.</span></span>|
|<span data-ttu-id="ac98b-254">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ac98b-254">passwordMinimumLength</span></span>|<span data-ttu-id="ac98b-255">Int32</span><span class="sxs-lookup"><span data-stu-id="ac98b-255">Int32</span></span>|<span data-ttu-id="ac98b-256">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="ac98b-256">The minimum password length.</span></span>|
|<span data-ttu-id="ac98b-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ac98b-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ac98b-258">Int32</span><span class="sxs-lookup"><span data-stu-id="ac98b-258">Int32</span></span>|<span data-ttu-id="ac98b-259">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="ac98b-259">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ac98b-260">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ac98b-260">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ac98b-261">Int32</span><span class="sxs-lookup"><span data-stu-id="ac98b-261">Int32</span></span>|<span data-ttu-id="ac98b-262">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="ac98b-262">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ac98b-263">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ac98b-263">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ac98b-264">Int32</span><span class="sxs-lookup"><span data-stu-id="ac98b-264">Int32</span></span>|<span data-ttu-id="ac98b-265">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="ac98b-265">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="ac98b-266">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="ac98b-266">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ac98b-267">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ac98b-267">passwordRequiredType</span></span>|[<span data-ttu-id="ac98b-268">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ac98b-268">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ac98b-269">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="ac98b-269">The required password type.</span></span> <span data-ttu-id="ac98b-270">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ac98b-270">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ac98b-271">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ac98b-271">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ac98b-272">Int32</span><span class="sxs-lookup"><span data-stu-id="ac98b-272">Int32</span></span>|<span data-ttu-id="ac98b-273">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="ac98b-273">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="ac98b-274">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="ac98b-274">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="ac98b-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-275">Boolean</span></span>|<span data-ttu-id="ac98b-276">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="ac98b-276">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="ac98b-277">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="ac98b-277">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="ac98b-278">updateClassification</span><span class="sxs-lookup"><span data-stu-id="ac98b-278">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="ac98b-279">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="ac98b-279">The minimum update classification to install automatically.</span></span> <span data-ttu-id="ac98b-280">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="ac98b-280">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="ac98b-281">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="ac98b-281">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="ac98b-282">updateClassification</span><span class="sxs-lookup"><span data-stu-id="ac98b-282">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="ac98b-283">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="ac98b-283">The minimum update classification to install automatically.</span></span> <span data-ttu-id="ac98b-284">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="ac98b-284">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="ac98b-285">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="ac98b-285">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="ac98b-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac98b-286">Boolean</span></span>|<span data-ttu-id="ac98b-287">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="ac98b-287">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="ac98b-288">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="ac98b-288">userAccountControlSettings</span></span>|[<span data-ttu-id="ac98b-289">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="ac98b-289">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="ac98b-290">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac98b-290">The user account control settings.</span></span> <span data-ttu-id="ac98b-291">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="ac98b-291">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="ac98b-292">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="ac98b-292">workFoldersUrl</span></span>|<span data-ttu-id="ac98b-293">String</span><span class="sxs-lookup"><span data-stu-id="ac98b-293">String</span></span>|<span data-ttu-id="ac98b-294">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="ac98b-294">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="ac98b-295">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac98b-295">Response</span></span>
<span data-ttu-id="ac98b-296">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac98b-296">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac98b-297">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac98b-297">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac98b-298">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac98b-298">Request</span></span>
<span data-ttu-id="ac98b-299">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac98b-299">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac98b-300">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac98b-300">Response</span></span>
<span data-ttu-id="ac98b-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac98b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




