---
title: Criar androidDeviceOwnerGeneralDeviceConfiguration
description: Crie um novo objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a3076636b8961a93bd6a9313070514942fbfb3a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156165"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="84259-103">Criar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="84259-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="84259-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84259-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84259-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84259-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84259-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84259-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84259-107">Crie um novo [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84259-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84259-108">Prerequisites</span></span>
<span data-ttu-id="84259-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84259-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84259-111">Permission type</span></span>|<span data-ttu-id="84259-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84259-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84259-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84259-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84259-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84259-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84259-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84259-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84259-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84259-116">Not supported.</span></span>|
|<span data-ttu-id="84259-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84259-117">Application</span></span>|<span data-ttu-id="84259-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84259-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84259-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84259-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84259-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84259-120">Request headers</span></span>
|<span data-ttu-id="84259-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84259-121">Header</span></span>|<span data-ttu-id="84259-122">Valor</span><span class="sxs-lookup"><span data-stu-id="84259-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84259-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84259-123">Authorization</span></span>|<span data-ttu-id="84259-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84259-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84259-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84259-125">Accept</span></span>|<span data-ttu-id="84259-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84259-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84259-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84259-127">Request body</span></span>
<span data-ttu-id="84259-128">No corpo da solicitação, fornece uma representação JSON do objeto androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84259-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="84259-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84259-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="84259-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84259-130">Property</span></span>|<span data-ttu-id="84259-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="84259-131">Type</span></span>|<span data-ttu-id="84259-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="84259-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84259-133">id</span><span class="sxs-lookup"><span data-stu-id="84259-133">id</span></span>|<span data-ttu-id="84259-134">String</span><span class="sxs-lookup"><span data-stu-id="84259-134">String</span></span>|<span data-ttu-id="84259-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="84259-135">Key of the entity.</span></span> <span data-ttu-id="84259-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84259-137">lastModifiedDateTime</span></span>|<span data-ttu-id="84259-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84259-138">DateTimeOffset</span></span>|<span data-ttu-id="84259-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="84259-139">DateTime the object was last modified.</span></span> <span data-ttu-id="84259-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84259-141">roleScopeTagIds</span></span>|<span data-ttu-id="84259-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="84259-142">String collection</span></span>|<span data-ttu-id="84259-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="84259-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84259-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84259-145">supportsScopeTags</span></span>|<span data-ttu-id="84259-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-146">Boolean</span></span>|<span data-ttu-id="84259-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="84259-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84259-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="84259-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84259-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="84259-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84259-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84259-150">This property is read-only.</span></span> <span data-ttu-id="84259-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="84259-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="84259-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="84259-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="84259-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="84259-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="84259-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="84259-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="84259-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="84259-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="84259-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="84259-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="84259-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="84259-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="84259-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="84259-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="84259-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="84259-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="84259-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84259-164">createdDateTime</span></span>|<span data-ttu-id="84259-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84259-165">DateTimeOffset</span></span>|<span data-ttu-id="84259-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="84259-166">DateTime the object was created.</span></span> <span data-ttu-id="84259-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-168">description</span><span class="sxs-lookup"><span data-stu-id="84259-168">description</span></span>|<span data-ttu-id="84259-169">String</span><span class="sxs-lookup"><span data-stu-id="84259-169">String</span></span>|<span data-ttu-id="84259-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84259-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-172">displayName</span><span class="sxs-lookup"><span data-stu-id="84259-172">displayName</span></span>|<span data-ttu-id="84259-173">String</span><span class="sxs-lookup"><span data-stu-id="84259-173">String</span></span>|<span data-ttu-id="84259-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84259-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-176">versão</span><span class="sxs-lookup"><span data-stu-id="84259-176">version</span></span>|<span data-ttu-id="84259-177">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-177">Int32</span></span>|<span data-ttu-id="84259-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-178">Version of the device configuration.</span></span> <span data-ttu-id="84259-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84259-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84259-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="84259-180">accountsBlockModification</span></span>|<span data-ttu-id="84259-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-181">Boolean</span></span>|<span data-ttu-id="84259-182">Indica se a adição ou remoção de contas está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="84259-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="84259-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="84259-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="84259-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-184">Boolean</span></span>|<span data-ttu-id="84259-185">Indica se o usuário tem permissão ou não para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="84259-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="84259-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="84259-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="84259-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="84259-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="84259-188">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84259-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="84259-189">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="84259-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="84259-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="84259-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="84259-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="84259-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="84259-192">Indica a política de permissão para solicitações de permissões de tempo de execução se uma delas não estiver definida especificamente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84259-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="84259-193">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="84259-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="84259-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="84259-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="84259-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-195">Boolean</span></span>|<span data-ttu-id="84259-196">Se todos os aplicativos devem ou não ignorar qualquer dica de uso pela primeira vez que eles possam ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="84259-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="84259-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="84259-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="84259-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-198">Boolean</span></span>|<span data-ttu-id="84259-199">Indica se um usuário será ou não bloqueado para configurar o bluetooth.</span><span class="sxs-lookup"><span data-stu-id="84259-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="84259-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="84259-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="84259-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-201">Boolean</span></span>|<span data-ttu-id="84259-202">Indica se um usuário será ou não bloqueado de compartilhar contatos via bluetooth.</span><span class="sxs-lookup"><span data-stu-id="84259-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="84259-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-203">cameraBlocked</span></span>|<span data-ttu-id="84259-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-204">Boolean</span></span>|<span data-ttu-id="84259-205">Indica se o uso da câmera deve ou não ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="84259-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="84259-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="84259-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="84259-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-207">Boolean</span></span>|<span data-ttu-id="84259-208">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84259-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="84259-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="84259-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="84259-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-210">Boolean</span></span>|<span data-ttu-id="84259-211">Indica se os usuários são ou não bloqueados de qualquer configuração de credencial de certificado.</span><span class="sxs-lookup"><span data-stu-id="84259-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="84259-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="84259-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-213">Boolean</span></span>|<span data-ttu-id="84259-214">Indica se você deseja ou não configurar o Microsoft Launcher.</span><span class="sxs-lookup"><span data-stu-id="84259-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="84259-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="84259-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-216">Boolean</span></span>|<span data-ttu-id="84259-217">Indica se o papel de parede deve ou não ser configurado nos dispositivos de alvo.</span><span class="sxs-lookup"><span data-stu-id="84259-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="84259-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="84259-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="84259-219">String</span><span class="sxs-lookup"><span data-stu-id="84259-219">String</span></span>|<span data-ttu-id="84259-220">Indica a URL do arquivo de imagem a ser usado como papel de parede nos dispositivos de alvo.</span><span class="sxs-lookup"><span data-stu-id="84259-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="84259-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="84259-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="84259-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-222">Boolean</span></span>|<span data-ttu-id="84259-223">Indica se o usuário pode ou não modificar o papel de parede para personalizar seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="84259-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="84259-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-225">Boolean</span></span>|<span data-ttu-id="84259-226">Indica se você deseja ou não habilitar o feed do launcher no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="84259-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="84259-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="84259-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-228">Boolean</span></span>|<span data-ttu-id="84259-229">Indica se o usuário pode ou não modificar o feed do launcher no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="84259-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="84259-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="84259-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="84259-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="84259-232">Indica se você deseja ou não configurar o encaixe do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="84259-233">Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="84259-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="84259-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="84259-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="84259-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-235">Boolean</span></span>|<span data-ttu-id="84259-236">Indica se o usuário pode ou não modificar a configuração do encaixe do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="84259-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="84259-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="84259-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="84259-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="84259-239">Indica a configuração de posicionamento da barra de pesquisa no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="84259-240">Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="84259-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="84259-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="84259-241">enrollmentProfile</span></span>|[<span data-ttu-id="84259-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="84259-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="84259-243">Indica qual perfil de registro você deseja configurar.</span><span class="sxs-lookup"><span data-stu-id="84259-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="84259-244">Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="84259-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="84259-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-245">dataRoamingBlocked</span></span>|<span data-ttu-id="84259-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-246">Boolean</span></span>|<span data-ttu-id="84259-247">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="84259-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="84259-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="84259-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-249">Boolean</span></span>|<span data-ttu-id="84259-250">Indica se o usuário será ou não bloqueado alterando manualmente a data ou hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="84259-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="84259-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="84259-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="84259-252">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="84259-252">String collection</span></span>|<span data-ttu-id="84259-253">Lista de emails da conta do Google que serão necessários para autenticar depois que um dispositivo for redefinido de fábrica antes que ele possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="84259-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="84259-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-254">factoryResetBlocked</span></span>|<span data-ttu-id="84259-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-255">Boolean</span></span>|<span data-ttu-id="84259-256">Indica se a opção de redefinição de fábrica nas configurações está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="84259-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="84259-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="84259-257">globalProxy</span></span>|[<span data-ttu-id="84259-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="84259-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="84259-259">O proxy é definido diretamente com hosts host, porta e hosts excluídos.</span><span class="sxs-lookup"><span data-stu-id="84259-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="84259-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-260">googleAccountsBlocked</span></span>|<span data-ttu-id="84259-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-261">Boolean</span></span>|<span data-ttu-id="84259-262">Indica se as contas do Google serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="84259-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="84259-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="84259-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-264">Boolean</span></span>|<span data-ttu-id="84259-265">Indica se um usuário pode acessar o aplicativo Configurações do dispositivo no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="84259-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-267">Boolean</span></span>|<span data-ttu-id="84259-268">Se o menu ligar/desligar é mostrado quando um usuário pressiona por muito tempo o botão Ligar/Desligar de um dispositivo no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="84259-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="84259-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="84259-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="84259-271">Indica se as informações do sistema e as notificações estão desabilitadas no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="84259-272">Os valores possíveis são: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span><span class="sxs-lookup"><span data-stu-id="84259-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="84259-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="84259-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="84259-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-274">Boolean</span></span>|<span data-ttu-id="84259-275">Indica se as caixas de diálogo de erro do sistema para aplicativos com falha ou sem resposta são mostradas no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="84259-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="84259-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="84259-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="84259-278">Indica quais recursos de navegação estão habilitados no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="84259-279">Os valores possíveis são: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span><span class="sxs-lookup"><span data-stu-id="84259-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="84259-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="84259-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-281">Boolean</span></span>|<span data-ttu-id="84259-282">Se o modo de economia de tela deve ou não ser habilitado ou não no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="84259-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="84259-284">String</span><span class="sxs-lookup"><span data-stu-id="84259-284">String</span></span>|<span data-ttu-id="84259-285">URL para uma imagem que será a economia de tela do dispositivo no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="84259-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="84259-287">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-287">Int32</span></span>|<span data-ttu-id="84259-288">O número de segundos que o dispositivo exibirá a economia de tela no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="84259-289">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="84259-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="84259-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="84259-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="84259-291">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-291">Int32</span></span>|<span data-ttu-id="84259-292">O número de segundos que o dispositivo precisa ficar inativo para que a economia de tela seja mostrada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="84259-293">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="84259-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="84259-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="84259-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="84259-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-295">Boolean</span></span>|<span data-ttu-id="84259-296">Se a tela do dispositivo deve ou não mostrar a economia de tela se o áudio/vídeo estiver sendo exibido no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="84259-297">kioskModeApps</span></span>|<span data-ttu-id="84259-298">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="84259-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="84259-299">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="84259-300">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="84259-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="84259-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="84259-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="84259-302">String</span><span class="sxs-lookup"><span data-stu-id="84259-302">String</span></span>|<span data-ttu-id="84259-303">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo está no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="84259-304">kioskModeExitCode</span></span>|<span data-ttu-id="84259-305">String</span><span class="sxs-lookup"><span data-stu-id="84259-305">String</span></span>|<span data-ttu-id="84259-306">Código de saída para permitir que um usuário escape do Modo de Quiosque quando o dispositivo estiver no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="84259-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-308">Boolean</span></span>|<span data-ttu-id="84259-309">Se um botão página principal virtual será exibido ou não quando o dispositivo estiver no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="84259-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="84259-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="84259-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="84259-312">Indica se o botão página principal virtual é um botão página página principal ou um botão página página início flutuante.</span><span class="sxs-lookup"><span data-stu-id="84259-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="84259-313">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="84259-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="84259-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="84259-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-315">Boolean</span></span>|<span data-ttu-id="84259-316">Se um usuário poderá ou não definir as configurações de Bluetooth no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="84259-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-318">Boolean</span></span>|<span data-ttu-id="84259-319">Se um usuário poderá ou não definir as configurações Wi-Fi no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="84259-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-321">Boolean</span></span>|<span data-ttu-id="84259-322">Se um usuário poderá ou não usar a lanterna no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="84259-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-324">Boolean</span></span>|<span data-ttu-id="84259-325">Se um usuário pode ou não alterar o volume de mídia no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="84259-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="84259-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-327">Boolean</span></span>|<span data-ttu-id="84259-328">Se um usuário poderá ou não acessar informações básicas do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="84259-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="84259-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="84259-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-330">Boolean</span></span>|<span data-ttu-id="84259-331">Se o ponto de entrada Configurações Gerenciadas deve ou não ser exibido na tela inicial gerenciada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="84259-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-333">Boolean</span></span>|<span data-ttu-id="84259-334">Se um usuário poderá ou não acessar facilmente o menu de depuração no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="84259-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="84259-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-336">Boolean</span></span>|<span data-ttu-id="84259-337">Se os selos de notificação de aplicativo serão exibidos ou não no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="84259-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="84259-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="84259-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="84259-340">Configuração de orientação da tela inicial gerenciada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="84259-341">Os valores possíveis são: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="84259-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="84259-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="84259-342">kioskModeIconSize</span></span>|[<span data-ttu-id="84259-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="84259-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="84259-344">Configuração do tamanho do ícone para a tela inicial gerenciada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="84259-345">Os possíveis valores são: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="84259-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="84259-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="84259-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="84259-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="84259-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="84259-348">Configuração de ícone de pasta para tela inicial gerenciada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="84259-349">Os valores possíveis são: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="84259-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="84259-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="84259-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="84259-351">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="84259-351">String collection</span></span>|<span data-ttu-id="84259-352">O conjunto restrito de SSIDs WIFI disponíveis para o usuário configurar no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="84259-353">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="84259-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="84259-354">kioskModeAppOrderEnabled</span><span class="sxs-lookup"><span data-stu-id="84259-354">kioskModeAppOrderEnabled</span></span>|<span data-ttu-id="84259-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-355">Boolean</span></span>|<span data-ttu-id="84259-356">Se o pedido do aplicativo será habilitado ou não no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-356">Whether or not to enable app ordering in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-357">kioskModeAppsInFolderOrderedByName</span><span class="sxs-lookup"><span data-stu-id="84259-357">kioskModeAppsInFolderOrderedByName</span></span>|<span data-ttu-id="84259-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-358">Boolean</span></span>|<span data-ttu-id="84259-359">Se os aplicativos serão ou não alfabéticos em uma pasta no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-359">Whether or not to alphabetize applications within a folder in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-360">kioskModeGridHeight</span><span class="sxs-lookup"><span data-stu-id="84259-360">kioskModeGridHeight</span></span>|<span data-ttu-id="84259-361">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-361">Int32</span></span>|<span data-ttu-id="84259-362">Número de linhas para grade da Tela Inicial Gerenciada com ordenação de aplicativos habilitada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-362">Number of rows for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="84259-363">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="84259-363">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="84259-364">kioskModeGridWidth</span><span class="sxs-lookup"><span data-stu-id="84259-364">kioskModeGridWidth</span></span>|<span data-ttu-id="84259-365">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-365">Int32</span></span>|<span data-ttu-id="84259-366">Número de colunas para grade da Tela Inicial Gerenciada com ordenação de aplicativos habilitada no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-366">Number of columns for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="84259-367">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="84259-367">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="84259-368">kioskModeLockHomeScreen</span><span class="sxs-lookup"><span data-stu-id="84259-368">kioskModeLockHomeScreen</span></span>|<span data-ttu-id="84259-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-369">Boolean</span></span>|<span data-ttu-id="84259-370">Se a tela inicial será ou não lock para o usuário final no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-370">Whether or not to lock home screen to the end user in Kiosk Mode.</span></span>|
|<span data-ttu-id="84259-371">kioskModeManagedFolders</span><span class="sxs-lookup"><span data-stu-id="84259-371">kioskModeManagedFolders</span></span>|<span data-ttu-id="84259-372">[Coleção androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)</span><span class="sxs-lookup"><span data-stu-id="84259-372">[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) collection</span></span>|<span data-ttu-id="84259-373">Uma lista de pastas gerenciadas para um dispositivo no Modo de Quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-373">A list of managed folders for a device in Kiosk Mode.</span></span> <span data-ttu-id="84259-374">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="84259-374">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="84259-375">kioskModeAppPositions</span><span class="sxs-lookup"><span data-stu-id="84259-375">kioskModeAppPositions</span></span>|<span data-ttu-id="84259-376">[Coleção androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)</span><span class="sxs-lookup"><span data-stu-id="84259-376">[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) collection</span></span>|<span data-ttu-id="84259-377">A ordenação de itens na tela inicial gerenciada do modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="84259-377">The ordering of items on Kiosk Mode Managed Home Screen.</span></span> <span data-ttu-id="84259-378">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="84259-378">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="84259-379">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="84259-379">microphoneForceMute</span></span>|<span data-ttu-id="84259-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-380">Boolean</span></span>|<span data-ttu-id="84259-381">Indica se o microfone deve ou não ser bloqueado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-381">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="84259-382">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="84259-382">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="84259-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-383">Boolean</span></span>|<span data-ttu-id="84259-384">Indica se o dispositivo permitirá ou não a conexão a uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="84259-384">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="84259-385">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="84259-385">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="84259-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-386">Boolean</span></span>|<span data-ttu-id="84259-387">Indica se o raio de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84259-387">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="84259-388">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="84259-388">passwordBlockKeyguard</span></span>|<span data-ttu-id="84259-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-389">Boolean</span></span>|<span data-ttu-id="84259-390">Indica se a keyguard está ou não desabilitada.</span><span class="sxs-lookup"><span data-stu-id="84259-390">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="84259-391">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="84259-391">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="84259-392">[Coleção androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="84259-392">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="84259-393">Lista de recursos de proteção de chaves do dispositivo a ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84259-393">List of device keyguard features to block.</span></span> <span data-ttu-id="84259-394">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="84259-394">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="84259-395">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="84259-395">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="84259-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="84259-396">passwordExpirationDays</span></span>|<span data-ttu-id="84259-397">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-397">Int32</span></span>|<span data-ttu-id="84259-398">Indica quanto tempo uma senha pode ser definida antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="84259-398">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="84259-399">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="84259-399">Valid values 1 to 365</span></span>|
|<span data-ttu-id="84259-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="84259-400">passwordMinimumLength</span></span>|<span data-ttu-id="84259-401">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-401">Int32</span></span>|<span data-ttu-id="84259-402">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-402">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="84259-403">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="84259-404">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-404">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="84259-405">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-405">Int32</span></span>|<span data-ttu-id="84259-406">Indica o número mínimo de caracteres de carta necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-406">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="84259-407">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-407">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-408">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-408">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="84259-409">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-409">Int32</span></span>|<span data-ttu-id="84259-410">Indica o número mínimo de caracteres de casos inferiores necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-410">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="84259-411">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-411">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-412">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-412">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="84259-413">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-413">Int32</span></span>|<span data-ttu-id="84259-414">Indica o número mínimo de caracteres sem letra necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-414">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="84259-415">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-415">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-416">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-416">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="84259-417">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-417">Int32</span></span>|<span data-ttu-id="84259-418">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-418">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="84259-419">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-419">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-420">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-420">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="84259-421">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-421">Int32</span></span>|<span data-ttu-id="84259-422">Indica o número mínimo de caracteres de símbolos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-422">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="84259-423">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-423">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-424">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-424">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="84259-425">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-425">Int32</span></span>|<span data-ttu-id="84259-426">Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-426">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="84259-427">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-427">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-428">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="84259-428">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="84259-429">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-429">Int32</span></span>|<span data-ttu-id="84259-430">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="84259-430">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="84259-431">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="84259-431">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="84259-432">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-432">Int32</span></span>|<span data-ttu-id="84259-433">Indica a duração do histórico de senhas, em que o usuário não poderá inserir uma nova senha que seja a mesma de qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="84259-433">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="84259-434">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="84259-434">Valid values 0 to 24</span></span>|
|<span data-ttu-id="84259-435">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="84259-435">passwordRequiredType</span></span>|[<span data-ttu-id="84259-436">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="84259-436">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="84259-437">Indica a qualidade mínima de senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-437">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="84259-438">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="84259-438">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="84259-439">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="84259-439">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="84259-440">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-440">Int32</span></span>|<span data-ttu-id="84259-441">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes de o dispositivo ser apagado.</span><span class="sxs-lookup"><span data-stu-id="84259-441">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="84259-442">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="84259-442">Valid values 4 to 11</span></span>|
|<span data-ttu-id="84259-443">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="84259-443">playStoreMode</span></span>|[<span data-ttu-id="84259-444">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="84259-444">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="84259-445">Indica o modo da Play Store do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-445">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="84259-446">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="84259-446">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="84259-447">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-447">safeBootBlocked</span></span>|<span data-ttu-id="84259-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-448">Boolean</span></span>|<span data-ttu-id="84259-449">Indica se a reinicialização do dispositivo na inicialização segura está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="84259-449">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="84259-450">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-450">screenCaptureBlocked</span></span>|<span data-ttu-id="84259-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-451">Boolean</span></span>|<span data-ttu-id="84259-452">Indica se a funcionalidade deve ou não ser desabilitada para fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="84259-452">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="84259-453">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="84259-453">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="84259-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-454">Boolean</span></span>|<span data-ttu-id="84259-455">Indica se o usuário será ou não bloqueado da habilitação de recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84259-455">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="84259-456">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="84259-456">securityRequireVerifyApps</span></span>|<span data-ttu-id="84259-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-457">Boolean</span></span>|<span data-ttu-id="84259-458">Indica se os aplicativos são necessários ou não.</span><span class="sxs-lookup"><span data-stu-id="84259-458">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="84259-459">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-459">statusBarBlocked</span></span>|<span data-ttu-id="84259-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-460">Boolean</span></span>|<span data-ttu-id="84259-461">Indica se ou a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="84259-461">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="84259-462">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="84259-462">stayOnModes</span></span>|<span data-ttu-id="84259-463">[Coleção androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="84259-463">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="84259-464">Lista de modos em que a exibição do dispositivo se manterá ligado.</span><span class="sxs-lookup"><span data-stu-id="84259-464">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="84259-465">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="84259-465">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="84259-466">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="84259-466">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="84259-467">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="84259-467">storageAllowUsb</span></span>|<span data-ttu-id="84259-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-468">Boolean</span></span>|<span data-ttu-id="84259-469">Indica se o armazenamento em massa USB será ou não permitir.</span><span class="sxs-lookup"><span data-stu-id="84259-469">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="84259-470">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="84259-470">storageBlockExternalMedia</span></span>|<span data-ttu-id="84259-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-471">Boolean</span></span>|<span data-ttu-id="84259-472">Indica se a mídia externa deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84259-472">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="84259-473">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="84259-473">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="84259-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-474">Boolean</span></span>|<span data-ttu-id="84259-475">Indica se a transferência de arquivos USB deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="84259-475">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="84259-476">systemUpdateWindowStartMinutesAfterMidafter</span><span class="sxs-lookup"><span data-stu-id="84259-476">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="84259-477">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-477">Int32</span></span>|<span data-ttu-id="84259-478">Indica o número de minutos após a meia-noite em que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="84259-478">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="84259-479">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="84259-479">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="84259-480">systemUpdateWindowEndMinutesAfterMidafter</span><span class="sxs-lookup"><span data-stu-id="84259-480">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="84259-481">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-481">Int32</span></span>|<span data-ttu-id="84259-482">Indica o número de minutos após a meia-noite em que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="84259-482">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="84259-483">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="84259-483">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="84259-484">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="84259-484">systemUpdateInstallType</span></span>|[<span data-ttu-id="84259-485">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="84259-485">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="84259-486">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="84259-486">The type of system update configuration.</span></span> <span data-ttu-id="84259-487">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="84259-487">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="84259-488">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-488">systemWindowsBlocked</span></span>|<span data-ttu-id="84259-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-489">Boolean</span></span>|<span data-ttu-id="84259-490">Se as janelas de prompt do sistema Android serão ou não bloqueados, como notualizações do sistema, atividades de telefone e alertas do sistema.</span><span class="sxs-lookup"><span data-stu-id="84259-490">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="84259-491">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="84259-491">usersBlockAdd</span></span>|<span data-ttu-id="84259-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-492">Boolean</span></span>|<span data-ttu-id="84259-493">Indica se a adição de usuários e perfis está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="84259-493">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="84259-494">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="84259-494">usersBlockRemove</span></span>|<span data-ttu-id="84259-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-495">Boolean</span></span>|<span data-ttu-id="84259-496">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="84259-496">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="84259-497">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="84259-497">volumeBlockAdjustment</span></span>|<span data-ttu-id="84259-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-498">Boolean</span></span>|<span data-ttu-id="84259-499">Indica se o ajuste do volume mestre está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="84259-499">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="84259-500">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="84259-500">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="84259-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-501">Boolean</span></span>|<span data-ttu-id="84259-502">Se um nome de pacote VPN sempre em dia for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="84259-502">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="84259-503">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="84259-503">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="84259-504">String</span><span class="sxs-lookup"><span data-stu-id="84259-504">String</span></span>|<span data-ttu-id="84259-505">Nome do pacote do aplicativo Android para aplicativo que lidará com uma conexão VPN sempre on.</span><span class="sxs-lookup"><span data-stu-id="84259-505">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="84259-506">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="84259-506">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="84259-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-507">Boolean</span></span>|<span data-ttu-id="84259-508">Indica se o usuário será ou não bloqueado para editar as configurações de conexão wi-fi.</span><span class="sxs-lookup"><span data-stu-id="84259-508">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="84259-509">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="84259-509">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="84259-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-510">Boolean</span></span>|<span data-ttu-id="84259-511">Indica se o usuário será ou não bloqueado de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="84259-511">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="84259-512">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="84259-512">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="84259-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-513">Boolean</span></span>|<span data-ttu-id="84259-514">Indica se o usuário pode instalar aplicativos de fontes desconhecidas no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="84259-514">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="84259-515">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-515">personalProfileCameraBlocked</span></span>|<span data-ttu-id="84259-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-516">Boolean</span></span>|<span data-ttu-id="84259-517">Indica se o uso da câmera no perfil pessoal deve ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="84259-517">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="84259-518">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="84259-518">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="84259-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="84259-519">Boolean</span></span>|<span data-ttu-id="84259-520">Indica se a funcionalidade deve ser desabilitada para fazer capturas de tela no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="84259-520">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="84259-521">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="84259-521">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="84259-522">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-522">Int32</span></span>|<span data-ttu-id="84259-523">Indica o número de dias que uma senha de perfil de trabalho pode ser definida antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="84259-523">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="84259-524">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="84259-524">Valid values 1 to 365</span></span>|
|<span data-ttu-id="84259-525">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="84259-525">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="84259-526">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-526">Int32</span></span>|<span data-ttu-id="84259-527">Indica o comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84259-527">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="84259-528">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-528">Valid values 4 to 16</span></span>|
|<span data-ttu-id="84259-529">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-529">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="84259-530">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-530">Int32</span></span>|<span data-ttu-id="84259-531">Indica o número mínimo de caracteres numéricos necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84259-531">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="84259-532">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-532">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-533">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-533">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="84259-534">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-534">Int32</span></span>|<span data-ttu-id="84259-535">Indica o número mínimo de caracteres sem letra necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84259-535">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="84259-536">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-536">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-537">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-537">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="84259-538">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-538">Int32</span></span>|<span data-ttu-id="84259-539">Indica o número mínimo de caracteres de carta necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84259-539">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="84259-540">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-540">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-541">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-541">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="84259-542">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-542">Int32</span></span>|<span data-ttu-id="84259-543">Indica o número mínimo de caracteres de casos inferiores necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84259-543">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="84259-544">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-544">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-545">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-545">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="84259-546">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-546">Int32</span></span>|<span data-ttu-id="84259-547">Indica o número mínimo de caracteres de letra maiúscula necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84259-547">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="84259-548">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-548">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-549">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="84259-549">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="84259-550">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-550">Int32</span></span>|<span data-ttu-id="84259-551">Indica o número mínimo de caracteres de símbolos necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84259-551">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="84259-552">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="84259-552">Valid values 1 to 16</span></span>|
|<span data-ttu-id="84259-553">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="84259-553">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="84259-554">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-554">Int32</span></span>|<span data-ttu-id="84259-555">Indica a duração do histórico de senhas do perfil de trabalho, em que o usuário não poderá inserir uma nova senha igual à de qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="84259-555">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="84259-556">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="84259-556">Valid values 0 to 24</span></span>|
|<span data-ttu-id="84259-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="84259-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="84259-558">Int32</span><span class="sxs-lookup"><span data-stu-id="84259-558">Int32</span></span>|<span data-ttu-id="84259-559">Indica o número de vezes que um usuário pode inserir uma senha de perfil de trabalho incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="84259-559">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="84259-560">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="84259-560">Valid values 4 to 11</span></span>|
|<span data-ttu-id="84259-561">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="84259-561">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="84259-562">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="84259-562">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="84259-563">Indica a qualidade mínima de senha necessária na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="84259-563">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="84259-564">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="84259-564">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="84259-565">Resposta</span><span class="sxs-lookup"><span data-stu-id="84259-565">Response</span></span>
<span data-ttu-id="84259-566">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84259-566">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84259-567">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84259-567">Example</span></span>

### <a name="request"></a><span data-ttu-id="84259-568">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84259-568">Request</span></span>
<span data-ttu-id="84259-569">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84259-569">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="84259-570">Resposta</span><span class="sxs-lookup"><span data-stu-id="84259-570">Response</span></span>
<span data-ttu-id="84259-p160">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84259-p160">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




