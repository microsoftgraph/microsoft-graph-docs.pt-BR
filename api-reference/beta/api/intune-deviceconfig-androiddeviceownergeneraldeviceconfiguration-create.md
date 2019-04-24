---
title: Criar androidDeviceOwnerGeneralDeviceConfiguration
description: Criar um novo objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa5f2ac532e4b8e912b47a50be755ab0ceb495fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32481021"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="73d75-103">Criar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="73d75-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="73d75-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73d75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73d75-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73d75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73d75-106">Criar um novo objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="73d75-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73d75-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73d75-107">Prerequisites</span></span>
<span data-ttu-id="73d75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73d75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73d75-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73d75-110">Permission type</span></span>|<span data-ttu-id="73d75-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73d75-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73d75-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73d75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73d75-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d75-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73d75-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73d75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73d75-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73d75-115">Not supported.</span></span>|
|<span data-ttu-id="73d75-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73d75-116">Application</span></span>|<span data-ttu-id="73d75-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73d75-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73d75-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73d75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="73d75-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73d75-119">Request headers</span></span>
|<span data-ttu-id="73d75-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73d75-120">Header</span></span>|<span data-ttu-id="73d75-121">Valor</span><span class="sxs-lookup"><span data-stu-id="73d75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73d75-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73d75-122">Authorization</span></span>|<span data-ttu-id="73d75-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73d75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73d75-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73d75-124">Accept</span></span>|<span data-ttu-id="73d75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73d75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73d75-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73d75-126">Request body</span></span>
<span data-ttu-id="73d75-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="73d75-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="73d75-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="73d75-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="73d75-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73d75-129">Property</span></span>|<span data-ttu-id="73d75-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="73d75-130">Type</span></span>|<span data-ttu-id="73d75-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="73d75-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73d75-132">id</span><span class="sxs-lookup"><span data-stu-id="73d75-132">id</span></span>|<span data-ttu-id="73d75-133">String</span><span class="sxs-lookup"><span data-stu-id="73d75-133">String</span></span>|<span data-ttu-id="73d75-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73d75-134">Key of the entity.</span></span> <span data-ttu-id="73d75-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73d75-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73d75-136">lastModifiedDateTime</span></span>|<span data-ttu-id="73d75-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73d75-137">DateTimeOffset</span></span>|<span data-ttu-id="73d75-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="73d75-138">DateTime the object was last modified.</span></span> <span data-ttu-id="73d75-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73d75-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73d75-140">roleScopeTagIds</span></span>|<span data-ttu-id="73d75-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73d75-141">String collection</span></span>|<span data-ttu-id="73d75-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="73d75-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73d75-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73d75-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73d75-144">supportsScopeTags</span></span>|<span data-ttu-id="73d75-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-145">Boolean</span></span>|<span data-ttu-id="73d75-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="73d75-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73d75-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="73d75-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73d75-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="73d75-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73d75-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73d75-149">This property is read-only.</span></span> <span data-ttu-id="73d75-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73d75-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73d75-151">createdDateTime</span></span>|<span data-ttu-id="73d75-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73d75-152">DateTimeOffset</span></span>|<span data-ttu-id="73d75-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="73d75-153">DateTime the object was created.</span></span> <span data-ttu-id="73d75-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73d75-155">description</span><span class="sxs-lookup"><span data-stu-id="73d75-155">description</span></span>|<span data-ttu-id="73d75-156">String</span><span class="sxs-lookup"><span data-stu-id="73d75-156">String</span></span>|<span data-ttu-id="73d75-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73d75-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73d75-159">displayName</span><span class="sxs-lookup"><span data-stu-id="73d75-159">displayName</span></span>|<span data-ttu-id="73d75-160">String</span><span class="sxs-lookup"><span data-stu-id="73d75-160">String</span></span>|<span data-ttu-id="73d75-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73d75-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73d75-163">versão</span><span class="sxs-lookup"><span data-stu-id="73d75-163">version</span></span>|<span data-ttu-id="73d75-164">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-164">Int32</span></span>|<span data-ttu-id="73d75-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-165">Version of the device configuration.</span></span> <span data-ttu-id="73d75-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73d75-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="73d75-167">accountsBlockModification</span></span>|<span data-ttu-id="73d75-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-168">Boolean</span></span>|<span data-ttu-id="73d75-169">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="73d75-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="73d75-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="73d75-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="73d75-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-171">Boolean</span></span>|<span data-ttu-id="73d75-172">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="73d75-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="73d75-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="73d75-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="73d75-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="73d75-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="73d75-175">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73d75-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="73d75-176">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="73d75-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="73d75-177">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="73d75-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="73d75-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="73d75-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="73d75-179">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="73d75-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="73d75-180">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="73d75-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="73d75-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="73d75-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="73d75-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-182">Boolean</span></span>|<span data-ttu-id="73d75-183">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="73d75-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="73d75-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="73d75-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="73d75-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-185">Boolean</span></span>|<span data-ttu-id="73d75-186">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="73d75-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="73d75-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="73d75-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="73d75-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-188">Boolean</span></span>|<span data-ttu-id="73d75-189">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="73d75-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="73d75-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="73d75-190">cameraBlocked</span></span>|<span data-ttu-id="73d75-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-191">Boolean</span></span>|<span data-ttu-id="73d75-192">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="73d75-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="73d75-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="73d75-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="73d75-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="73d75-194">Boolean</span></span>|<span data-ttu-id="73d75-195">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="73d75-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="73d75-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="73d75-196">dataRoamingBlocked</span></span>|<span data-ttu-id="73d75-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-197">Boolean</span></span>|<span data-ttu-id="73d75-198">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="73d75-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="73d75-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="73d75-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="73d75-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-200">Boolean</span></span>|<span data-ttu-id="73d75-201">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="73d75-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="73d75-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="73d75-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="73d75-203">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73d75-203">String collection</span></span>|<span data-ttu-id="73d75-204">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="73d75-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="73d75-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="73d75-205">factoryResetBlocked</span></span>|<span data-ttu-id="73d75-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="73d75-206">Boolean</span></span>|<span data-ttu-id="73d75-207">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="73d75-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="73d75-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="73d75-208">kioskModeApps</span></span>|<span data-ttu-id="73d75-209">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="73d75-210">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="73d75-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="73d75-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="73d75-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="73d75-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="73d75-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="73d75-213">String</span><span class="sxs-lookup"><span data-stu-id="73d75-213">String</span></span>|<span data-ttu-id="73d75-214">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="73d75-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="73d75-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="73d75-215">kioskModeExitCode</span></span>|<span data-ttu-id="73d75-216">String</span><span class="sxs-lookup"><span data-stu-id="73d75-216">String</span></span>|<span data-ttu-id="73d75-217">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="73d75-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="73d75-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="73d75-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="73d75-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-219">Boolean</span></span>|<span data-ttu-id="73d75-220">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="73d75-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="73d75-221">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="73d75-221">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="73d75-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-222">Boolean</span></span>|<span data-ttu-id="73d75-223">Se permitirá ou não que um usuário defina configurações de Bluetooth no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="73d75-223">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="73d75-224">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="73d75-224">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="73d75-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-225">Boolean</span></span>|<span data-ttu-id="73d75-226">Se permitirá ou não que um usuário defina configurações de Wi-Fi no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="73d75-226">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="73d75-227">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="73d75-227">microphoneForceMute</span></span>|<span data-ttu-id="73d75-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-228">Boolean</span></span>|<span data-ttu-id="73d75-229">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="73d75-229">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="73d75-230">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="73d75-230">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="73d75-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-231">Boolean</span></span>|<span data-ttu-id="73d75-232">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="73d75-232">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="73d75-233">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="73d75-233">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="73d75-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-234">Boolean</span></span>|<span data-ttu-id="73d75-235">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="73d75-235">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="73d75-236">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="73d75-236">passwordBlockKeyguard</span></span>|<span data-ttu-id="73d75-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-237">Boolean</span></span>|<span data-ttu-id="73d75-238">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="73d75-238">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="73d75-239">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="73d75-239">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="73d75-240">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-240">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="73d75-241">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="73d75-241">List of device keyguard features to block.</span></span> <span data-ttu-id="73d75-242">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="73d75-242">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="73d75-243">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="73d75-243">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="73d75-244">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="73d75-244">passwordExpirationDays</span></span>|<span data-ttu-id="73d75-245">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-245">Int32</span></span>|<span data-ttu-id="73d75-246">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="73d75-246">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="73d75-247">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="73d75-247">Valid values 1 to 365</span></span>|
|<span data-ttu-id="73d75-248">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="73d75-248">passwordMinimumLength</span></span>|<span data-ttu-id="73d75-249">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-249">Int32</span></span>|<span data-ttu-id="73d75-250">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-250">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="73d75-251">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="73d75-251">Valid values 4 to 16</span></span>|
|<span data-ttu-id="73d75-252">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="73d75-252">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="73d75-253">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-253">Int32</span></span>|<span data-ttu-id="73d75-254">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-254">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="73d75-255">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="73d75-255">Valid values 1 to 16</span></span>|
|<span data-ttu-id="73d75-256">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="73d75-256">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="73d75-257">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-257">Int32</span></span>|<span data-ttu-id="73d75-258">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-258">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="73d75-259">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="73d75-259">Valid values 1 to 16</span></span>|
|<span data-ttu-id="73d75-260">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="73d75-260">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="73d75-261">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-261">Int32</span></span>|<span data-ttu-id="73d75-262">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-262">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="73d75-263">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="73d75-263">Valid values 1 to 16</span></span>|
|<span data-ttu-id="73d75-264">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="73d75-264">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="73d75-265">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-265">Int32</span></span>|<span data-ttu-id="73d75-266">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-266">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="73d75-267">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="73d75-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="73d75-268">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="73d75-268">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="73d75-269">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-269">Int32</span></span>|<span data-ttu-id="73d75-270">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-270">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="73d75-271">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="73d75-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="73d75-272">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="73d75-272">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="73d75-273">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-273">Int32</span></span>|<span data-ttu-id="73d75-274">Indica o número mínimo de caracteres de caseletter superior necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-274">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="73d75-275">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="73d75-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="73d75-276">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="73d75-276">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="73d75-277">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-277">Int32</span></span>|<span data-ttu-id="73d75-278">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="73d75-278">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="73d75-279">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="73d75-279">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="73d75-280">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-280">Int32</span></span>|<span data-ttu-id="73d75-281">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="73d75-281">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="73d75-282">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="73d75-282">Valid values 0 to 24</span></span>|
|<span data-ttu-id="73d75-283">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="73d75-283">passwordRequiredType</span></span>|[<span data-ttu-id="73d75-284">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="73d75-284">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="73d75-285">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-285">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="73d75-286">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="73d75-286">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="73d75-287">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="73d75-287">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="73d75-288">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-288">Int32</span></span>|<span data-ttu-id="73d75-289">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="73d75-289">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="73d75-290">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="73d75-290">Valid values 4 to 11</span></span>|
|<span data-ttu-id="73d75-291">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="73d75-291">playStoreMode</span></span>|[<span data-ttu-id="73d75-292">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="73d75-292">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="73d75-293">Indica o modo de repositório de execução do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-293">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="73d75-294">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="73d75-294">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="73d75-295">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="73d75-295">safeBootBlocked</span></span>|<span data-ttu-id="73d75-296">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-296">Boolean</span></span>|<span data-ttu-id="73d75-297">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="73d75-297">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="73d75-298">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="73d75-298">screenCaptureBlocked</span></span>|<span data-ttu-id="73d75-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="73d75-299">Boolean</span></span>|<span data-ttu-id="73d75-300">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="73d75-300">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="73d75-301">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="73d75-301">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="73d75-302">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-302">Boolean</span></span>|<span data-ttu-id="73d75-303">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73d75-303">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="73d75-304">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="73d75-304">securityRequireVerifyApps</span></span>|<span data-ttu-id="73d75-305">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-305">Boolean</span></span>|<span data-ttu-id="73d75-306">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="73d75-306">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="73d75-307">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="73d75-307">statusBarBlocked</span></span>|<span data-ttu-id="73d75-308">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-308">Boolean</span></span>|<span data-ttu-id="73d75-309">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="73d75-309">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="73d75-310">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="73d75-310">stayOnModes</span></span>|<span data-ttu-id="73d75-311">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="73d75-311">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="73d75-312">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="73d75-312">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="73d75-313">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="73d75-313">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="73d75-314">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="73d75-314">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="73d75-315">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="73d75-315">storageAllowUsb</span></span>|<span data-ttu-id="73d75-316">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-316">Boolean</span></span>|<span data-ttu-id="73d75-317">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="73d75-317">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="73d75-318">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="73d75-318">storageBlockExternalMedia</span></span>|<span data-ttu-id="73d75-319">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-319">Boolean</span></span>|<span data-ttu-id="73d75-320">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="73d75-320">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="73d75-321">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="73d75-321">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="73d75-322">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-322">Boolean</span></span>|<span data-ttu-id="73d75-323">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="73d75-323">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="73d75-324">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="73d75-324">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="73d75-325">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-325">Int32</span></span>|<span data-ttu-id="73d75-326">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="73d75-326">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="73d75-327">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="73d75-327">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="73d75-328">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="73d75-328">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="73d75-329">Int32</span><span class="sxs-lookup"><span data-stu-id="73d75-329">Int32</span></span>|<span data-ttu-id="73d75-330">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="73d75-330">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="73d75-331">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="73d75-331">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="73d75-332">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="73d75-332">systemUpdateInstallType</span></span>|[<span data-ttu-id="73d75-333">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="73d75-333">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="73d75-334">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="73d75-334">The type of system update configuration.</span></span> <span data-ttu-id="73d75-335">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="73d75-335">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="73d75-336">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="73d75-336">systemWindowsBlocked</span></span>|<span data-ttu-id="73d75-337">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-337">Boolean</span></span>|<span data-ttu-id="73d75-338">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="73d75-338">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="73d75-339">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="73d75-339">usersBlockAdd</span></span>|<span data-ttu-id="73d75-340">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-340">Boolean</span></span>|<span data-ttu-id="73d75-341">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="73d75-341">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="73d75-342">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="73d75-342">usersBlockRemove</span></span>|<span data-ttu-id="73d75-343">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-343">Boolean</span></span>|<span data-ttu-id="73d75-344">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="73d75-344">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="73d75-345">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="73d75-345">volumeBlockAdjustment</span></span>|<span data-ttu-id="73d75-346">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-346">Boolean</span></span>|<span data-ttu-id="73d75-347">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="73d75-347">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="73d75-348">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="73d75-348">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="73d75-349">String</span><span class="sxs-lookup"><span data-stu-id="73d75-349">String</span></span>|<span data-ttu-id="73d75-350">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="73d75-350">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="73d75-351">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="73d75-351">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="73d75-352">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-352">Boolean</span></span>|<span data-ttu-id="73d75-353">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="73d75-353">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="73d75-354">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="73d75-354">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="73d75-355">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-355">Boolean</span></span>|<span data-ttu-id="73d75-356">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="73d75-356">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="73d75-357">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="73d75-357">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="73d75-358">Booliano</span><span class="sxs-lookup"><span data-stu-id="73d75-358">Boolean</span></span>|<span data-ttu-id="73d75-359">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="73d75-359">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="73d75-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="73d75-360">Response</span></span>
<span data-ttu-id="73d75-361">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73d75-361">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73d75-362">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73d75-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="73d75-363">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73d75-363">Request</span></span>
<span data-ttu-id="73d75-364">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73d75-364">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73d75-365">Resposta</span><span class="sxs-lookup"><span data-stu-id="73d75-365">Response</span></span>
<span data-ttu-id="73d75-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73d75-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





