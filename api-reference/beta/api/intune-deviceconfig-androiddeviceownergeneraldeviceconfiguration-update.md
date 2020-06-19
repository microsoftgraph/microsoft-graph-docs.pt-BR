---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc6746dca524394be358d1a4c31fc5cfe53c001b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793112"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="16f28-103">Atualizar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="16f28-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="16f28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16f28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16f28-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16f28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16f28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16f28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16f28-107">Atualiza as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="16f28-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16f28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16f28-108">Prerequisites</span></span>
<span data-ttu-id="16f28-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="16f28-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="16f28-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16f28-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16f28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16f28-111">Permission type</span></span>|<span data-ttu-id="16f28-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16f28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16f28-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16f28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16f28-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16f28-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16f28-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16f28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16f28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16f28-116">Not supported.</span></span>|
|<span data-ttu-id="16f28-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16f28-117">Application</span></span>|<span data-ttu-id="16f28-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16f28-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16f28-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16f28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="16f28-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16f28-120">Request headers</span></span>
|<span data-ttu-id="16f28-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16f28-121">Header</span></span>|<span data-ttu-id="16f28-122">Valor</span><span class="sxs-lookup"><span data-stu-id="16f28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16f28-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="16f28-123">Authorization</span></span>|<span data-ttu-id="16f28-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16f28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16f28-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16f28-125">Accept</span></span>|<span data-ttu-id="16f28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16f28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16f28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16f28-127">Request body</span></span>
<span data-ttu-id="16f28-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="16f28-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="16f28-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16f28-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="16f28-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16f28-130">Property</span></span>|<span data-ttu-id="16f28-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="16f28-131">Type</span></span>|<span data-ttu-id="16f28-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="16f28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16f28-133">id</span><span class="sxs-lookup"><span data-stu-id="16f28-133">id</span></span>|<span data-ttu-id="16f28-134">String</span><span class="sxs-lookup"><span data-stu-id="16f28-134">String</span></span>|<span data-ttu-id="16f28-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16f28-135">Key of the entity.</span></span> <span data-ttu-id="16f28-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16f28-137">lastModifiedDateTime</span></span>|<span data-ttu-id="16f28-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16f28-138">DateTimeOffset</span></span>|<span data-ttu-id="16f28-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="16f28-139">DateTime the object was last modified.</span></span> <span data-ttu-id="16f28-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16f28-141">roleScopeTagIds</span></span>|<span data-ttu-id="16f28-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="16f28-142">String collection</span></span>|<span data-ttu-id="16f28-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="16f28-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="16f28-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="16f28-145">supportsScopeTags</span></span>|<span data-ttu-id="16f28-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-146">Boolean</span></span>|<span data-ttu-id="16f28-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="16f28-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="16f28-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="16f28-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="16f28-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="16f28-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="16f28-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16f28-150">This property is read-only.</span></span> <span data-ttu-id="16f28-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="16f28-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="16f28-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="16f28-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="16f28-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="16f28-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="16f28-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="16f28-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="16f28-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="16f28-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="16f28-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="16f28-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="16f28-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="16f28-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="16f28-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="16f28-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="16f28-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="16f28-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="16f28-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16f28-164">createdDateTime</span></span>|<span data-ttu-id="16f28-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16f28-165">DateTimeOffset</span></span>|<span data-ttu-id="16f28-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="16f28-166">DateTime the object was created.</span></span> <span data-ttu-id="16f28-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-168">description</span><span class="sxs-lookup"><span data-stu-id="16f28-168">description</span></span>|<span data-ttu-id="16f28-169">String</span><span class="sxs-lookup"><span data-stu-id="16f28-169">String</span></span>|<span data-ttu-id="16f28-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16f28-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-172">displayName</span><span class="sxs-lookup"><span data-stu-id="16f28-172">displayName</span></span>|<span data-ttu-id="16f28-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16f28-173">String</span></span>|<span data-ttu-id="16f28-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16f28-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-176">versão</span><span class="sxs-lookup"><span data-stu-id="16f28-176">version</span></span>|<span data-ttu-id="16f28-177">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-177">Int32</span></span>|<span data-ttu-id="16f28-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-178">Version of the device configuration.</span></span> <span data-ttu-id="16f28-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16f28-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="16f28-180">accountsBlockModification</span></span>|<span data-ttu-id="16f28-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-181">Boolean</span></span>|<span data-ttu-id="16f28-182">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="16f28-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="16f28-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="16f28-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="16f28-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-184">Boolean</span></span>|<span data-ttu-id="16f28-185">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="16f28-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="16f28-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="16f28-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="16f28-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="16f28-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="16f28-188">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="16f28-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="16f28-189">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="16f28-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="16f28-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="16f28-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="16f28-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="16f28-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="16f28-192">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="16f28-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="16f28-193">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="16f28-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="16f28-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="16f28-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="16f28-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-195">Boolean</span></span>|<span data-ttu-id="16f28-196">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="16f28-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="16f28-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="16f28-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="16f28-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-198">Boolean</span></span>|<span data-ttu-id="16f28-199">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="16f28-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="16f28-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="16f28-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="16f28-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-201">Boolean</span></span>|<span data-ttu-id="16f28-202">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="16f28-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="16f28-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-203">cameraBlocked</span></span>|<span data-ttu-id="16f28-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-204">Boolean</span></span>|<span data-ttu-id="16f28-205">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="16f28-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="16f28-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="16f28-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="16f28-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-207">Boolean</span></span>|<span data-ttu-id="16f28-208">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="16f28-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="16f28-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="16f28-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="16f28-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-210">Boolean</span></span>|<span data-ttu-id="16f28-211">Indica se os usuários devem ou não ser bloqueados de qualquer configuração de credencial de certificado.</span><span class="sxs-lookup"><span data-stu-id="16f28-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="16f28-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="16f28-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-213">Boolean</span></span>|<span data-ttu-id="16f28-214">Indica se você deseja ou não configurar o iniciador Microsoft.</span><span class="sxs-lookup"><span data-stu-id="16f28-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="16f28-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="16f28-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-216">Boolean</span></span>|<span data-ttu-id="16f28-217">Indica se o papel de parede deve ou não ser configurado nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="16f28-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="16f28-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="16f28-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="16f28-219">String</span><span class="sxs-lookup"><span data-stu-id="16f28-219">String</span></span>|<span data-ttu-id="16f28-220">Indica a URL do arquivo de imagem a ser usado como papel de parede nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="16f28-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="16f28-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="16f28-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="16f28-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-222">Boolean</span></span>|<span data-ttu-id="16f28-223">Indica se o usuário pode ou não modificar o papel de parede para personalizar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="16f28-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="16f28-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-225">Boolean</span></span>|<span data-ttu-id="16f28-226">Indica se você deseja ou não habilitar o feed do inicializador no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="16f28-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="16f28-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="16f28-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-228">Boolean</span></span>|<span data-ttu-id="16f28-229">Indica se o usuário pode ou não modificar o feed do inicializador no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="16f28-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="16f28-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="16f28-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="16f28-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="16f28-232">Indica se você deseja ou não configurar o encaixe de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="16f28-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="16f28-233">Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="16f28-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="16f28-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="16f28-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="16f28-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-235">Boolean</span></span>|<span data-ttu-id="16f28-236">Indica se o usuário pode ou não modificar a configuração de encaixe do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="16f28-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="16f28-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="16f28-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="16f28-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="16f28-239">Indica a configuração de posicionamento da barra de pesquisa no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="16f28-240">Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="16f28-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="16f28-241">microsoftLauncherSearchBarPlacementAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="16f28-241">microsoftLauncherSearchBarPlacementAllowUserModification</span></span>|<span data-ttu-id="16f28-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-242">Boolean</span></span>|<span data-ttu-id="16f28-243">Indica se o usuário pode modificar o posicionamento da barra de pesquisa no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-243">Indicates whether the user can modify the search bar placement on the device.</span></span>|
|<span data-ttu-id="16f28-244">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="16f28-244">enrollmentProfile</span></span>|[<span data-ttu-id="16f28-245">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="16f28-245">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="16f28-246">Indica o perfil de registro que você deseja configurar.</span><span class="sxs-lookup"><span data-stu-id="16f28-246">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="16f28-247">Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="16f28-247">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="16f28-248">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-248">dataRoamingBlocked</span></span>|<span data-ttu-id="16f28-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-249">Boolean</span></span>|<span data-ttu-id="16f28-250">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="16f28-250">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="16f28-251">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-251">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="16f28-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-252">Boolean</span></span>|<span data-ttu-id="16f28-253">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="16f28-253">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="16f28-254">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="16f28-254">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="16f28-255">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="16f28-255">String collection</span></span>|<span data-ttu-id="16f28-256">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="16f28-256">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="16f28-257">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-257">factoryResetBlocked</span></span>|<span data-ttu-id="16f28-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-258">Boolean</span></span>|<span data-ttu-id="16f28-259">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="16f28-259">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="16f28-260">globalProxy</span><span class="sxs-lookup"><span data-stu-id="16f28-260">globalProxy</span></span>|[<span data-ttu-id="16f28-261">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="16f28-261">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="16f28-262">O proxy é configurado diretamente com hosts, porta e hosts excluídos.</span><span class="sxs-lookup"><span data-stu-id="16f28-262">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="16f28-263">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-263">googleAccountsBlocked</span></span>|<span data-ttu-id="16f28-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-264">Boolean</span></span>|<span data-ttu-id="16f28-265">Indica se as contas do Google serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="16f28-265">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="16f28-266">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-266">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="16f28-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-267">Boolean</span></span>|<span data-ttu-id="16f28-268">Se o modo de proteção de tela deve ou não ser habilitado ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-268">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-269">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="16f28-269">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="16f28-270">String</span><span class="sxs-lookup"><span data-stu-id="16f28-270">String</span></span>|<span data-ttu-id="16f28-271">URL de uma imagem que será a proteção de tela do dispositivo no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-271">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-272">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="16f28-272">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="16f28-273">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-273">Int32</span></span>|<span data-ttu-id="16f28-274">O número de segundos que o dispositivo exibirá a proteção de tela no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-274">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="16f28-275">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="16f28-275">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="16f28-276">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="16f28-276">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="16f28-277">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-277">Int32</span></span>|<span data-ttu-id="16f28-278">O número de segundos que o dispositivo precisa estar inativo para que a proteção de tela seja mostrada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-278">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="16f28-279">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="16f28-279">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="16f28-280">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="16f28-280">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="16f28-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-281">Boolean</span></span>|<span data-ttu-id="16f28-282">Se a tela do dispositivo deve ou não mostrar a proteção de tela se áudio/vídeo estiver em execução no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-282">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-283">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="16f28-283">kioskModeApps</span></span>|<span data-ttu-id="16f28-284">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-284">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="16f28-285">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-285">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="16f28-286">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="16f28-286">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="16f28-287">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="16f28-287">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="16f28-288">String</span><span class="sxs-lookup"><span data-stu-id="16f28-288">String</span></span>|<span data-ttu-id="16f28-289">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-289">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-290">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="16f28-290">kioskModeExitCode</span></span>|<span data-ttu-id="16f28-291">String</span><span class="sxs-lookup"><span data-stu-id="16f28-291">String</span></span>|<span data-ttu-id="16f28-292">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-292">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-293">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-293">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="16f28-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-294">Boolean</span></span>|<span data-ttu-id="16f28-295">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-295">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-296">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="16f28-296">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="16f28-297">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="16f28-297">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="16f28-298">Indica se o botão de Home virtual é um botão deslizar para cima ou um botão de início flutuante.</span><span class="sxs-lookup"><span data-stu-id="16f28-298">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="16f28-299">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="16f28-299">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="16f28-300">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-300">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="16f28-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-301">Boolean</span></span>|<span data-ttu-id="16f28-302">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-302">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-303">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-303">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="16f28-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-304">Boolean</span></span>|<span data-ttu-id="16f28-305">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-305">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-306">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-306">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="16f28-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-307">Boolean</span></span>|<span data-ttu-id="16f28-308">Se permitirá ou não que um usuário use a lanterna no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-308">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-309">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="16f28-309">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="16f28-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-310">Boolean</span></span>|<span data-ttu-id="16f28-311">Se permitirá ou não que um usuário altere o volume de mídia no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="16f28-311">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="16f28-312">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="16f28-312">microphoneForceMute</span></span>|<span data-ttu-id="16f28-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-313">Boolean</span></span>|<span data-ttu-id="16f28-314">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="16f28-314">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="16f28-315">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="16f28-315">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="16f28-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-316">Boolean</span></span>|<span data-ttu-id="16f28-317">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="16f28-317">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="16f28-318">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="16f28-318">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="16f28-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-319">Boolean</span></span>|<span data-ttu-id="16f28-320">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="16f28-320">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="16f28-321">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="16f28-321">passwordBlockKeyguard</span></span>|<span data-ttu-id="16f28-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-322">Boolean</span></span>|<span data-ttu-id="16f28-323">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="16f28-323">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="16f28-324">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="16f28-324">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="16f28-325">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-325">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="16f28-326">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="16f28-326">List of device keyguard features to block.</span></span> <span data-ttu-id="16f28-327">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="16f28-327">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="16f28-328">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="16f28-328">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="16f28-329">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="16f28-329">passwordExpirationDays</span></span>|<span data-ttu-id="16f28-330">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-330">Int32</span></span>|<span data-ttu-id="16f28-331">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="16f28-331">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="16f28-332">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="16f28-332">Valid values 1 to 365</span></span>|
|<span data-ttu-id="16f28-333">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="16f28-333">passwordMinimumLength</span></span>|<span data-ttu-id="16f28-334">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-334">Int32</span></span>|<span data-ttu-id="16f28-335">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-335">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="16f28-336">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="16f28-336">Valid values 4 to 16</span></span>|
|<span data-ttu-id="16f28-337">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="16f28-337">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="16f28-338">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-338">Int32</span></span>|<span data-ttu-id="16f28-339">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-339">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="16f28-340">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="16f28-340">Valid values 1 to 16</span></span>|
|<span data-ttu-id="16f28-341">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="16f28-341">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="16f28-342">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-342">Int32</span></span>|<span data-ttu-id="16f28-343">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-343">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="16f28-344">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="16f28-344">Valid values 1 to 16</span></span>|
|<span data-ttu-id="16f28-345">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="16f28-345">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="16f28-346">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-346">Int32</span></span>|<span data-ttu-id="16f28-347">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-347">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="16f28-348">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="16f28-348">Valid values 1 to 16</span></span>|
|<span data-ttu-id="16f28-349">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="16f28-349">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="16f28-350">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-350">Int32</span></span>|<span data-ttu-id="16f28-351">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-351">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="16f28-352">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="16f28-352">Valid values 1 to 16</span></span>|
|<span data-ttu-id="16f28-353">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="16f28-353">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="16f28-354">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-354">Int32</span></span>|<span data-ttu-id="16f28-355">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-355">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="16f28-356">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="16f28-356">Valid values 1 to 16</span></span>|
|<span data-ttu-id="16f28-357">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="16f28-357">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="16f28-358">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-358">Int32</span></span>|<span data-ttu-id="16f28-359">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-359">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="16f28-360">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="16f28-360">Valid values 1 to 16</span></span>|
|<span data-ttu-id="16f28-361">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="16f28-361">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="16f28-362">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-362">Int32</span></span>|<span data-ttu-id="16f28-363">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="16f28-363">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="16f28-364">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="16f28-364">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="16f28-365">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-365">Int32</span></span>|<span data-ttu-id="16f28-366">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="16f28-366">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="16f28-367">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="16f28-367">Valid values 0 to 24</span></span>|
|<span data-ttu-id="16f28-368">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="16f28-368">passwordRequiredType</span></span>|[<span data-ttu-id="16f28-369">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="16f28-369">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="16f28-370">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-370">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="16f28-371">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="16f28-371">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="16f28-372">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="16f28-372">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="16f28-373">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-373">Int32</span></span>|<span data-ttu-id="16f28-374">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="16f28-374">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="16f28-375">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="16f28-375">Valid values 4 to 11</span></span>|
|<span data-ttu-id="16f28-376">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="16f28-376">playStoreMode</span></span>|[<span data-ttu-id="16f28-377">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="16f28-377">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="16f28-378">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-378">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="16f28-379">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="16f28-379">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="16f28-380">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-380">safeBootBlocked</span></span>|<span data-ttu-id="16f28-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-381">Boolean</span></span>|<span data-ttu-id="16f28-382">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="16f28-382">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="16f28-383">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-383">screenCaptureBlocked</span></span>|<span data-ttu-id="16f28-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-384">Boolean</span></span>|<span data-ttu-id="16f28-385">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="16f28-385">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="16f28-386">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="16f28-386">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="16f28-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-387">Boolean</span></span>|<span data-ttu-id="16f28-388">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16f28-388">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="16f28-389">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="16f28-389">securityRequireVerifyApps</span></span>|<span data-ttu-id="16f28-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-390">Boolean</span></span>|<span data-ttu-id="16f28-391">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="16f28-391">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="16f28-392">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-392">statusBarBlocked</span></span>|<span data-ttu-id="16f28-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-393">Boolean</span></span>|<span data-ttu-id="16f28-394">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="16f28-394">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="16f28-395">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="16f28-395">stayOnModes</span></span>|<span data-ttu-id="16f28-396">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="16f28-396">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="16f28-397">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="16f28-397">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="16f28-398">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="16f28-398">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="16f28-399">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="16f28-399">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="16f28-400">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="16f28-400">storageAllowUsb</span></span>|<span data-ttu-id="16f28-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-401">Boolean</span></span>|<span data-ttu-id="16f28-402">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="16f28-402">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="16f28-403">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="16f28-403">storageBlockExternalMedia</span></span>|<span data-ttu-id="16f28-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-404">Boolean</span></span>|<span data-ttu-id="16f28-405">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="16f28-405">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="16f28-406">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="16f28-406">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="16f28-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-407">Boolean</span></span>|<span data-ttu-id="16f28-408">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="16f28-408">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="16f28-409">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="16f28-409">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="16f28-410">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-410">Int32</span></span>|<span data-ttu-id="16f28-411">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="16f28-411">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="16f28-412">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="16f28-412">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="16f28-413">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="16f28-413">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="16f28-414">Int32</span><span class="sxs-lookup"><span data-stu-id="16f28-414">Int32</span></span>|<span data-ttu-id="16f28-415">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="16f28-415">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="16f28-416">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="16f28-416">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="16f28-417">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="16f28-417">systemUpdateInstallType</span></span>|[<span data-ttu-id="16f28-418">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="16f28-418">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="16f28-419">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="16f28-419">The type of system update configuration.</span></span> <span data-ttu-id="16f28-420">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="16f28-420">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="16f28-421">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="16f28-421">systemWindowsBlocked</span></span>|<span data-ttu-id="16f28-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-422">Boolean</span></span>|<span data-ttu-id="16f28-423">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="16f28-423">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="16f28-424">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="16f28-424">usersBlockAdd</span></span>|<span data-ttu-id="16f28-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-425">Boolean</span></span>|<span data-ttu-id="16f28-426">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="16f28-426">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="16f28-427">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="16f28-427">usersBlockRemove</span></span>|<span data-ttu-id="16f28-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-428">Boolean</span></span>|<span data-ttu-id="16f28-429">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="16f28-429">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="16f28-430">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="16f28-430">volumeBlockAdjustment</span></span>|<span data-ttu-id="16f28-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-431">Boolean</span></span>|<span data-ttu-id="16f28-432">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="16f28-432">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="16f28-433">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="16f28-433">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="16f28-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-434">Boolean</span></span>|<span data-ttu-id="16f28-435">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="16f28-435">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="16f28-436">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="16f28-436">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="16f28-437">String</span><span class="sxs-lookup"><span data-stu-id="16f28-437">String</span></span>|<span data-ttu-id="16f28-438">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="16f28-438">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="16f28-439">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="16f28-439">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="16f28-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-440">Boolean</span></span>|<span data-ttu-id="16f28-441">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="16f28-441">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="16f28-442">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="16f28-442">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="16f28-443">Boolean</span><span class="sxs-lookup"><span data-stu-id="16f28-443">Boolean</span></span>|<span data-ttu-id="16f28-444">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="16f28-444">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="16f28-445">Resposta</span><span class="sxs-lookup"><span data-stu-id="16f28-445">Response</span></span>
<span data-ttu-id="16f28-446">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16f28-446">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16f28-447">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16f28-447">Example</span></span>

### <a name="request"></a><span data-ttu-id="16f28-448">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16f28-448">Request</span></span>
<span data-ttu-id="16f28-449">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16f28-449">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5044

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
  "microsoftLauncherSearchBarPlacementAllowUserModification": true,
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

### <a name="response"></a><span data-ttu-id="16f28-450">Resposta</span><span class="sxs-lookup"><span data-stu-id="16f28-450">Response</span></span>
<span data-ttu-id="16f28-451">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="16f28-451">Here is an example of the response.</span></span> <span data-ttu-id="16f28-452">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="16f28-452">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16f28-453">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="16f28-453">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5216

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
  "microsoftLauncherSearchBarPlacementAllowUserModification": true,
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



