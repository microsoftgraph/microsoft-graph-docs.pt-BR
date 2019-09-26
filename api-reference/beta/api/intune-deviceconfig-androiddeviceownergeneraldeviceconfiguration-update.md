---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 859566d2c5490dd6ad51fb5cb22e00d6b236b745
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37169857"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="63fb9-103">Atualizar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="63fb9-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="63fb9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63fb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63fb9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63fb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63fb9-106">Atualiza as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="63fb9-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63fb9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63fb9-107">Prerequisites</span></span>
<span data-ttu-id="63fb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63fb9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63fb9-110">Permission type</span></span>|<span data-ttu-id="63fb9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63fb9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63fb9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63fb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63fb9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63fb9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63fb9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63fb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63fb9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63fb9-115">Not supported.</span></span>|
|<span data-ttu-id="63fb9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63fb9-116">Application</span></span>|<span data-ttu-id="63fb9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63fb9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63fb9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63fb9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="63fb9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63fb9-119">Request headers</span></span>
|<span data-ttu-id="63fb9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63fb9-120">Header</span></span>|<span data-ttu-id="63fb9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63fb9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63fb9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63fb9-122">Authorization</span></span>|<span data-ttu-id="63fb9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63fb9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63fb9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63fb9-124">Accept</span></span>|<span data-ttu-id="63fb9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63fb9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63fb9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63fb9-126">Request body</span></span>
<span data-ttu-id="63fb9-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="63fb9-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="63fb9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63fb9-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="63fb9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63fb9-129">Property</span></span>|<span data-ttu-id="63fb9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="63fb9-130">Type</span></span>|<span data-ttu-id="63fb9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="63fb9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63fb9-132">id</span><span class="sxs-lookup"><span data-stu-id="63fb9-132">id</span></span>|<span data-ttu-id="63fb9-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63fb9-133">String</span></span>|<span data-ttu-id="63fb9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="63fb9-134">Key of the entity.</span></span> <span data-ttu-id="63fb9-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63fb9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="63fb9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63fb9-137">DateTimeOffset</span></span>|<span data-ttu-id="63fb9-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="63fb9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="63fb9-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63fb9-140">roleScopeTagIds</span></span>|<span data-ttu-id="63fb9-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="63fb9-141">String collection</span></span>|<span data-ttu-id="63fb9-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="63fb9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="63fb9-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="63fb9-144">supportsScopeTags</span></span>|<span data-ttu-id="63fb9-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-145">Boolean</span></span>|<span data-ttu-id="63fb9-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="63fb9-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="63fb9-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="63fb9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="63fb9-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63fb9-149">This property is read-only.</span></span> <span data-ttu-id="63fb9-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="63fb9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="63fb9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="63fb9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="63fb9-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="63fb9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="63fb9-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="63fb9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="63fb9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="63fb9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="63fb9-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="63fb9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="63fb9-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="63fb9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="63fb9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="63fb9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="63fb9-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="63fb9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="63fb9-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63fb9-163">createdDateTime</span></span>|<span data-ttu-id="63fb9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63fb9-164">DateTimeOffset</span></span>|<span data-ttu-id="63fb9-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-165">DateTime the object was created.</span></span> <span data-ttu-id="63fb9-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-167">descrição</span><span class="sxs-lookup"><span data-stu-id="63fb9-167">description</span></span>|<span data-ttu-id="63fb9-168">String</span><span class="sxs-lookup"><span data-stu-id="63fb9-168">String</span></span>|<span data-ttu-id="63fb9-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63fb9-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="63fb9-171">displayName</span></span>|<span data-ttu-id="63fb9-172">String</span><span class="sxs-lookup"><span data-stu-id="63fb9-172">String</span></span>|<span data-ttu-id="63fb9-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63fb9-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-175">versão</span><span class="sxs-lookup"><span data-stu-id="63fb9-175">version</span></span>|<span data-ttu-id="63fb9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-176">Int32</span></span>|<span data-ttu-id="63fb9-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-177">Version of the device configuration.</span></span> <span data-ttu-id="63fb9-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63fb9-179">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="63fb9-179">accountsBlockModification</span></span>|<span data-ttu-id="63fb9-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-180">Boolean</span></span>|<span data-ttu-id="63fb9-181">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="63fb9-182">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="63fb9-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="63fb9-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-183">Boolean</span></span>|<span data-ttu-id="63fb9-184">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="63fb9-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="63fb9-185">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="63fb9-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="63fb9-186">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="63fb9-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="63fb9-187">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="63fb9-188">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="63fb9-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="63fb9-189">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="63fb9-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="63fb9-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="63fb9-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="63fb9-191">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="63fb9-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="63fb9-192">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="63fb9-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="63fb9-193">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="63fb9-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="63fb9-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-194">Boolean</span></span>|<span data-ttu-id="63fb9-195">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="63fb9-196">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="63fb9-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="63fb9-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-197">Boolean</span></span>|<span data-ttu-id="63fb9-198">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="63fb9-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="63fb9-199">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="63fb9-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="63fb9-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-200">Boolean</span></span>|<span data-ttu-id="63fb9-201">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="63fb9-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="63fb9-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="63fb9-202">cameraBlocked</span></span>|<span data-ttu-id="63fb9-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-203">Boolean</span></span>|<span data-ttu-id="63fb9-204">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="63fb9-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="63fb9-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="63fb9-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="63fb9-206">Boolean</span></span>|<span data-ttu-id="63fb9-207">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="63fb9-208">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="63fb9-208">dataRoamingBlocked</span></span>|<span data-ttu-id="63fb9-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-209">Boolean</span></span>|<span data-ttu-id="63fb9-210">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="63fb9-210">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="63fb9-211">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="63fb9-211">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="63fb9-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-212">Boolean</span></span>|<span data-ttu-id="63fb9-213">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="63fb9-213">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="63fb9-214">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="63fb9-214">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="63fb9-215">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="63fb9-215">String collection</span></span>|<span data-ttu-id="63fb9-216">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-216">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="63fb9-217">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="63fb9-217">factoryResetBlocked</span></span>|<span data-ttu-id="63fb9-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="63fb9-218">Boolean</span></span>|<span data-ttu-id="63fb9-219">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-219">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="63fb9-220">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="63fb9-220">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="63fb9-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-221">Boolean</span></span>|<span data-ttu-id="63fb9-222">Se o modo de proteção de tela deve ou não ser habilitado ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-222">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-223">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="63fb9-223">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="63fb9-224">String</span><span class="sxs-lookup"><span data-stu-id="63fb9-224">String</span></span>|<span data-ttu-id="63fb9-225">URL de uma imagem que será a proteção de tela do dispositivo no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-225">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-226">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="63fb9-226">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="63fb9-227">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-227">Int32</span></span>|<span data-ttu-id="63fb9-228">O número de segundos que o dispositivo exibirá a proteção de tela no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-228">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="63fb9-229">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="63fb9-229">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="63fb9-230">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="63fb9-230">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="63fb9-231">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-231">Int32</span></span>|<span data-ttu-id="63fb9-232">O número de segundos que o dispositivo precisa estar inativo para que a proteção de tela seja mostrada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-232">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="63fb9-233">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="63fb9-233">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="63fb9-234">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="63fb9-234">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="63fb9-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-235">Boolean</span></span>|<span data-ttu-id="63fb9-236">Se a tela do dispositivo deve ou não mostrar a proteção de tela se áudio/vídeo estiver em execução no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-236">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-237">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="63fb9-237">kioskModeApps</span></span>|<span data-ttu-id="63fb9-238">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-238">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="63fb9-239">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-239">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="63fb9-240">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="63fb9-240">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="63fb9-241">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="63fb9-241">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="63fb9-242">String</span><span class="sxs-lookup"><span data-stu-id="63fb9-242">String</span></span>|<span data-ttu-id="63fb9-243">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-243">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-244">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="63fb9-244">kioskModeExitCode</span></span>|<span data-ttu-id="63fb9-245">String</span><span class="sxs-lookup"><span data-stu-id="63fb9-245">String</span></span>|<span data-ttu-id="63fb9-246">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-246">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-247">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="63fb9-247">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="63fb9-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-248">Boolean</span></span>|<span data-ttu-id="63fb9-249">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-249">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-250">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="63fb9-250">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="63fb9-251">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="63fb9-251">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="63fb9-252">Indica se o botão de Home virtual é um botão deslizar para cima ou um botão de início flutuante.</span><span class="sxs-lookup"><span data-stu-id="63fb9-252">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="63fb9-253">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="63fb9-253">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="63fb9-254">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="63fb9-254">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="63fb9-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-255">Boolean</span></span>|<span data-ttu-id="63fb9-256">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-256">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-257">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="63fb9-257">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="63fb9-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-258">Boolean</span></span>|<span data-ttu-id="63fb9-259">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-259">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-260">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="63fb9-260">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="63fb9-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-261">Boolean</span></span>|<span data-ttu-id="63fb9-262">Se permitirá ou não que um usuário use a lanterna no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-262">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-263">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="63fb9-263">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="63fb9-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-264">Boolean</span></span>|<span data-ttu-id="63fb9-265">Se permitirá ou não que um usuário altere o volume de mídia no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63fb9-265">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="63fb9-266">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="63fb9-266">microphoneForceMute</span></span>|<span data-ttu-id="63fb9-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-267">Boolean</span></span>|<span data-ttu-id="63fb9-268">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-268">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="63fb9-269">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="63fb9-269">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="63fb9-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-270">Boolean</span></span>|<span data-ttu-id="63fb9-271">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="63fb9-271">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="63fb9-272">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="63fb9-272">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="63fb9-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-273">Boolean</span></span>|<span data-ttu-id="63fb9-274">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-274">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="63fb9-275">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="63fb9-275">passwordBlockKeyguard</span></span>|<span data-ttu-id="63fb9-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-276">Boolean</span></span>|<span data-ttu-id="63fb9-277">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="63fb9-277">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="63fb9-278">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="63fb9-278">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="63fb9-279">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-279">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="63fb9-280">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="63fb9-280">List of device keyguard features to block.</span></span> <span data-ttu-id="63fb9-281">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="63fb9-281">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="63fb9-282">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="63fb9-282">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="63fb9-283">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="63fb9-283">passwordExpirationDays</span></span>|<span data-ttu-id="63fb9-284">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-284">Int32</span></span>|<span data-ttu-id="63fb9-285">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="63fb9-285">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="63fb9-286">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="63fb9-286">Valid values 1 to 365</span></span>|
|<span data-ttu-id="63fb9-287">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="63fb9-287">passwordMinimumLength</span></span>|<span data-ttu-id="63fb9-288">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-288">Int32</span></span>|<span data-ttu-id="63fb9-289">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-289">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="63fb9-290">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="63fb9-290">Valid values 4 to 16</span></span>|
|<span data-ttu-id="63fb9-291">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="63fb9-291">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="63fb9-292">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-292">Int32</span></span>|<span data-ttu-id="63fb9-293">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-293">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="63fb9-294">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="63fb9-294">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63fb9-295">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="63fb9-295">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="63fb9-296">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-296">Int32</span></span>|<span data-ttu-id="63fb9-297">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-297">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="63fb9-298">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="63fb9-298">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63fb9-299">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="63fb9-299">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="63fb9-300">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-300">Int32</span></span>|<span data-ttu-id="63fb9-301">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-301">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="63fb9-302">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="63fb9-302">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63fb9-303">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="63fb9-303">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="63fb9-304">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-304">Int32</span></span>|<span data-ttu-id="63fb9-305">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-305">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="63fb9-306">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="63fb9-306">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63fb9-307">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="63fb9-307">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="63fb9-308">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-308">Int32</span></span>|<span data-ttu-id="63fb9-309">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-309">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="63fb9-310">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="63fb9-310">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63fb9-311">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="63fb9-311">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="63fb9-312">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-312">Int32</span></span>|<span data-ttu-id="63fb9-313">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-313">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="63fb9-314">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="63fb9-314">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63fb9-315">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="63fb9-315">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="63fb9-316">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-316">Int32</span></span>|<span data-ttu-id="63fb9-317">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="63fb9-317">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="63fb9-318">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="63fb9-318">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="63fb9-319">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-319">Int32</span></span>|<span data-ttu-id="63fb9-320">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="63fb9-320">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="63fb9-321">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="63fb9-321">Valid values 0 to 24</span></span>|
|<span data-ttu-id="63fb9-322">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="63fb9-322">passwordRequiredType</span></span>|[<span data-ttu-id="63fb9-323">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="63fb9-323">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="63fb9-324">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-324">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="63fb9-325">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="63fb9-325">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="63fb9-326">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="63fb9-326">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="63fb9-327">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-327">Int32</span></span>|<span data-ttu-id="63fb9-328">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-328">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="63fb9-329">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="63fb9-329">Valid values 4 to 11</span></span>|
|<span data-ttu-id="63fb9-330">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="63fb9-330">playStoreMode</span></span>|[<span data-ttu-id="63fb9-331">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="63fb9-331">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="63fb9-332">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-332">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="63fb9-333">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="63fb9-333">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="63fb9-334">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="63fb9-334">safeBootBlocked</span></span>|<span data-ttu-id="63fb9-335">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-335">Boolean</span></span>|<span data-ttu-id="63fb9-336">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-336">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="63fb9-337">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="63fb9-337">screenCaptureBlocked</span></span>|<span data-ttu-id="63fb9-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="63fb9-338">Boolean</span></span>|<span data-ttu-id="63fb9-339">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-339">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="63fb9-340">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="63fb9-340">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="63fb9-341">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-341">Boolean</span></span>|<span data-ttu-id="63fb9-342">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63fb9-342">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="63fb9-343">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="63fb9-343">securityRequireVerifyApps</span></span>|<span data-ttu-id="63fb9-344">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-344">Boolean</span></span>|<span data-ttu-id="63fb9-345">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="63fb9-345">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="63fb9-346">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="63fb9-346">statusBarBlocked</span></span>|<span data-ttu-id="63fb9-347">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-347">Boolean</span></span>|<span data-ttu-id="63fb9-348">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="63fb9-348">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="63fb9-349">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="63fb9-349">stayOnModes</span></span>|<span data-ttu-id="63fb9-350">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="63fb9-350">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="63fb9-351">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-351">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="63fb9-352">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="63fb9-352">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="63fb9-353">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="63fb9-353">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="63fb9-354">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="63fb9-354">storageAllowUsb</span></span>|<span data-ttu-id="63fb9-355">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-355">Boolean</span></span>|<span data-ttu-id="63fb9-356">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="63fb9-356">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="63fb9-357">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="63fb9-357">storageBlockExternalMedia</span></span>|<span data-ttu-id="63fb9-358">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-358">Boolean</span></span>|<span data-ttu-id="63fb9-359">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-359">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="63fb9-360">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="63fb9-360">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="63fb9-361">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-361">Boolean</span></span>|<span data-ttu-id="63fb9-362">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-362">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="63fb9-363">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="63fb9-363">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="63fb9-364">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-364">Int32</span></span>|<span data-ttu-id="63fb9-365">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-365">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="63fb9-366">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="63fb9-366">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="63fb9-367">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="63fb9-367">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="63fb9-368">Int32</span><span class="sxs-lookup"><span data-stu-id="63fb9-368">Int32</span></span>|<span data-ttu-id="63fb9-369">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="63fb9-369">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="63fb9-370">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="63fb9-370">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="63fb9-371">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="63fb9-371">systemUpdateInstallType</span></span>|[<span data-ttu-id="63fb9-372">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="63fb9-372">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="63fb9-373">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="63fb9-373">The type of system update configuration.</span></span> <span data-ttu-id="63fb9-374">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="63fb9-374">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="63fb9-375">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="63fb9-375">systemWindowsBlocked</span></span>|<span data-ttu-id="63fb9-376">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-376">Boolean</span></span>|<span data-ttu-id="63fb9-377">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="63fb9-377">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="63fb9-378">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="63fb9-378">usersBlockAdd</span></span>|<span data-ttu-id="63fb9-379">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-379">Boolean</span></span>|<span data-ttu-id="63fb9-380">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="63fb9-380">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="63fb9-381">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="63fb9-381">usersBlockRemove</span></span>|<span data-ttu-id="63fb9-382">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-382">Boolean</span></span>|<span data-ttu-id="63fb9-383">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-383">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="63fb9-384">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="63fb9-384">volumeBlockAdjustment</span></span>|<span data-ttu-id="63fb9-385">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-385">Boolean</span></span>|<span data-ttu-id="63fb9-386">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="63fb9-386">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="63fb9-387">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="63fb9-387">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="63fb9-388">String</span><span class="sxs-lookup"><span data-stu-id="63fb9-388">String</span></span>|<span data-ttu-id="63fb9-389">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="63fb9-389">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="63fb9-390">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="63fb9-390">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="63fb9-391">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-391">Boolean</span></span>|<span data-ttu-id="63fb9-392">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="63fb9-392">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="63fb9-393">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="63fb9-393">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="63fb9-394">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-394">Boolean</span></span>|<span data-ttu-id="63fb9-395">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="63fb9-395">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="63fb9-396">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="63fb9-396">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="63fb9-397">Booliano</span><span class="sxs-lookup"><span data-stu-id="63fb9-397">Boolean</span></span>|<span data-ttu-id="63fb9-398">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="63fb9-398">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="63fb9-399">Resposta</span><span class="sxs-lookup"><span data-stu-id="63fb9-399">Response</span></span>
<span data-ttu-id="63fb9-400">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63fb9-400">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63fb9-401">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63fb9-401">Example</span></span>

### <a name="request"></a><span data-ttu-id="63fb9-402">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63fb9-402">Request</span></span>
<span data-ttu-id="63fb9-403">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63fb9-403">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4123

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="63fb9-404">Resposta</span><span class="sxs-lookup"><span data-stu-id="63fb9-404">Response</span></span>
<span data-ttu-id="63fb9-p136">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63fb9-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4295

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




