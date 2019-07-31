---
title: Criar androidDeviceOwnerGeneralDeviceConfiguration
description: Criar um novo objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6c7868832c15d0c325d19012a8378ec4c36a426
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958162"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="faf8f-103">Criar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="faf8f-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="faf8f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="faf8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faf8f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="faf8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faf8f-106">Criar um novo objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="faf8f-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faf8f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="faf8f-107">Prerequisites</span></span>
<span data-ttu-id="faf8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faf8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf8f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="faf8f-110">Permission type</span></span>|<span data-ttu-id="faf8f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="faf8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faf8f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="faf8f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="faf8f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf8f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="faf8f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="faf8f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faf8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faf8f-115">Not supported.</span></span>|
|<span data-ttu-id="faf8f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="faf8f-116">Application</span></span>|<span data-ttu-id="faf8f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faf8f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faf8f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="faf8f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="faf8f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="faf8f-119">Request headers</span></span>
|<span data-ttu-id="faf8f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="faf8f-120">Header</span></span>|<span data-ttu-id="faf8f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="faf8f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faf8f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="faf8f-122">Authorization</span></span>|<span data-ttu-id="faf8f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="faf8f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faf8f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="faf8f-124">Accept</span></span>|<span data-ttu-id="faf8f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="faf8f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faf8f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="faf8f-126">Request body</span></span>
<span data-ttu-id="faf8f-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="faf8f-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="faf8f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="faf8f-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="faf8f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faf8f-129">Property</span></span>|<span data-ttu-id="faf8f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="faf8f-130">Type</span></span>|<span data-ttu-id="faf8f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="faf8f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faf8f-132">id</span><span class="sxs-lookup"><span data-stu-id="faf8f-132">id</span></span>|<span data-ttu-id="faf8f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="faf8f-133">String</span></span>|<span data-ttu-id="faf8f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="faf8f-134">Key of the entity.</span></span> <span data-ttu-id="faf8f-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faf8f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="faf8f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faf8f-137">DateTimeOffset</span></span>|<span data-ttu-id="faf8f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="faf8f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="faf8f-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="faf8f-140">roleScopeTagIds</span></span>|<span data-ttu-id="faf8f-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="faf8f-141">String collection</span></span>|<span data-ttu-id="faf8f-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="faf8f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="faf8f-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="faf8f-144">supportsScopeTags</span></span>|<span data-ttu-id="faf8f-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-145">Boolean</span></span>|<span data-ttu-id="faf8f-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="faf8f-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="faf8f-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="faf8f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="faf8f-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="faf8f-149">This property is read-only.</span></span> <span data-ttu-id="faf8f-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="faf8f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="faf8f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="faf8f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="faf8f-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="faf8f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="faf8f-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="faf8f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="faf8f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="faf8f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="faf8f-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="faf8f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="faf8f-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="faf8f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="faf8f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="faf8f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="faf8f-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="faf8f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="faf8f-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="faf8f-163">createdDateTime</span></span>|<span data-ttu-id="faf8f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faf8f-164">DateTimeOffset</span></span>|<span data-ttu-id="faf8f-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-165">DateTime the object was created.</span></span> <span data-ttu-id="faf8f-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-167">descrição</span><span class="sxs-lookup"><span data-stu-id="faf8f-167">description</span></span>|<span data-ttu-id="faf8f-168">String</span><span class="sxs-lookup"><span data-stu-id="faf8f-168">String</span></span>|<span data-ttu-id="faf8f-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="faf8f-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="faf8f-171">displayName</span></span>|<span data-ttu-id="faf8f-172">String</span><span class="sxs-lookup"><span data-stu-id="faf8f-172">String</span></span>|<span data-ttu-id="faf8f-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="faf8f-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-175">versão</span><span class="sxs-lookup"><span data-stu-id="faf8f-175">version</span></span>|<span data-ttu-id="faf8f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-176">Int32</span></span>|<span data-ttu-id="faf8f-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-177">Version of the device configuration.</span></span> <span data-ttu-id="faf8f-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faf8f-179">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="faf8f-179">accountsBlockModification</span></span>|<span data-ttu-id="faf8f-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-180">Boolean</span></span>|<span data-ttu-id="faf8f-181">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="faf8f-182">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="faf8f-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="faf8f-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-183">Boolean</span></span>|<span data-ttu-id="faf8f-184">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="faf8f-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="faf8f-185">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="faf8f-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="faf8f-186">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="faf8f-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="faf8f-187">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="faf8f-188">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="faf8f-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="faf8f-189">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="faf8f-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="faf8f-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="faf8f-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="faf8f-191">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="faf8f-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="faf8f-192">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="faf8f-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="faf8f-193">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="faf8f-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="faf8f-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-194">Boolean</span></span>|<span data-ttu-id="faf8f-195">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="faf8f-196">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="faf8f-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="faf8f-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-197">Boolean</span></span>|<span data-ttu-id="faf8f-198">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="faf8f-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="faf8f-199">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="faf8f-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="faf8f-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-200">Boolean</span></span>|<span data-ttu-id="faf8f-201">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="faf8f-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="faf8f-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="faf8f-202">cameraBlocked</span></span>|<span data-ttu-id="faf8f-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-203">Boolean</span></span>|<span data-ttu-id="faf8f-204">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="faf8f-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="faf8f-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="faf8f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf8f-206">Boolean</span></span>|<span data-ttu-id="faf8f-207">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="faf8f-208">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="faf8f-208">dataRoamingBlocked</span></span>|<span data-ttu-id="faf8f-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-209">Boolean</span></span>|<span data-ttu-id="faf8f-210">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="faf8f-210">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="faf8f-211">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="faf8f-211">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="faf8f-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-212">Boolean</span></span>|<span data-ttu-id="faf8f-213">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="faf8f-213">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="faf8f-214">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="faf8f-214">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="faf8f-215">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="faf8f-215">String collection</span></span>|<span data-ttu-id="faf8f-216">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-216">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="faf8f-217">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="faf8f-217">factoryResetBlocked</span></span>|<span data-ttu-id="faf8f-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf8f-218">Boolean</span></span>|<span data-ttu-id="faf8f-219">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-219">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="faf8f-220">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="faf8f-220">kioskModeApps</span></span>|<span data-ttu-id="faf8f-221">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-221">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="faf8f-222">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="faf8f-222">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="faf8f-223">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="faf8f-223">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="faf8f-224">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="faf8f-224">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="faf8f-225">String</span><span class="sxs-lookup"><span data-stu-id="faf8f-225">String</span></span>|<span data-ttu-id="faf8f-226">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="faf8f-226">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="faf8f-227">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="faf8f-227">kioskModeExitCode</span></span>|<span data-ttu-id="faf8f-228">String</span><span class="sxs-lookup"><span data-stu-id="faf8f-228">String</span></span>|<span data-ttu-id="faf8f-229">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="faf8f-229">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="faf8f-230">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="faf8f-230">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="faf8f-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-231">Boolean</span></span>|<span data-ttu-id="faf8f-232">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="faf8f-232">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="faf8f-233">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="faf8f-233">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="faf8f-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-234">Boolean</span></span>|<span data-ttu-id="faf8f-235">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="faf8f-235">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="faf8f-236">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="faf8f-236">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="faf8f-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-237">Boolean</span></span>|<span data-ttu-id="faf8f-238">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="faf8f-238">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="faf8f-239">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="faf8f-239">microphoneForceMute</span></span>|<span data-ttu-id="faf8f-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-240">Boolean</span></span>|<span data-ttu-id="faf8f-241">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-241">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="faf8f-242">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="faf8f-242">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="faf8f-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-243">Boolean</span></span>|<span data-ttu-id="faf8f-244">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="faf8f-244">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="faf8f-245">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="faf8f-245">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="faf8f-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-246">Boolean</span></span>|<span data-ttu-id="faf8f-247">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-247">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="faf8f-248">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="faf8f-248">passwordBlockKeyguard</span></span>|<span data-ttu-id="faf8f-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-249">Boolean</span></span>|<span data-ttu-id="faf8f-250">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="faf8f-250">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="faf8f-251">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="faf8f-251">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="faf8f-252">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-252">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="faf8f-253">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="faf8f-253">List of device keyguard features to block.</span></span> <span data-ttu-id="faf8f-254">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="faf8f-254">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="faf8f-255">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="faf8f-255">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="faf8f-256">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="faf8f-256">passwordExpirationDays</span></span>|<span data-ttu-id="faf8f-257">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-257">Int32</span></span>|<span data-ttu-id="faf8f-258">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="faf8f-258">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="faf8f-259">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="faf8f-259">Valid values 1 to 365</span></span>|
|<span data-ttu-id="faf8f-260">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="faf8f-260">passwordMinimumLength</span></span>|<span data-ttu-id="faf8f-261">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-261">Int32</span></span>|<span data-ttu-id="faf8f-262">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-262">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="faf8f-263">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="faf8f-263">Valid values 4 to 16</span></span>|
|<span data-ttu-id="faf8f-264">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="faf8f-264">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="faf8f-265">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-265">Int32</span></span>|<span data-ttu-id="faf8f-266">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-266">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="faf8f-267">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="faf8f-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="faf8f-268">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="faf8f-268">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="faf8f-269">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-269">Int32</span></span>|<span data-ttu-id="faf8f-270">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-270">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="faf8f-271">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="faf8f-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="faf8f-272">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="faf8f-272">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="faf8f-273">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-273">Int32</span></span>|<span data-ttu-id="faf8f-274">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-274">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="faf8f-275">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="faf8f-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="faf8f-276">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="faf8f-276">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="faf8f-277">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-277">Int32</span></span>|<span data-ttu-id="faf8f-278">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-278">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="faf8f-279">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="faf8f-279">Valid values 1 to 16</span></span>|
|<span data-ttu-id="faf8f-280">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="faf8f-280">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="faf8f-281">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-281">Int32</span></span>|<span data-ttu-id="faf8f-282">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-282">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="faf8f-283">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="faf8f-283">Valid values 1 to 16</span></span>|
|<span data-ttu-id="faf8f-284">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="faf8f-284">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="faf8f-285">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-285">Int32</span></span>|<span data-ttu-id="faf8f-286">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-286">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="faf8f-287">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="faf8f-287">Valid values 1 to 16</span></span>|
|<span data-ttu-id="faf8f-288">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="faf8f-288">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="faf8f-289">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-289">Int32</span></span>|<span data-ttu-id="faf8f-290">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="faf8f-290">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="faf8f-291">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="faf8f-291">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="faf8f-292">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-292">Int32</span></span>|<span data-ttu-id="faf8f-293">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="faf8f-293">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="faf8f-294">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="faf8f-294">Valid values 0 to 24</span></span>|
|<span data-ttu-id="faf8f-295">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="faf8f-295">passwordRequiredType</span></span>|[<span data-ttu-id="faf8f-296">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="faf8f-296">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="faf8f-297">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-297">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="faf8f-298">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="faf8f-298">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="faf8f-299">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="faf8f-299">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="faf8f-300">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-300">Int32</span></span>|<span data-ttu-id="faf8f-301">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-301">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="faf8f-302">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="faf8f-302">Valid values 4 to 11</span></span>|
|<span data-ttu-id="faf8f-303">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="faf8f-303">playStoreMode</span></span>|[<span data-ttu-id="faf8f-304">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="faf8f-304">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="faf8f-305">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-305">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="faf8f-306">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="faf8f-306">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="faf8f-307">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="faf8f-307">safeBootBlocked</span></span>|<span data-ttu-id="faf8f-308">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-308">Boolean</span></span>|<span data-ttu-id="faf8f-309">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-309">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="faf8f-310">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="faf8f-310">screenCaptureBlocked</span></span>|<span data-ttu-id="faf8f-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="faf8f-311">Boolean</span></span>|<span data-ttu-id="faf8f-312">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-312">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="faf8f-313">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="faf8f-313">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="faf8f-314">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-314">Boolean</span></span>|<span data-ttu-id="faf8f-315">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="faf8f-315">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="faf8f-316">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="faf8f-316">securityRequireVerifyApps</span></span>|<span data-ttu-id="faf8f-317">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-317">Boolean</span></span>|<span data-ttu-id="faf8f-318">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="faf8f-318">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="faf8f-319">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="faf8f-319">statusBarBlocked</span></span>|<span data-ttu-id="faf8f-320">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-320">Boolean</span></span>|<span data-ttu-id="faf8f-321">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="faf8f-321">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="faf8f-322">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="faf8f-322">stayOnModes</span></span>|<span data-ttu-id="faf8f-323">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="faf8f-323">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="faf8f-324">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-324">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="faf8f-325">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="faf8f-325">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="faf8f-326">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="faf8f-326">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="faf8f-327">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="faf8f-327">storageAllowUsb</span></span>|<span data-ttu-id="faf8f-328">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-328">Boolean</span></span>|<span data-ttu-id="faf8f-329">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="faf8f-329">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="faf8f-330">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="faf8f-330">storageBlockExternalMedia</span></span>|<span data-ttu-id="faf8f-331">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-331">Boolean</span></span>|<span data-ttu-id="faf8f-332">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-332">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="faf8f-333">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="faf8f-333">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="faf8f-334">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-334">Boolean</span></span>|<span data-ttu-id="faf8f-335">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-335">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="faf8f-336">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="faf8f-336">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="faf8f-337">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-337">Int32</span></span>|<span data-ttu-id="faf8f-338">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-338">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="faf8f-339">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="faf8f-339">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="faf8f-340">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="faf8f-340">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="faf8f-341">Int32</span><span class="sxs-lookup"><span data-stu-id="faf8f-341">Int32</span></span>|<span data-ttu-id="faf8f-342">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="faf8f-342">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="faf8f-343">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="faf8f-343">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="faf8f-344">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="faf8f-344">systemUpdateInstallType</span></span>|[<span data-ttu-id="faf8f-345">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="faf8f-345">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="faf8f-346">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="faf8f-346">The type of system update configuration.</span></span> <span data-ttu-id="faf8f-347">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="faf8f-347">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="faf8f-348">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="faf8f-348">systemWindowsBlocked</span></span>|<span data-ttu-id="faf8f-349">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-349">Boolean</span></span>|<span data-ttu-id="faf8f-350">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="faf8f-350">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="faf8f-351">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="faf8f-351">usersBlockAdd</span></span>|<span data-ttu-id="faf8f-352">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-352">Boolean</span></span>|<span data-ttu-id="faf8f-353">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="faf8f-353">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="faf8f-354">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="faf8f-354">usersBlockRemove</span></span>|<span data-ttu-id="faf8f-355">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-355">Boolean</span></span>|<span data-ttu-id="faf8f-356">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-356">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="faf8f-357">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="faf8f-357">volumeBlockAdjustment</span></span>|<span data-ttu-id="faf8f-358">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-358">Boolean</span></span>|<span data-ttu-id="faf8f-359">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="faf8f-359">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="faf8f-360">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="faf8f-360">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="faf8f-361">String</span><span class="sxs-lookup"><span data-stu-id="faf8f-361">String</span></span>|<span data-ttu-id="faf8f-362">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="faf8f-362">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="faf8f-363">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="faf8f-363">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="faf8f-364">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-364">Boolean</span></span>|<span data-ttu-id="faf8f-365">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="faf8f-365">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="faf8f-366">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="faf8f-366">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="faf8f-367">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-367">Boolean</span></span>|<span data-ttu-id="faf8f-368">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="faf8f-368">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="faf8f-369">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="faf8f-369">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="faf8f-370">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf8f-370">Boolean</span></span>|<span data-ttu-id="faf8f-371">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="faf8f-371">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="faf8f-372">Resposta</span><span class="sxs-lookup"><span data-stu-id="faf8f-372">Response</span></span>
<span data-ttu-id="faf8f-373">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faf8f-373">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faf8f-374">Exemplo</span><span class="sxs-lookup"><span data-stu-id="faf8f-374">Example</span></span>

### <a name="request"></a><span data-ttu-id="faf8f-375">Solicitação</span><span class="sxs-lookup"><span data-stu-id="faf8f-375">Request</span></span>
<span data-ttu-id="faf8f-376">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="faf8f-376">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3678

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
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
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

### <a name="response"></a><span data-ttu-id="faf8f-377">Resposta</span><span class="sxs-lookup"><span data-stu-id="faf8f-377">Response</span></span>
<span data-ttu-id="faf8f-p133">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="faf8f-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3850

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
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
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





