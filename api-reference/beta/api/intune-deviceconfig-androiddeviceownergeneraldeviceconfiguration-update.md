---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c9efd699bcbf1eaf9e968e38d0a7a6f72d5ef4a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450052"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="26efa-103">Atualizar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="26efa-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="26efa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="26efa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26efa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26efa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26efa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26efa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26efa-107">Atualiza as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="26efa-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26efa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26efa-108">Prerequisites</span></span>
<span data-ttu-id="26efa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26efa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26efa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26efa-111">Permission type</span></span>|<span data-ttu-id="26efa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26efa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26efa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26efa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26efa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26efa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26efa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26efa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26efa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26efa-116">Not supported.</span></span>|
|<span data-ttu-id="26efa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26efa-117">Application</span></span>|<span data-ttu-id="26efa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26efa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26efa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26efa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="26efa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26efa-120">Request headers</span></span>
|<span data-ttu-id="26efa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26efa-121">Header</span></span>|<span data-ttu-id="26efa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="26efa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26efa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26efa-123">Authorization</span></span>|<span data-ttu-id="26efa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26efa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26efa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26efa-125">Accept</span></span>|<span data-ttu-id="26efa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26efa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26efa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26efa-127">Request body</span></span>
<span data-ttu-id="26efa-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="26efa-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="26efa-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26efa-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="26efa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26efa-130">Property</span></span>|<span data-ttu-id="26efa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26efa-131">Type</span></span>|<span data-ttu-id="26efa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26efa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26efa-133">id</span><span class="sxs-lookup"><span data-stu-id="26efa-133">id</span></span>|<span data-ttu-id="26efa-134">String</span><span class="sxs-lookup"><span data-stu-id="26efa-134">String</span></span>|<span data-ttu-id="26efa-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26efa-135">Key of the entity.</span></span> <span data-ttu-id="26efa-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26efa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="26efa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26efa-138">DateTimeOffset</span></span>|<span data-ttu-id="26efa-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="26efa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="26efa-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26efa-141">roleScopeTagIds</span></span>|<span data-ttu-id="26efa-142">String collection</span><span class="sxs-lookup"><span data-stu-id="26efa-142">String collection</span></span>|<span data-ttu-id="26efa-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="26efa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26efa-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="26efa-145">supportsScopeTags</span></span>|<span data-ttu-id="26efa-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-146">Boolean</span></span>|<span data-ttu-id="26efa-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="26efa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="26efa-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="26efa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="26efa-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="26efa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="26efa-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26efa-150">This property is read-only.</span></span> <span data-ttu-id="26efa-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26efa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="26efa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26efa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="26efa-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="26efa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="26efa-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26efa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="26efa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26efa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="26efa-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="26efa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="26efa-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="26efa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="26efa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="26efa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="26efa-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="26efa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="26efa-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26efa-164">createdDateTime</span></span>|<span data-ttu-id="26efa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26efa-165">DateTimeOffset</span></span>|<span data-ttu-id="26efa-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="26efa-166">DateTime the object was created.</span></span> <span data-ttu-id="26efa-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-168">description</span><span class="sxs-lookup"><span data-stu-id="26efa-168">description</span></span>|<span data-ttu-id="26efa-169">String</span><span class="sxs-lookup"><span data-stu-id="26efa-169">String</span></span>|<span data-ttu-id="26efa-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26efa-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="26efa-172">displayName</span></span>|<span data-ttu-id="26efa-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26efa-173">String</span></span>|<span data-ttu-id="26efa-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26efa-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-176">versão</span><span class="sxs-lookup"><span data-stu-id="26efa-176">version</span></span>|<span data-ttu-id="26efa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-177">Int32</span></span>|<span data-ttu-id="26efa-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-178">Version of the device configuration.</span></span> <span data-ttu-id="26efa-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26efa-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="26efa-180">accountsBlockModification</span></span>|<span data-ttu-id="26efa-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-181">Boolean</span></span>|<span data-ttu-id="26efa-182">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="26efa-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="26efa-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="26efa-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="26efa-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-184">Boolean</span></span>|<span data-ttu-id="26efa-185">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="26efa-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="26efa-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="26efa-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="26efa-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="26efa-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="26efa-188">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="26efa-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="26efa-189">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="26efa-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="26efa-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="26efa-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="26efa-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="26efa-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="26efa-192">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="26efa-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="26efa-193">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="26efa-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="26efa-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="26efa-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="26efa-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-195">Boolean</span></span>|<span data-ttu-id="26efa-196">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="26efa-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="26efa-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="26efa-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="26efa-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-198">Boolean</span></span>|<span data-ttu-id="26efa-199">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="26efa-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="26efa-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="26efa-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="26efa-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-201">Boolean</span></span>|<span data-ttu-id="26efa-202">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="26efa-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="26efa-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-203">cameraBlocked</span></span>|<span data-ttu-id="26efa-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-204">Boolean</span></span>|<span data-ttu-id="26efa-205">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="26efa-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="26efa-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="26efa-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="26efa-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-207">Boolean</span></span>|<span data-ttu-id="26efa-208">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="26efa-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="26efa-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="26efa-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="26efa-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-210">Boolean</span></span>|<span data-ttu-id="26efa-211">Indica se os usuários devem ou não ser bloqueados de qualquer configuração de credencial de certificado.</span><span class="sxs-lookup"><span data-stu-id="26efa-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="26efa-212">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-212">dataRoamingBlocked</span></span>|<span data-ttu-id="26efa-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-213">Boolean</span></span>|<span data-ttu-id="26efa-214">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="26efa-214">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="26efa-215">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-215">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="26efa-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-216">Boolean</span></span>|<span data-ttu-id="26efa-217">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="26efa-217">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="26efa-218">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="26efa-218">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="26efa-219">String collection</span><span class="sxs-lookup"><span data-stu-id="26efa-219">String collection</span></span>|<span data-ttu-id="26efa-220">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="26efa-220">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="26efa-221">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-221">factoryResetBlocked</span></span>|<span data-ttu-id="26efa-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-222">Boolean</span></span>|<span data-ttu-id="26efa-223">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="26efa-223">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="26efa-224">globalProxy</span><span class="sxs-lookup"><span data-stu-id="26efa-224">globalProxy</span></span>|[<span data-ttu-id="26efa-225">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="26efa-225">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="26efa-226">O proxy é configurado diretamente com hosts, porta e hosts excluídos.</span><span class="sxs-lookup"><span data-stu-id="26efa-226">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="26efa-227">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-227">googleAccountsBlocked</span></span>|<span data-ttu-id="26efa-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-228">Boolean</span></span>|<span data-ttu-id="26efa-229">Indica se as contas do Google serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="26efa-229">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="26efa-230">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26efa-230">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="26efa-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-231">Boolean</span></span>|<span data-ttu-id="26efa-232">Se o modo de proteção de tela deve ou não ser habilitado ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-232">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-233">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="26efa-233">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="26efa-234">String</span><span class="sxs-lookup"><span data-stu-id="26efa-234">String</span></span>|<span data-ttu-id="26efa-235">URL de uma imagem que será a proteção de tela do dispositivo no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-235">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-236">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="26efa-236">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="26efa-237">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-237">Int32</span></span>|<span data-ttu-id="26efa-238">O número de segundos que o dispositivo exibirá a proteção de tela no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-238">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="26efa-239">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="26efa-239">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="26efa-240">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="26efa-240">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="26efa-241">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-241">Int32</span></span>|<span data-ttu-id="26efa-242">O número de segundos que o dispositivo precisa estar inativo para que a proteção de tela seja mostrada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-242">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="26efa-243">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="26efa-243">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="26efa-244">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="26efa-244">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="26efa-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-245">Boolean</span></span>|<span data-ttu-id="26efa-246">Se a tela do dispositivo deve ou não mostrar a proteção de tela se áudio/vídeo estiver em execução no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-246">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-247">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="26efa-247">kioskModeApps</span></span>|<span data-ttu-id="26efa-248">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-248">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="26efa-249">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-249">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="26efa-250">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="26efa-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="26efa-251">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="26efa-251">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="26efa-252">String</span><span class="sxs-lookup"><span data-stu-id="26efa-252">String</span></span>|<span data-ttu-id="26efa-253">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-253">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-254">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="26efa-254">kioskModeExitCode</span></span>|<span data-ttu-id="26efa-255">String</span><span class="sxs-lookup"><span data-stu-id="26efa-255">String</span></span>|<span data-ttu-id="26efa-256">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-256">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-257">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="26efa-257">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="26efa-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-258">Boolean</span></span>|<span data-ttu-id="26efa-259">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-259">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-260">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="26efa-260">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="26efa-261">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="26efa-261">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="26efa-262">Indica se o botão de Home virtual é um botão deslizar para cima ou um botão de início flutuante.</span><span class="sxs-lookup"><span data-stu-id="26efa-262">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="26efa-263">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="26efa-263">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="26efa-264">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26efa-264">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="26efa-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-265">Boolean</span></span>|<span data-ttu-id="26efa-266">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-266">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-267">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26efa-267">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="26efa-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-268">Boolean</span></span>|<span data-ttu-id="26efa-269">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-269">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-270">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26efa-270">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="26efa-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-271">Boolean</span></span>|<span data-ttu-id="26efa-272">Se permitirá ou não que um usuário use a lanterna no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-272">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-273">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26efa-273">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="26efa-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-274">Boolean</span></span>|<span data-ttu-id="26efa-275">Se permitirá ou não que um usuário altere o volume de mídia no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="26efa-275">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="26efa-276">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="26efa-276">microphoneForceMute</span></span>|<span data-ttu-id="26efa-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-277">Boolean</span></span>|<span data-ttu-id="26efa-278">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="26efa-278">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="26efa-279">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="26efa-279">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="26efa-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-280">Boolean</span></span>|<span data-ttu-id="26efa-281">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="26efa-281">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="26efa-282">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="26efa-282">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="26efa-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-283">Boolean</span></span>|<span data-ttu-id="26efa-284">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="26efa-284">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="26efa-285">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="26efa-285">passwordBlockKeyguard</span></span>|<span data-ttu-id="26efa-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-286">Boolean</span></span>|<span data-ttu-id="26efa-287">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="26efa-287">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="26efa-288">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="26efa-288">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="26efa-289">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-289">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="26efa-290">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="26efa-290">List of device keyguard features to block.</span></span> <span data-ttu-id="26efa-291">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="26efa-291">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="26efa-292">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="26efa-292">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="26efa-293">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="26efa-293">passwordExpirationDays</span></span>|<span data-ttu-id="26efa-294">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-294">Int32</span></span>|<span data-ttu-id="26efa-295">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="26efa-295">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="26efa-296">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="26efa-296">Valid values 1 to 365</span></span>|
|<span data-ttu-id="26efa-297">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="26efa-297">passwordMinimumLength</span></span>|<span data-ttu-id="26efa-298">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-298">Int32</span></span>|<span data-ttu-id="26efa-299">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-299">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="26efa-300">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="26efa-300">Valid values 4 to 16</span></span>|
|<span data-ttu-id="26efa-301">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="26efa-301">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="26efa-302">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-302">Int32</span></span>|<span data-ttu-id="26efa-303">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-303">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="26efa-304">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="26efa-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26efa-305">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="26efa-305">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="26efa-306">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-306">Int32</span></span>|<span data-ttu-id="26efa-307">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-307">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="26efa-308">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="26efa-308">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26efa-309">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="26efa-309">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="26efa-310">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-310">Int32</span></span>|<span data-ttu-id="26efa-311">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-311">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="26efa-312">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="26efa-312">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26efa-313">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="26efa-313">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="26efa-314">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-314">Int32</span></span>|<span data-ttu-id="26efa-315">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-315">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="26efa-316">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="26efa-316">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26efa-317">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="26efa-317">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="26efa-318">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-318">Int32</span></span>|<span data-ttu-id="26efa-319">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-319">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="26efa-320">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="26efa-320">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26efa-321">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="26efa-321">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="26efa-322">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-322">Int32</span></span>|<span data-ttu-id="26efa-323">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-323">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="26efa-324">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="26efa-324">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26efa-325">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="26efa-325">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="26efa-326">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-326">Int32</span></span>|<span data-ttu-id="26efa-327">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="26efa-327">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="26efa-328">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="26efa-328">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="26efa-329">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-329">Int32</span></span>|<span data-ttu-id="26efa-330">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="26efa-330">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="26efa-331">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="26efa-331">Valid values 0 to 24</span></span>|
|<span data-ttu-id="26efa-332">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="26efa-332">passwordRequiredType</span></span>|[<span data-ttu-id="26efa-333">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="26efa-333">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="26efa-334">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-334">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="26efa-335">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="26efa-335">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="26efa-336">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="26efa-336">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="26efa-337">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-337">Int32</span></span>|<span data-ttu-id="26efa-338">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="26efa-338">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="26efa-339">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="26efa-339">Valid values 4 to 11</span></span>|
|<span data-ttu-id="26efa-340">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="26efa-340">playStoreMode</span></span>|[<span data-ttu-id="26efa-341">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="26efa-341">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="26efa-342">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-342">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="26efa-343">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="26efa-343">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="26efa-344">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-344">safeBootBlocked</span></span>|<span data-ttu-id="26efa-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-345">Boolean</span></span>|<span data-ttu-id="26efa-346">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="26efa-346">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="26efa-347">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-347">screenCaptureBlocked</span></span>|<span data-ttu-id="26efa-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-348">Boolean</span></span>|<span data-ttu-id="26efa-349">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="26efa-349">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="26efa-350">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="26efa-350">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="26efa-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-351">Boolean</span></span>|<span data-ttu-id="26efa-352">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26efa-352">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="26efa-353">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="26efa-353">securityRequireVerifyApps</span></span>|<span data-ttu-id="26efa-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-354">Boolean</span></span>|<span data-ttu-id="26efa-355">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="26efa-355">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="26efa-356">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-356">statusBarBlocked</span></span>|<span data-ttu-id="26efa-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-357">Boolean</span></span>|<span data-ttu-id="26efa-358">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="26efa-358">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="26efa-359">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="26efa-359">stayOnModes</span></span>|<span data-ttu-id="26efa-360">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="26efa-360">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="26efa-361">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="26efa-361">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="26efa-362">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="26efa-362">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="26efa-363">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="26efa-363">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="26efa-364">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="26efa-364">storageAllowUsb</span></span>|<span data-ttu-id="26efa-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-365">Boolean</span></span>|<span data-ttu-id="26efa-366">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="26efa-366">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="26efa-367">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="26efa-367">storageBlockExternalMedia</span></span>|<span data-ttu-id="26efa-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-368">Boolean</span></span>|<span data-ttu-id="26efa-369">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="26efa-369">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="26efa-370">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="26efa-370">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="26efa-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-371">Boolean</span></span>|<span data-ttu-id="26efa-372">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="26efa-372">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="26efa-373">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="26efa-373">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="26efa-374">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-374">Int32</span></span>|<span data-ttu-id="26efa-375">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="26efa-375">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="26efa-376">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="26efa-376">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="26efa-377">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="26efa-377">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="26efa-378">Int32</span><span class="sxs-lookup"><span data-stu-id="26efa-378">Int32</span></span>|<span data-ttu-id="26efa-379">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="26efa-379">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="26efa-380">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="26efa-380">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="26efa-381">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="26efa-381">systemUpdateInstallType</span></span>|[<span data-ttu-id="26efa-382">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="26efa-382">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="26efa-383">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="26efa-383">The type of system update configuration.</span></span> <span data-ttu-id="26efa-384">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="26efa-384">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="26efa-385">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="26efa-385">systemWindowsBlocked</span></span>|<span data-ttu-id="26efa-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-386">Boolean</span></span>|<span data-ttu-id="26efa-387">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="26efa-387">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="26efa-388">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="26efa-388">usersBlockAdd</span></span>|<span data-ttu-id="26efa-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-389">Boolean</span></span>|<span data-ttu-id="26efa-390">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="26efa-390">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="26efa-391">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="26efa-391">usersBlockRemove</span></span>|<span data-ttu-id="26efa-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-392">Boolean</span></span>|<span data-ttu-id="26efa-393">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="26efa-393">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="26efa-394">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="26efa-394">volumeBlockAdjustment</span></span>|<span data-ttu-id="26efa-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-395">Boolean</span></span>|<span data-ttu-id="26efa-396">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="26efa-396">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="26efa-397">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="26efa-397">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="26efa-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-398">Boolean</span></span>|<span data-ttu-id="26efa-399">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="26efa-399">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="26efa-400">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="26efa-400">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="26efa-401">String</span><span class="sxs-lookup"><span data-stu-id="26efa-401">String</span></span>|<span data-ttu-id="26efa-402">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="26efa-402">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="26efa-403">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="26efa-403">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="26efa-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-404">Boolean</span></span>|<span data-ttu-id="26efa-405">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="26efa-405">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="26efa-406">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="26efa-406">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="26efa-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="26efa-407">Boolean</span></span>|<span data-ttu-id="26efa-408">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="26efa-408">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="26efa-409">Resposta</span><span class="sxs-lookup"><span data-stu-id="26efa-409">Response</span></span>
<span data-ttu-id="26efa-410">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26efa-410">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26efa-411">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26efa-411">Example</span></span>

### <a name="request"></a><span data-ttu-id="26efa-412">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26efa-412">Request</span></span>
<span data-ttu-id="26efa-413">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26efa-413">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26efa-414">Resposta</span><span class="sxs-lookup"><span data-stu-id="26efa-414">Response</span></span>
<span data-ttu-id="26efa-p136">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26efa-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





