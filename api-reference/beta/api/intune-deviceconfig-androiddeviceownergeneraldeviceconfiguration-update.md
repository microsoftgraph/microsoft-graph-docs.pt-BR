---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ca9452f034600275acbd59d9a86b7d0c7487910
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123341"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="8dc76-103">Atualizar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8dc76-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="8dc76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dc76-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8dc76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dc76-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8dc76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dc76-107">Atualiza as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8dc76-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dc76-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8dc76-108">Prerequisites</span></span>
<span data-ttu-id="8dc76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dc76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dc76-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dc76-111">Permission type</span></span>|<span data-ttu-id="8dc76-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8dc76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dc76-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dc76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8dc76-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc76-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8dc76-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dc76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dc76-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dc76-116">Not supported.</span></span>|
|<span data-ttu-id="8dc76-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dc76-117">Application</span></span>|<span data-ttu-id="8dc76-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc76-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dc76-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dc76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8dc76-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc76-120">Request headers</span></span>
|<span data-ttu-id="8dc76-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8dc76-121">Header</span></span>|<span data-ttu-id="8dc76-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8dc76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dc76-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8dc76-123">Authorization</span></span>|<span data-ttu-id="8dc76-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dc76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dc76-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8dc76-125">Accept</span></span>|<span data-ttu-id="8dc76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8dc76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dc76-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc76-127">Request body</span></span>
<span data-ttu-id="8dc76-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8dc76-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="8dc76-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dc76-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="8dc76-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dc76-130">Property</span></span>|<span data-ttu-id="8dc76-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dc76-131">Type</span></span>|<span data-ttu-id="8dc76-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc76-133">id</span><span class="sxs-lookup"><span data-stu-id="8dc76-133">id</span></span>|<span data-ttu-id="8dc76-134">String</span><span class="sxs-lookup"><span data-stu-id="8dc76-134">String</span></span>|<span data-ttu-id="8dc76-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8dc76-135">Key of the entity.</span></span> <span data-ttu-id="8dc76-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dc76-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8dc76-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dc76-138">DateTimeOffset</span></span>|<span data-ttu-id="8dc76-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8dc76-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8dc76-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8dc76-141">roleScopeTagIds</span></span>|<span data-ttu-id="8dc76-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-142">String collection</span></span>|<span data-ttu-id="8dc76-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8dc76-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8dc76-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8dc76-145">supportsScopeTags</span></span>|<span data-ttu-id="8dc76-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-146">Boolean</span></span>|<span data-ttu-id="8dc76-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8dc76-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8dc76-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8dc76-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8dc76-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8dc76-150">This property is read-only.</span></span> <span data-ttu-id="8dc76-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8dc76-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8dc76-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8dc76-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8dc76-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="8dc76-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8dc76-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8dc76-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8dc76-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8dc76-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8dc76-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="8dc76-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8dc76-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8dc76-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8dc76-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8dc76-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8dc76-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="8dc76-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8dc76-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8dc76-164">createdDateTime</span></span>|<span data-ttu-id="8dc76-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dc76-165">DateTimeOffset</span></span>|<span data-ttu-id="8dc76-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-166">DateTime the object was created.</span></span> <span data-ttu-id="8dc76-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-168">descrição</span><span class="sxs-lookup"><span data-stu-id="8dc76-168">description</span></span>|<span data-ttu-id="8dc76-169">String</span><span class="sxs-lookup"><span data-stu-id="8dc76-169">String</span></span>|<span data-ttu-id="8dc76-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8dc76-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8dc76-172">displayName</span></span>|<span data-ttu-id="8dc76-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-173">String</span></span>|<span data-ttu-id="8dc76-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8dc76-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-176">versão</span><span class="sxs-lookup"><span data-stu-id="8dc76-176">version</span></span>|<span data-ttu-id="8dc76-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-177">Int32</span></span>|<span data-ttu-id="8dc76-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-178">Version of the device configuration.</span></span> <span data-ttu-id="8dc76-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dc76-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="8dc76-180">accountsBlockModification</span></span>|<span data-ttu-id="8dc76-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-181">Boolean</span></span>|<span data-ttu-id="8dc76-182">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="8dc76-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="8dc76-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="8dc76-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-184">Boolean</span></span>|<span data-ttu-id="8dc76-185">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="8dc76-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="8dc76-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="8dc76-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="8dc76-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="8dc76-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="8dc76-188">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="8dc76-189">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="8dc76-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="8dc76-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="8dc76-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="8dc76-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="8dc76-192">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="8dc76-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="8dc76-193">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="8dc76-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="8dc76-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="8dc76-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-195">Boolean</span></span>|<span data-ttu-id="8dc76-196">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="8dc76-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="8dc76-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="8dc76-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-198">Boolean</span></span>|<span data-ttu-id="8dc76-199">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8dc76-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="8dc76-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="8dc76-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="8dc76-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-201">Boolean</span></span>|<span data-ttu-id="8dc76-202">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8dc76-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="8dc76-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-203">cameraBlocked</span></span>|<span data-ttu-id="8dc76-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-204">Boolean</span></span>|<span data-ttu-id="8dc76-205">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="8dc76-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="8dc76-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="8dc76-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dc76-207">Boolean</span></span>|<span data-ttu-id="8dc76-208">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="8dc76-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="8dc76-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-210">Boolean</span></span>|<span data-ttu-id="8dc76-211">Indica se os usuários devem ou não ser bloqueados de qualquer configuração de credencial de certificado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="8dc76-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="8dc76-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-213">Boolean</span></span>|<span data-ttu-id="8dc76-214">Indica se você deseja ou não configurar o iniciador Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8dc76-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="8dc76-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="8dc76-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-216">Boolean</span></span>|<span data-ttu-id="8dc76-217">Indica se o papel de parede deve ou não ser configurado nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="8dc76-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="8dc76-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="8dc76-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="8dc76-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-219">String</span></span>|<span data-ttu-id="8dc76-220">Indica a URL do arquivo de imagem a ser usado como papel de parede nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="8dc76-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="8dc76-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="8dc76-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="8dc76-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-222">Boolean</span></span>|<span data-ttu-id="8dc76-223">Indica se o usuário pode ou não modificar o papel de parede para personalizar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="8dc76-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="8dc76-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-225">Boolean</span></span>|<span data-ttu-id="8dc76-226">Indica se você deseja ou não habilitar o feed do inicializador no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="8dc76-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="8dc76-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="8dc76-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-228">Boolean</span></span>|<span data-ttu-id="8dc76-229">Indica se o usuário pode ou não modificar o feed do inicializador no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="8dc76-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8dc76-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="8dc76-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="8dc76-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="8dc76-232">Indica se você deseja ou não configurar o encaixe de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8dc76-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="8dc76-233">Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="8dc76-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="8dc76-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="8dc76-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-235">Boolean</span></span>|<span data-ttu-id="8dc76-236">Indica se o usuário pode ou não modificar a configuração de encaixe do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="8dc76-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="8dc76-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="8dc76-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="8dc76-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="8dc76-239">Indica a configuração de posicionamento da barra de pesquisa no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="8dc76-240">Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="8dc76-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8dc76-241">enrollmentProfile</span></span>|[<span data-ttu-id="8dc76-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="8dc76-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="8dc76-243">Indica o perfil de registro que você deseja configurar.</span><span class="sxs-lookup"><span data-stu-id="8dc76-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="8dc76-244">Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="8dc76-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-245">dataRoamingBlocked</span></span>|<span data-ttu-id="8dc76-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-246">Boolean</span></span>|<span data-ttu-id="8dc76-247">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="8dc76-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="8dc76-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="8dc76-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-249">Boolean</span></span>|<span data-ttu-id="8dc76-250">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="8dc76-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="8dc76-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="8dc76-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="8dc76-252">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-252">String collection</span></span>|<span data-ttu-id="8dc76-253">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="8dc76-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-254">factoryResetBlocked</span></span>|<span data-ttu-id="8dc76-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dc76-255">Boolean</span></span>|<span data-ttu-id="8dc76-256">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="8dc76-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="8dc76-257">globalProxy</span></span>|[<span data-ttu-id="8dc76-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="8dc76-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="8dc76-259">O proxy é configurado diretamente com hosts, porta e hosts excluídos.</span><span class="sxs-lookup"><span data-stu-id="8dc76-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="8dc76-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-260">googleAccountsBlocked</span></span>|<span data-ttu-id="8dc76-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-261">Boolean</span></span>|<span data-ttu-id="8dc76-262">Indica se as contas do Google serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="8dc76-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="8dc76-263">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-263">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="8dc76-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-264">Boolean</span></span>|<span data-ttu-id="8dc76-265">Se o modo de proteção de tela deve ou não ser habilitado ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-265">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-266">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="8dc76-266">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="8dc76-267">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-267">String</span></span>|<span data-ttu-id="8dc76-268">URL de uma imagem que será a proteção de tela do dispositivo no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-268">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-269">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="8dc76-269">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="8dc76-270">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-270">Int32</span></span>|<span data-ttu-id="8dc76-271">O número de segundos que o dispositivo exibirá a proteção de tela no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-271">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="8dc76-272">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="8dc76-272">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="8dc76-273">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="8dc76-273">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="8dc76-274">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-274">Int32</span></span>|<span data-ttu-id="8dc76-275">O número de segundos que o dispositivo precisa estar inativo para que a proteção de tela seja mostrada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-275">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="8dc76-276">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="8dc76-276">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="8dc76-277">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-277">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="8dc76-278">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-278">Boolean</span></span>|<span data-ttu-id="8dc76-279">Se a tela do dispositivo deve ou não mostrar a proteção de tela se áudio/vídeo estiver em execução no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-279">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-280">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="8dc76-280">kioskModeApps</span></span>|<span data-ttu-id="8dc76-281">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-281">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8dc76-282">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-282">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="8dc76-283">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8dc76-283">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8dc76-284">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="8dc76-284">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="8dc76-285">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-285">String</span></span>|<span data-ttu-id="8dc76-286">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-286">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-287">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="8dc76-287">kioskModeExitCode</span></span>|<span data-ttu-id="8dc76-288">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-288">String</span></span>|<span data-ttu-id="8dc76-289">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-289">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-290">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-290">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="8dc76-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-291">Boolean</span></span>|<span data-ttu-id="8dc76-292">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-292">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-293">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="8dc76-293">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="8dc76-294">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="8dc76-294">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="8dc76-295">Indica se o botão de Home virtual é um botão deslizar para cima ou um botão de início flutuante.</span><span class="sxs-lookup"><span data-stu-id="8dc76-295">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="8dc76-296">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-296">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="8dc76-297">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-297">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="8dc76-298">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-298">Boolean</span></span>|<span data-ttu-id="8dc76-299">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-299">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-300">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-300">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="8dc76-301">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-301">Boolean</span></span>|<span data-ttu-id="8dc76-302">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-302">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-303">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-303">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="8dc76-304">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-304">Boolean</span></span>|<span data-ttu-id="8dc76-305">Se permitirá ou não que um usuário use a lanterna no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-305">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-306">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-306">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="8dc76-307">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-307">Boolean</span></span>|<span data-ttu-id="8dc76-308">Se permitirá ou não que um usuário altere o volume de mídia no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-308">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-309">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="8dc76-309">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="8dc76-310">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-310">Boolean</span></span>|<span data-ttu-id="8dc76-311">Se permitirá ou não que um usuário acesse informações básicas de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8dc76-311">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="8dc76-312">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-312">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="8dc76-313">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-313">Boolean</span></span>|<span data-ttu-id="8dc76-314">Se o ponto de entrada de configurações gerenciadas deve ou não ser exibido na tela inicial gerenciada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-314">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-315">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="8dc76-315">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="8dc76-316">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-316">Boolean</span></span>|<span data-ttu-id="8dc76-317">Se permitirá que um usuário acesse facilmente o menu Depurar no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-317">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-318">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="8dc76-318">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="8dc76-319">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-319">Boolean</span></span>|<span data-ttu-id="8dc76-320">Se deve ou não exibir os crachás de notificação de aplicativo no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-320">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="8dc76-321">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="8dc76-321">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="8dc76-322">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="8dc76-322">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="8dc76-323">Configuração de orientação de tela para a tela inicial gerenciada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-323">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="8dc76-324">Os valores possíveis são: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-324">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="8dc76-325">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="8dc76-325">kioskModeIconSize</span></span>|[<span data-ttu-id="8dc76-326">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="8dc76-326">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="8dc76-327">Configuração de tamanho de ícone para a tela inicial gerenciada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-327">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="8dc76-328">Os possíveis valores são: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-328">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="8dc76-329">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="8dc76-329">kioskModeFolderIcon</span></span>|[<span data-ttu-id="8dc76-330">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="8dc76-330">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="8dc76-331">Configuração de ícone de pasta para a tela inicial gerenciada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-331">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="8dc76-332">Os valores possíveis são: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-332">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="8dc76-333">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="8dc76-333">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="8dc76-334">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-334">String collection</span></span>|<span data-ttu-id="8dc76-335">O conjunto restrito de SSIDs WIFI disponíveis para o usuário configurar no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8dc76-335">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="8dc76-336">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8dc76-336">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8dc76-337">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="8dc76-337">microphoneForceMute</span></span>|<span data-ttu-id="8dc76-338">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-338">Boolean</span></span>|<span data-ttu-id="8dc76-339">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-339">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="8dc76-340">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="8dc76-340">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="8dc76-341">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-341">Boolean</span></span>|<span data-ttu-id="8dc76-342">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="8dc76-342">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="8dc76-343">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="8dc76-343">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="8dc76-344">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-344">Boolean</span></span>|<span data-ttu-id="8dc76-345">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-345">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="8dc76-346">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="8dc76-346">passwordBlockKeyguard</span></span>|<span data-ttu-id="8dc76-347">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-347">Boolean</span></span>|<span data-ttu-id="8dc76-348">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="8dc76-348">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="8dc76-349">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="8dc76-349">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="8dc76-350">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-350">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="8dc76-351">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="8dc76-351">List of device keyguard features to block.</span></span> <span data-ttu-id="8dc76-352">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="8dc76-352">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="8dc76-353">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-353">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="8dc76-354">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8dc76-354">passwordExpirationDays</span></span>|<span data-ttu-id="8dc76-355">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-355">Int32</span></span>|<span data-ttu-id="8dc76-356">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="8dc76-356">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="8dc76-357">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="8dc76-357">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8dc76-358">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8dc76-358">passwordMinimumLength</span></span>|<span data-ttu-id="8dc76-359">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-359">Int32</span></span>|<span data-ttu-id="8dc76-360">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-360">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="8dc76-361">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="8dc76-361">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8dc76-362">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="8dc76-362">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="8dc76-363">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-363">Int32</span></span>|<span data-ttu-id="8dc76-364">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-364">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="8dc76-365">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="8dc76-365">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8dc76-366">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="8dc76-366">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="8dc76-367">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-367">Int32</span></span>|<span data-ttu-id="8dc76-368">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-368">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="8dc76-369">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="8dc76-369">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8dc76-370">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="8dc76-370">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="8dc76-371">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-371">Int32</span></span>|<span data-ttu-id="8dc76-372">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-372">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="8dc76-373">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="8dc76-373">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8dc76-374">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="8dc76-374">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="8dc76-375">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-375">Int32</span></span>|<span data-ttu-id="8dc76-376">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-376">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="8dc76-377">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="8dc76-377">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8dc76-378">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="8dc76-378">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="8dc76-379">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-379">Int32</span></span>|<span data-ttu-id="8dc76-380">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-380">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="8dc76-381">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="8dc76-381">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8dc76-382">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="8dc76-382">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="8dc76-383">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-383">Int32</span></span>|<span data-ttu-id="8dc76-384">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-384">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="8dc76-385">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="8dc76-385">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8dc76-386">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8dc76-386">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8dc76-387">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-387">Int32</span></span>|<span data-ttu-id="8dc76-388">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="8dc76-388">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8dc76-389">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="8dc76-389">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="8dc76-390">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-390">Int32</span></span>|<span data-ttu-id="8dc76-391">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="8dc76-391">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="8dc76-392">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="8dc76-392">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8dc76-393">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8dc76-393">passwordRequiredType</span></span>|[<span data-ttu-id="8dc76-394">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8dc76-394">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="8dc76-395">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-395">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="8dc76-396">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-396">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="8dc76-397">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8dc76-397">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8dc76-398">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-398">Int32</span></span>|<span data-ttu-id="8dc76-399">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-399">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="8dc76-400">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="8dc76-400">Valid values 4 to 11</span></span>|
|<span data-ttu-id="8dc76-401">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="8dc76-401">playStoreMode</span></span>|[<span data-ttu-id="8dc76-402">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="8dc76-402">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="8dc76-403">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-403">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="8dc76-404">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-404">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="8dc76-405">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-405">safeBootBlocked</span></span>|<span data-ttu-id="8dc76-406">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-406">Boolean</span></span>|<span data-ttu-id="8dc76-407">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-407">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="8dc76-408">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-408">screenCaptureBlocked</span></span>|<span data-ttu-id="8dc76-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dc76-409">Boolean</span></span>|<span data-ttu-id="8dc76-410">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-410">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="8dc76-411">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="8dc76-411">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="8dc76-412">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-412">Boolean</span></span>|<span data-ttu-id="8dc76-413">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8dc76-413">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="8dc76-414">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8dc76-414">securityRequireVerifyApps</span></span>|<span data-ttu-id="8dc76-415">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-415">Boolean</span></span>|<span data-ttu-id="8dc76-416">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="8dc76-416">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="8dc76-417">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-417">statusBarBlocked</span></span>|<span data-ttu-id="8dc76-418">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-418">Boolean</span></span>|<span data-ttu-id="8dc76-419">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="8dc76-419">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="8dc76-420">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="8dc76-420">stayOnModes</span></span>|<span data-ttu-id="8dc76-421">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="8dc76-421">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="8dc76-422">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-422">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="8dc76-423">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="8dc76-423">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="8dc76-424">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-424">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="8dc76-425">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="8dc76-425">storageAllowUsb</span></span>|<span data-ttu-id="8dc76-426">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-426">Boolean</span></span>|<span data-ttu-id="8dc76-427">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="8dc76-427">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="8dc76-428">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="8dc76-428">storageBlockExternalMedia</span></span>|<span data-ttu-id="8dc76-429">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-429">Boolean</span></span>|<span data-ttu-id="8dc76-430">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-430">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="8dc76-431">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="8dc76-431">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="8dc76-432">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-432">Boolean</span></span>|<span data-ttu-id="8dc76-433">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-433">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="8dc76-434">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="8dc76-434">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="8dc76-435">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-435">Int32</span></span>|<span data-ttu-id="8dc76-436">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-436">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="8dc76-437">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="8dc76-437">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8dc76-438">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="8dc76-438">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="8dc76-439">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc76-439">Int32</span></span>|<span data-ttu-id="8dc76-440">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="8dc76-440">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="8dc76-441">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="8dc76-441">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8dc76-442">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="8dc76-442">systemUpdateInstallType</span></span>|[<span data-ttu-id="8dc76-443">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="8dc76-443">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="8dc76-444">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="8dc76-444">The type of system update configuration.</span></span> <span data-ttu-id="8dc76-445">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="8dc76-445">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="8dc76-446">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="8dc76-446">systemWindowsBlocked</span></span>|<span data-ttu-id="8dc76-447">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-447">Boolean</span></span>|<span data-ttu-id="8dc76-448">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="8dc76-448">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="8dc76-449">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="8dc76-449">usersBlockAdd</span></span>|<span data-ttu-id="8dc76-450">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-450">Boolean</span></span>|<span data-ttu-id="8dc76-451">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="8dc76-451">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="8dc76-452">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="8dc76-452">usersBlockRemove</span></span>|<span data-ttu-id="8dc76-453">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-453">Boolean</span></span>|<span data-ttu-id="8dc76-454">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-454">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="8dc76-455">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="8dc76-455">volumeBlockAdjustment</span></span>|<span data-ttu-id="8dc76-456">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-456">Boolean</span></span>|<span data-ttu-id="8dc76-457">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="8dc76-457">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="8dc76-458">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="8dc76-458">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="8dc76-459">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-459">Boolean</span></span>|<span data-ttu-id="8dc76-460">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="8dc76-460">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="8dc76-461">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="8dc76-461">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="8dc76-462">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dc76-462">String</span></span>|<span data-ttu-id="8dc76-463">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="8dc76-463">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="8dc76-464">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="8dc76-464">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="8dc76-465">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-465">Boolean</span></span>|<span data-ttu-id="8dc76-466">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="8dc76-466">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="8dc76-467">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="8dc76-467">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="8dc76-468">Booliano</span><span class="sxs-lookup"><span data-stu-id="8dc76-468">Boolean</span></span>|<span data-ttu-id="8dc76-469">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="8dc76-469">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8dc76-470">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dc76-470">Response</span></span>
<span data-ttu-id="8dc76-471">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dc76-471">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dc76-472">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dc76-472">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dc76-473">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc76-473">Request</span></span>
<span data-ttu-id="8dc76-474">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dc76-474">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5359

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
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
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
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
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
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="8dc76-475">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dc76-475">Response</span></span>
<span data-ttu-id="8dc76-p143">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dc76-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5531

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
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
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
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
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
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```



