---
title: Criar androidDeviceOwnerGeneralDeviceConfiguration
description: Criar um novo objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa5f2ac532e4b8e912b47a50be755ab0ceb495fa
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771765"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="98e32-103">Criar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="98e32-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="98e32-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98e32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98e32-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98e32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98e32-106">Criar um novo objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="98e32-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98e32-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98e32-107">Prerequisites</span></span>
<span data-ttu-id="98e32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98e32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98e32-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98e32-110">Permission type</span></span>|<span data-ttu-id="98e32-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98e32-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98e32-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98e32-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98e32-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98e32-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98e32-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98e32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98e32-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98e32-115">Not supported.</span></span>|
|<span data-ttu-id="98e32-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98e32-116">Application</span></span>|<span data-ttu-id="98e32-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98e32-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98e32-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98e32-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="98e32-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98e32-119">Request headers</span></span>
|<span data-ttu-id="98e32-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98e32-120">Header</span></span>|<span data-ttu-id="98e32-121">Valor</span><span class="sxs-lookup"><span data-stu-id="98e32-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98e32-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="98e32-122">Authorization</span></span>|<span data-ttu-id="98e32-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98e32-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98e32-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98e32-124">Accept</span></span>|<span data-ttu-id="98e32-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98e32-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98e32-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98e32-126">Request body</span></span>
<span data-ttu-id="98e32-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="98e32-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="98e32-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="98e32-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="98e32-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98e32-129">Property</span></span>|<span data-ttu-id="98e32-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="98e32-130">Type</span></span>|<span data-ttu-id="98e32-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="98e32-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98e32-132">id</span><span class="sxs-lookup"><span data-stu-id="98e32-132">id</span></span>|<span data-ttu-id="98e32-133">String</span><span class="sxs-lookup"><span data-stu-id="98e32-133">String</span></span>|<span data-ttu-id="98e32-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98e32-134">Key of the entity.</span></span> <span data-ttu-id="98e32-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e32-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98e32-136">lastModifiedDateTime</span></span>|<span data-ttu-id="98e32-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e32-137">DateTimeOffset</span></span>|<span data-ttu-id="98e32-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="98e32-138">DateTime the object was last modified.</span></span> <span data-ttu-id="98e32-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e32-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="98e32-140">roleScopeTagIds</span></span>|<span data-ttu-id="98e32-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="98e32-141">String collection</span></span>|<span data-ttu-id="98e32-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="98e32-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="98e32-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e32-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="98e32-144">supportsScopeTags</span></span>|<span data-ttu-id="98e32-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-145">Boolean</span></span>|<span data-ttu-id="98e32-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="98e32-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="98e32-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="98e32-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="98e32-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="98e32-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="98e32-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="98e32-149">This property is read-only.</span></span> <span data-ttu-id="98e32-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e32-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98e32-151">createdDateTime</span></span>|<span data-ttu-id="98e32-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e32-152">DateTimeOffset</span></span>|<span data-ttu-id="98e32-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="98e32-153">DateTime the object was created.</span></span> <span data-ttu-id="98e32-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e32-155">description</span><span class="sxs-lookup"><span data-stu-id="98e32-155">description</span></span>|<span data-ttu-id="98e32-156">String</span><span class="sxs-lookup"><span data-stu-id="98e32-156">String</span></span>|<span data-ttu-id="98e32-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="98e32-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e32-159">displayName</span><span class="sxs-lookup"><span data-stu-id="98e32-159">displayName</span></span>|<span data-ttu-id="98e32-160">String</span><span class="sxs-lookup"><span data-stu-id="98e32-160">String</span></span>|<span data-ttu-id="98e32-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="98e32-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e32-163">versão</span><span class="sxs-lookup"><span data-stu-id="98e32-163">version</span></span>|<span data-ttu-id="98e32-164">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-164">Int32</span></span>|<span data-ttu-id="98e32-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-165">Version of the device configuration.</span></span> <span data-ttu-id="98e32-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98e32-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="98e32-167">accountsBlockModification</span></span>|<span data-ttu-id="98e32-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-168">Boolean</span></span>|<span data-ttu-id="98e32-169">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="98e32-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="98e32-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="98e32-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="98e32-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-171">Boolean</span></span>|<span data-ttu-id="98e32-172">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="98e32-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="98e32-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="98e32-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="98e32-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="98e32-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="98e32-175">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98e32-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="98e32-176">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="98e32-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="98e32-177">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="98e32-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="98e32-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="98e32-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="98e32-179">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="98e32-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="98e32-180">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="98e32-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="98e32-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="98e32-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="98e32-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-182">Boolean</span></span>|<span data-ttu-id="98e32-183">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="98e32-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="98e32-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="98e32-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="98e32-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-185">Boolean</span></span>|<span data-ttu-id="98e32-186">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="98e32-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="98e32-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="98e32-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="98e32-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-188">Boolean</span></span>|<span data-ttu-id="98e32-189">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="98e32-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="98e32-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="98e32-190">cameraBlocked</span></span>|<span data-ttu-id="98e32-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-191">Boolean</span></span>|<span data-ttu-id="98e32-192">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="98e32-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="98e32-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="98e32-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="98e32-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="98e32-194">Boolean</span></span>|<span data-ttu-id="98e32-195">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98e32-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="98e32-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="98e32-196">dataRoamingBlocked</span></span>|<span data-ttu-id="98e32-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-197">Boolean</span></span>|<span data-ttu-id="98e32-198">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="98e32-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="98e32-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="98e32-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="98e32-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-200">Boolean</span></span>|<span data-ttu-id="98e32-201">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="98e32-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="98e32-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="98e32-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="98e32-203">Coleção String</span><span class="sxs-lookup"><span data-stu-id="98e32-203">String collection</span></span>|<span data-ttu-id="98e32-204">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="98e32-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="98e32-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="98e32-205">factoryResetBlocked</span></span>|<span data-ttu-id="98e32-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="98e32-206">Boolean</span></span>|<span data-ttu-id="98e32-207">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="98e32-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="98e32-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="98e32-208">kioskModeApps</span></span>|<span data-ttu-id="98e32-209">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="98e32-210">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98e32-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="98e32-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="98e32-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="98e32-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="98e32-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="98e32-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e32-213">String</span></span>|<span data-ttu-id="98e32-214">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98e32-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="98e32-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="98e32-215">kioskModeExitCode</span></span>|<span data-ttu-id="98e32-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e32-216">String</span></span>|<span data-ttu-id="98e32-217">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98e32-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="98e32-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="98e32-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="98e32-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-219">Boolean</span></span>|<span data-ttu-id="98e32-220">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98e32-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="98e32-221">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="98e32-221">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="98e32-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-222">Boolean</span></span>|<span data-ttu-id="98e32-223">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98e32-223">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="98e32-224">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="98e32-224">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="98e32-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-225">Boolean</span></span>|<span data-ttu-id="98e32-226">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98e32-226">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="98e32-227">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="98e32-227">microphoneForceMute</span></span>|<span data-ttu-id="98e32-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-228">Boolean</span></span>|<span data-ttu-id="98e32-229">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98e32-229">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="98e32-230">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="98e32-230">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="98e32-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-231">Boolean</span></span>|<span data-ttu-id="98e32-232">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="98e32-232">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="98e32-233">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="98e32-233">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="98e32-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-234">Boolean</span></span>|<span data-ttu-id="98e32-235">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98e32-235">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="98e32-236">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="98e32-236">passwordBlockKeyguard</span></span>|<span data-ttu-id="98e32-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-237">Boolean</span></span>|<span data-ttu-id="98e32-238">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="98e32-238">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="98e32-239">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="98e32-239">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="98e32-240">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="98e32-241">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="98e32-241">List of device keyguard features to block.</span></span> <span data-ttu-id="98e32-242">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="98e32-242">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="98e32-243">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="98e32-243">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="98e32-244">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="98e32-244">passwordExpirationDays</span></span>|<span data-ttu-id="98e32-245">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-245">Int32</span></span>|<span data-ttu-id="98e32-246">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="98e32-246">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="98e32-247">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="98e32-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="98e32-248">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="98e32-248">passwordMinimumLength</span></span>|<span data-ttu-id="98e32-249">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-249">Int32</span></span>|<span data-ttu-id="98e32-250">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-250">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="98e32-251">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="98e32-251">Valid values 4 to 16</span></span>|
|<span data-ttu-id="98e32-252">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="98e32-252">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="98e32-253">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-253">Int32</span></span>|<span data-ttu-id="98e32-254">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-254">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="98e32-255">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="98e32-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="98e32-256">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="98e32-256">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="98e32-257">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-257">Int32</span></span>|<span data-ttu-id="98e32-258">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-258">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="98e32-259">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="98e32-259">Valid values 1 to 16</span></span>|
|<span data-ttu-id="98e32-260">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="98e32-260">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="98e32-261">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-261">Int32</span></span>|<span data-ttu-id="98e32-262">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-262">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="98e32-263">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="98e32-263">Valid values 1 to 16</span></span>|
|<span data-ttu-id="98e32-264">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="98e32-264">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="98e32-265">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-265">Int32</span></span>|<span data-ttu-id="98e32-266">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-266">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="98e32-267">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="98e32-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="98e32-268">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="98e32-268">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="98e32-269">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-269">Int32</span></span>|<span data-ttu-id="98e32-270">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-270">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="98e32-271">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="98e32-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="98e32-272">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="98e32-272">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="98e32-273">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-273">Int32</span></span>|<span data-ttu-id="98e32-274">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-274">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="98e32-275">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="98e32-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="98e32-276">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="98e32-276">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="98e32-277">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-277">Int32</span></span>|<span data-ttu-id="98e32-278">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="98e32-278">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="98e32-279">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="98e32-279">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="98e32-280">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-280">Int32</span></span>|<span data-ttu-id="98e32-281">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="98e32-281">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="98e32-282">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="98e32-282">Valid values 0 to 24</span></span>|
|<span data-ttu-id="98e32-283">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="98e32-283">passwordRequiredType</span></span>|[<span data-ttu-id="98e32-284">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="98e32-284">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="98e32-285">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-285">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="98e32-286">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="98e32-286">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="98e32-287">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="98e32-287">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="98e32-288">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-288">Int32</span></span>|<span data-ttu-id="98e32-289">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="98e32-289">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="98e32-290">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="98e32-290">Valid values 4 to 11</span></span>|
|<span data-ttu-id="98e32-291">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="98e32-291">playStoreMode</span></span>|[<span data-ttu-id="98e32-292">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="98e32-292">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="98e32-293">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-293">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="98e32-294">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="98e32-294">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="98e32-295">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="98e32-295">safeBootBlocked</span></span>|<span data-ttu-id="98e32-296">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-296">Boolean</span></span>|<span data-ttu-id="98e32-297">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="98e32-297">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="98e32-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="98e32-298">screenCaptureBlocked</span></span>|<span data-ttu-id="98e32-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="98e32-299">Boolean</span></span>|<span data-ttu-id="98e32-300">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="98e32-300">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="98e32-301">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="98e32-301">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="98e32-302">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-302">Boolean</span></span>|<span data-ttu-id="98e32-303">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98e32-303">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="98e32-304">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="98e32-304">securityRequireVerifyApps</span></span>|<span data-ttu-id="98e32-305">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-305">Boolean</span></span>|<span data-ttu-id="98e32-306">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="98e32-306">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="98e32-307">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="98e32-307">statusBarBlocked</span></span>|<span data-ttu-id="98e32-308">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-308">Boolean</span></span>|<span data-ttu-id="98e32-309">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="98e32-309">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="98e32-310">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="98e32-310">stayOnModes</span></span>|<span data-ttu-id="98e32-311">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="98e32-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="98e32-312">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="98e32-312">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="98e32-313">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="98e32-313">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="98e32-314">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="98e32-314">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="98e32-315">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="98e32-315">storageAllowUsb</span></span>|<span data-ttu-id="98e32-316">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-316">Boolean</span></span>|<span data-ttu-id="98e32-317">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="98e32-317">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="98e32-318">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="98e32-318">storageBlockExternalMedia</span></span>|<span data-ttu-id="98e32-319">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-319">Boolean</span></span>|<span data-ttu-id="98e32-320">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98e32-320">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="98e32-321">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="98e32-321">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="98e32-322">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-322">Boolean</span></span>|<span data-ttu-id="98e32-323">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98e32-323">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="98e32-324">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="98e32-324">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="98e32-325">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-325">Int32</span></span>|<span data-ttu-id="98e32-326">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="98e32-326">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="98e32-327">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="98e32-327">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="98e32-328">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="98e32-328">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="98e32-329">Int32</span><span class="sxs-lookup"><span data-stu-id="98e32-329">Int32</span></span>|<span data-ttu-id="98e32-330">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="98e32-330">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="98e32-331">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="98e32-331">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="98e32-332">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="98e32-332">systemUpdateInstallType</span></span>|[<span data-ttu-id="98e32-333">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="98e32-333">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="98e32-334">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="98e32-334">The type of system update configuration.</span></span> <span data-ttu-id="98e32-335">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="98e32-335">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="98e32-336">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="98e32-336">systemWindowsBlocked</span></span>|<span data-ttu-id="98e32-337">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-337">Boolean</span></span>|<span data-ttu-id="98e32-338">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="98e32-338">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="98e32-339">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="98e32-339">usersBlockAdd</span></span>|<span data-ttu-id="98e32-340">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-340">Boolean</span></span>|<span data-ttu-id="98e32-341">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="98e32-341">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="98e32-342">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="98e32-342">usersBlockRemove</span></span>|<span data-ttu-id="98e32-343">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-343">Boolean</span></span>|<span data-ttu-id="98e32-344">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="98e32-344">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="98e32-345">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="98e32-345">volumeBlockAdjustment</span></span>|<span data-ttu-id="98e32-346">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-346">Boolean</span></span>|<span data-ttu-id="98e32-347">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="98e32-347">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="98e32-348">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="98e32-348">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="98e32-349">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e32-349">String</span></span>|<span data-ttu-id="98e32-350">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="98e32-350">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="98e32-351">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="98e32-351">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="98e32-352">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-352">Boolean</span></span>|<span data-ttu-id="98e32-353">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="98e32-353">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="98e32-354">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="98e32-354">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="98e32-355">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-355">Boolean</span></span>|<span data-ttu-id="98e32-356">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="98e32-356">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="98e32-357">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="98e32-357">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="98e32-358">Booliano</span><span class="sxs-lookup"><span data-stu-id="98e32-358">Boolean</span></span>|<span data-ttu-id="98e32-359">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="98e32-359">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="98e32-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="98e32-360">Response</span></span>
<span data-ttu-id="98e32-361">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98e32-361">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98e32-362">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98e32-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="98e32-363">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98e32-363">Request</span></span>
<span data-ttu-id="98e32-364">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98e32-364">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2905

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="98e32-365">Resposta</span><span class="sxs-lookup"><span data-stu-id="98e32-365">Response</span></span>
<span data-ttu-id="98e32-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98e32-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3077

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





