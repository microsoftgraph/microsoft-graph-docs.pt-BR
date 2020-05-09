---
title: Criar androidDeviceOwnerGeneralDeviceConfiguration
description: Criar um novo objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be9f2b0fd08f09cfa96d227d879c0f9cb6931358
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178742"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="f0520-103">Criar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0520-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="f0520-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0520-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0520-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0520-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0520-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0520-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0520-107">Criar um novo objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f0520-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0520-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0520-108">Prerequisites</span></span>
<span data-ttu-id="f0520-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0520-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0520-111">Permission type</span></span>|<span data-ttu-id="f0520-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0520-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0520-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0520-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0520-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0520-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0520-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0520-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0520-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0520-116">Not supported.</span></span>|
|<span data-ttu-id="f0520-117">Application</span><span class="sxs-lookup"><span data-stu-id="f0520-117">Application</span></span>|<span data-ttu-id="f0520-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0520-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0520-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0520-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f0520-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0520-120">Request headers</span></span>
|<span data-ttu-id="f0520-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0520-121">Header</span></span>|<span data-ttu-id="f0520-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f0520-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0520-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0520-123">Authorization</span></span>|<span data-ttu-id="f0520-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0520-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0520-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0520-125">Accept</span></span>|<span data-ttu-id="f0520-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0520-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0520-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0520-127">Request body</span></span>
<span data-ttu-id="f0520-128">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0520-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="f0520-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0520-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="f0520-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0520-130">Property</span></span>|<span data-ttu-id="f0520-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0520-131">Type</span></span>|<span data-ttu-id="f0520-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0520-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0520-133">id</span><span class="sxs-lookup"><span data-stu-id="f0520-133">id</span></span>|<span data-ttu-id="f0520-134">String</span><span class="sxs-lookup"><span data-stu-id="f0520-134">String</span></span>|<span data-ttu-id="f0520-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f0520-135">Key of the entity.</span></span> <span data-ttu-id="f0520-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0520-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f0520-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0520-138">DateTimeOffset</span></span>|<span data-ttu-id="f0520-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f0520-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f0520-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0520-141">roleScopeTagIds</span></span>|<span data-ttu-id="f0520-142">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0520-142">String collection</span></span>|<span data-ttu-id="f0520-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f0520-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f0520-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f0520-145">supportsScopeTags</span></span>|<span data-ttu-id="f0520-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-146">Boolean</span></span>|<span data-ttu-id="f0520-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f0520-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f0520-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f0520-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f0520-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f0520-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f0520-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0520-150">This property is read-only.</span></span> <span data-ttu-id="f0520-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f0520-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f0520-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f0520-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f0520-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f0520-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f0520-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f0520-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f0520-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f0520-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f0520-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f0520-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f0520-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f0520-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f0520-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f0520-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f0520-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f0520-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f0520-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0520-164">createdDateTime</span></span>|<span data-ttu-id="f0520-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0520-165">DateTimeOffset</span></span>|<span data-ttu-id="f0520-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f0520-166">DateTime the object was created.</span></span> <span data-ttu-id="f0520-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-168">description</span><span class="sxs-lookup"><span data-stu-id="f0520-168">description</span></span>|<span data-ttu-id="f0520-169">String</span><span class="sxs-lookup"><span data-stu-id="f0520-169">String</span></span>|<span data-ttu-id="f0520-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0520-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f0520-172">displayName</span></span>|<span data-ttu-id="f0520-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0520-173">String</span></span>|<span data-ttu-id="f0520-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0520-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-176">versão</span><span class="sxs-lookup"><span data-stu-id="f0520-176">version</span></span>|<span data-ttu-id="f0520-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-177">Int32</span></span>|<span data-ttu-id="f0520-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-178">Version of the device configuration.</span></span> <span data-ttu-id="f0520-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0520-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="f0520-180">accountsBlockModification</span></span>|<span data-ttu-id="f0520-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-181">Boolean</span></span>|<span data-ttu-id="f0520-182">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="f0520-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="f0520-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="f0520-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="f0520-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-184">Boolean</span></span>|<span data-ttu-id="f0520-185">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="f0520-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="f0520-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="f0520-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="f0520-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="f0520-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="f0520-188">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f0520-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="f0520-189">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="f0520-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="f0520-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="f0520-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="f0520-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="f0520-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="f0520-192">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="f0520-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="f0520-193">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="f0520-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="f0520-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="f0520-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="f0520-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-195">Boolean</span></span>|<span data-ttu-id="f0520-196">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="f0520-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="f0520-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0520-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="f0520-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-198">Boolean</span></span>|<span data-ttu-id="f0520-199">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="f0520-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="f0520-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="f0520-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="f0520-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-201">Boolean</span></span>|<span data-ttu-id="f0520-202">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="f0520-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="f0520-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-203">cameraBlocked</span></span>|<span data-ttu-id="f0520-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-204">Boolean</span></span>|<span data-ttu-id="f0520-205">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="f0520-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="f0520-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="f0520-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="f0520-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-207">Boolean</span></span>|<span data-ttu-id="f0520-208">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f0520-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="f0520-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="f0520-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="f0520-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-210">Boolean</span></span>|<span data-ttu-id="f0520-211">Indica se os usuários devem ou não ser bloqueados de qualquer configuração de credencial de certificado.</span><span class="sxs-lookup"><span data-stu-id="f0520-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="f0520-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="f0520-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="f0520-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-213">Boolean</span></span>|<span data-ttu-id="f0520-214">Indica se você deseja ou não configurar o iniciador Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f0520-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="f0520-215">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f0520-215">enrollmentProfile</span></span>|[<span data-ttu-id="f0520-216">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="f0520-216">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="f0520-217">Indica o perfil de registro que você deseja configurar.</span><span class="sxs-lookup"><span data-stu-id="f0520-217">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="f0520-218">Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="f0520-218">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="f0520-219">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-219">dataRoamingBlocked</span></span>|<span data-ttu-id="f0520-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-220">Boolean</span></span>|<span data-ttu-id="f0520-221">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="f0520-221">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="f0520-222">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-222">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="f0520-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-223">Boolean</span></span>|<span data-ttu-id="f0520-224">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="f0520-224">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="f0520-225">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="f0520-225">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="f0520-226">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0520-226">String collection</span></span>|<span data-ttu-id="f0520-227">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="f0520-227">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="f0520-228">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-228">factoryResetBlocked</span></span>|<span data-ttu-id="f0520-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-229">Boolean</span></span>|<span data-ttu-id="f0520-230">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="f0520-230">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="f0520-231">globalProxy</span><span class="sxs-lookup"><span data-stu-id="f0520-231">globalProxy</span></span>|[<span data-ttu-id="f0520-232">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="f0520-232">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="f0520-233">O proxy é configurado diretamente com hosts, porta e hosts excluídos.</span><span class="sxs-lookup"><span data-stu-id="f0520-233">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="f0520-234">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-234">googleAccountsBlocked</span></span>|<span data-ttu-id="f0520-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-235">Boolean</span></span>|<span data-ttu-id="f0520-236">Indica se as contas do Google serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="f0520-236">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="f0520-237">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="f0520-237">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="f0520-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-238">Boolean</span></span>|<span data-ttu-id="f0520-239">Se o modo de proteção de tela deve ou não ser habilitado ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-239">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-240">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="f0520-240">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="f0520-241">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f0520-241">String</span></span>|<span data-ttu-id="f0520-242">URL de uma imagem que será a proteção de tela do dispositivo no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-242">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-243">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="f0520-243">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="f0520-244">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-244">Int32</span></span>|<span data-ttu-id="f0520-245">O número de segundos que o dispositivo exibirá a proteção de tela no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-245">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="f0520-246">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="f0520-246">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="f0520-247">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="f0520-247">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="f0520-248">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-248">Int32</span></span>|<span data-ttu-id="f0520-249">O número de segundos que o dispositivo precisa estar inativo para que a proteção de tela seja mostrada no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-249">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="f0520-250">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="f0520-250">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="f0520-251">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="f0520-251">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="f0520-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-252">Boolean</span></span>|<span data-ttu-id="f0520-253">Se a tela do dispositivo deve ou não mostrar a proteção de tela se áudio/vídeo estiver em execução no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-253">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-254">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="f0520-254">kioskModeApps</span></span>|<span data-ttu-id="f0520-255">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-255">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f0520-256">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-256">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="f0520-257">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f0520-257">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f0520-258">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="f0520-258">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="f0520-259">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f0520-259">String</span></span>|<span data-ttu-id="f0520-260">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-260">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-261">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="f0520-261">kioskModeExitCode</span></span>|<span data-ttu-id="f0520-262">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f0520-262">String</span></span>|<span data-ttu-id="f0520-263">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-263">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-264">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="f0520-264">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="f0520-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-265">Boolean</span></span>|<span data-ttu-id="f0520-266">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-266">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-267">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="f0520-267">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="f0520-268">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="f0520-268">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="f0520-269">Indica se o botão de Home virtual é um botão deslizar para cima ou um botão de início flutuante.</span><span class="sxs-lookup"><span data-stu-id="f0520-269">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="f0520-270">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="f0520-270">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="f0520-271">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="f0520-271">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="f0520-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-272">Boolean</span></span>|<span data-ttu-id="f0520-273">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-273">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-274">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="f0520-274">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="f0520-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-275">Boolean</span></span>|<span data-ttu-id="f0520-276">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-276">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-277">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="f0520-277">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="f0520-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-278">Boolean</span></span>|<span data-ttu-id="f0520-279">Se permitirá ou não que um usuário use a lanterna no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-279">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-280">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="f0520-280">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="f0520-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-281">Boolean</span></span>|<span data-ttu-id="f0520-282">Se permitirá ou não que um usuário altere o volume de mídia no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0520-282">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0520-283">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="f0520-283">microphoneForceMute</span></span>|<span data-ttu-id="f0520-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-284">Boolean</span></span>|<span data-ttu-id="f0520-285">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f0520-285">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="f0520-286">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="f0520-286">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="f0520-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-287">Boolean</span></span>|<span data-ttu-id="f0520-288">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="f0520-288">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="f0520-289">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="f0520-289">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="f0520-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-290">Boolean</span></span>|<span data-ttu-id="f0520-291">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f0520-291">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="f0520-292">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="f0520-292">passwordBlockKeyguard</span></span>|<span data-ttu-id="f0520-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-293">Boolean</span></span>|<span data-ttu-id="f0520-294">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="f0520-294">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="f0520-295">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="f0520-295">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="f0520-296">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-296">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="f0520-297">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f0520-297">List of device keyguard features to block.</span></span> <span data-ttu-id="f0520-298">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="f0520-298">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="f0520-299">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="f0520-299">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="f0520-300">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f0520-300">passwordExpirationDays</span></span>|<span data-ttu-id="f0520-301">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-301">Int32</span></span>|<span data-ttu-id="f0520-302">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="f0520-302">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="f0520-303">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="f0520-303">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f0520-304">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f0520-304">passwordMinimumLength</span></span>|<span data-ttu-id="f0520-305">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-305">Int32</span></span>|<span data-ttu-id="f0520-306">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-306">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="f0520-307">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="f0520-307">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f0520-308">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f0520-308">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="f0520-309">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-309">Int32</span></span>|<span data-ttu-id="f0520-310">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-310">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="f0520-311">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="f0520-311">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f0520-312">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f0520-312">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="f0520-313">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-313">Int32</span></span>|<span data-ttu-id="f0520-314">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-314">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="f0520-315">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="f0520-315">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f0520-316">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f0520-316">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="f0520-317">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-317">Int32</span></span>|<span data-ttu-id="f0520-318">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-318">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="f0520-319">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="f0520-319">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f0520-320">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="f0520-320">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="f0520-321">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-321">Int32</span></span>|<span data-ttu-id="f0520-322">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-322">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="f0520-323">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="f0520-323">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f0520-324">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="f0520-324">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="f0520-325">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-325">Int32</span></span>|<span data-ttu-id="f0520-326">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-326">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="f0520-327">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="f0520-327">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f0520-328">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f0520-328">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="f0520-329">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-329">Int32</span></span>|<span data-ttu-id="f0520-330">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-330">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="f0520-331">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="f0520-331">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f0520-332">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f0520-332">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f0520-333">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-333">Int32</span></span>|<span data-ttu-id="f0520-334">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="f0520-334">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f0520-335">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="f0520-335">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="f0520-336">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-336">Int32</span></span>|<span data-ttu-id="f0520-337">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="f0520-337">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="f0520-338">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="f0520-338">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f0520-339">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f0520-339">passwordRequiredType</span></span>|[<span data-ttu-id="f0520-340">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f0520-340">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="f0520-341">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-341">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="f0520-342">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="f0520-342">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="f0520-343">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f0520-343">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f0520-344">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-344">Int32</span></span>|<span data-ttu-id="f0520-345">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="f0520-345">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="f0520-346">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="f0520-346">Valid values 4 to 11</span></span>|
|<span data-ttu-id="f0520-347">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="f0520-347">playStoreMode</span></span>|[<span data-ttu-id="f0520-348">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="f0520-348">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="f0520-349">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-349">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="f0520-350">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="f0520-350">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="f0520-351">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-351">safeBootBlocked</span></span>|<span data-ttu-id="f0520-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-352">Boolean</span></span>|<span data-ttu-id="f0520-353">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="f0520-353">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="f0520-354">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-354">screenCaptureBlocked</span></span>|<span data-ttu-id="f0520-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-355">Boolean</span></span>|<span data-ttu-id="f0520-356">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="f0520-356">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="f0520-357">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="f0520-357">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="f0520-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-358">Boolean</span></span>|<span data-ttu-id="f0520-359">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0520-359">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="f0520-360">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f0520-360">securityRequireVerifyApps</span></span>|<span data-ttu-id="f0520-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-361">Boolean</span></span>|<span data-ttu-id="f0520-362">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="f0520-362">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="f0520-363">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-363">statusBarBlocked</span></span>|<span data-ttu-id="f0520-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-364">Boolean</span></span>|<span data-ttu-id="f0520-365">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="f0520-365">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="f0520-366">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="f0520-366">stayOnModes</span></span>|<span data-ttu-id="f0520-367">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="f0520-367">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="f0520-368">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="f0520-368">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="f0520-369">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="f0520-369">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="f0520-370">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="f0520-370">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="f0520-371">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="f0520-371">storageAllowUsb</span></span>|<span data-ttu-id="f0520-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-372">Boolean</span></span>|<span data-ttu-id="f0520-373">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="f0520-373">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="f0520-374">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="f0520-374">storageBlockExternalMedia</span></span>|<span data-ttu-id="f0520-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-375">Boolean</span></span>|<span data-ttu-id="f0520-376">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f0520-376">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="f0520-377">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="f0520-377">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="f0520-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-378">Boolean</span></span>|<span data-ttu-id="f0520-379">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f0520-379">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="f0520-380">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="f0520-380">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="f0520-381">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-381">Int32</span></span>|<span data-ttu-id="f0520-382">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="f0520-382">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="f0520-383">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="f0520-383">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="f0520-384">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="f0520-384">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="f0520-385">Int32</span><span class="sxs-lookup"><span data-stu-id="f0520-385">Int32</span></span>|<span data-ttu-id="f0520-386">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="f0520-386">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="f0520-387">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="f0520-387">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="f0520-388">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="f0520-388">systemUpdateInstallType</span></span>|[<span data-ttu-id="f0520-389">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="f0520-389">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="f0520-390">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="f0520-390">The type of system update configuration.</span></span> <span data-ttu-id="f0520-391">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="f0520-391">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="f0520-392">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="f0520-392">systemWindowsBlocked</span></span>|<span data-ttu-id="f0520-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-393">Boolean</span></span>|<span data-ttu-id="f0520-394">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="f0520-394">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="f0520-395">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="f0520-395">usersBlockAdd</span></span>|<span data-ttu-id="f0520-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-396">Boolean</span></span>|<span data-ttu-id="f0520-397">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="f0520-397">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="f0520-398">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="f0520-398">usersBlockRemove</span></span>|<span data-ttu-id="f0520-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-399">Boolean</span></span>|<span data-ttu-id="f0520-400">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="f0520-400">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="f0520-401">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="f0520-401">volumeBlockAdjustment</span></span>|<span data-ttu-id="f0520-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-402">Boolean</span></span>|<span data-ttu-id="f0520-403">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="f0520-403">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="f0520-404">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="f0520-404">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="f0520-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-405">Boolean</span></span>|<span data-ttu-id="f0520-406">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="f0520-406">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="f0520-407">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="f0520-407">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="f0520-408">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f0520-408">String</span></span>|<span data-ttu-id="f0520-409">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="f0520-409">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="f0520-410">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="f0520-410">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="f0520-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-411">Boolean</span></span>|<span data-ttu-id="f0520-412">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="f0520-412">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="f0520-413">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="f0520-413">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="f0520-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0520-414">Boolean</span></span>|<span data-ttu-id="f0520-415">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="f0520-415">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="f0520-416">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0520-416">Response</span></span>
<span data-ttu-id="f0520-417">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0520-417">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0520-418">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0520-418">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0520-419">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0520-419">Request</span></span>
<span data-ttu-id="f0520-420">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0520-420">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4467

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

### <a name="response"></a><span data-ttu-id="f0520-421">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0520-421">Response</span></span>
<span data-ttu-id="f0520-p137">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0520-p137">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4639

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



