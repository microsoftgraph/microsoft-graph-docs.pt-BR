---
title: Atualizar androidGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto androidGeneralDeviceConfiguration.
ms.openlocfilehash: e8ec4865cb5c031f698b5e1660b546a3fcf09bdd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006630"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="81249-103">Atualizar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="81249-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="81249-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="81249-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81249-105">Atualizar as propriedades de um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81249-105">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81249-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81249-106">Prerequisites</span></span>
<span data-ttu-id="81249-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81249-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81249-109">Permission type</span></span>|<span data-ttu-id="81249-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81249-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81249-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81249-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81249-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81249-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="81249-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81249-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81249-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81249-114">Not supported.</span></span>|
|<span data-ttu-id="81249-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81249-115">Application</span></span>|<span data-ttu-id="81249-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81249-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81249-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81249-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="81249-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81249-118">Request headers</span></span>
|<span data-ttu-id="81249-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81249-119">Header</span></span>|<span data-ttu-id="81249-120">Valor</span><span class="sxs-lookup"><span data-stu-id="81249-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81249-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="81249-121">Authorization</span></span>|<span data-ttu-id="81249-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81249-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81249-123">Accept</span><span class="sxs-lookup"><span data-stu-id="81249-123">Accept</span></span>|<span data-ttu-id="81249-124">application/json</span><span class="sxs-lookup"><span data-stu-id="81249-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81249-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81249-125">Request body</span></span>
<span data-ttu-id="81249-126">No corpo da solicitação, forneça uma representação JSON do objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81249-126">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="81249-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81249-127">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="81249-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81249-128">Property</span></span>|<span data-ttu-id="81249-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="81249-129">Type</span></span>|<span data-ttu-id="81249-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="81249-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81249-131">id</span><span class="sxs-lookup"><span data-stu-id="81249-131">id</span></span>|<span data-ttu-id="81249-132">String</span><span class="sxs-lookup"><span data-stu-id="81249-132">String</span></span>|<span data-ttu-id="81249-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="81249-133">Key of the entity.</span></span> <span data-ttu-id="81249-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81249-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81249-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81249-135">lastModifiedDateTime</span></span>|<span data-ttu-id="81249-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81249-136">DateTimeOffset</span></span>|<span data-ttu-id="81249-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="81249-137">DateTime the object was last modified.</span></span> <span data-ttu-id="81249-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81249-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81249-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81249-139">createdDateTime</span></span>|<span data-ttu-id="81249-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81249-140">DateTimeOffset</span></span>|<span data-ttu-id="81249-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="81249-141">DateTime the object was created.</span></span> <span data-ttu-id="81249-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81249-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81249-143">description</span><span class="sxs-lookup"><span data-stu-id="81249-143">description</span></span>|<span data-ttu-id="81249-144">String</span><span class="sxs-lookup"><span data-stu-id="81249-144">String</span></span>|<span data-ttu-id="81249-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81249-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="81249-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81249-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81249-147">displayName</span><span class="sxs-lookup"><span data-stu-id="81249-147">displayName</span></span>|<span data-ttu-id="81249-148">String</span><span class="sxs-lookup"><span data-stu-id="81249-148">String</span></span>|<span data-ttu-id="81249-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81249-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="81249-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81249-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81249-151">version</span><span class="sxs-lookup"><span data-stu-id="81249-151">version</span></span>|<span data-ttu-id="81249-152">Int32</span><span class="sxs-lookup"><span data-stu-id="81249-152">Int32</span></span>|<span data-ttu-id="81249-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81249-153">Version of the device configuration.</span></span> <span data-ttu-id="81249-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81249-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81249-155">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="81249-155">appsBlockClipboardSharing</span></span>|<span data-ttu-id="81249-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-156">Boolean</span></span>|<span data-ttu-id="81249-157">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="81249-157">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="81249-158">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="81249-158">appsBlockCopyPaste</span></span>|<span data-ttu-id="81249-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-159">Boolean</span></span>|<span data-ttu-id="81249-160">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="81249-160">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="81249-161">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="81249-161">appsBlockYouTube</span></span>|<span data-ttu-id="81249-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-162">Boolean</span></span>|<span data-ttu-id="81249-163">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-163">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="81249-164">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-164">bluetoothBlocked</span></span>|<span data-ttu-id="81249-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-165">Boolean</span></span>|<span data-ttu-id="81249-166">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-166">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="81249-167">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-167">cameraBlocked</span></span>|<span data-ttu-id="81249-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-168">Boolean</span></span>|<span data-ttu-id="81249-169">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-169">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="81249-170">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="81249-170">cellularBlockDataRoaming</span></span>|<span data-ttu-id="81249-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-171">Boolean</span></span>|<span data-ttu-id="81249-172">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-172">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="81249-173">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="81249-173">cellularBlockMessaging</span></span>|<span data-ttu-id="81249-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-174">Boolean</span></span>|<span data-ttu-id="81249-175">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="81249-175">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="81249-176">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="81249-176">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="81249-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-177">Boolean</span></span>|<span data-ttu-id="81249-178">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-178">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="81249-179">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="81249-179">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="81249-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-180">Boolean</span></span>|<span data-ttu-id="81249-181">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="81249-181">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="81249-182">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="81249-182">compliantAppsList</span></span>|<span data-ttu-id="81249-183">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="81249-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="81249-184">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="81249-184">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="81249-185">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="81249-185">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="81249-186">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="81249-186">compliantAppListType</span></span>|[<span data-ttu-id="81249-187">appListType</span><span class="sxs-lookup"><span data-stu-id="81249-187">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="81249-188">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="81249-188">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="81249-189">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="81249-189">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="81249-190">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="81249-190">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="81249-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-191">Boolean</span></span>|<span data-ttu-id="81249-192">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-192">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="81249-193">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-193">locationServicesBlocked</span></span>|<span data-ttu-id="81249-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-194">Boolean</span></span>|<span data-ttu-id="81249-195">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="81249-195">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="81249-196">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="81249-196">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="81249-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-197">Boolean</span></span>|<span data-ttu-id="81249-198">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="81249-198">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="81249-199">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-199">googlePlayStoreBlocked</span></span>|<span data-ttu-id="81249-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-200">Boolean</span></span>|<span data-ttu-id="81249-201">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="81249-201">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="81249-202">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="81249-202">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="81249-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-203">Boolean</span></span>|<span data-ttu-id="81249-204">Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="81249-204">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="81249-205">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="81249-205">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="81249-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-206">Boolean</span></span>|<span data-ttu-id="81249-207">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="81249-207">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="81249-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="81249-208">kioskModeApps</span></span>|<span data-ttu-id="81249-209">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="81249-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="81249-210">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="81249-210">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="81249-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="81249-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="81249-212">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-212">nfcBlocked</span></span>|<span data-ttu-id="81249-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-213">Boolean</span></span>|<span data-ttu-id="81249-214">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="81249-214">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="81249-215">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="81249-215">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="81249-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-216">Boolean</span></span>|<span data-ttu-id="81249-217">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-217">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="81249-218">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="81249-218">passwordBlockTrustAgents</span></span>|<span data-ttu-id="81249-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-219">Boolean</span></span>|<span data-ttu-id="81249-220">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="81249-220">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="81249-221">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="81249-221">passwordExpirationDays</span></span>|<span data-ttu-id="81249-222">Int32</span><span class="sxs-lookup"><span data-stu-id="81249-222">Int32</span></span>|<span data-ttu-id="81249-223">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="81249-223">Number of days before the password expires.</span></span> <span data-ttu-id="81249-224">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="81249-224">Valid values 1 to 365</span></span>|
|<span data-ttu-id="81249-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="81249-225">passwordMinimumLength</span></span>|<span data-ttu-id="81249-226">Int32</span><span class="sxs-lookup"><span data-stu-id="81249-226">Int32</span></span>|<span data-ttu-id="81249-227">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="81249-227">Minimum length of passwords.</span></span> <span data-ttu-id="81249-228">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="81249-228">Valid values 4 to 16</span></span>|
|<span data-ttu-id="81249-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="81249-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="81249-230">Int32</span><span class="sxs-lookup"><span data-stu-id="81249-230">Int32</span></span>|<span data-ttu-id="81249-231">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="81249-231">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="81249-232">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="81249-232">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="81249-233">Int32</span><span class="sxs-lookup"><span data-stu-id="81249-233">Int32</span></span>|<span data-ttu-id="81249-234">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="81249-234">Number of previous passwords to block.</span></span> <span data-ttu-id="81249-235">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="81249-235">Valid values 0 to 24</span></span>|
|<span data-ttu-id="81249-236">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="81249-236">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="81249-237">Int32</span><span class="sxs-lookup"><span data-stu-id="81249-237">Int32</span></span>|<span data-ttu-id="81249-238">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="81249-238">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="81249-239">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="81249-239">Valid values 4 to 11</span></span>|
|<span data-ttu-id="81249-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="81249-240">passwordRequiredType</span></span>|[<span data-ttu-id="81249-241">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="81249-241">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="81249-242">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="81249-242">Type of password that is required.</span></span> <span data-ttu-id="81249-243">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="81249-243">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="81249-244">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="81249-244">passwordRequired</span></span>|<span data-ttu-id="81249-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-245">Boolean</span></span>|<span data-ttu-id="81249-246">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="81249-246">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="81249-247">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-247">powerOffBlocked</span></span>|<span data-ttu-id="81249-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-248">Boolean</span></span>|<span data-ttu-id="81249-249">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-249">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="81249-250">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-250">factoryResetBlocked</span></span>|<span data-ttu-id="81249-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-251">Boolean</span></span>|<span data-ttu-id="81249-252">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="81249-252">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="81249-253">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-253">screenCaptureBlocked</span></span>|<span data-ttu-id="81249-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-254">Boolean</span></span>|<span data-ttu-id="81249-255">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="81249-255">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="81249-256">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="81249-256">deviceSharingAllowed</span></span>|<span data-ttu-id="81249-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-257">Boolean</span></span>|<span data-ttu-id="81249-258">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="81249-258">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="81249-259">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="81249-259">storageBlockGoogleBackup</span></span>|<span data-ttu-id="81249-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-260">Boolean</span></span>|<span data-ttu-id="81249-261">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-261">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="81249-262">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="81249-262">storageBlockRemovableStorage</span></span>|<span data-ttu-id="81249-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-263">Boolean</span></span>|<span data-ttu-id="81249-264">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-264">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="81249-265">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="81249-265">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="81249-266">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-266">Boolean</span></span>|<span data-ttu-id="81249-267">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="81249-267">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="81249-268">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="81249-268">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="81249-269">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-269">Boolean</span></span>|<span data-ttu-id="81249-270">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="81249-270">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="81249-271">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-271">voiceAssistantBlocked</span></span>|<span data-ttu-id="81249-272">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-272">Boolean</span></span>|<span data-ttu-id="81249-273">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-273">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="81249-274">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-274">voiceDialingBlocked</span></span>|<span data-ttu-id="81249-275">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-275">Boolean</span></span>|<span data-ttu-id="81249-276">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="81249-276">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="81249-277">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="81249-277">webBrowserBlockPopups</span></span>|<span data-ttu-id="81249-278">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-278">Boolean</span></span>|<span data-ttu-id="81249-279">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="81249-279">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="81249-280">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="81249-280">webBrowserBlockAutofill</span></span>|<span data-ttu-id="81249-281">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-281">Boolean</span></span>|<span data-ttu-id="81249-282">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-282">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="81249-283">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="81249-283">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="81249-284">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-284">Boolean</span></span>|<span data-ttu-id="81249-285">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-285">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="81249-286">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-286">webBrowserBlocked</span></span>|<span data-ttu-id="81249-287">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-287">Boolean</span></span>|<span data-ttu-id="81249-288">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="81249-288">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="81249-289">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="81249-289">webBrowserCookieSettings</span></span>|[<span data-ttu-id="81249-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="81249-290">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="81249-291">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="81249-291">Cookie settings within the web browser.</span></span> <span data-ttu-id="81249-292">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="81249-292">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="81249-293">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="81249-293">wiFiBlocked</span></span>|<span data-ttu-id="81249-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-294">Boolean</span></span>|<span data-ttu-id="81249-295">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="81249-295">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="81249-296">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="81249-296">appsInstallAllowList</span></span>|<span data-ttu-id="81249-297">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="81249-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="81249-298">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="81249-298">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="81249-299">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="81249-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="81249-300">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="81249-300">appsLaunchBlockList</span></span>|<span data-ttu-id="81249-301">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="81249-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="81249-302">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="81249-302">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="81249-303">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="81249-303">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="81249-304">appsHideList</span><span class="sxs-lookup"><span data-stu-id="81249-304">appsHideList</span></span>|<span data-ttu-id="81249-305">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="81249-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="81249-306">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="81249-306">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="81249-307">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="81249-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="81249-308">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="81249-308">securityRequireVerifyApps</span></span>|<span data-ttu-id="81249-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="81249-309">Boolean</span></span>|<span data-ttu-id="81249-310">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="81249-310">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="81249-311">Resposta</span><span class="sxs-lookup"><span data-stu-id="81249-311">Response</span></span>
<span data-ttu-id="81249-312">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81249-312">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81249-313">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81249-313">Example</span></span>
### <a name="request"></a><span data-ttu-id="81249-314">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81249-314">Request</span></span>
<span data-ttu-id="81249-315">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81249-315">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3033

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="81249-316">Resposta</span><span class="sxs-lookup"><span data-stu-id="81249-316">Response</span></span>
<span data-ttu-id="81249-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81249-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



