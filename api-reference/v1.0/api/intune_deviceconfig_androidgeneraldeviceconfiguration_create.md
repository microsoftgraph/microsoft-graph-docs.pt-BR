# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="b4e7f-101">Criar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4e7f-101">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b4e7f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4e7f-103">Criar um novo objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4e7f-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4e7f-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4e7f-104">Prerequisites</span></span>
<span data-ttu-id="b4e7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4e7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4e7f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4e7f-107">Permission type</span></span>|<span data-ttu-id="b4e7f-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4e7f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b4e7f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4e7f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4e7f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4e7f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-112">Not supported.</span></span>|
|<span data-ttu-id="b4e7f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4e7f-113">Application</span></span>|<span data-ttu-id="b4e7f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4e7f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4e7f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4e7f-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4e7f-116">Request headers</span></span>
|<span data-ttu-id="b4e7f-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4e7f-117">Header</span></span>|<span data-ttu-id="b4e7f-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b4e7f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4e7f-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4e7f-119">Authorization</span></span>|<span data-ttu-id="b4e7f-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b4e7f-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4e7f-121">Accept</span></span>|<span data-ttu-id="b4e7f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b4e7f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4e7f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4e7f-123">Request body</span></span>
<span data-ttu-id="b4e7f-124">No corpo da solicitação, forneça uma representação JSON do objeto androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b4e7f-125">A tabela a seguir mostra as propriedades que são necessárias ao criar androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="b4e7f-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4e7f-126">Property</span></span>|<span data-ttu-id="b4e7f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4e7f-127">Type</span></span>|<span data-ttu-id="b4e7f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4e7f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e7f-129">id</span><span class="sxs-lookup"><span data-stu-id="b4e7f-129">id</span></span>|<span data-ttu-id="b4e7f-130">String</span><span class="sxs-lookup"><span data-stu-id="b4e7f-130">String</span></span>|<span data-ttu-id="b4e7f-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-131">Key of the setting.</span></span> <span data-ttu-id="b4e7f-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e7f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4e7f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b4e7f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4e7f-134">DateTimeOffset</span></span>|<span data-ttu-id="b4e7f-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="b4e7f-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e7f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4e7f-137">createdDateTime</span></span>|<span data-ttu-id="b4e7f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4e7f-138">DateTimeOffset</span></span>|<span data-ttu-id="b4e7f-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-139">DateTime the object was created.</span></span> <span data-ttu-id="b4e7f-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e7f-141">descrição</span><span class="sxs-lookup"><span data-stu-id="b4e7f-141">description</span></span>|<span data-ttu-id="b4e7f-142">String</span><span class="sxs-lookup"><span data-stu-id="b4e7f-142">String</span></span>|<span data-ttu-id="b4e7f-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4e7f-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e7f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b4e7f-145">displayName</span></span>|<span data-ttu-id="b4e7f-146">String</span><span class="sxs-lookup"><span data-stu-id="b4e7f-146">String</span></span>|<span data-ttu-id="b4e7f-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4e7f-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e7f-149">version</span><span class="sxs-lookup"><span data-stu-id="b4e7f-149">version</span></span>|<span data-ttu-id="b4e7f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b4e7f-150">Int32</span></span>|<span data-ttu-id="b4e7f-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-151">Version of the device configuration.</span></span> <span data-ttu-id="b4e7f-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4e7f-153">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="b4e7f-153">appsBlockClipboardSharing</span></span>|<span data-ttu-id="b4e7f-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-154">Boolean</span></span>|<span data-ttu-id="b4e7f-155">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-155">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="b4e7f-156">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="b4e7f-156">appsBlockCopyPaste</span></span>|<span data-ttu-id="b4e7f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-157">Boolean</span></span>|<span data-ttu-id="b4e7f-158">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-158">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="b4e7f-159">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="b4e7f-159">appsBlockYouTube</span></span>|<span data-ttu-id="b4e7f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-160">Boolean</span></span>|<span data-ttu-id="b4e7f-161">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-161">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="b4e7f-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-162">bluetoothBlocked</span></span>|<span data-ttu-id="b4e7f-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-163">Boolean</span></span>|<span data-ttu-id="b4e7f-164">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-164">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="b4e7f-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-165">cameraBlocked</span></span>|<span data-ttu-id="b4e7f-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-166">Boolean</span></span>|<span data-ttu-id="b4e7f-167">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-167">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="b4e7f-168">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b4e7f-168">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b4e7f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-169">Boolean</span></span>|<span data-ttu-id="b4e7f-170">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-170">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b4e7f-171">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="b4e7f-171">cellularBlockMessaging</span></span>|<span data-ttu-id="b4e7f-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-172">Boolean</span></span>|<span data-ttu-id="b4e7f-173">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-173">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="b4e7f-174">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="b4e7f-174">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="b4e7f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-175">Boolean</span></span>|<span data-ttu-id="b4e7f-176">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-176">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="b4e7f-177">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="b4e7f-177">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="b4e7f-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-178">Boolean</span></span>|<span data-ttu-id="b4e7f-179">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-179">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="b4e7f-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b4e7f-180">compliantAppsList</span></span>|<span data-ttu-id="b4e7f-181">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-181">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b4e7f-182">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="b4e7f-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b4e7f-183">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b4e7f-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b4e7f-184">compliantAppListType</span></span>|<span data-ttu-id="b4e7f-185">String</span><span class="sxs-lookup"><span data-stu-id="b4e7f-185">String</span></span>|<span data-ttu-id="b4e7f-186">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-186">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="b4e7f-187">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b4e7f-188">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b4e7f-188">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b4e7f-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-189">Boolean</span></span>|<span data-ttu-id="b4e7f-190">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-190">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b4e7f-191">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-191">locationServicesBlocked</span></span>|<span data-ttu-id="b4e7f-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-192">Boolean</span></span>|<span data-ttu-id="b4e7f-193">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-193">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="b4e7f-194">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="b4e7f-194">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="b4e7f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-195">Boolean</span></span>|<span data-ttu-id="b4e7f-196">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-196">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="b4e7f-197">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-197">googlePlayStoreBlocked</span></span>|<span data-ttu-id="b4e7f-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-198">Boolean</span></span>|<span data-ttu-id="b4e7f-199">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-199">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="b4e7f-200">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="b4e7f-200">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="b4e7f-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-201">Boolean</span></span>|<span data-ttu-id="b4e7f-202">Indica se o botão de suspensão de tela deve ou não ser bloqueado no Modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-202">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="b4e7f-203">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b4e7f-203">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="b4e7f-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-204">Boolean</span></span>|<span data-ttu-id="b4e7f-205">Indica se os botões de volume devem ou não ser bloqueados no Modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-205">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="b4e7f-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="b4e7f-206">kioskModeApps</span></span>|<span data-ttu-id="b4e7f-207">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-207">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b4e7f-208">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no Modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-208">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="b4e7f-209">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b4e7f-210">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-210">nfcBlocked</span></span>|<span data-ttu-id="b4e7f-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-211">Boolean</span></span>|<span data-ttu-id="b4e7f-212">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-212">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="b4e7f-213">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b4e7f-213">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="b4e7f-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-214">Boolean</span></span>|<span data-ttu-id="b4e7f-215">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-215">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b4e7f-216">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="b4e7f-216">passwordBlockTrustAgents</span></span>|<span data-ttu-id="b4e7f-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-217">Boolean</span></span>|<span data-ttu-id="b4e7f-218">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-218">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="b4e7f-219">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b4e7f-219">passwordExpirationDays</span></span>|<span data-ttu-id="b4e7f-220">Int32</span><span class="sxs-lookup"><span data-stu-id="b4e7f-220">Int32</span></span>|<span data-ttu-id="b4e7f-221">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-221">Number of days before the password expires.</span></span> <span data-ttu-id="b4e7f-222">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="b4e7f-222">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b4e7f-223">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b4e7f-223">passwordMinimumLength</span></span>|<span data-ttu-id="b4e7f-224">Int32</span><span class="sxs-lookup"><span data-stu-id="b4e7f-224">Int32</span></span>|<span data-ttu-id="b4e7f-225">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-225">Minimum length of passwords.</span></span> <span data-ttu-id="b4e7f-226">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="b4e7f-226">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b4e7f-227">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b4e7f-227">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b4e7f-228">Int32</span><span class="sxs-lookup"><span data-stu-id="b4e7f-228">Int32</span></span>|<span data-ttu-id="b4e7f-229">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-229">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b4e7f-230">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b4e7f-230">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b4e7f-231">Int32</span><span class="sxs-lookup"><span data-stu-id="b4e7f-231">Int32</span></span>|<span data-ttu-id="b4e7f-232">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-232">Number of previous passwords to block.</span></span> <span data-ttu-id="b4e7f-233">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="b4e7f-233">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b4e7f-234">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b4e7f-234">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b4e7f-235">Int32</span><span class="sxs-lookup"><span data-stu-id="b4e7f-235">Int32</span></span>|<span data-ttu-id="b4e7f-236">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-236">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="b4e7f-237">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="b4e7f-237">Valid values 4 to 11</span></span>|
|<span data-ttu-id="b4e7f-238">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b4e7f-238">passwordRequiredType</span></span>|<span data-ttu-id="b4e7f-239">String</span><span class="sxs-lookup"><span data-stu-id="b4e7f-239">String</span></span>|<span data-ttu-id="b4e7f-240">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-240">Type of password that is required.</span></span> <span data-ttu-id="b4e7f-241">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-241">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`.</span></span>|
|<span data-ttu-id="b4e7f-242">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b4e7f-242">passwordRequired</span></span>|<span data-ttu-id="b4e7f-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-243">Boolean</span></span>|<span data-ttu-id="b4e7f-244">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-244">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="b4e7f-245">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-245">powerOffBlocked</span></span>|<span data-ttu-id="b4e7f-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-246">Boolean</span></span>|<span data-ttu-id="b4e7f-247">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-247">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="b4e7f-248">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-248">factoryResetBlocked</span></span>|<span data-ttu-id="b4e7f-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-249">Boolean</span></span>|<span data-ttu-id="b4e7f-250">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-250">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="b4e7f-251">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-251">screenCaptureBlocked</span></span>|<span data-ttu-id="b4e7f-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-252">Boolean</span></span>|<span data-ttu-id="b4e7f-253">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-253">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="b4e7f-254">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="b4e7f-254">deviceSharingAllowed</span></span>|<span data-ttu-id="b4e7f-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-255">Boolean</span></span>|<span data-ttu-id="b4e7f-256">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-256">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="b4e7f-257">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="b4e7f-257">storageBlockGoogleBackup</span></span>|<span data-ttu-id="b4e7f-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-258">Boolean</span></span>|<span data-ttu-id="b4e7f-259">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-259">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="b4e7f-260">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="b4e7f-260">storageBlockRemovableStorage</span></span>|<span data-ttu-id="b4e7f-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-261">Boolean</span></span>|<span data-ttu-id="b4e7f-262">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-262">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="b4e7f-263">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="b4e7f-263">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="b4e7f-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-264">Boolean</span></span>|<span data-ttu-id="b4e7f-265">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-265">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="b4e7f-266">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="b4e7f-266">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="b4e7f-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-267">Boolean</span></span>|<span data-ttu-id="b4e7f-268">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-268">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="b4e7f-269">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-269">voiceAssistantBlocked</span></span>|<span data-ttu-id="b4e7f-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-270">Boolean</span></span>|<span data-ttu-id="b4e7f-271">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-271">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="b4e7f-272">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-272">voiceDialingBlocked</span></span>|<span data-ttu-id="b4e7f-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-273">Boolean</span></span>|<span data-ttu-id="b4e7f-274">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-274">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="b4e7f-275">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b4e7f-275">webBrowserBlockPopups</span></span>|<span data-ttu-id="b4e7f-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-276">Boolean</span></span>|<span data-ttu-id="b4e7f-277">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-277">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="b4e7f-278">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b4e7f-278">webBrowserBlockAutofill</span></span>|<span data-ttu-id="b4e7f-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-279">Boolean</span></span>|<span data-ttu-id="b4e7f-280">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-280">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="b4e7f-281">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b4e7f-281">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="b4e7f-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-282">Boolean</span></span>|<span data-ttu-id="b4e7f-283">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-283">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="b4e7f-284">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-284">webBrowserBlocked</span></span>|<span data-ttu-id="b4e7f-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-285">Boolean</span></span>|<span data-ttu-id="b4e7f-286">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-286">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="b4e7f-287">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b4e7f-287">webBrowserCookieSettings</span></span>|<span data-ttu-id="b4e7f-288">String</span><span class="sxs-lookup"><span data-stu-id="b4e7f-288">String</span></span>|<span data-ttu-id="b4e7f-289">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-289">Cookie settings within the web browser.</span></span> <span data-ttu-id="b4e7f-290">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-290">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="b4e7f-291">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="b4e7f-291">wiFiBlocked</span></span>|<span data-ttu-id="b4e7f-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-292">Boolean</span></span>|<span data-ttu-id="b4e7f-293">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-293">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="b4e7f-294">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="b4e7f-294">appsInstallAllowList</span></span>|<span data-ttu-id="b4e7f-295">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-295">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b4e7f-296">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-296">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="b4e7f-297">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-297">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b4e7f-298">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="b4e7f-298">appsLaunchBlockList</span></span>|<span data-ttu-id="b4e7f-299">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-299">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b4e7f-300">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-300">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="b4e7f-301">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-301">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b4e7f-302">appsHideList</span><span class="sxs-lookup"><span data-stu-id="b4e7f-302">appsHideList</span></span>|<span data-ttu-id="b4e7f-303">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4e7f-303">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="b4e7f-304">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-304">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="b4e7f-305">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-305">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b4e7f-306">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b4e7f-306">securityRequireVerifyApps</span></span>|<span data-ttu-id="b4e7f-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e7f-307">Boolean</span></span>|<span data-ttu-id="b4e7f-308">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-308">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="b4e7f-309">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4e7f-309">Response</span></span>
<span data-ttu-id="b4e7f-310">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-310">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4e7f-311">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4e7f-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4e7f-312">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4e7f-312">Request</span></span>
<span data-ttu-id="b4e7f-313">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-313">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3097

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="b4e7f-314">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4e7f-314">Response</span></span>
<span data-ttu-id="b4e7f-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4e7f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



