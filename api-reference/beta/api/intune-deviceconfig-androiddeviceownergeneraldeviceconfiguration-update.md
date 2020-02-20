---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dbd3350a23f805caddb7b9ce22f0b812a4efd9e2
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160260"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="5c762-103">Atualizar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c762-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="5c762-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c762-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c762-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c762-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c762-106">Atualiza as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5c762-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c762-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c762-107">Prerequisites</span></span>
<span data-ttu-id="5c762-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c762-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c762-110">Permission type</span></span>|<span data-ttu-id="5c762-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c762-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c762-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c762-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c762-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c762-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c762-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c762-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c762-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c762-115">Not supported.</span></span>|
|<span data-ttu-id="5c762-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c762-116">Application</span></span>|<span data-ttu-id="5c762-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c762-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c762-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c762-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5c762-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c762-119">Request headers</span></span>
|<span data-ttu-id="5c762-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c762-120">Header</span></span>|<span data-ttu-id="5c762-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5c762-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c762-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c762-122">Authorization</span></span>|<span data-ttu-id="5c762-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c762-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c762-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c762-124">Accept</span></span>|<span data-ttu-id="5c762-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c762-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c762-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c762-126">Request body</span></span>
<span data-ttu-id="5c762-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5c762-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="5c762-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c762-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="5c762-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c762-129">Property</span></span>|<span data-ttu-id="5c762-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c762-130">Type</span></span>|<span data-ttu-id="5c762-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c762-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c762-132">id</span><span class="sxs-lookup"><span data-stu-id="5c762-132">id</span></span>|<span data-ttu-id="5c762-133">String</span><span class="sxs-lookup"><span data-stu-id="5c762-133">String</span></span>|<span data-ttu-id="5c762-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5c762-134">Key of the entity.</span></span> <span data-ttu-id="5c762-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c762-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5c762-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c762-137">DateTimeOffset</span></span>|<span data-ttu-id="5c762-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5c762-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5c762-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c762-140">roleScopeTagIds</span></span>|<span data-ttu-id="5c762-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c762-141">String collection</span></span>|<span data-ttu-id="5c762-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5c762-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c762-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5c762-144">supportsScopeTags</span></span>|<span data-ttu-id="5c762-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-145">Boolean</span></span>|<span data-ttu-id="5c762-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5c762-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5c762-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5c762-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5c762-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5c762-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5c762-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c762-149">This property is read-only.</span></span> <span data-ttu-id="5c762-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5c762-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5c762-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5c762-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5c762-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5c762-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5c762-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5c762-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5c762-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5c762-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5c762-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5c762-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5c762-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5c762-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5c762-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5c762-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5c762-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5c762-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5c762-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c762-163">createdDateTime</span></span>|<span data-ttu-id="5c762-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c762-164">DateTimeOffset</span></span>|<span data-ttu-id="5c762-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5c762-165">DateTime the object was created.</span></span> <span data-ttu-id="5c762-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-167">descrição</span><span class="sxs-lookup"><span data-stu-id="5c762-167">description</span></span>|<span data-ttu-id="5c762-168">String</span><span class="sxs-lookup"><span data-stu-id="5c762-168">String</span></span>|<span data-ttu-id="5c762-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c762-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5c762-171">displayName</span></span>|<span data-ttu-id="5c762-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c762-172">String</span></span>|<span data-ttu-id="5c762-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c762-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-175">versão</span><span class="sxs-lookup"><span data-stu-id="5c762-175">version</span></span>|<span data-ttu-id="5c762-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-176">Int32</span></span>|<span data-ttu-id="5c762-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-177">Version of the device configuration.</span></span> <span data-ttu-id="5c762-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c762-179">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="5c762-179">accountsBlockModification</span></span>|<span data-ttu-id="5c762-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-180">Boolean</span></span>|<span data-ttu-id="5c762-181">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="5c762-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="5c762-182">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="5c762-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="5c762-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-183">Boolean</span></span>|<span data-ttu-id="5c762-184">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="5c762-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="5c762-185">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="5c762-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="5c762-186">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="5c762-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="5c762-187">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c762-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="5c762-188">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="5c762-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="5c762-189">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="5c762-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="5c762-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="5c762-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="5c762-191">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="5c762-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="5c762-192">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="5c762-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="5c762-193">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="5c762-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="5c762-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-194">Boolean</span></span>|<span data-ttu-id="5c762-195">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="5c762-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="5c762-196">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c762-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="5c762-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-197">Boolean</span></span>|<span data-ttu-id="5c762-198">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="5c762-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="5c762-199">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="5c762-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="5c762-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-200">Boolean</span></span>|<span data-ttu-id="5c762-201">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="5c762-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="5c762-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-202">cameraBlocked</span></span>|<span data-ttu-id="5c762-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-203">Boolean</span></span>|<span data-ttu-id="5c762-204">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="5c762-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="5c762-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="5c762-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="5c762-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c762-206">Boolean</span></span>|<span data-ttu-id="5c762-207">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="5c762-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="5c762-208">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="5c762-208">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="5c762-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-209">Boolean</span></span>|<span data-ttu-id="5c762-210">Indica se os usuários devem ou não ser bloqueados de qualquer configuração de credencial de certificado.</span><span class="sxs-lookup"><span data-stu-id="5c762-210">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="5c762-211">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-211">dataRoamingBlocked</span></span>|<span data-ttu-id="5c762-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-212">Boolean</span></span>|<span data-ttu-id="5c762-213">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="5c762-213">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="5c762-214">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-214">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="5c762-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-215">Boolean</span></span>|<span data-ttu-id="5c762-216">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c762-216">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="5c762-217">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="5c762-217">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="5c762-218">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c762-218">String collection</span></span>|<span data-ttu-id="5c762-219">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="5c762-219">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="5c762-220">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-220">factoryResetBlocked</span></span>|<span data-ttu-id="5c762-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c762-221">Boolean</span></span>|<span data-ttu-id="5c762-222">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="5c762-222">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="5c762-223">globalProxy</span><span class="sxs-lookup"><span data-stu-id="5c762-223">globalProxy</span></span>|[<span data-ttu-id="5c762-224">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="5c762-224">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="5c762-225">O proxy é configurado diretamente com hosts, porta e hosts excluídos.</span><span class="sxs-lookup"><span data-stu-id="5c762-225">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="5c762-226">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-226">googleAccountsBlocked</span></span>|<span data-ttu-id="5c762-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-227">Boolean</span></span>|<span data-ttu-id="5c762-228">Indica se as contas do Google serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="5c762-228">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="5c762-229">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5c762-229">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="5c762-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-230">Boolean</span></span>|<span data-ttu-id="5c762-231">Se o modo de proteção de tela deve ou não ser habilitado ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-231">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-232">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="5c762-232">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="5c762-233">String</span><span class="sxs-lookup"><span data-stu-id="5c762-233">String</span></span>|<span data-ttu-id="5c762-234">URL de uma imagem que será a proteção de tela do dispositivo no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-234">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-235">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="5c762-235">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="5c762-236">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-236">Int32</span></span>|<span data-ttu-id="5c762-237">O número de segundos que o dispositivo exibirá a proteção de tela no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-237">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="5c762-238">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="5c762-238">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="5c762-239">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="5c762-239">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="5c762-240">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-240">Int32</span></span>|<span data-ttu-id="5c762-241">O número de segundos que o dispositivo precisa estar inativo para que a proteção de tela seja mostrada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-241">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="5c762-242">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="5c762-242">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="5c762-243">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="5c762-243">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="5c762-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-244">Boolean</span></span>|<span data-ttu-id="5c762-245">Se a tela do dispositivo deve ou não mostrar a proteção de tela se áudio/vídeo estiver em execução no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-245">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-246">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="5c762-246">kioskModeApps</span></span>|<span data-ttu-id="5c762-247">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-247">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5c762-248">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-248">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="5c762-249">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5c762-249">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5c762-250">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="5c762-250">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="5c762-251">String</span><span class="sxs-lookup"><span data-stu-id="5c762-251">String</span></span>|<span data-ttu-id="5c762-252">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-252">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-253">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="5c762-253">kioskModeExitCode</span></span>|<span data-ttu-id="5c762-254">String</span><span class="sxs-lookup"><span data-stu-id="5c762-254">String</span></span>|<span data-ttu-id="5c762-255">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-255">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-256">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="5c762-256">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="5c762-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-257">Boolean</span></span>|<span data-ttu-id="5c762-258">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-258">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-259">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="5c762-259">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="5c762-260">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="5c762-260">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="5c762-261">Indica se o botão de Home virtual é um botão deslizar para cima ou um botão de início flutuante.</span><span class="sxs-lookup"><span data-stu-id="5c762-261">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="5c762-262">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="5c762-262">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="5c762-263">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5c762-263">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="5c762-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-264">Boolean</span></span>|<span data-ttu-id="5c762-265">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-265">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-266">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5c762-266">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="5c762-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-267">Boolean</span></span>|<span data-ttu-id="5c762-268">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-268">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-269">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5c762-269">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="5c762-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-270">Boolean</span></span>|<span data-ttu-id="5c762-271">Se permitirá ou não que um usuário use a lanterna no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-271">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-272">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="5c762-272">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="5c762-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-273">Boolean</span></span>|<span data-ttu-id="5c762-274">Se permitirá ou não que um usuário altere o volume de mídia no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="5c762-274">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="5c762-275">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="5c762-275">microphoneForceMute</span></span>|<span data-ttu-id="5c762-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-276">Boolean</span></span>|<span data-ttu-id="5c762-277">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="5c762-277">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="5c762-278">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="5c762-278">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="5c762-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-279">Boolean</span></span>|<span data-ttu-id="5c762-280">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="5c762-280">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="5c762-281">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="5c762-281">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="5c762-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-282">Boolean</span></span>|<span data-ttu-id="5c762-283">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="5c762-283">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="5c762-284">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="5c762-284">passwordBlockKeyguard</span></span>|<span data-ttu-id="5c762-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-285">Boolean</span></span>|<span data-ttu-id="5c762-286">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="5c762-286">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="5c762-287">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="5c762-287">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="5c762-288">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-288">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="5c762-289">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="5c762-289">List of device keyguard features to block.</span></span> <span data-ttu-id="5c762-290">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="5c762-290">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="5c762-291">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="5c762-291">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="5c762-292">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5c762-292">passwordExpirationDays</span></span>|<span data-ttu-id="5c762-293">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-293">Int32</span></span>|<span data-ttu-id="5c762-294">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="5c762-294">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="5c762-295">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="5c762-295">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5c762-296">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5c762-296">passwordMinimumLength</span></span>|<span data-ttu-id="5c762-297">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-297">Int32</span></span>|<span data-ttu-id="5c762-298">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-298">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="5c762-299">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="5c762-299">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5c762-300">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="5c762-300">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="5c762-301">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-301">Int32</span></span>|<span data-ttu-id="5c762-302">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-302">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="5c762-303">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5c762-303">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5c762-304">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="5c762-304">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="5c762-305">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-305">Int32</span></span>|<span data-ttu-id="5c762-306">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-306">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="5c762-307">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5c762-307">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5c762-308">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="5c762-308">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="5c762-309">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-309">Int32</span></span>|<span data-ttu-id="5c762-310">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-310">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="5c762-311">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5c762-311">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5c762-312">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="5c762-312">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="5c762-313">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-313">Int32</span></span>|<span data-ttu-id="5c762-314">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-314">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="5c762-315">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5c762-315">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5c762-316">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="5c762-316">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="5c762-317">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-317">Int32</span></span>|<span data-ttu-id="5c762-318">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-318">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="5c762-319">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5c762-319">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5c762-320">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="5c762-320">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="5c762-321">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-321">Int32</span></span>|<span data-ttu-id="5c762-322">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-322">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="5c762-323">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5c762-323">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5c762-324">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="5c762-324">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="5c762-325">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-325">Int32</span></span>|<span data-ttu-id="5c762-326">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="5c762-326">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="5c762-327">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="5c762-327">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="5c762-328">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-328">Int32</span></span>|<span data-ttu-id="5c762-329">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="5c762-329">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="5c762-330">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="5c762-330">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5c762-331">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5c762-331">passwordRequiredType</span></span>|[<span data-ttu-id="5c762-332">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5c762-332">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="5c762-333">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-333">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="5c762-334">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="5c762-334">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="5c762-335">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="5c762-335">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="5c762-336">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-336">Int32</span></span>|<span data-ttu-id="5c762-337">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="5c762-337">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="5c762-338">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="5c762-338">Valid values 4 to 11</span></span>|
|<span data-ttu-id="5c762-339">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="5c762-339">playStoreMode</span></span>|[<span data-ttu-id="5c762-340">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="5c762-340">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="5c762-341">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-341">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="5c762-342">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="5c762-342">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="5c762-343">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-343">safeBootBlocked</span></span>|<span data-ttu-id="5c762-344">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-344">Boolean</span></span>|<span data-ttu-id="5c762-345">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="5c762-345">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="5c762-346">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-346">screenCaptureBlocked</span></span>|<span data-ttu-id="5c762-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c762-347">Boolean</span></span>|<span data-ttu-id="5c762-348">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="5c762-348">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="5c762-349">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="5c762-349">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="5c762-350">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-350">Boolean</span></span>|<span data-ttu-id="5c762-351">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c762-351">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="5c762-352">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="5c762-352">securityRequireVerifyApps</span></span>|<span data-ttu-id="5c762-353">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-353">Boolean</span></span>|<span data-ttu-id="5c762-354">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="5c762-354">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="5c762-355">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-355">statusBarBlocked</span></span>|<span data-ttu-id="5c762-356">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-356">Boolean</span></span>|<span data-ttu-id="5c762-357">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="5c762-357">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="5c762-358">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="5c762-358">stayOnModes</span></span>|<span data-ttu-id="5c762-359">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="5c762-359">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="5c762-360">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="5c762-360">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="5c762-361">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="5c762-361">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="5c762-362">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="5c762-362">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="5c762-363">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="5c762-363">storageAllowUsb</span></span>|<span data-ttu-id="5c762-364">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-364">Boolean</span></span>|<span data-ttu-id="5c762-365">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="5c762-365">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="5c762-366">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="5c762-366">storageBlockExternalMedia</span></span>|<span data-ttu-id="5c762-367">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-367">Boolean</span></span>|<span data-ttu-id="5c762-368">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="5c762-368">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="5c762-369">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="5c762-369">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="5c762-370">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-370">Boolean</span></span>|<span data-ttu-id="5c762-371">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="5c762-371">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="5c762-372">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="5c762-372">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="5c762-373">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-373">Int32</span></span>|<span data-ttu-id="5c762-374">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="5c762-374">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="5c762-375">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="5c762-375">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="5c762-376">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="5c762-376">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="5c762-377">Int32</span><span class="sxs-lookup"><span data-stu-id="5c762-377">Int32</span></span>|<span data-ttu-id="5c762-378">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="5c762-378">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="5c762-379">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="5c762-379">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="5c762-380">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="5c762-380">systemUpdateInstallType</span></span>|[<span data-ttu-id="5c762-381">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="5c762-381">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="5c762-382">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="5c762-382">The type of system update configuration.</span></span> <span data-ttu-id="5c762-383">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="5c762-383">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="5c762-384">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="5c762-384">systemWindowsBlocked</span></span>|<span data-ttu-id="5c762-385">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-385">Boolean</span></span>|<span data-ttu-id="5c762-386">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="5c762-386">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="5c762-387">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="5c762-387">usersBlockAdd</span></span>|<span data-ttu-id="5c762-388">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-388">Boolean</span></span>|<span data-ttu-id="5c762-389">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="5c762-389">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="5c762-390">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="5c762-390">usersBlockRemove</span></span>|<span data-ttu-id="5c762-391">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-391">Boolean</span></span>|<span data-ttu-id="5c762-392">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="5c762-392">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="5c762-393">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="5c762-393">volumeBlockAdjustment</span></span>|<span data-ttu-id="5c762-394">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-394">Boolean</span></span>|<span data-ttu-id="5c762-395">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="5c762-395">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="5c762-396">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="5c762-396">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="5c762-397">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-397">Boolean</span></span>|<span data-ttu-id="5c762-398">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="5c762-398">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="5c762-399">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="5c762-399">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="5c762-400">String</span><span class="sxs-lookup"><span data-stu-id="5c762-400">String</span></span>|<span data-ttu-id="5c762-401">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="5c762-401">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="5c762-402">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="5c762-402">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="5c762-403">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-403">Boolean</span></span>|<span data-ttu-id="5c762-404">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="5c762-404">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="5c762-405">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="5c762-405">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="5c762-406">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c762-406">Boolean</span></span>|<span data-ttu-id="5c762-407">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="5c762-407">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="5c762-408">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c762-408">Response</span></span>
<span data-ttu-id="5c762-409">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c762-409">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c762-410">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c762-410">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c762-411">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c762-411">Request</span></span>
<span data-ttu-id="5c762-412">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c762-412">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4374

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

### <a name="response"></a><span data-ttu-id="5c762-413">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c762-413">Response</span></span>
<span data-ttu-id="5c762-p136">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c762-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4546

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





