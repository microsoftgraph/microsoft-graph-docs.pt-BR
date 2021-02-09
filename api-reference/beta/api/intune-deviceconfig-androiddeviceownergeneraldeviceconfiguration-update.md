---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a64994ec79fe60e121d920027576302837bcbaa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155241"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="c0fee-103">Atualizar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0fee-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="c0fee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0fee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0fee-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0fee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0fee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0fee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0fee-107">Atualizar as propriedades de um [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0fee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0fee-108">Prerequisites</span></span>
<span data-ttu-id="c0fee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0fee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0fee-111">Permission type</span></span>|<span data-ttu-id="c0fee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0fee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0fee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0fee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0fee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0fee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0fee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0fee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0fee-116">Not supported.</span></span>|
|<span data-ttu-id="c0fee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0fee-117">Application</span></span>|<span data-ttu-id="c0fee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0fee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0fee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c0fee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0fee-120">Request headers</span></span>
|<span data-ttu-id="c0fee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0fee-121">Header</span></span>|<span data-ttu-id="c0fee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0fee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0fee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0fee-123">Authorization</span></span>|<span data-ttu-id="c0fee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0fee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0fee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0fee-125">Accept</span></span>|<span data-ttu-id="c0fee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0fee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0fee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0fee-127">Request body</span></span>
<span data-ttu-id="c0fee-128">No corpo da solicitação, fornece uma representação JSON do objeto [androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="c0fee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0fee-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="c0fee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0fee-130">Property</span></span>|<span data-ttu-id="c0fee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0fee-131">Type</span></span>|<span data-ttu-id="c0fee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0fee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0fee-133">id</span><span class="sxs-lookup"><span data-stu-id="c0fee-133">id</span></span>|<span data-ttu-id="c0fee-134">String</span><span class="sxs-lookup"><span data-stu-id="c0fee-134">String</span></span>|<span data-ttu-id="c0fee-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c0fee-135">Key of the entity.</span></span> <span data-ttu-id="c0fee-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0fee-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c0fee-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0fee-138">DateTimeOffset</span></span>|<span data-ttu-id="c0fee-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c0fee-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c0fee-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c0fee-141">roleScopeTagIds</span></span>|<span data-ttu-id="c0fee-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0fee-142">String collection</span></span>|<span data-ttu-id="c0fee-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="c0fee-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c0fee-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c0fee-145">supportsScopeTags</span></span>|<span data-ttu-id="c0fee-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-146">Boolean</span></span>|<span data-ttu-id="c0fee-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c0fee-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c0fee-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0fee-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c0fee-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0fee-150">This property is read-only.</span></span> <span data-ttu-id="c0fee-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c0fee-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c0fee-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c0fee-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c0fee-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="c0fee-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c0fee-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c0fee-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c0fee-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c0fee-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c0fee-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="c0fee-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c0fee-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c0fee-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c0fee-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c0fee-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c0fee-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="c0fee-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c0fee-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0fee-164">createdDateTime</span></span>|<span data-ttu-id="c0fee-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0fee-165">DateTimeOffset</span></span>|<span data-ttu-id="c0fee-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-166">DateTime the object was created.</span></span> <span data-ttu-id="c0fee-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-168">description</span><span class="sxs-lookup"><span data-stu-id="c0fee-168">description</span></span>|<span data-ttu-id="c0fee-169">String</span><span class="sxs-lookup"><span data-stu-id="c0fee-169">String</span></span>|<span data-ttu-id="c0fee-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c0fee-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c0fee-172">displayName</span></span>|<span data-ttu-id="c0fee-173">String</span><span class="sxs-lookup"><span data-stu-id="c0fee-173">String</span></span>|<span data-ttu-id="c0fee-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c0fee-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-176">versão</span><span class="sxs-lookup"><span data-stu-id="c0fee-176">version</span></span>|<span data-ttu-id="c0fee-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-177">Int32</span></span>|<span data-ttu-id="c0fee-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-178">Version of the device configuration.</span></span> <span data-ttu-id="c0fee-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0fee-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="c0fee-180">accountsBlockModification</span></span>|<span data-ttu-id="c0fee-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-181">Boolean</span></span>|<span data-ttu-id="c0fee-182">Indica se a adição ou remoção de contas está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="c0fee-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="c0fee-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c0fee-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="c0fee-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-184">Boolean</span></span>|<span data-ttu-id="c0fee-185">Indica se o usuário tem permissão ou não para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="c0fee-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="c0fee-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="c0fee-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="c0fee-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="c0fee-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="c0fee-188">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="c0fee-189">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="c0fee-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="c0fee-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="c0fee-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="c0fee-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="c0fee-192">Indica a política de permissão para solicitações de permissões de tempo de execução se uma delas não estiver definida especificamente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="c0fee-193">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="c0fee-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="c0fee-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="c0fee-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-195">Boolean</span></span>|<span data-ttu-id="c0fee-196">Se todos os aplicativos devem ou não ignorar qualquer dica de uso pela primeira vez que eles possam ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="c0fee-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0fee-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="c0fee-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-198">Boolean</span></span>|<span data-ttu-id="c0fee-199">Indica se um usuário será ou não bloqueado para configurar o bluetooth.</span><span class="sxs-lookup"><span data-stu-id="c0fee-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="c0fee-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="c0fee-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="c0fee-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-201">Boolean</span></span>|<span data-ttu-id="c0fee-202">Indica se um usuário será ou não bloqueado de compartilhar contatos via bluetooth.</span><span class="sxs-lookup"><span data-stu-id="c0fee-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="c0fee-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-203">cameraBlocked</span></span>|<span data-ttu-id="c0fee-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-204">Boolean</span></span>|<span data-ttu-id="c0fee-205">Indica se o uso da câmera deve ou não ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="c0fee-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="c0fee-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="c0fee-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-207">Boolean</span></span>|<span data-ttu-id="c0fee-208">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="c0fee-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="c0fee-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-210">Boolean</span></span>|<span data-ttu-id="c0fee-211">Indica se os usuários são ou não bloqueados de qualquer configuração de credencial de certificado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="c0fee-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="c0fee-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-213">Boolean</span></span>|<span data-ttu-id="c0fee-214">Indica se você deseja ou não configurar o Microsoft Launcher.</span><span class="sxs-lookup"><span data-stu-id="c0fee-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="c0fee-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="c0fee-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-216">Boolean</span></span>|<span data-ttu-id="c0fee-217">Indica se o papel de parede deve ou não ser configurado nos dispositivos de alvo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="c0fee-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="c0fee-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="c0fee-219">String</span><span class="sxs-lookup"><span data-stu-id="c0fee-219">String</span></span>|<span data-ttu-id="c0fee-220">Indica a URL do arquivo de imagem a ser usado como papel de parede nos dispositivos de alvo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="c0fee-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="c0fee-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="c0fee-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-222">Boolean</span></span>|<span data-ttu-id="c0fee-223">Indica se o usuário pode ou não modificar o papel de parede para personalizar seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="c0fee-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="c0fee-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-225">Boolean</span></span>|<span data-ttu-id="c0fee-226">Indica se você deseja ou não habilitar o feed do launcher no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="c0fee-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="c0fee-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="c0fee-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-228">Boolean</span></span>|<span data-ttu-id="c0fee-229">Indica se o usuário pode ou não modificar o feed do launcher no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="c0fee-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0fee-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="c0fee-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="c0fee-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="c0fee-232">Indica se você deseja ou não configurar o encaixe do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="c0fee-233">Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="c0fee-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="c0fee-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="c0fee-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-235">Boolean</span></span>|<span data-ttu-id="c0fee-236">Indica se o usuário pode ou não modificar a configuração do encaixe do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="c0fee-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0fee-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="c0fee-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="c0fee-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="c0fee-239">Indica a configuração de posicionamento da barra de pesquisa no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="c0fee-240">Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="c0fee-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c0fee-241">enrollmentProfile</span></span>|[<span data-ttu-id="c0fee-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="c0fee-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="c0fee-243">Indica qual perfil de registro você deseja configurar.</span><span class="sxs-lookup"><span data-stu-id="c0fee-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="c0fee-244">Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="c0fee-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-245">dataRoamingBlocked</span></span>|<span data-ttu-id="c0fee-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-246">Boolean</span></span>|<span data-ttu-id="c0fee-247">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="c0fee-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="c0fee-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="c0fee-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-249">Boolean</span></span>|<span data-ttu-id="c0fee-250">Indica se o usuário será ou não bloqueado alterando manualmente a data ou hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="c0fee-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="c0fee-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="c0fee-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="c0fee-252">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0fee-252">String collection</span></span>|<span data-ttu-id="c0fee-253">Lista de emails da conta do Google que serão necessários para autenticar depois que um dispositivo for redefinido de fábrica antes que ele possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="c0fee-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="c0fee-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-254">factoryResetBlocked</span></span>|<span data-ttu-id="c0fee-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-255">Boolean</span></span>|<span data-ttu-id="c0fee-256">Indica se a opção de redefinição de fábrica nas configurações está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="c0fee-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="c0fee-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="c0fee-257">globalProxy</span></span>|[<span data-ttu-id="c0fee-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="c0fee-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="c0fee-259">O proxy é definido diretamente com hosts host, porta e hosts excluídos.</span><span class="sxs-lookup"><span data-stu-id="c0fee-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="c0fee-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-260">googleAccountsBlocked</span></span>|<span data-ttu-id="c0fee-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-261">Boolean</span></span>|<span data-ttu-id="c0fee-262">Indica se as contas do Google serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="c0fee-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="c0fee-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="c0fee-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-264">Boolean</span></span>|<span data-ttu-id="c0fee-265">Indica se um usuário pode acessar o aplicativo Configurações do dispositivo no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="c0fee-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-267">Boolean</span></span>|<span data-ttu-id="c0fee-268">Se o menu ligar/desligar é mostrado quando um usuário pressiona por muito tempo o botão Ligar/Desligar de um dispositivo no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="c0fee-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="c0fee-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="c0fee-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="c0fee-271">Indica se as informações do sistema e as notificações estão desabilitadas no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-272">Os valores possíveis são: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="c0fee-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="c0fee-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="c0fee-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-274">Boolean</span></span>|<span data-ttu-id="c0fee-275">Indica se as caixas de diálogo de erro do sistema para aplicativos com falha ou sem resposta são mostradas no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="c0fee-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="c0fee-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="c0fee-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="c0fee-278">Indica quais recursos de navegação estão habilitados no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-279">Os valores possíveis são: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="c0fee-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="c0fee-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-281">Boolean</span></span>|<span data-ttu-id="c0fee-282">Se o modo de economia de tela deve ou não ser habilitado ou não no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="c0fee-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="c0fee-284">String</span><span class="sxs-lookup"><span data-stu-id="c0fee-284">String</span></span>|<span data-ttu-id="c0fee-285">URL para uma imagem que será a economia de tela do dispositivo no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="c0fee-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="c0fee-287">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-287">Int32</span></span>|<span data-ttu-id="c0fee-288">O número de segundos que o dispositivo exibirá a economia de tela no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-289">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="c0fee-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="c0fee-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="c0fee-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="c0fee-291">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-291">Int32</span></span>|<span data-ttu-id="c0fee-292">O número de segundos que o dispositivo precisa ficar inativo para que a economia de tela seja mostrada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-293">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="c0fee-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="c0fee-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="c0fee-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-295">Boolean</span></span>|<span data-ttu-id="c0fee-296">Se a tela do dispositivo deve ou não mostrar a economia de tela se o áudio/vídeo estiver sendo exibido no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="c0fee-297">kioskModeApps</span></span>|<span data-ttu-id="c0fee-298">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c0fee-299">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-300">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c0fee-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c0fee-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="c0fee-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="c0fee-302">String</span><span class="sxs-lookup"><span data-stu-id="c0fee-302">String</span></span>|<span data-ttu-id="c0fee-303">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo está no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="c0fee-304">kioskModeExitCode</span></span>|<span data-ttu-id="c0fee-305">String</span><span class="sxs-lookup"><span data-stu-id="c0fee-305">String</span></span>|<span data-ttu-id="c0fee-306">Código de saída para permitir que um usuário escape do Modo de Quiosque quando o dispositivo estiver no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="c0fee-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-308">Boolean</span></span>|<span data-ttu-id="c0fee-309">Se um botão página principal virtual será exibido ou não quando o dispositivo estiver no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="c0fee-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="c0fee-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="c0fee-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="c0fee-312">Indica se o botão página principal virtual é um botão página página principal ou um botão página página início flutuante.</span><span class="sxs-lookup"><span data-stu-id="c0fee-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="c0fee-313">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="c0fee-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="c0fee-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-315">Boolean</span></span>|<span data-ttu-id="c0fee-316">Se um usuário poderá ou não definir as configurações de Bluetooth no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="c0fee-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-318">Boolean</span></span>|<span data-ttu-id="c0fee-319">Se um usuário poderá ou não definir as configurações Wi-Fi no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="c0fee-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-321">Boolean</span></span>|<span data-ttu-id="c0fee-322">Se um usuário poderá ou não usar a lanterna no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="c0fee-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-324">Boolean</span></span>|<span data-ttu-id="c0fee-325">Se um usuário pode ou não alterar o volume de mídia no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="c0fee-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="c0fee-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-327">Boolean</span></span>|<span data-ttu-id="c0fee-328">Se um usuário poderá ou não acessar informações básicas do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="c0fee-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="c0fee-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-330">Boolean</span></span>|<span data-ttu-id="c0fee-331">Se o ponto de entrada Configurações Gerenciadas deve ou não ser exibido na tela inicial gerenciada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="c0fee-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-333">Boolean</span></span>|<span data-ttu-id="c0fee-334">Se um usuário poderá ou não acessar facilmente o menu de depuração no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="c0fee-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="c0fee-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-336">Boolean</span></span>|<span data-ttu-id="c0fee-337">Se os selos de notificação de aplicativo serão exibidos ou não no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="c0fee-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="c0fee-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="c0fee-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="c0fee-340">Configuração de orientação da tela inicial gerenciada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-341">Os valores possíveis são: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="c0fee-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="c0fee-342">kioskModeIconSize</span></span>|[<span data-ttu-id="c0fee-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="c0fee-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="c0fee-344">Configuração do tamanho do ícone para a tela inicial gerenciada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-345">Os possíveis valores são: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="c0fee-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="c0fee-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="c0fee-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="c0fee-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="c0fee-348">Configuração de ícone de pasta para tela inicial gerenciada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-349">Os valores possíveis são: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="c0fee-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="c0fee-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="c0fee-351">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0fee-351">String collection</span></span>|<span data-ttu-id="c0fee-352">O conjunto restrito de SSIDs WIFI disponíveis para o usuário configurar no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-353">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c0fee-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c0fee-354">kioskModeAppOrderEnabled</span><span class="sxs-lookup"><span data-stu-id="c0fee-354">kioskModeAppOrderEnabled</span></span>|<span data-ttu-id="c0fee-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-355">Boolean</span></span>|<span data-ttu-id="c0fee-356">Se o pedido do aplicativo será habilitado ou não no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-356">Whether or not to enable app ordering in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-357">kioskModeAppsInFolderOrderedByName</span><span class="sxs-lookup"><span data-stu-id="c0fee-357">kioskModeAppsInFolderOrderedByName</span></span>|<span data-ttu-id="c0fee-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-358">Boolean</span></span>|<span data-ttu-id="c0fee-359">Se os aplicativos serão ou não alfabéticos em uma pasta no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-359">Whether or not to alphabetize applications within a folder in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-360">kioskModeGridHeight</span><span class="sxs-lookup"><span data-stu-id="c0fee-360">kioskModeGridHeight</span></span>|<span data-ttu-id="c0fee-361">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-361">Int32</span></span>|<span data-ttu-id="c0fee-362">Número de linhas para grade da Tela Inicial Gerenciada com ordenação de aplicativos habilitada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-362">Number of rows for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-363">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="c0fee-363">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="c0fee-364">kioskModeGridWidth</span><span class="sxs-lookup"><span data-stu-id="c0fee-364">kioskModeGridWidth</span></span>|<span data-ttu-id="c0fee-365">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-365">Int32</span></span>|<span data-ttu-id="c0fee-366">Número de colunas para grade da Tela Inicial Gerenciada com ordenação de aplicativos habilitada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-366">Number of columns for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-367">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="c0fee-367">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="c0fee-368">kioskModeLockHomeScreen</span><span class="sxs-lookup"><span data-stu-id="c0fee-368">kioskModeLockHomeScreen</span></span>|<span data-ttu-id="c0fee-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-369">Boolean</span></span>|<span data-ttu-id="c0fee-370">Se a tela inicial será ou não lock para o usuário final no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-370">Whether or not to lock home screen to the end user in Kiosk Mode.</span></span>|
|<span data-ttu-id="c0fee-371">kioskModeManagedFolders</span><span class="sxs-lookup"><span data-stu-id="c0fee-371">kioskModeManagedFolders</span></span>|<span data-ttu-id="c0fee-372">[Coleção androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-372">[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) collection</span></span>|<span data-ttu-id="c0fee-373">Uma lista de pastas gerenciadas para um dispositivo no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-373">A list of managed folders for a device in Kiosk Mode.</span></span> <span data-ttu-id="c0fee-374">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c0fee-374">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c0fee-375">kioskModeAppPositions</span><span class="sxs-lookup"><span data-stu-id="c0fee-375">kioskModeAppPositions</span></span>|<span data-ttu-id="c0fee-376">[Coleção androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-376">[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) collection</span></span>|<span data-ttu-id="c0fee-377">A ordenação de itens na tela inicial gerenciada do modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="c0fee-377">The ordering of items on Kiosk Mode Managed Home Screen.</span></span> <span data-ttu-id="c0fee-378">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c0fee-378">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c0fee-379">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="c0fee-379">microphoneForceMute</span></span>|<span data-ttu-id="c0fee-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-380">Boolean</span></span>|<span data-ttu-id="c0fee-381">Indica se o microfone deve ou não ser bloqueado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-381">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="c0fee-382">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="c0fee-382">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="c0fee-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-383">Boolean</span></span>|<span data-ttu-id="c0fee-384">Indica se o dispositivo permitirá ou não a conexão a uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="c0fee-384">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="c0fee-385">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="c0fee-385">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="c0fee-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-386">Boolean</span></span>|<span data-ttu-id="c0fee-387">Indica se o raio de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-387">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="c0fee-388">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="c0fee-388">passwordBlockKeyguard</span></span>|<span data-ttu-id="c0fee-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-389">Boolean</span></span>|<span data-ttu-id="c0fee-390">Indica se a keyguard está ou não desabilitada.</span><span class="sxs-lookup"><span data-stu-id="c0fee-390">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="c0fee-391">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="c0fee-391">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="c0fee-392">[Coleção androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-392">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="c0fee-393">Lista de recursos de proteção de chaves do dispositivo a ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-393">List of device keyguard features to block.</span></span> <span data-ttu-id="c0fee-394">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="c0fee-394">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="c0fee-395">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-395">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="c0fee-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c0fee-396">passwordExpirationDays</span></span>|<span data-ttu-id="c0fee-397">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-397">Int32</span></span>|<span data-ttu-id="c0fee-398">Indica quanto tempo uma senha pode ser definida antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="c0fee-398">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="c0fee-399">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="c0fee-399">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c0fee-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c0fee-400">passwordMinimumLength</span></span>|<span data-ttu-id="c0fee-401">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-401">Int32</span></span>|<span data-ttu-id="c0fee-402">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-402">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="c0fee-403">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c0fee-404">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-404">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="c0fee-405">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-405">Int32</span></span>|<span data-ttu-id="c0fee-406">Indica o número mínimo de caracteres de carta necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-406">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="c0fee-407">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-407">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-408">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-408">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="c0fee-409">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-409">Int32</span></span>|<span data-ttu-id="c0fee-410">Indica o número mínimo de caracteres de casos inferiores necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-410">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="c0fee-411">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-411">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-412">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-412">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="c0fee-413">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-413">Int32</span></span>|<span data-ttu-id="c0fee-414">Indica o número mínimo de caracteres sem letra necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-414">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="c0fee-415">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-415">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-416">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-416">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="c0fee-417">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-417">Int32</span></span>|<span data-ttu-id="c0fee-418">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-418">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="c0fee-419">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-419">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-420">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-420">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="c0fee-421">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-421">Int32</span></span>|<span data-ttu-id="c0fee-422">Indica o número mínimo de caracteres de símbolos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-422">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="c0fee-423">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-423">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-424">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-424">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="c0fee-425">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-425">Int32</span></span>|<span data-ttu-id="c0fee-426">Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-426">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="c0fee-427">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-427">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-428">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c0fee-428">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c0fee-429">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-429">Int32</span></span>|<span data-ttu-id="c0fee-430">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="c0fee-430">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c0fee-431">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="c0fee-431">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="c0fee-432">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-432">Int32</span></span>|<span data-ttu-id="c0fee-433">Indica a duração do histórico de senhas, em que o usuário não poderá inserir uma nova senha que seja a mesma de qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="c0fee-433">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="c0fee-434">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="c0fee-434">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c0fee-435">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c0fee-435">passwordRequiredType</span></span>|[<span data-ttu-id="c0fee-436">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c0fee-436">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="c0fee-437">Indica a qualidade mínima de senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-437">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="c0fee-438">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-438">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="c0fee-439">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c0fee-439">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c0fee-440">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-440">Int32</span></span>|<span data-ttu-id="c0fee-441">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-441">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="c0fee-442">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="c0fee-442">Valid values 4 to 11</span></span>|
|<span data-ttu-id="c0fee-443">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="c0fee-443">playStoreMode</span></span>|[<span data-ttu-id="c0fee-444">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="c0fee-444">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="c0fee-445">Indica o modo da Play Store do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-445">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="c0fee-446">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-446">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="c0fee-447">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-447">safeBootBlocked</span></span>|<span data-ttu-id="c0fee-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-448">Boolean</span></span>|<span data-ttu-id="c0fee-449">Indica se a reinicialização do dispositivo na inicialização segura está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="c0fee-449">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="c0fee-450">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-450">screenCaptureBlocked</span></span>|<span data-ttu-id="c0fee-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-451">Boolean</span></span>|<span data-ttu-id="c0fee-452">Indica se a funcionalidade deve ou não ser desabilitada para fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="c0fee-452">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="c0fee-453">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="c0fee-453">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="c0fee-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-454">Boolean</span></span>|<span data-ttu-id="c0fee-455">Indica se o usuário será ou não bloqueado da habilitação de recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0fee-455">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="c0fee-456">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c0fee-456">securityRequireVerifyApps</span></span>|<span data-ttu-id="c0fee-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-457">Boolean</span></span>|<span data-ttu-id="c0fee-458">Indica se os aplicativos são necessários ou não.</span><span class="sxs-lookup"><span data-stu-id="c0fee-458">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="c0fee-459">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-459">statusBarBlocked</span></span>|<span data-ttu-id="c0fee-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-460">Boolean</span></span>|<span data-ttu-id="c0fee-461">Indica se ou a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="c0fee-461">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="c0fee-462">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="c0fee-462">stayOnModes</span></span>|<span data-ttu-id="c0fee-463">[Coleção androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="c0fee-463">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="c0fee-464">Lista de modos em que a exibição do dispositivo se manterá ligado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-464">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="c0fee-465">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="c0fee-465">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="c0fee-466">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-466">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="c0fee-467">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="c0fee-467">storageAllowUsb</span></span>|<span data-ttu-id="c0fee-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-468">Boolean</span></span>|<span data-ttu-id="c0fee-469">Indica se o armazenamento em massa USB será ou não permitir.</span><span class="sxs-lookup"><span data-stu-id="c0fee-469">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="c0fee-470">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="c0fee-470">storageBlockExternalMedia</span></span>|<span data-ttu-id="c0fee-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-471">Boolean</span></span>|<span data-ttu-id="c0fee-472">Indica se a mídia externa deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-472">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="c0fee-473">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="c0fee-473">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="c0fee-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-474">Boolean</span></span>|<span data-ttu-id="c0fee-475">Indica se a transferência de arquivo USB deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-475">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="c0fee-476">systemUpdateWindowStartMinutesAfterMidafter</span><span class="sxs-lookup"><span data-stu-id="c0fee-476">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="c0fee-477">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-477">Int32</span></span>|<span data-ttu-id="c0fee-478">Indica o número de minutos após a meia-noite em que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="c0fee-478">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="c0fee-479">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="c0fee-479">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="c0fee-480">systemUpdateWindowEndMinutesAfterMidafter</span><span class="sxs-lookup"><span data-stu-id="c0fee-480">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="c0fee-481">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-481">Int32</span></span>|<span data-ttu-id="c0fee-482">Indica o número de minutos após a meia-noite em que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="c0fee-482">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="c0fee-483">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="c0fee-483">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="c0fee-484">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="c0fee-484">systemUpdateInstallType</span></span>|[<span data-ttu-id="c0fee-485">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="c0fee-485">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="c0fee-486">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="c0fee-486">The type of system update configuration.</span></span> <span data-ttu-id="c0fee-487">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-487">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="c0fee-488">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-488">systemWindowsBlocked</span></span>|<span data-ttu-id="c0fee-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-489">Boolean</span></span>|<span data-ttu-id="c0fee-490">Se as janelas de prompt do sistema Android serão ou não bloqueados, como notualizações do sistema, atividades de telefone e alertas do sistema.</span><span class="sxs-lookup"><span data-stu-id="c0fee-490">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="c0fee-491">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="c0fee-491">usersBlockAdd</span></span>|<span data-ttu-id="c0fee-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-492">Boolean</span></span>|<span data-ttu-id="c0fee-493">Indica se a adição de usuários e perfis está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="c0fee-493">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="c0fee-494">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="c0fee-494">usersBlockRemove</span></span>|<span data-ttu-id="c0fee-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-495">Boolean</span></span>|<span data-ttu-id="c0fee-496">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="c0fee-496">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="c0fee-497">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="c0fee-497">volumeBlockAdjustment</span></span>|<span data-ttu-id="c0fee-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-498">Boolean</span></span>|<span data-ttu-id="c0fee-499">Indica se o ajuste do volume mestre está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="c0fee-499">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="c0fee-500">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="c0fee-500">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="c0fee-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-501">Boolean</span></span>|<span data-ttu-id="c0fee-502">Se um nome de pacote VPN sempre em uso for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="c0fee-502">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="c0fee-503">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="c0fee-503">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="c0fee-504">String</span><span class="sxs-lookup"><span data-stu-id="c0fee-504">String</span></span>|<span data-ttu-id="c0fee-505">Nome do pacote do aplicativo Android para o aplicativo que lidará com uma conexão VPN sempre on.</span><span class="sxs-lookup"><span data-stu-id="c0fee-505">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="c0fee-506">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="c0fee-506">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="c0fee-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-507">Boolean</span></span>|<span data-ttu-id="c0fee-508">Indica se o usuário será ou não bloqueado de editar as configurações de conexão wi-fi.</span><span class="sxs-lookup"><span data-stu-id="c0fee-508">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="c0fee-509">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="c0fee-509">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="c0fee-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-510">Boolean</span></span>|<span data-ttu-id="c0fee-511">Indica se o usuário será ou não bloqueado de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="c0fee-511">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="c0fee-512">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c0fee-512">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="c0fee-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-513">Boolean</span></span>|<span data-ttu-id="c0fee-514">Indica se o usuário pode instalar aplicativos de fontes desconhecidas no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="c0fee-514">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="c0fee-515">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-515">personalProfileCameraBlocked</span></span>|<span data-ttu-id="c0fee-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-516">Boolean</span></span>|<span data-ttu-id="c0fee-517">Indica se o uso da câmera no perfil pessoal deve ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-517">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="c0fee-518">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c0fee-518">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="c0fee-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0fee-519">Boolean</span></span>|<span data-ttu-id="c0fee-520">Indica se a funcionalidade deve ser desabilitada para fazer capturas de tela no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="c0fee-520">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="c0fee-521">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c0fee-521">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="c0fee-522">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-522">Int32</span></span>|<span data-ttu-id="c0fee-523">Indica o número de dias que uma senha de perfil de trabalho pode ser definida antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="c0fee-523">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="c0fee-524">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="c0fee-524">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c0fee-525">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c0fee-525">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="c0fee-526">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-526">Int32</span></span>|<span data-ttu-id="c0fee-527">Indica o comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0fee-527">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="c0fee-528">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-528">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c0fee-529">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-529">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="c0fee-530">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-530">Int32</span></span>|<span data-ttu-id="c0fee-531">Indica o número mínimo de caracteres numéricos necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0fee-531">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="c0fee-532">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-532">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-533">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-533">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="c0fee-534">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-534">Int32</span></span>|<span data-ttu-id="c0fee-535">Indica o número mínimo de caracteres sem letra necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0fee-535">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="c0fee-536">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-536">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-537">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-537">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="c0fee-538">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-538">Int32</span></span>|<span data-ttu-id="c0fee-539">Indica o número mínimo de caracteres de carta necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0fee-539">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="c0fee-540">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-540">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-541">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-541">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="c0fee-542">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-542">Int32</span></span>|<span data-ttu-id="c0fee-543">Indica o número mínimo de caracteres de casos inferiores necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0fee-543">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="c0fee-544">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-544">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-545">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-545">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="c0fee-546">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-546">Int32</span></span>|<span data-ttu-id="c0fee-547">Indica o número mínimo de caracteres de letra maiúscula necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0fee-547">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="c0fee-548">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-548">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-549">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="c0fee-549">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="c0fee-550">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-550">Int32</span></span>|<span data-ttu-id="c0fee-551">Indica o número mínimo de caracteres de símbolos necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0fee-551">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="c0fee-552">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c0fee-552">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c0fee-553">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="c0fee-553">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="c0fee-554">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-554">Int32</span></span>|<span data-ttu-id="c0fee-555">Indica a duração do histórico de senhas do perfil de trabalho, em que o usuário não poderá inserir uma nova senha igual à de qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="c0fee-555">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="c0fee-556">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="c0fee-556">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c0fee-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c0fee-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c0fee-558">Int32</span><span class="sxs-lookup"><span data-stu-id="c0fee-558">Int32</span></span>|<span data-ttu-id="c0fee-559">Indica o número de vezes que um usuário pode inserir uma senha de perfil de trabalho incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="c0fee-559">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="c0fee-560">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="c0fee-560">Valid values 4 to 11</span></span>|
|<span data-ttu-id="c0fee-561">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c0fee-561">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="c0fee-562">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c0fee-562">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="c0fee-563">Indica a qualidade mínima de senha necessária na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c0fee-563">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="c0fee-564">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="c0fee-564">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="c0fee-565">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0fee-565">Response</span></span>
<span data-ttu-id="c0fee-566">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0fee-566">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0fee-567">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0fee-567">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0fee-568">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0fee-568">Request</span></span>
<span data-ttu-id="c0fee-569">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0fee-569">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7313

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
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
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
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
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
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```

### <a name="response"></a><span data-ttu-id="c0fee-570">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0fee-570">Response</span></span>
<span data-ttu-id="c0fee-p160">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0fee-p160">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7485

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
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
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
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
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
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```




