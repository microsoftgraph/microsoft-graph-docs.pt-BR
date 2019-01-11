---
title: Criar androidDeviceOwnerGeneralDeviceConfiguration
description: Crie um novo objeto de androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a7802762fc88e45a434614a8101f4690f8c4bc1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812685"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="2536a-103">Criar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2536a-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="2536a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2536a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2536a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2536a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2536a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2536a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2536a-107">Crie um novo objeto de [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2536a-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2536a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2536a-108">Prerequisites</span></span>
<span data-ttu-id="2536a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2536a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2536a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2536a-111">Permission type</span></span>|<span data-ttu-id="2536a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2536a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2536a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2536a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2536a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2536a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2536a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2536a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2536a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2536a-116">Not supported.</span></span>|
|<span data-ttu-id="2536a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2536a-117">Application</span></span>|<span data-ttu-id="2536a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2536a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2536a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2536a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2536a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2536a-120">Request headers</span></span>
|<span data-ttu-id="2536a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2536a-121">Header</span></span>|<span data-ttu-id="2536a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2536a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2536a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2536a-123">Authorization</span></span>|<span data-ttu-id="2536a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2536a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2536a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2536a-125">Accept</span></span>|<span data-ttu-id="2536a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2536a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2536a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2536a-127">Request body</span></span>
<span data-ttu-id="2536a-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2536a-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="2536a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2536a-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="2536a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2536a-130">Property</span></span>|<span data-ttu-id="2536a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2536a-131">Type</span></span>|<span data-ttu-id="2536a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2536a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2536a-133">id</span><span class="sxs-lookup"><span data-stu-id="2536a-133">id</span></span>|<span data-ttu-id="2536a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2536a-134">String</span></span>|<span data-ttu-id="2536a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2536a-135">Key of the entity.</span></span> <span data-ttu-id="2536a-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2536a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2536a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2536a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2536a-138">DateTimeOffset</span></span>|<span data-ttu-id="2536a-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2536a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2536a-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2536a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2536a-141">roleScopeTagIds</span></span>|<span data-ttu-id="2536a-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2536a-142">String collection</span></span>|<span data-ttu-id="2536a-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="2536a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2536a-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2536a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2536a-145">supportsScopeTags</span></span>|<span data-ttu-id="2536a-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-146">Boolean</span></span>|<span data-ttu-id="2536a-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2536a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2536a-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2536a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2536a-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="2536a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2536a-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2536a-150">This property is read-only.</span></span> <span data-ttu-id="2536a-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2536a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2536a-152">createdDateTime</span></span>|<span data-ttu-id="2536a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2536a-153">DateTimeOffset</span></span>|<span data-ttu-id="2536a-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2536a-154">DateTime the object was created.</span></span> <span data-ttu-id="2536a-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2536a-156">description</span><span class="sxs-lookup"><span data-stu-id="2536a-156">description</span></span>|<span data-ttu-id="2536a-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2536a-157">String</span></span>|<span data-ttu-id="2536a-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2536a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2536a-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2536a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2536a-160">displayName</span></span>|<span data-ttu-id="2536a-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2536a-161">String</span></span>|<span data-ttu-id="2536a-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2536a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2536a-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2536a-164">version</span><span class="sxs-lookup"><span data-stu-id="2536a-164">version</span></span>|<span data-ttu-id="2536a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2536a-165">Int32</span></span>|<span data-ttu-id="2536a-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2536a-166">Version of the device configuration.</span></span> <span data-ttu-id="2536a-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2536a-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="2536a-168">accountsBlockModification</span></span>|<span data-ttu-id="2536a-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-169">Boolean</span></span>|<span data-ttu-id="2536a-170">Indica se ou não adicionando ou removendo contas está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2536a-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="2536a-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="2536a-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="2536a-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-172">Boolean</span></span>|<span data-ttu-id="2536a-173">Indica se o usuário será permitido ou não para habilitar a configuração de fontes desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="2536a-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="2536a-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="2536a-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="2536a-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="2536a-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="2536a-176">Indica o valor da política de atualização automática de app.</span><span class="sxs-lookup"><span data-stu-id="2536a-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="2536a-177">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="2536a-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="2536a-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="2536a-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="2536a-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2536a-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="2536a-180">Indica a política de permissão para as solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente.</span><span class="sxs-lookup"><span data-stu-id="2536a-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="2536a-181">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="2536a-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="2536a-182">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="2536a-182">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="2536a-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-183">Boolean</span></span>|<span data-ttu-id="2536a-184">Indica se deve ou não bloquear um usuário configurando bluetooth.</span><span class="sxs-lookup"><span data-stu-id="2536a-184">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="2536a-185">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="2536a-185">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="2536a-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-186">Boolean</span></span>|<span data-ttu-id="2536a-187">Indica se deve ou não bloquear um usuário compartilhando contatos via bluetooth.</span><span class="sxs-lookup"><span data-stu-id="2536a-187">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="2536a-188">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="2536a-188">cameraBlocked</span></span>|<span data-ttu-id="2536a-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-189">Boolean</span></span>|<span data-ttu-id="2536a-190">Indica se ou não desabilitar o uso da câmera.</span><span class="sxs-lookup"><span data-stu-id="2536a-190">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="2536a-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="2536a-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="2536a-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-192">Boolean</span></span>|<span data-ttu-id="2536a-193">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2536a-193">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="2536a-194">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="2536a-194">dataRoamingBlocked</span></span>|<span data-ttu-id="2536a-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-195">Boolean</span></span>|<span data-ttu-id="2536a-196">Indica se deve ou não bloquear um usuário a partir de dados de roaming.</span><span class="sxs-lookup"><span data-stu-id="2536a-196">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="2536a-197">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="2536a-197">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="2536a-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-198">Boolean</span></span>|<span data-ttu-id="2536a-199">Indica se ou não impedir que o usuário altere manualmente a data ou hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="2536a-199">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="2536a-200">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="2536a-200">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="2536a-201">String collection</span><span class="sxs-lookup"><span data-stu-id="2536a-201">String collection</span></span>|<span data-ttu-id="2536a-202">Lista de emails de conta do Google que serão necessários para autenticar depois que um dispositivo é redefinida antes que ele pode ser configurado de fábrica.</span><span class="sxs-lookup"><span data-stu-id="2536a-202">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="2536a-203">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="2536a-203">factoryResetBlocked</span></span>|<span data-ttu-id="2536a-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-204">Boolean</span></span>|<span data-ttu-id="2536a-205">Indica se ou não a opção de redefinição de fábrica nas configurações está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="2536a-205">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="2536a-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="2536a-206">kioskModeApps</span></span>|<span data-ttu-id="2536a-207">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2536a-208">Uma lista de aplicativos gerenciados que será exibido quando o dispositivo estiver no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="2536a-208">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="2536a-209">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2536a-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2536a-210">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="2536a-210">microphoneForceMute</span></span>|<span data-ttu-id="2536a-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-211">Boolean</span></span>|<span data-ttu-id="2536a-212">Indica se deve ou não bloquear o mudo do microfone no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2536a-212">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="2536a-213">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="2536a-213">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="2536a-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-214">Boolean</span></span>|<span data-ttu-id="2536a-215">Indica se ou não o dispositivo permitirá a conexão com uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="2536a-215">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="2536a-216">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="2536a-216">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="2536a-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-217">Boolean</span></span>|<span data-ttu-id="2536a-218">Indica se deve ou não bloquear feixe de saída NFC.</span><span class="sxs-lookup"><span data-stu-id="2536a-218">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="2536a-219">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="2536a-219">passwordBlockKeyguard</span></span>|<span data-ttu-id="2536a-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-220">Boolean</span></span>|<span data-ttu-id="2536a-221">Indica se ou não o keyguard está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2536a-221">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="2536a-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2536a-222">passwordExpirationDays</span></span>|<span data-ttu-id="2536a-223">Int32</span><span class="sxs-lookup"><span data-stu-id="2536a-223">Int32</span></span>|<span data-ttu-id="2536a-224">Indica a quantidade de tempo em segundos que uma senha pode ser definida para antes que ele expire e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="2536a-224">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="2536a-225">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="2536a-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2536a-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2536a-226">passwordMinimumLength</span></span>|<span data-ttu-id="2536a-227">Int32</span><span class="sxs-lookup"><span data-stu-id="2536a-227">Int32</span></span>|<span data-ttu-id="2536a-228">Indica o comprimento mínimo da senha necessário no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2536a-228">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="2536a-229">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="2536a-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2536a-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2536a-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2536a-231">Int32</span><span class="sxs-lookup"><span data-stu-id="2536a-231">Int32</span></span>|<span data-ttu-id="2536a-232">Milissegundos de inatividade antes que os tempos de tela check-out.</span><span class="sxs-lookup"><span data-stu-id="2536a-232">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2536a-233">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="2536a-233">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="2536a-234">Int32</span><span class="sxs-lookup"><span data-stu-id="2536a-234">Int32</span></span>|<span data-ttu-id="2536a-235">Indica o tamanho do histórico de senhas, onde o usuário não será capaz de inserir uma nova senha que é o mesmo que qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="2536a-235">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="2536a-236">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="2536a-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2536a-237">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2536a-237">passwordRequiredType</span></span>|[<span data-ttu-id="2536a-238">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2536a-238">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="2536a-239">Indica a qualidade mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2536a-239">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="2536a-240">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2536a-240">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2536a-241">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2536a-241">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2536a-242">Int32</span><span class="sxs-lookup"><span data-stu-id="2536a-242">Int32</span></span>|<span data-ttu-id="2536a-243">Indica o número de vezes que um usuário pode digitar uma senha incorreta antes que o dispositivo é apagado.</span><span class="sxs-lookup"><span data-stu-id="2536a-243">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="2536a-244">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="2536a-244">Valid values 4 to 11</span></span>|
|<span data-ttu-id="2536a-245">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="2536a-245">safeBootBlocked</span></span>|<span data-ttu-id="2536a-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-246">Boolean</span></span>|<span data-ttu-id="2536a-247">Indica se ou não reinicializar que o dispositivo em inicialização segura está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2536a-247">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="2536a-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="2536a-248">screenCaptureBlocked</span></span>|<span data-ttu-id="2536a-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-249">Boolean</span></span>|<span data-ttu-id="2536a-250">Indica se ou não desabilitar a capacidade de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="2536a-250">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="2536a-251">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="2536a-251">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="2536a-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-252">Boolean</span></span>|<span data-ttu-id="2536a-253">Indica se deve ou não bloquear o usuário desde a habilitação de recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2536a-253">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="2536a-254">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="2536a-254">securityRequireVerifyApps</span></span>|<span data-ttu-id="2536a-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-255">Boolean</span></span>|<span data-ttu-id="2536a-256">Indica se ou não verifique apps é necessário.</span><span class="sxs-lookup"><span data-stu-id="2536a-256">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="2536a-257">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="2536a-257">statusBarBlocked</span></span>|<span data-ttu-id="2536a-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-258">Boolean</span></span>|<span data-ttu-id="2536a-259">Indica se o status ou barra estiver desabilitada, incluindo notificações, configurações rápidas e outras camadas da tela.</span><span class="sxs-lookup"><span data-stu-id="2536a-259">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="2536a-260">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="2536a-260">stayOnModes</span></span>|<span data-ttu-id="2536a-261">coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="2536a-261">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="2536a-262">Lista de modos nos quais a exibição do dispositivo permanecerão ativadas.</span><span class="sxs-lookup"><span data-stu-id="2536a-262">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="2536a-263">Essa coleção pode conter um máximo de 4 elementos.</span><span class="sxs-lookup"><span data-stu-id="2536a-263">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="2536a-264">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="2536a-264">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="2536a-265">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="2536a-265">storageAllowUsb</span></span>|<span data-ttu-id="2536a-266">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-266">Boolean</span></span>|<span data-ttu-id="2536a-267">Indica se deve ou não permitir o armazenamento em massa USB.</span><span class="sxs-lookup"><span data-stu-id="2536a-267">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="2536a-268">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="2536a-268">storageBlockExternalMedia</span></span>|<span data-ttu-id="2536a-269">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-269">Boolean</span></span>|<span data-ttu-id="2536a-270">Indica se o bloqueio da mídia externa ou não.</span><span class="sxs-lookup"><span data-stu-id="2536a-270">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="2536a-271">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="2536a-271">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="2536a-272">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-272">Boolean</span></span>|<span data-ttu-id="2536a-273">Indica se o bloqueio da transferência de arquivos USB ou não.</span><span class="sxs-lookup"><span data-stu-id="2536a-273">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="2536a-274">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="2536a-274">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="2536a-275">Int32</span><span class="sxs-lookup"><span data-stu-id="2536a-275">Int32</span></span>|<span data-ttu-id="2536a-276">Indica o número de minutos após a meia-noite que inicia a janela de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="2536a-276">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="2536a-277">Valores válidos 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="2536a-277">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="2536a-278">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="2536a-278">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="2536a-279">Int32</span><span class="sxs-lookup"><span data-stu-id="2536a-279">Int32</span></span>|<span data-ttu-id="2536a-280">Indica o número de minutos após a meia-noite que termine a janela de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="2536a-280">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="2536a-281">Valores válidos 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="2536a-281">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="2536a-282">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="2536a-282">systemUpdateInstallType</span></span>|[<span data-ttu-id="2536a-283">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="2536a-283">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="2536a-284">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="2536a-284">The type of system update configuration.</span></span> <span data-ttu-id="2536a-285">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="2536a-285">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="2536a-286">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="2536a-286">usersBlockAdd</span></span>|<span data-ttu-id="2536a-287">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-287">Boolean</span></span>|<span data-ttu-id="2536a-288">Indica se ou não a adição de usuários e perfis está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2536a-288">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="2536a-289">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="2536a-289">usersBlockRemove</span></span>|<span data-ttu-id="2536a-290">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-290">Boolean</span></span>|<span data-ttu-id="2536a-291">Indica se ou não desabilitar a remoção de outros usuários do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2536a-291">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="2536a-292">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="2536a-292">volumeBlockAdjustment</span></span>|<span data-ttu-id="2536a-293">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-293">Boolean</span></span>|<span data-ttu-id="2536a-294">Indica se ou não ajustar que o volume de mestre está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2536a-294">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="2536a-295">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="2536a-295">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="2536a-296">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-296">Boolean</span></span>|<span data-ttu-id="2536a-297">Indica se deve ou não bloquear as configurações de conexão wifi de edição do usuário.</span><span class="sxs-lookup"><span data-stu-id="2536a-297">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="2536a-298">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="2536a-298">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="2536a-299">Booliano</span><span class="sxs-lookup"><span data-stu-id="2536a-299">Boolean</span></span>|<span data-ttu-id="2536a-300">Indica se deve ou não bloquear edição apenas as redes definidas pela política do usuário.</span><span class="sxs-lookup"><span data-stu-id="2536a-300">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="2536a-301">Resposta</span><span class="sxs-lookup"><span data-stu-id="2536a-301">Response</span></span>
<span data-ttu-id="2536a-302">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2536a-302">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2536a-303">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2536a-303">Example</span></span>
### <a name="request"></a><span data-ttu-id="2536a-304">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2536a-304">Request</span></span>
<span data-ttu-id="2536a-305">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2536a-305">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2156

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="2536a-306">Resposta</span><span class="sxs-lookup"><span data-stu-id="2536a-306">Response</span></span>
<span data-ttu-id="2536a-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2536a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2264

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





