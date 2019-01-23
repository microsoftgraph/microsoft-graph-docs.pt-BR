---
title: Criar androidDeviceOwnerGeneralDeviceConfiguration
description: Crie um novo objeto de androidDeviceOwnerGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93df53db7c19df9134370f9dbd703d99f631b688
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421218"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="acf9c-103">Criar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="acf9c-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="acf9c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="acf9c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="acf9c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="acf9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acf9c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="acf9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acf9c-107">Crie um novo objeto de [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="acf9c-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acf9c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="acf9c-108">Prerequisites</span></span>
<span data-ttu-id="acf9c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="acf9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="acf9c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acf9c-111">Permission type</span></span>|<span data-ttu-id="acf9c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="acf9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acf9c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acf9c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="acf9c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acf9c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="acf9c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acf9c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acf9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acf9c-116">Not supported.</span></span>|
|<span data-ttu-id="acf9c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acf9c-117">Application</span></span>|<span data-ttu-id="acf9c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acf9c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acf9c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acf9c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="acf9c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acf9c-120">Request headers</span></span>
|<span data-ttu-id="acf9c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="acf9c-121">Header</span></span>|<span data-ttu-id="acf9c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="acf9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acf9c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="acf9c-123">Authorization</span></span>|<span data-ttu-id="acf9c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acf9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acf9c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="acf9c-125">Accept</span></span>|<span data-ttu-id="acf9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="acf9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acf9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acf9c-127">Request body</span></span>
<span data-ttu-id="acf9c-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="acf9c-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="acf9c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="acf9c-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="acf9c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acf9c-130">Property</span></span>|<span data-ttu-id="acf9c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="acf9c-131">Type</span></span>|<span data-ttu-id="acf9c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="acf9c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acf9c-133">id</span><span class="sxs-lookup"><span data-stu-id="acf9c-133">id</span></span>|<span data-ttu-id="acf9c-134">String</span><span class="sxs-lookup"><span data-stu-id="acf9c-134">String</span></span>|<span data-ttu-id="acf9c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="acf9c-135">Key of the entity.</span></span> <span data-ttu-id="acf9c-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acf9c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acf9c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="acf9c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acf9c-138">DateTimeOffset</span></span>|<span data-ttu-id="acf9c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="acf9c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="acf9c-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acf9c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="acf9c-141">roleScopeTagIds</span></span>|<span data-ttu-id="acf9c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="acf9c-142">String collection</span></span>|<span data-ttu-id="acf9c-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="acf9c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="acf9c-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acf9c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="acf9c-145">supportsScopeTags</span></span>|<span data-ttu-id="acf9c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-146">Boolean</span></span>|<span data-ttu-id="acf9c-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="acf9c-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="acf9c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="acf9c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="acf9c-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acf9c-150">This property is read-only.</span></span> <span data-ttu-id="acf9c-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acf9c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acf9c-152">createdDateTime</span></span>|<span data-ttu-id="acf9c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acf9c-153">DateTimeOffset</span></span>|<span data-ttu-id="acf9c-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-154">DateTime the object was created.</span></span> <span data-ttu-id="acf9c-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acf9c-156">description</span><span class="sxs-lookup"><span data-stu-id="acf9c-156">description</span></span>|<span data-ttu-id="acf9c-157">String</span><span class="sxs-lookup"><span data-stu-id="acf9c-157">String</span></span>|<span data-ttu-id="acf9c-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="acf9c-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acf9c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="acf9c-160">displayName</span></span>|<span data-ttu-id="acf9c-161">String</span><span class="sxs-lookup"><span data-stu-id="acf9c-161">String</span></span>|<span data-ttu-id="acf9c-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="acf9c-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acf9c-164">version</span><span class="sxs-lookup"><span data-stu-id="acf9c-164">version</span></span>|<span data-ttu-id="acf9c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="acf9c-165">Int32</span></span>|<span data-ttu-id="acf9c-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-166">Version of the device configuration.</span></span> <span data-ttu-id="acf9c-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="acf9c-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="acf9c-168">accountsBlockModification</span></span>|<span data-ttu-id="acf9c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-169">Boolean</span></span>|<span data-ttu-id="acf9c-170">Indica se ou não adicionando ou removendo contas está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="acf9c-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="acf9c-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="acf9c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-172">Boolean</span></span>|<span data-ttu-id="acf9c-173">Indica se o usuário será permitido ou não para habilitar a configuração de fontes desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="acf9c-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="acf9c-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="acf9c-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="acf9c-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="acf9c-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="acf9c-176">Indica o valor da política de atualização automática de app.</span><span class="sxs-lookup"><span data-stu-id="acf9c-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="acf9c-177">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="acf9c-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="acf9c-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="acf9c-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="acf9c-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="acf9c-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="acf9c-180">Indica a política de permissão para as solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="acf9c-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="acf9c-181">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="acf9c-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="acf9c-182">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="acf9c-182">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="acf9c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-183">Boolean</span></span>|<span data-ttu-id="acf9c-184">Se deseja ou não recomendável todos os aplicativos pule as dicas de primeiro uso de tempo que podem ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-184">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="acf9c-185">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="acf9c-185">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="acf9c-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-186">Boolean</span></span>|<span data-ttu-id="acf9c-187">Indica se deve ou não bloquear um usuário configurando bluetooth.</span><span class="sxs-lookup"><span data-stu-id="acf9c-187">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="acf9c-188">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="acf9c-188">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="acf9c-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-189">Boolean</span></span>|<span data-ttu-id="acf9c-190">Indica se deve ou não bloquear um usuário compartilhando contatos via bluetooth.</span><span class="sxs-lookup"><span data-stu-id="acf9c-190">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="acf9c-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="acf9c-191">cameraBlocked</span></span>|<span data-ttu-id="acf9c-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-192">Boolean</span></span>|<span data-ttu-id="acf9c-193">Indica se ou não desabilitar o uso da câmera.</span><span class="sxs-lookup"><span data-stu-id="acf9c-193">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="acf9c-194">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="acf9c-194">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="acf9c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-195">Boolean</span></span>|<span data-ttu-id="acf9c-196">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-196">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="acf9c-197">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="acf9c-197">dataRoamingBlocked</span></span>|<span data-ttu-id="acf9c-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-198">Boolean</span></span>|<span data-ttu-id="acf9c-199">Indica se deve ou não bloquear um usuário a partir de dados de roaming.</span><span class="sxs-lookup"><span data-stu-id="acf9c-199">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="acf9c-200">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="acf9c-200">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="acf9c-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-201">Boolean</span></span>|<span data-ttu-id="acf9c-202">Indica se ou não impedir que o usuário altere manualmente a data ou hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="acf9c-202">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="acf9c-203">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="acf9c-203">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="acf9c-204">String collection</span><span class="sxs-lookup"><span data-stu-id="acf9c-204">String collection</span></span>|<span data-ttu-id="acf9c-205">Lista de emails de conta do Google que serão necessários para autenticar depois que um dispositivo é redefinida antes que ele pode ser configurado de fábrica.</span><span class="sxs-lookup"><span data-stu-id="acf9c-205">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="acf9c-206">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="acf9c-206">factoryResetBlocked</span></span>|<span data-ttu-id="acf9c-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-207">Boolean</span></span>|<span data-ttu-id="acf9c-208">Indica se ou não a opção de redefinição de fábrica nas configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="acf9c-208">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="acf9c-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="acf9c-209">kioskModeApps</span></span>|<span data-ttu-id="acf9c-210">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="acf9c-211">Uma lista de aplicativos gerenciados que será exibido quando o dispositivo estiver no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="acf9c-211">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="acf9c-212">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="acf9c-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="acf9c-213">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="acf9c-213">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="acf9c-214">String</span><span class="sxs-lookup"><span data-stu-id="acf9c-214">String</span></span>|<span data-ttu-id="acf9c-215">URL para uma imagem publicamente acessível a ser usado para a parede quando o dispositivo está no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="acf9c-215">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="acf9c-216">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="acf9c-216">kioskModeExitCode</span></span>|<span data-ttu-id="acf9c-217">String</span><span class="sxs-lookup"><span data-stu-id="acf9c-217">String</span></span>|<span data-ttu-id="acf9c-218">Saia do código para permitir que um usuário sai do modo de quiosque quando o dispositivo está no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="acf9c-218">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="acf9c-219">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="acf9c-219">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="acf9c-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-220">Boolean</span></span>|<span data-ttu-id="acf9c-221">Se deseja ou não exibir um botão de residencial virtual quando o dispositivo está no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="acf9c-221">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="acf9c-222">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="acf9c-222">microphoneForceMute</span></span>|<span data-ttu-id="acf9c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-223">Boolean</span></span>|<span data-ttu-id="acf9c-224">Indica se deve ou não bloquear o mudo do microfone no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-224">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="acf9c-225">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="acf9c-225">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="acf9c-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-226">Boolean</span></span>|<span data-ttu-id="acf9c-227">Indica se ou não o dispositivo permitirá a conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="acf9c-227">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="acf9c-228">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="acf9c-228">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="acf9c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-229">Boolean</span></span>|<span data-ttu-id="acf9c-230">Indica se deve ou não bloquear feixe de saída NFC.</span><span class="sxs-lookup"><span data-stu-id="acf9c-230">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="acf9c-231">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="acf9c-231">passwordBlockKeyguard</span></span>|<span data-ttu-id="acf9c-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-232">Boolean</span></span>|<span data-ttu-id="acf9c-233">Indica se ou não o keyguard está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-233">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="acf9c-234">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="acf9c-234">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="acf9c-235">coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="acf9c-236">Lista de recursos do dispositivo keyguard bloquear.</span><span class="sxs-lookup"><span data-stu-id="acf9c-236">List of device keyguard features to block.</span></span> <span data-ttu-id="acf9c-237">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="acf9c-237">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="acf9c-238">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="acf9c-238">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="acf9c-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="acf9c-239">passwordExpirationDays</span></span>|<span data-ttu-id="acf9c-240">Int32</span><span class="sxs-lookup"><span data-stu-id="acf9c-240">Int32</span></span>|<span data-ttu-id="acf9c-241">Indica a quantidade de tempo em segundos que uma senha pode ser definida para antes que ele expire e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="acf9c-241">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="acf9c-242">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="acf9c-242">Valid values 1 to 365</span></span>|
|<span data-ttu-id="acf9c-243">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="acf9c-243">passwordMinimumLength</span></span>|<span data-ttu-id="acf9c-244">Int32</span><span class="sxs-lookup"><span data-stu-id="acf9c-244">Int32</span></span>|<span data-ttu-id="acf9c-245">Indica o comprimento mínimo da senha necessário no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-245">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="acf9c-246">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="acf9c-246">Valid values 4 to 16</span></span>|
|<span data-ttu-id="acf9c-247">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="acf9c-247">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="acf9c-248">Int32</span><span class="sxs-lookup"><span data-stu-id="acf9c-248">Int32</span></span>|<span data-ttu-id="acf9c-249">Milissegundos de inatividade antes que os tempos de tela check-out.</span><span class="sxs-lookup"><span data-stu-id="acf9c-249">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="acf9c-250">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="acf9c-250">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="acf9c-251">Int32</span><span class="sxs-lookup"><span data-stu-id="acf9c-251">Int32</span></span>|<span data-ttu-id="acf9c-252">Indica o tamanho do histórico de senhas, onde o usuário não será capaz de inserir uma nova senha que é o mesmo que qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="acf9c-252">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="acf9c-253">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="acf9c-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="acf9c-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="acf9c-254">passwordRequiredType</span></span>|[<span data-ttu-id="acf9c-255">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="acf9c-255">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="acf9c-256">Indica a qualidade mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-256">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="acf9c-257">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="acf9c-257">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="acf9c-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="acf9c-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="acf9c-259">Int32</span><span class="sxs-lookup"><span data-stu-id="acf9c-259">Int32</span></span>|<span data-ttu-id="acf9c-260">Indica o número de vezes que um usuário pode digitar uma senha incorreta antes que o dispositivo é apagado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-260">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="acf9c-261">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="acf9c-261">Valid values 4 to 11</span></span>|
|<span data-ttu-id="acf9c-262">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="acf9c-262">safeBootBlocked</span></span>|<span data-ttu-id="acf9c-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-263">Boolean</span></span>|<span data-ttu-id="acf9c-264">Indica se ou não reinicializar que o dispositivo em inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-264">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="acf9c-265">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="acf9c-265">screenCaptureBlocked</span></span>|<span data-ttu-id="acf9c-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-266">Boolean</span></span>|<span data-ttu-id="acf9c-267">Indica se ou não desabilitar a capacidade de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="acf9c-267">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="acf9c-268">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="acf9c-268">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="acf9c-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-269">Boolean</span></span>|<span data-ttu-id="acf9c-270">Indica se deve ou não bloquear o usuário desde a habilitação de recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-270">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="acf9c-271">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="acf9c-271">securityRequireVerifyApps</span></span>|<span data-ttu-id="acf9c-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-272">Boolean</span></span>|<span data-ttu-id="acf9c-273">Indica se ou não verifique apps é necessário.</span><span class="sxs-lookup"><span data-stu-id="acf9c-273">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="acf9c-274">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="acf9c-274">statusBarBlocked</span></span>|<span data-ttu-id="acf9c-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-275">Boolean</span></span>|<span data-ttu-id="acf9c-276">Indica se o status ou barra estiver desabilitada, incluindo notificações, configurações rápidas e outras camadas da tela.</span><span class="sxs-lookup"><span data-stu-id="acf9c-276">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="acf9c-277">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="acf9c-277">stayOnModes</span></span>|<span data-ttu-id="acf9c-278">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="acf9c-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="acf9c-279">Lista de modos nos quais a exibição do dispositivo permanecerão ativadas.</span><span class="sxs-lookup"><span data-stu-id="acf9c-279">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="acf9c-280">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="acf9c-280">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="acf9c-281">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="acf9c-281">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="acf9c-282">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="acf9c-282">storageAllowUsb</span></span>|<span data-ttu-id="acf9c-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-283">Boolean</span></span>|<span data-ttu-id="acf9c-284">Indica se deve ou não permitir o armazenamento em massa USB.</span><span class="sxs-lookup"><span data-stu-id="acf9c-284">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="acf9c-285">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="acf9c-285">storageBlockExternalMedia</span></span>|<span data-ttu-id="acf9c-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-286">Boolean</span></span>|<span data-ttu-id="acf9c-287">Indica se o bloqueio da mídia externa ou não.</span><span class="sxs-lookup"><span data-stu-id="acf9c-287">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="acf9c-288">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="acf9c-288">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="acf9c-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-289">Boolean</span></span>|<span data-ttu-id="acf9c-290">Indica se o bloqueio da transferência de arquivos USB ou não.</span><span class="sxs-lookup"><span data-stu-id="acf9c-290">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="acf9c-291">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="acf9c-291">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="acf9c-292">Int32</span><span class="sxs-lookup"><span data-stu-id="acf9c-292">Int32</span></span>|<span data-ttu-id="acf9c-293">Indica o número de minutos após a meia-noite que inicia a janela de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="acf9c-293">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="acf9c-294">Valores válidos 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="acf9c-294">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="acf9c-295">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="acf9c-295">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="acf9c-296">Int32</span><span class="sxs-lookup"><span data-stu-id="acf9c-296">Int32</span></span>|<span data-ttu-id="acf9c-297">Indica o número de minutos após a meia-noite que termine a janela de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="acf9c-297">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="acf9c-298">Valores válidos 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="acf9c-298">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="acf9c-299">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="acf9c-299">systemUpdateInstallType</span></span>|[<span data-ttu-id="acf9c-300">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="acf9c-300">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="acf9c-301">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="acf9c-301">The type of system update configuration.</span></span> <span data-ttu-id="acf9c-302">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="acf9c-302">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="acf9c-303">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="acf9c-303">systemWindowsBlocked</span></span>|<span data-ttu-id="acf9c-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-304">Boolean</span></span>|<span data-ttu-id="acf9c-305">Se deseja ou não bloquear Android sistema Avisar windows, como brindes, atividades de telefone e alertas do sistema.</span><span class="sxs-lookup"><span data-stu-id="acf9c-305">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="acf9c-306">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="acf9c-306">usersBlockAdd</span></span>|<span data-ttu-id="acf9c-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-307">Boolean</span></span>|<span data-ttu-id="acf9c-308">Indica se ou não a adição de usuários e perfis está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-308">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="acf9c-309">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="acf9c-309">usersBlockRemove</span></span>|<span data-ttu-id="acf9c-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-310">Boolean</span></span>|<span data-ttu-id="acf9c-311">Indica se ou não desabilitar a remoção de outros usuários do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="acf9c-311">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="acf9c-312">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="acf9c-312">volumeBlockAdjustment</span></span>|<span data-ttu-id="acf9c-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-313">Boolean</span></span>|<span data-ttu-id="acf9c-314">Indica se ou não ajustar que o volume de mestre está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-314">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="acf9c-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="acf9c-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="acf9c-316">String</span><span class="sxs-lookup"><span data-stu-id="acf9c-316">String</span></span>|<span data-ttu-id="acf9c-317">Nome do pacote app Android para app que lidará com uma conexão VPN sempre ativa.</span><span class="sxs-lookup"><span data-stu-id="acf9c-317">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="acf9c-318">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="acf9c-318">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="acf9c-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-319">Boolean</span></span>|<span data-ttu-id="acf9c-320">Se o nome do pacote de uma VPN sempre diante for especificado, ou não ao tráfego de rede de bloqueio quando esse VPN é desconectado.</span><span class="sxs-lookup"><span data-stu-id="acf9c-320">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="acf9c-321">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="acf9c-321">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="acf9c-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-322">Boolean</span></span>|<span data-ttu-id="acf9c-323">Indica se deve ou não bloquear as configurações de conexão wifi de edição do usuário.</span><span class="sxs-lookup"><span data-stu-id="acf9c-323">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="acf9c-324">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="acf9c-324">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="acf9c-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf9c-325">Boolean</span></span>|<span data-ttu-id="acf9c-326">Indica se deve ou não bloquear edição apenas as redes definidas pela política do usuário.</span><span class="sxs-lookup"><span data-stu-id="acf9c-326">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="acf9c-327">Resposta</span><span class="sxs-lookup"><span data-stu-id="acf9c-327">Response</span></span>
<span data-ttu-id="acf9c-328">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acf9c-328">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acf9c-329">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acf9c-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="acf9c-330">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acf9c-330">Request</span></span>
<span data-ttu-id="acf9c-331">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="acf9c-331">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="acf9c-332">Resposta</span><span class="sxs-lookup"><span data-stu-id="acf9c-332">Response</span></span>
<span data-ttu-id="acf9c-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="acf9c-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




