---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1af234832c874c69892c4676cf7d990a7b7f5ac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967871"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="93399-103">Atualizar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="93399-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="93399-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93399-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93399-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93399-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93399-106">Atualiza as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="93399-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93399-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93399-107">Prerequisites</span></span>
<span data-ttu-id="93399-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93399-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93399-110">Permission type</span></span>|<span data-ttu-id="93399-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93399-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93399-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93399-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93399-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93399-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93399-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93399-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93399-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93399-115">Not supported.</span></span>|
|<span data-ttu-id="93399-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93399-116">Application</span></span>|<span data-ttu-id="93399-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93399-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93399-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93399-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="93399-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93399-119">Request headers</span></span>
|<span data-ttu-id="93399-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93399-120">Header</span></span>|<span data-ttu-id="93399-121">Valor</span><span class="sxs-lookup"><span data-stu-id="93399-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93399-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="93399-122">Authorization</span></span>|<span data-ttu-id="93399-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93399-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93399-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93399-124">Accept</span></span>|<span data-ttu-id="93399-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93399-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93399-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93399-126">Request body</span></span>
<span data-ttu-id="93399-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="93399-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="93399-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="93399-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="93399-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93399-129">Property</span></span>|<span data-ttu-id="93399-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="93399-130">Type</span></span>|<span data-ttu-id="93399-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="93399-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93399-132">id</span><span class="sxs-lookup"><span data-stu-id="93399-132">id</span></span>|<span data-ttu-id="93399-133">String</span><span class="sxs-lookup"><span data-stu-id="93399-133">String</span></span>|<span data-ttu-id="93399-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="93399-134">Key of the entity.</span></span> <span data-ttu-id="93399-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93399-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93399-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93399-136">lastModifiedDateTime</span></span>|<span data-ttu-id="93399-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93399-137">DateTimeOffset</span></span>|<span data-ttu-id="93399-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="93399-138">DateTime the object was last modified.</span></span> <span data-ttu-id="93399-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93399-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93399-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93399-140">roleScopeTagIds</span></span>|<span data-ttu-id="93399-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="93399-141">String collection</span></span>|<span data-ttu-id="93399-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="93399-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="93399-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93399-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93399-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="93399-144">supportsScopeTags</span></span>|<span data-ttu-id="93399-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-145">Boolean</span></span>|<span data-ttu-id="93399-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="93399-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="93399-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="93399-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="93399-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="93399-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="93399-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93399-149">This property is read-only.</span></span> <span data-ttu-id="93399-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93399-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93399-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93399-151">createdDateTime</span></span>|<span data-ttu-id="93399-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93399-152">DateTimeOffset</span></span>|<span data-ttu-id="93399-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="93399-153">DateTime the object was created.</span></span> <span data-ttu-id="93399-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93399-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93399-155">descrição</span><span class="sxs-lookup"><span data-stu-id="93399-155">description</span></span>|<span data-ttu-id="93399-156">String</span><span class="sxs-lookup"><span data-stu-id="93399-156">String</span></span>|<span data-ttu-id="93399-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93399-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="93399-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93399-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93399-159">displayName</span><span class="sxs-lookup"><span data-stu-id="93399-159">displayName</span></span>|<span data-ttu-id="93399-160">String</span><span class="sxs-lookup"><span data-stu-id="93399-160">String</span></span>|<span data-ttu-id="93399-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93399-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="93399-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93399-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93399-163">versão</span><span class="sxs-lookup"><span data-stu-id="93399-163">version</span></span>|<span data-ttu-id="93399-164">Int32</span><span class="sxs-lookup"><span data-stu-id="93399-164">Int32</span></span>|<span data-ttu-id="93399-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93399-165">Version of the device configuration.</span></span> <span data-ttu-id="93399-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93399-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93399-167">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="93399-167">accountsBlockModification</span></span>|<span data-ttu-id="93399-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-168">Boolean</span></span>|<span data-ttu-id="93399-169">Indica se a adição ou a remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="93399-169">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="93399-170">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="93399-170">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="93399-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-171">Boolean</span></span>|<span data-ttu-id="93399-172">Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="93399-172">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="93399-173">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="93399-173">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="93399-174">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="93399-174">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="93399-175">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="93399-175">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="93399-176">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="93399-176">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="93399-177">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="93399-177">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="93399-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="93399-178">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="93399-179">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="93399-179">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="93399-180">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="93399-180">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="93399-181">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="93399-181">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="93399-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-182">Boolean</span></span>|<span data-ttu-id="93399-183">Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="93399-183">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="93399-184">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="93399-184">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="93399-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-185">Boolean</span></span>|<span data-ttu-id="93399-186">Indica se um usuário será ou não impedido de configurar o Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="93399-186">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="93399-187">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="93399-187">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="93399-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-188">Boolean</span></span>|<span data-ttu-id="93399-189">Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="93399-189">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="93399-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="93399-190">cameraBlocked</span></span>|<span data-ttu-id="93399-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-191">Boolean</span></span>|<span data-ttu-id="93399-192">Indica se o uso da câmera deve ou não ser desativado.</span><span class="sxs-lookup"><span data-stu-id="93399-192">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="93399-193">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="93399-193">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="93399-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-194">Boolean</span></span>|<span data-ttu-id="93399-195">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="93399-195">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="93399-196">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="93399-196">dataRoamingBlocked</span></span>|<span data-ttu-id="93399-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-197">Boolean</span></span>|<span data-ttu-id="93399-198">Indica se um usuário será ou não bloqueado de roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="93399-198">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="93399-199">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="93399-199">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="93399-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-200">Boolean</span></span>|<span data-ttu-id="93399-201">Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="93399-201">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="93399-202">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="93399-202">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="93399-203">Coleção String</span><span class="sxs-lookup"><span data-stu-id="93399-203">String collection</span></span>|<span data-ttu-id="93399-204">Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.</span><span class="sxs-lookup"><span data-stu-id="93399-204">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="93399-205">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="93399-205">factoryResetBlocked</span></span>|<span data-ttu-id="93399-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-206">Boolean</span></span>|<span data-ttu-id="93399-207">Indica se a opção de redefinição de fábrica em configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="93399-207">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="93399-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="93399-208">kioskModeApps</span></span>|<span data-ttu-id="93399-209">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="93399-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="93399-210">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="93399-210">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="93399-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="93399-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="93399-212">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="93399-212">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="93399-213">String</span><span class="sxs-lookup"><span data-stu-id="93399-213">String</span></span>|<span data-ttu-id="93399-214">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="93399-214">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="93399-215">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="93399-215">kioskModeExitCode</span></span>|<span data-ttu-id="93399-216">String</span><span class="sxs-lookup"><span data-stu-id="93399-216">String</span></span>|<span data-ttu-id="93399-217">Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="93399-217">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="93399-218">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="93399-218">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="93399-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-219">Boolean</span></span>|<span data-ttu-id="93399-220">Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="93399-220">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="93399-221">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="93399-221">microphoneForceMute</span></span>|<span data-ttu-id="93399-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-222">Boolean</span></span>|<span data-ttu-id="93399-223">Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="93399-223">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="93399-224">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="93399-224">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="93399-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-225">Boolean</span></span>|<span data-ttu-id="93399-226">Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="93399-226">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="93399-227">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="93399-227">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="93399-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-228">Boolean</span></span>|<span data-ttu-id="93399-229">Indica se o feixe de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="93399-229">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="93399-230">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="93399-230">passwordBlockKeyguard</span></span>|<span data-ttu-id="93399-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-231">Boolean</span></span>|<span data-ttu-id="93399-232">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="93399-232">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="93399-233">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="93399-233">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="93399-234">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="93399-234">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="93399-235">Lista de recursos de keyguard de dispositivo para bloquear.</span><span class="sxs-lookup"><span data-stu-id="93399-235">List of device keyguard features to block.</span></span> <span data-ttu-id="93399-236">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="93399-236">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="93399-237">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="93399-237">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="93399-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="93399-238">passwordExpirationDays</span></span>|<span data-ttu-id="93399-239">Int32</span><span class="sxs-lookup"><span data-stu-id="93399-239">Int32</span></span>|<span data-ttu-id="93399-240">Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="93399-240">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="93399-241">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="93399-241">Valid values 1 to 365</span></span>|
|<span data-ttu-id="93399-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="93399-242">passwordMinimumLength</span></span>|<span data-ttu-id="93399-243">Int32</span><span class="sxs-lookup"><span data-stu-id="93399-243">Int32</span></span>|<span data-ttu-id="93399-244">Indica o comprimento mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93399-244">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="93399-245">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="93399-245">Valid values 4 to 16</span></span>|
|<span data-ttu-id="93399-246">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="93399-246">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="93399-247">Int32</span><span class="sxs-lookup"><span data-stu-id="93399-247">Int32</span></span>|<span data-ttu-id="93399-248">Milissegundos de inatividade antes da tela expirar.</span><span class="sxs-lookup"><span data-stu-id="93399-248">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="93399-249">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="93399-249">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="93399-250">Int32</span><span class="sxs-lookup"><span data-stu-id="93399-250">Int32</span></span>|<span data-ttu-id="93399-251">Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="93399-251">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="93399-252">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="93399-252">Valid values 0 to 24</span></span>|
|<span data-ttu-id="93399-253">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="93399-253">passwordRequiredType</span></span>|[<span data-ttu-id="93399-254">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="93399-254">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="93399-255">Indica a qualidade mínima da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93399-255">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="93399-256">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="93399-256">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="93399-257">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="93399-257">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="93399-258">Int32</span><span class="sxs-lookup"><span data-stu-id="93399-258">Int32</span></span>|<span data-ttu-id="93399-259">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="93399-259">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="93399-260">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="93399-260">Valid values 4 to 11</span></span>|
|<span data-ttu-id="93399-261">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="93399-261">safeBootBlocked</span></span>|<span data-ttu-id="93399-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-262">Boolean</span></span>|<span data-ttu-id="93399-263">Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="93399-263">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="93399-264">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="93399-264">screenCaptureBlocked</span></span>|<span data-ttu-id="93399-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-265">Boolean</span></span>|<span data-ttu-id="93399-266">Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="93399-266">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="93399-267">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="93399-267">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="93399-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-268">Boolean</span></span>|<span data-ttu-id="93399-269">Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93399-269">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="93399-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="93399-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="93399-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-271">Boolean</span></span>|<span data-ttu-id="93399-272">Indica se os aplicativos devem ou não ser verificados.</span><span class="sxs-lookup"><span data-stu-id="93399-272">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="93399-273">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="93399-273">statusBarBlocked</span></span>|<span data-ttu-id="93399-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-274">Boolean</span></span>|<span data-ttu-id="93399-275">Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="93399-275">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="93399-276">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="93399-276">stayOnModes</span></span>|<span data-ttu-id="93399-277">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="93399-277">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="93399-278">Lista de modos em que a exibição do dispositivo permanecerá ligada.</span><span class="sxs-lookup"><span data-stu-id="93399-278">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="93399-279">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="93399-279">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="93399-280">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="93399-280">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="93399-281">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="93399-281">storageAllowUsb</span></span>|<span data-ttu-id="93399-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-282">Boolean</span></span>|<span data-ttu-id="93399-283">Indica se o armazenamento em massa USB deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="93399-283">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="93399-284">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="93399-284">storageBlockExternalMedia</span></span>|<span data-ttu-id="93399-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-285">Boolean</span></span>|<span data-ttu-id="93399-286">Indica se a mídia externa deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="93399-286">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="93399-287">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="93399-287">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="93399-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-288">Boolean</span></span>|<span data-ttu-id="93399-289">Indica se a transferência de arquivos USB deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="93399-289">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="93399-290">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="93399-290">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="93399-291">Int32</span><span class="sxs-lookup"><span data-stu-id="93399-291">Int32</span></span>|<span data-ttu-id="93399-292">Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="93399-292">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="93399-293">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="93399-293">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="93399-294">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="93399-294">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="93399-295">Int32</span><span class="sxs-lookup"><span data-stu-id="93399-295">Int32</span></span>|<span data-ttu-id="93399-296">Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="93399-296">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="93399-297">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="93399-297">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="93399-298">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="93399-298">systemUpdateInstallType</span></span>|[<span data-ttu-id="93399-299">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="93399-299">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="93399-300">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="93399-300">The type of system update configuration.</span></span> <span data-ttu-id="93399-301">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="93399-301">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="93399-302">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="93399-302">systemWindowsBlocked</span></span>|<span data-ttu-id="93399-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-303">Boolean</span></span>|<span data-ttu-id="93399-304">Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.</span><span class="sxs-lookup"><span data-stu-id="93399-304">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="93399-305">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="93399-305">usersBlockAdd</span></span>|<span data-ttu-id="93399-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-306">Boolean</span></span>|<span data-ttu-id="93399-307">Indica se os usuários e perfis serão ou não desabilitados.</span><span class="sxs-lookup"><span data-stu-id="93399-307">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="93399-308">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="93399-308">usersBlockRemove</span></span>|<span data-ttu-id="93399-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-309">Boolean</span></span>|<span data-ttu-id="93399-310">Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.</span><span class="sxs-lookup"><span data-stu-id="93399-310">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="93399-311">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="93399-311">volumeBlockAdjustment</span></span>|<span data-ttu-id="93399-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-312">Boolean</span></span>|<span data-ttu-id="93399-313">Indica se o ajuste do volume mestre está ou não desabilitado.</span><span class="sxs-lookup"><span data-stu-id="93399-313">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="93399-314">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="93399-314">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="93399-315">String</span><span class="sxs-lookup"><span data-stu-id="93399-315">String</span></span>|<span data-ttu-id="93399-316">Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="93399-316">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="93399-317">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="93399-317">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="93399-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-318">Boolean</span></span>|<span data-ttu-id="93399-319">Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="93399-319">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="93399-320">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="93399-320">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="93399-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-321">Boolean</span></span>|<span data-ttu-id="93399-322">Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="93399-322">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="93399-323">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="93399-323">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="93399-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="93399-324">Boolean</span></span>|<span data-ttu-id="93399-325">Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="93399-325">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="93399-326">Resposta</span><span class="sxs-lookup"><span data-stu-id="93399-326">Response</span></span>
<span data-ttu-id="93399-327">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93399-327">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93399-328">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93399-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="93399-329">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93399-329">Request</span></span>
<span data-ttu-id="93399-330">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93399-330">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2517

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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

### <a name="response"></a><span data-ttu-id="93399-331">Resposta</span><span class="sxs-lookup"><span data-stu-id="93399-331">Response</span></span>
<span data-ttu-id="93399-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93399-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2689

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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




