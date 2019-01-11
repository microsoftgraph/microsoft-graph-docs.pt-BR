---
title: Atualizar androidGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 175546ec4f91067605b8af05eb517563c1f4897e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887700"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="319d9-103">Atualizar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="319d9-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="319d9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="319d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="319d9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="319d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="319d9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="319d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="319d9-107">Atualizar as propriedades de um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319d9-107">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="319d9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="319d9-108">Prerequisites</span></span>
<span data-ttu-id="319d9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="319d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="319d9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="319d9-111">Permission type</span></span>|<span data-ttu-id="319d9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="319d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="319d9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="319d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="319d9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="319d9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="319d9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="319d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="319d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="319d9-116">Not supported.</span></span>|
|<span data-ttu-id="319d9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="319d9-117">Application</span></span>|<span data-ttu-id="319d9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="319d9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="319d9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="319d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="319d9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="319d9-120">Request headers</span></span>
|<span data-ttu-id="319d9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="319d9-121">Header</span></span>|<span data-ttu-id="319d9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="319d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="319d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="319d9-123">Authorization</span></span>|<span data-ttu-id="319d9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="319d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="319d9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="319d9-125">Accept</span></span>|<span data-ttu-id="319d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="319d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="319d9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="319d9-127">Request body</span></span>
<span data-ttu-id="319d9-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319d9-128">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="319d9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319d9-129">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="319d9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="319d9-130">Property</span></span>|<span data-ttu-id="319d9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="319d9-131">Type</span></span>|<span data-ttu-id="319d9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="319d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="319d9-133">id</span><span class="sxs-lookup"><span data-stu-id="319d9-133">id</span></span>|<span data-ttu-id="319d9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="319d9-134">String</span></span>|<span data-ttu-id="319d9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="319d9-135">Key of the entity.</span></span> <span data-ttu-id="319d9-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319d9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="319d9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="319d9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319d9-138">DateTimeOffset</span></span>|<span data-ttu-id="319d9-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="319d9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="319d9-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319d9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="319d9-141">roleScopeTagIds</span></span>|<span data-ttu-id="319d9-142">String collection</span><span class="sxs-lookup"><span data-stu-id="319d9-142">String collection</span></span>|<span data-ttu-id="319d9-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="319d9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="319d9-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319d9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="319d9-145">supportsScopeTags</span></span>|<span data-ttu-id="319d9-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-146">Boolean</span></span>|<span data-ttu-id="319d9-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="319d9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="319d9-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="319d9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="319d9-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="319d9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="319d9-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="319d9-150">This property is read-only.</span></span> <span data-ttu-id="319d9-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319d9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="319d9-152">createdDateTime</span></span>|<span data-ttu-id="319d9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319d9-153">DateTimeOffset</span></span>|<span data-ttu-id="319d9-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="319d9-154">DateTime the object was created.</span></span> <span data-ttu-id="319d9-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319d9-156">description</span><span class="sxs-lookup"><span data-stu-id="319d9-156">description</span></span>|<span data-ttu-id="319d9-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="319d9-157">String</span></span>|<span data-ttu-id="319d9-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="319d9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="319d9-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319d9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="319d9-160">displayName</span></span>|<span data-ttu-id="319d9-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="319d9-161">String</span></span>|<span data-ttu-id="319d9-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="319d9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="319d9-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319d9-164">version</span><span class="sxs-lookup"><span data-stu-id="319d9-164">version</span></span>|<span data-ttu-id="319d9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="319d9-165">Int32</span></span>|<span data-ttu-id="319d9-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="319d9-166">Version of the device configuration.</span></span> <span data-ttu-id="319d9-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319d9-168">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="319d9-168">appsBlockClipboardSharing</span></span>|<span data-ttu-id="319d9-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-169">Boolean</span></span>|<span data-ttu-id="319d9-170">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="319d9-170">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="319d9-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="319d9-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="319d9-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-172">Boolean</span></span>|<span data-ttu-id="319d9-173">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="319d9-173">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="319d9-174">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="319d9-174">appsBlockYouTube</span></span>|<span data-ttu-id="319d9-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-175">Boolean</span></span>|<span data-ttu-id="319d9-176">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-176">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="319d9-177">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-177">bluetoothBlocked</span></span>|<span data-ttu-id="319d9-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-178">Boolean</span></span>|<span data-ttu-id="319d9-179">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-179">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="319d9-180">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-180">cameraBlocked</span></span>|<span data-ttu-id="319d9-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-181">Boolean</span></span>|<span data-ttu-id="319d9-182">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-182">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="319d9-183">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="319d9-183">cellularBlockDataRoaming</span></span>|<span data-ttu-id="319d9-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-184">Boolean</span></span>|<span data-ttu-id="319d9-185">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-185">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="319d9-186">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="319d9-186">cellularBlockMessaging</span></span>|<span data-ttu-id="319d9-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-187">Boolean</span></span>|<span data-ttu-id="319d9-188">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="319d9-188">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="319d9-189">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="319d9-189">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="319d9-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-190">Boolean</span></span>|<span data-ttu-id="319d9-191">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-191">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="319d9-192">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="319d9-192">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="319d9-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-193">Boolean</span></span>|<span data-ttu-id="319d9-194">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="319d9-194">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="319d9-195">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="319d9-195">compliantAppsList</span></span>|<span data-ttu-id="319d9-196">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="319d9-197">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="319d9-197">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="319d9-198">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="319d9-198">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="319d9-199">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="319d9-199">compliantAppListType</span></span>|[<span data-ttu-id="319d9-200">appListType</span><span class="sxs-lookup"><span data-stu-id="319d9-200">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="319d9-201">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="319d9-201">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="319d9-202">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="319d9-202">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="319d9-203">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="319d9-203">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="319d9-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-204">Boolean</span></span>|<span data-ttu-id="319d9-205">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-205">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="319d9-206">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-206">locationServicesBlocked</span></span>|<span data-ttu-id="319d9-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-207">Boolean</span></span>|<span data-ttu-id="319d9-208">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="319d9-208">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="319d9-209">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="319d9-209">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="319d9-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-210">Boolean</span></span>|<span data-ttu-id="319d9-211">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="319d9-211">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="319d9-212">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-212">googlePlayStoreBlocked</span></span>|<span data-ttu-id="319d9-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-213">Boolean</span></span>|<span data-ttu-id="319d9-214">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="319d9-214">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="319d9-215">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="319d9-215">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="319d9-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-216">Boolean</span></span>|<span data-ttu-id="319d9-217">Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="319d9-217">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="319d9-218">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="319d9-218">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="319d9-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-219">Boolean</span></span>|<span data-ttu-id="319d9-220">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="319d9-220">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="319d9-221">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="319d9-221">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="319d9-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-222">Boolean</span></span>|<span data-ttu-id="319d9-223">Indica se o bloqueio da mudança de data e hora durante o modo KNOX ou não.</span><span class="sxs-lookup"><span data-stu-id="319d9-223">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="319d9-224">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="319d9-224">kioskModeApps</span></span>|<span data-ttu-id="319d9-225">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="319d9-226">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="319d9-226">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="319d9-227">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="319d9-227">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="319d9-228">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-228">nfcBlocked</span></span>|<span data-ttu-id="319d9-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-229">Boolean</span></span>|<span data-ttu-id="319d9-230">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="319d9-230">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="319d9-231">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="319d9-231">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="319d9-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-232">Boolean</span></span>|<span data-ttu-id="319d9-233">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-233">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="319d9-234">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="319d9-234">passwordBlockTrustAgents</span></span>|<span data-ttu-id="319d9-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-235">Boolean</span></span>|<span data-ttu-id="319d9-236">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="319d9-236">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="319d9-237">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="319d9-237">passwordExpirationDays</span></span>|<span data-ttu-id="319d9-238">Int32</span><span class="sxs-lookup"><span data-stu-id="319d9-238">Int32</span></span>|<span data-ttu-id="319d9-239">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="319d9-239">Number of days before the password expires.</span></span> <span data-ttu-id="319d9-240">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="319d9-240">Valid values 1 to 365</span></span>|
|<span data-ttu-id="319d9-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="319d9-241">passwordMinimumLength</span></span>|<span data-ttu-id="319d9-242">Int32</span><span class="sxs-lookup"><span data-stu-id="319d9-242">Int32</span></span>|<span data-ttu-id="319d9-243">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="319d9-243">Minimum length of passwords.</span></span> <span data-ttu-id="319d9-244">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="319d9-244">Valid values 4 to 16</span></span>|
|<span data-ttu-id="319d9-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="319d9-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="319d9-246">Int32</span><span class="sxs-lookup"><span data-stu-id="319d9-246">Int32</span></span>|<span data-ttu-id="319d9-247">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="319d9-247">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="319d9-248">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="319d9-248">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="319d9-249">Int32</span><span class="sxs-lookup"><span data-stu-id="319d9-249">Int32</span></span>|<span data-ttu-id="319d9-250">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="319d9-250">Number of previous passwords to block.</span></span> <span data-ttu-id="319d9-251">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="319d9-251">Valid values 0 to 24</span></span>|
|<span data-ttu-id="319d9-252">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="319d9-252">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="319d9-253">Int32</span><span class="sxs-lookup"><span data-stu-id="319d9-253">Int32</span></span>|<span data-ttu-id="319d9-254">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="319d9-254">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="319d9-255">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="319d9-255">Valid values 4 to 11</span></span>|
|<span data-ttu-id="319d9-256">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="319d9-256">passwordRequiredType</span></span>|[<span data-ttu-id="319d9-257">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="319d9-257">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="319d9-258">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="319d9-258">Type of password that is required.</span></span> <span data-ttu-id="319d9-259">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="319d9-259">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="319d9-260">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="319d9-260">passwordRequired</span></span>|<span data-ttu-id="319d9-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-261">Boolean</span></span>|<span data-ttu-id="319d9-262">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="319d9-262">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="319d9-263">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-263">powerOffBlocked</span></span>|<span data-ttu-id="319d9-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-264">Boolean</span></span>|<span data-ttu-id="319d9-265">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-265">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="319d9-266">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-266">factoryResetBlocked</span></span>|<span data-ttu-id="319d9-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-267">Boolean</span></span>|<span data-ttu-id="319d9-268">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="319d9-268">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="319d9-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-269">screenCaptureBlocked</span></span>|<span data-ttu-id="319d9-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-270">Boolean</span></span>|<span data-ttu-id="319d9-271">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="319d9-271">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="319d9-272">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="319d9-272">deviceSharingAllowed</span></span>|<span data-ttu-id="319d9-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-273">Boolean</span></span>|<span data-ttu-id="319d9-274">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="319d9-274">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="319d9-275">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="319d9-275">storageBlockGoogleBackup</span></span>|<span data-ttu-id="319d9-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-276">Boolean</span></span>|<span data-ttu-id="319d9-277">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-277">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="319d9-278">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="319d9-278">storageBlockRemovableStorage</span></span>|<span data-ttu-id="319d9-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-279">Boolean</span></span>|<span data-ttu-id="319d9-280">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-280">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="319d9-281">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="319d9-281">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="319d9-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-282">Boolean</span></span>|<span data-ttu-id="319d9-283">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="319d9-283">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="319d9-284">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="319d9-284">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="319d9-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-285">Boolean</span></span>|<span data-ttu-id="319d9-286">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="319d9-286">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="319d9-287">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-287">voiceAssistantBlocked</span></span>|<span data-ttu-id="319d9-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-288">Boolean</span></span>|<span data-ttu-id="319d9-289">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-289">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="319d9-290">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-290">voiceDialingBlocked</span></span>|<span data-ttu-id="319d9-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-291">Boolean</span></span>|<span data-ttu-id="319d9-292">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="319d9-292">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="319d9-293">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="319d9-293">webBrowserBlockPopups</span></span>|<span data-ttu-id="319d9-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-294">Boolean</span></span>|<span data-ttu-id="319d9-295">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="319d9-295">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="319d9-296">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="319d9-296">webBrowserBlockAutofill</span></span>|<span data-ttu-id="319d9-297">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-297">Boolean</span></span>|<span data-ttu-id="319d9-298">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-298">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="319d9-299">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="319d9-299">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="319d9-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-300">Boolean</span></span>|<span data-ttu-id="319d9-301">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-301">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="319d9-302">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-302">webBrowserBlocked</span></span>|<span data-ttu-id="319d9-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-303">Boolean</span></span>|<span data-ttu-id="319d9-304">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="319d9-304">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="319d9-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="319d9-305">webBrowserCookieSettings</span></span>|[<span data-ttu-id="319d9-306">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="319d9-306">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="319d9-307">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="319d9-307">Cookie settings within the web browser.</span></span> <span data-ttu-id="319d9-308">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="319d9-308">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="319d9-309">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="319d9-309">wiFiBlocked</span></span>|<span data-ttu-id="319d9-310">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-310">Boolean</span></span>|<span data-ttu-id="319d9-311">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="319d9-311">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="319d9-312">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="319d9-312">appsInstallAllowList</span></span>|<span data-ttu-id="319d9-313">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="319d9-314">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="319d9-314">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="319d9-315">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="319d9-315">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="319d9-316">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="319d9-316">appsLaunchBlockList</span></span>|<span data-ttu-id="319d9-317">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="319d9-318">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="319d9-318">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="319d9-319">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="319d9-319">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="319d9-320">appsHideList</span><span class="sxs-lookup"><span data-stu-id="319d9-320">appsHideList</span></span>|<span data-ttu-id="319d9-321">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="319d9-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="319d9-322">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="319d9-322">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="319d9-323">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="319d9-323">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="319d9-324">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="319d9-324">securityRequireVerifyApps</span></span>|<span data-ttu-id="319d9-325">Booliano</span><span class="sxs-lookup"><span data-stu-id="319d9-325">Boolean</span></span>|<span data-ttu-id="319d9-326">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="319d9-326">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="319d9-327">Resposta</span><span class="sxs-lookup"><span data-stu-id="319d9-327">Response</span></span>
<span data-ttu-id="319d9-328">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="319d9-328">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="319d9-329">Exemplo</span><span class="sxs-lookup"><span data-stu-id="319d9-329">Example</span></span>
### <a name="request"></a><span data-ttu-id="319d9-330">Solicitação</span><span class="sxs-lookup"><span data-stu-id="319d9-330">Request</span></span>
<span data-ttu-id="319d9-331">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="319d9-331">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3153

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="319d9-332">Resposta</span><span class="sxs-lookup"><span data-stu-id="319d9-332">Response</span></span>
<span data-ttu-id="319d9-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="319d9-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3333

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```





