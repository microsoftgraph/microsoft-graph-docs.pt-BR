---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualize as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2166acb42eeb5690486cd40f510416ce5a9a224
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395556"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="7b428-103">Atualizar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b428-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="7b428-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7b428-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b428-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7b428-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b428-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7b428-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b428-107">Atualize as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7b428-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b428-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b428-108">Prerequisites</span></span>
<span data-ttu-id="7b428-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b428-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7b428-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b428-111">Permission type</span></span>|<span data-ttu-id="7b428-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7b428-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b428-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b428-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b428-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b428-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b428-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b428-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b428-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b428-116">Not supported.</span></span>|
|<span data-ttu-id="7b428-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b428-117">Application</span></span>|<span data-ttu-id="7b428-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b428-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b428-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b428-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7b428-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b428-120">Request headers</span></span>
|<span data-ttu-id="7b428-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b428-121">Header</span></span>|<span data-ttu-id="7b428-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7b428-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b428-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b428-123">Authorization</span></span>|<span data-ttu-id="7b428-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b428-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b428-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7b428-125">Accept</span></span>|<span data-ttu-id="7b428-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b428-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b428-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b428-127">Request body</span></span>
<span data-ttu-id="7b428-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7b428-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="7b428-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b428-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="7b428-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b428-130">Property</span></span>|<span data-ttu-id="7b428-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b428-131">Type</span></span>|<span data-ttu-id="7b428-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b428-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b428-133">id</span><span class="sxs-lookup"><span data-stu-id="7b428-133">id</span></span>|<span data-ttu-id="7b428-134">String</span><span class="sxs-lookup"><span data-stu-id="7b428-134">String</span></span>|<span data-ttu-id="7b428-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7b428-135">Key of the entity.</span></span> <span data-ttu-id="7b428-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b428-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b428-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7b428-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b428-138">DateTimeOffset</span></span>|<span data-ttu-id="7b428-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7b428-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7b428-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b428-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b428-141">roleScopeTagIds</span></span>|<span data-ttu-id="7b428-142">String collection</span><span class="sxs-lookup"><span data-stu-id="7b428-142">String collection</span></span>|<span data-ttu-id="7b428-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="7b428-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7b428-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b428-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7b428-145">supportsScopeTags</span></span>|<span data-ttu-id="7b428-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-146">Boolean</span></span>|<span data-ttu-id="7b428-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7b428-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7b428-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7b428-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7b428-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="7b428-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7b428-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b428-150">This property is read-only.</span></span> <span data-ttu-id="7b428-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b428-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b428-152">createdDateTime</span></span>|<span data-ttu-id="7b428-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b428-153">DateTimeOffset</span></span>|<span data-ttu-id="7b428-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7b428-154">DateTime the object was created.</span></span> <span data-ttu-id="7b428-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b428-156">description</span><span class="sxs-lookup"><span data-stu-id="7b428-156">description</span></span>|<span data-ttu-id="7b428-157">String</span><span class="sxs-lookup"><span data-stu-id="7b428-157">String</span></span>|<span data-ttu-id="7b428-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b428-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b428-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b428-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7b428-160">displayName</span></span>|<span data-ttu-id="7b428-161">String</span><span class="sxs-lookup"><span data-stu-id="7b428-161">String</span></span>|<span data-ttu-id="7b428-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b428-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b428-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b428-164">version</span><span class="sxs-lookup"><span data-stu-id="7b428-164">version</span></span>|<span data-ttu-id="7b428-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7b428-165">Int32</span></span>|<span data-ttu-id="7b428-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b428-166">Version of the device configuration.</span></span> <span data-ttu-id="7b428-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b428-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="7b428-168">accountsBlockModification</span></span>|<span data-ttu-id="7b428-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-169">Boolean</span></span>|<span data-ttu-id="7b428-170">Indica se ou não adicionando ou removendo contas está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="7b428-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="7b428-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="7b428-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="7b428-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-172">Boolean</span></span>|<span data-ttu-id="7b428-173">Indica se o usuário será permitido ou não para habilitar a configuração de fontes desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="7b428-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="7b428-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="7b428-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="7b428-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="7b428-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="7b428-176">Indica o valor da política de atualização automática de app.</span><span class="sxs-lookup"><span data-stu-id="7b428-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="7b428-177">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="7b428-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="7b428-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="7b428-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="7b428-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="7b428-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="7b428-180">Indica a política de permissão para as solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="7b428-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="7b428-181">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="7b428-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="7b428-182">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="7b428-182">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="7b428-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-183">Boolean</span></span>|<span data-ttu-id="7b428-184">Se deseja ou não recomendável todos os aplicativos pule as dicas de primeiro uso de tempo que podem ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="7b428-184">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="7b428-185">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b428-185">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="7b428-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-186">Boolean</span></span>|<span data-ttu-id="7b428-187">Indica se deve ou não bloquear um usuário configurando bluetooth.</span><span class="sxs-lookup"><span data-stu-id="7b428-187">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="7b428-188">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="7b428-188">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="7b428-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-189">Boolean</span></span>|<span data-ttu-id="7b428-190">Indica se deve ou não bloquear um usuário compartilhando contatos via bluetooth.</span><span class="sxs-lookup"><span data-stu-id="7b428-190">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="7b428-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="7b428-191">cameraBlocked</span></span>|<span data-ttu-id="7b428-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-192">Boolean</span></span>|<span data-ttu-id="7b428-193">Indica se ou não desabilitar o uso da câmera.</span><span class="sxs-lookup"><span data-stu-id="7b428-193">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="7b428-194">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="7b428-194">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="7b428-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-195">Boolean</span></span>|<span data-ttu-id="7b428-196">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7b428-196">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="7b428-197">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="7b428-197">dataRoamingBlocked</span></span>|<span data-ttu-id="7b428-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-198">Boolean</span></span>|<span data-ttu-id="7b428-199">Indica se deve ou não bloquear um usuário a partir de dados de roaming.</span><span class="sxs-lookup"><span data-stu-id="7b428-199">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="7b428-200">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="7b428-200">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="7b428-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-201">Boolean</span></span>|<span data-ttu-id="7b428-202">Indica se ou não impedir que o usuário altere manualmente a data ou hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="7b428-202">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="7b428-203">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="7b428-203">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="7b428-204">String collection</span><span class="sxs-lookup"><span data-stu-id="7b428-204">String collection</span></span>|<span data-ttu-id="7b428-205">Lista de emails de conta do Google que serão necessários para autenticar depois que um dispositivo é redefinida antes que ele pode ser configurado de fábrica.</span><span class="sxs-lookup"><span data-stu-id="7b428-205">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="7b428-206">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="7b428-206">factoryResetBlocked</span></span>|<span data-ttu-id="7b428-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-207">Boolean</span></span>|<span data-ttu-id="7b428-208">Indica se ou não a opção de redefinição de fábrica nas configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="7b428-208">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="7b428-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="7b428-209">kioskModeApps</span></span>|<span data-ttu-id="7b428-210">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7b428-211">Uma lista de aplicativos gerenciados que será exibido quando o dispositivo estiver no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7b428-211">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="7b428-212">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7b428-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7b428-213">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="7b428-213">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="7b428-214">String</span><span class="sxs-lookup"><span data-stu-id="7b428-214">String</span></span>|<span data-ttu-id="7b428-215">URL para uma imagem publicamente acessível a ser usado para a parede quando o dispositivo está no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7b428-215">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="7b428-216">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="7b428-216">kioskModeExitCode</span></span>|<span data-ttu-id="7b428-217">String</span><span class="sxs-lookup"><span data-stu-id="7b428-217">String</span></span>|<span data-ttu-id="7b428-218">Saia do código para permitir que um usuário sai do modo de quiosque quando o dispositivo está no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7b428-218">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="7b428-219">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="7b428-219">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="7b428-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-220">Boolean</span></span>|<span data-ttu-id="7b428-221">Se deseja ou não exibir um botão de residencial virtual quando o dispositivo está no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7b428-221">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="7b428-222">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="7b428-222">microphoneForceMute</span></span>|<span data-ttu-id="7b428-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-223">Boolean</span></span>|<span data-ttu-id="7b428-224">Indica se deve ou não bloquear o mudo do microfone no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b428-224">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="7b428-225">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="7b428-225">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="7b428-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-226">Boolean</span></span>|<span data-ttu-id="7b428-227">Indica se ou não o dispositivo permitirá a conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="7b428-227">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="7b428-228">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="7b428-228">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="7b428-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-229">Boolean</span></span>|<span data-ttu-id="7b428-230">Indica se deve ou não bloquear feixe de saída NFC.</span><span class="sxs-lookup"><span data-stu-id="7b428-230">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="7b428-231">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="7b428-231">passwordBlockKeyguard</span></span>|<span data-ttu-id="7b428-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-232">Boolean</span></span>|<span data-ttu-id="7b428-233">Indica se ou não o keyguard está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="7b428-233">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="7b428-234">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="7b428-234">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="7b428-235">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="7b428-236">Lista de recursos do dispositivo keyguard bloquear.</span><span class="sxs-lookup"><span data-stu-id="7b428-236">List of device keyguard features to block.</span></span> <span data-ttu-id="7b428-237">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="7b428-237">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="7b428-238">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="7b428-238">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="7b428-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7b428-239">passwordExpirationDays</span></span>|<span data-ttu-id="7b428-240">Int32</span><span class="sxs-lookup"><span data-stu-id="7b428-240">Int32</span></span>|<span data-ttu-id="7b428-241">Indica a quantidade de tempo em segundos que uma senha pode ser definida para antes que ele expire e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="7b428-241">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="7b428-242">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="7b428-242">Valid values 1 to 365</span></span>|
|<span data-ttu-id="7b428-243">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7b428-243">passwordMinimumLength</span></span>|<span data-ttu-id="7b428-244">Int32</span><span class="sxs-lookup"><span data-stu-id="7b428-244">Int32</span></span>|<span data-ttu-id="7b428-245">Indica o comprimento mínimo da senha necessário no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b428-245">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="7b428-246">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="7b428-246">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7b428-247">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7b428-247">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7b428-248">Int32</span><span class="sxs-lookup"><span data-stu-id="7b428-248">Int32</span></span>|<span data-ttu-id="7b428-249">Milissegundos de inatividade antes que os tempos de tela check-out.</span><span class="sxs-lookup"><span data-stu-id="7b428-249">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7b428-250">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="7b428-250">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="7b428-251">Int32</span><span class="sxs-lookup"><span data-stu-id="7b428-251">Int32</span></span>|<span data-ttu-id="7b428-252">Indica o tamanho do histórico de senhas, onde o usuário não será capaz de inserir uma nova senha que é o mesmo que qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="7b428-252">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="7b428-253">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="7b428-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7b428-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7b428-254">passwordRequiredType</span></span>|[<span data-ttu-id="7b428-255">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7b428-255">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="7b428-256">Indica a qualidade mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b428-256">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="7b428-257">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="7b428-257">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="7b428-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7b428-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7b428-259">Int32</span><span class="sxs-lookup"><span data-stu-id="7b428-259">Int32</span></span>|<span data-ttu-id="7b428-260">Indica o número de vezes que um usuário pode digitar uma senha incorreta antes que o dispositivo é apagado.</span><span class="sxs-lookup"><span data-stu-id="7b428-260">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="7b428-261">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="7b428-261">Valid values 4 to 11</span></span>|
|<span data-ttu-id="7b428-262">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="7b428-262">safeBootBlocked</span></span>|<span data-ttu-id="7b428-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-263">Boolean</span></span>|<span data-ttu-id="7b428-264">Indica se ou não reinicializar que o dispositivo em inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="7b428-264">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="7b428-265">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7b428-265">screenCaptureBlocked</span></span>|<span data-ttu-id="7b428-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-266">Boolean</span></span>|<span data-ttu-id="7b428-267">Indica se ou não desabilitar a capacidade de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="7b428-267">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="7b428-268">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="7b428-268">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="7b428-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-269">Boolean</span></span>|<span data-ttu-id="7b428-270">Indica se deve ou não bloquear o usuário desde a habilitação de recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b428-270">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="7b428-271">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="7b428-271">securityRequireVerifyApps</span></span>|<span data-ttu-id="7b428-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-272">Boolean</span></span>|<span data-ttu-id="7b428-273">Indica se ou não verifique apps é necessário.</span><span class="sxs-lookup"><span data-stu-id="7b428-273">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="7b428-274">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="7b428-274">statusBarBlocked</span></span>|<span data-ttu-id="7b428-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-275">Boolean</span></span>|<span data-ttu-id="7b428-276">Indica se o status ou barra estiver desabilitada, incluindo notificações, configurações rápidas e outras camadas da tela.</span><span class="sxs-lookup"><span data-stu-id="7b428-276">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="7b428-277">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="7b428-277">stayOnModes</span></span>|<span data-ttu-id="7b428-278">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="7b428-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="7b428-279">Lista de modos nos quais a exibição do dispositivo permanecerão ativadas.</span><span class="sxs-lookup"><span data-stu-id="7b428-279">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="7b428-280">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="7b428-280">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="7b428-281">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="7b428-281">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="7b428-282">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="7b428-282">storageAllowUsb</span></span>|<span data-ttu-id="7b428-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-283">Boolean</span></span>|<span data-ttu-id="7b428-284">Indica se deve ou não permitir o armazenamento em massa USB.</span><span class="sxs-lookup"><span data-stu-id="7b428-284">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="7b428-285">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="7b428-285">storageBlockExternalMedia</span></span>|<span data-ttu-id="7b428-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-286">Boolean</span></span>|<span data-ttu-id="7b428-287">Indica se o bloqueio da mídia externa ou não.</span><span class="sxs-lookup"><span data-stu-id="7b428-287">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="7b428-288">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="7b428-288">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="7b428-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-289">Boolean</span></span>|<span data-ttu-id="7b428-290">Indica se o bloqueio da transferência de arquivos USB ou não.</span><span class="sxs-lookup"><span data-stu-id="7b428-290">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="7b428-291">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="7b428-291">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="7b428-292">Int32</span><span class="sxs-lookup"><span data-stu-id="7b428-292">Int32</span></span>|<span data-ttu-id="7b428-293">Indica o número de minutos após a meia-noite que inicia a janela de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="7b428-293">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="7b428-294">Valores válidos 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="7b428-294">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="7b428-295">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="7b428-295">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="7b428-296">Int32</span><span class="sxs-lookup"><span data-stu-id="7b428-296">Int32</span></span>|<span data-ttu-id="7b428-297">Indica o número de minutos após a meia-noite que termine a janela de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="7b428-297">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="7b428-298">Valores válidos 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="7b428-298">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="7b428-299">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="7b428-299">systemUpdateInstallType</span></span>|[<span data-ttu-id="7b428-300">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="7b428-300">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="7b428-301">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="7b428-301">The type of system update configuration.</span></span> <span data-ttu-id="7b428-302">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="7b428-302">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="7b428-303">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="7b428-303">systemWindowsBlocked</span></span>|<span data-ttu-id="7b428-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-304">Boolean</span></span>|<span data-ttu-id="7b428-305">Se deseja ou não bloquear Android sistema Avisar windows, como brindes, atividades de telefone e alertas do sistema.</span><span class="sxs-lookup"><span data-stu-id="7b428-305">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="7b428-306">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="7b428-306">usersBlockAdd</span></span>|<span data-ttu-id="7b428-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-307">Boolean</span></span>|<span data-ttu-id="7b428-308">Indica se ou não a adição de usuários e perfis está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="7b428-308">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="7b428-309">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="7b428-309">usersBlockRemove</span></span>|<span data-ttu-id="7b428-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-310">Boolean</span></span>|<span data-ttu-id="7b428-311">Indica se ou não desabilitar a remoção de outros usuários do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b428-311">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="7b428-312">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="7b428-312">volumeBlockAdjustment</span></span>|<span data-ttu-id="7b428-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-313">Boolean</span></span>|<span data-ttu-id="7b428-314">Indica se ou não ajustar que o volume de mestre está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="7b428-314">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="7b428-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b428-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="7b428-316">String</span><span class="sxs-lookup"><span data-stu-id="7b428-316">String</span></span>|<span data-ttu-id="7b428-317">Nome do pacote app Android para app que lidará com uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="7b428-317">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="7b428-318">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="7b428-318">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="7b428-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-319">Boolean</span></span>|<span data-ttu-id="7b428-320">Se o nome do pacote de uma VPN sempre diante for especificado, ou não ao tráfego de rede de bloqueio quando esse VPN é desconectado.</span><span class="sxs-lookup"><span data-stu-id="7b428-320">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="7b428-321">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="7b428-321">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="7b428-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-322">Boolean</span></span>|<span data-ttu-id="7b428-323">Indica se deve ou não bloquear as configurações de conexão wifi de edição do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b428-323">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="7b428-324">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="7b428-324">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="7b428-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b428-325">Boolean</span></span>|<span data-ttu-id="7b428-326">Indica se deve ou não bloquear edição apenas as redes definidas pela política do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b428-326">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="7b428-327">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b428-327">Response</span></span>
<span data-ttu-id="7b428-328">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b428-328">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b428-329">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b428-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b428-330">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b428-330">Request</span></span>
<span data-ttu-id="7b428-331">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b428-331">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b428-332">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b428-332">Response</span></span>
<span data-ttu-id="7b428-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b428-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




