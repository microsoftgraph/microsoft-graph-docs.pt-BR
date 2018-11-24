# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="7caba-101">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7caba-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="7caba-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7caba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7caba-103">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7caba-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7caba-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7caba-104">Prerequisites</span></span>
<span data-ttu-id="7caba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7caba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7caba-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7caba-107">Permission type</span></span>|<span data-ttu-id="7caba-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7caba-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7caba-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7caba-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7caba-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7caba-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7caba-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7caba-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7caba-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7caba-112">Not supported.</span></span>|
|<span data-ttu-id="7caba-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7caba-113">Application</span></span>|<span data-ttu-id="7caba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7caba-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7caba-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7caba-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7caba-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7caba-116">Request headers</span></span>
|<span data-ttu-id="7caba-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7caba-117">Header</span></span>|<span data-ttu-id="7caba-118">Valor</span><span class="sxs-lookup"><span data-stu-id="7caba-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7caba-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="7caba-119">Authorization</span></span>|<span data-ttu-id="7caba-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7caba-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7caba-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7caba-121">Accept</span></span>|<span data-ttu-id="7caba-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7caba-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7caba-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7caba-123">Request body</span></span>
<span data-ttu-id="7caba-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7caba-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="7caba-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7caba-125">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="7caba-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7caba-126">Property</span></span>|<span data-ttu-id="7caba-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7caba-127">Type</span></span>|<span data-ttu-id="7caba-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7caba-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7caba-129">id</span><span class="sxs-lookup"><span data-stu-id="7caba-129">id</span></span>|<span data-ttu-id="7caba-130">String</span><span class="sxs-lookup"><span data-stu-id="7caba-130">String</span></span>|<span data-ttu-id="7caba-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7caba-131">Key of the entity.</span></span> <span data-ttu-id="7caba-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7caba-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7caba-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7caba-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7caba-134">DateTimeOffset</span></span>|<span data-ttu-id="7caba-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7caba-135">DateTime the object was last modified.</span></span> <span data-ttu-id="7caba-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7caba-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7caba-137">createdDateTime</span></span>|<span data-ttu-id="7caba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7caba-138">DateTimeOffset</span></span>|<span data-ttu-id="7caba-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7caba-139">DateTime the object was created.</span></span> <span data-ttu-id="7caba-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7caba-141">descrição</span><span class="sxs-lookup"><span data-stu-id="7caba-141">description</span></span>|<span data-ttu-id="7caba-142">String</span><span class="sxs-lookup"><span data-stu-id="7caba-142">String</span></span>|<span data-ttu-id="7caba-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7caba-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7caba-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7caba-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7caba-145">displayName</span></span>|<span data-ttu-id="7caba-146">String</span><span class="sxs-lookup"><span data-stu-id="7caba-146">String</span></span>|<span data-ttu-id="7caba-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7caba-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7caba-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7caba-149">version</span><span class="sxs-lookup"><span data-stu-id="7caba-149">version</span></span>|<span data-ttu-id="7caba-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7caba-150">Int32</span></span>|<span data-ttu-id="7caba-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7caba-151">Version of the device configuration.</span></span> <span data-ttu-id="7caba-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7caba-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="7caba-153">accountBlockModification</span></span>|<span data-ttu-id="7caba-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-154">Boolean</span></span>|<span data-ttu-id="7caba-155">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="7caba-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="7caba-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-157">Boolean</span></span>|<span data-ttu-id="7caba-158">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="7caba-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-159">airDropBlocked</span></span>|<span data-ttu-id="7caba-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-160">Boolean</span></span>|<span data-ttu-id="7caba-161">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="7caba-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="7caba-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-163">Boolean</span></span>|<span data-ttu-id="7caba-164">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7caba-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="7caba-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="7caba-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-166">Boolean</span></span>|<span data-ttu-id="7caba-167">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="7caba-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="7caba-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="7caba-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="7caba-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-169">Boolean</span></span>|<span data-ttu-id="7caba-170">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7caba-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="7caba-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="7caba-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-172">Boolean</span></span>|<span data-ttu-id="7caba-173">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="7caba-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-174">appleNewsBlocked</span></span>|<span data-ttu-id="7caba-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-175">Boolean</span></span>|<span data-ttu-id="7caba-176">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7caba-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="7caba-177">appsSingleAppModeList</span></span>|<span data-ttu-id="7caba-178">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="7caba-179">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="7caba-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="7caba-180">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-180">Supervised only.</span></span> <span data-ttu-id="7caba-181">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7caba-181">iOS 7.0 and later.</span></span> <span data-ttu-id="7caba-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7caba-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7caba-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="7caba-183">appsVisibilityList</span></span>|<span data-ttu-id="7caba-184">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="7caba-185">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="7caba-186">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="7caba-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7caba-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="7caba-187">appsVisibilityListType</span></span>|[<span data-ttu-id="7caba-188">appListType</span><span class="sxs-lookup"><span data-stu-id="7caba-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="7caba-189">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="7caba-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="7caba-190">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="7caba-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="7caba-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="7caba-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="7caba-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-192">Boolean</span></span>|<span data-ttu-id="7caba-193">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7caba-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-194">appStoreBlocked</span></span>|<span data-ttu-id="7caba-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-195">Boolean</span></span>|<span data-ttu-id="7caba-196">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="7caba-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="7caba-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="7caba-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="7caba-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-198">Boolean</span></span>|<span data-ttu-id="7caba-199">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7caba-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="7caba-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7caba-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="7caba-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-201">Boolean</span></span>|<span data-ttu-id="7caba-202">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="7caba-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="7caba-203">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7caba-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="7caba-204">appStoreRequirePassword</span></span>|<span data-ttu-id="7caba-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-205">Boolean</span></span>|<span data-ttu-id="7caba-206">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7caba-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="7caba-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="7caba-207">bluetoothBlockModification</span></span>|<span data-ttu-id="7caba-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-208">Boolean</span></span>|<span data-ttu-id="7caba-209">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="7caba-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-210">cameraBlocked</span></span>|<span data-ttu-id="7caba-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-211">Boolean</span></span>|<span data-ttu-id="7caba-212">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7caba-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="7caba-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="7caba-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="7caba-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-214">Boolean</span></span>|<span data-ttu-id="7caba-215">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7caba-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="7caba-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="7caba-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="7caba-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-217">Boolean</span></span>|<span data-ttu-id="7caba-218">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="7caba-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="7caba-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="7caba-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="7caba-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-220">Boolean</span></span>|<span data-ttu-id="7caba-221">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="7caba-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="7caba-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-223">Boolean</span></span>|<span data-ttu-id="7caba-224">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7caba-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="7caba-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="7caba-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="7caba-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-226">Boolean</span></span>|<span data-ttu-id="7caba-227">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7caba-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="7caba-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="7caba-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="7caba-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-229">Boolean</span></span>|<span data-ttu-id="7caba-230">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="7caba-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="7caba-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="7caba-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="7caba-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-232">Boolean</span></span>|<span data-ttu-id="7caba-233">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="7caba-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="7caba-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="7caba-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-235">Boolean</span></span>|<span data-ttu-id="7caba-236">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="7caba-237">compliantAppsList</span></span>|<span data-ttu-id="7caba-238">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="7caba-239">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="7caba-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="7caba-240">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="7caba-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7caba-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="7caba-241">compliantAppListType</span></span>|[<span data-ttu-id="7caba-242">appListType</span><span class="sxs-lookup"><span data-stu-id="7caba-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="7caba-243">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="7caba-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="7caba-244">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="7caba-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="7caba-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="7caba-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="7caba-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-246">Boolean</span></span>|<span data-ttu-id="7caba-247">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-248">definitionLookupBlocked</span></span>|<span data-ttu-id="7caba-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-249">Boolean</span></span>|<span data-ttu-id="7caba-250">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="7caba-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="7caba-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="7caba-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-252">Boolean</span></span>|<span data-ttu-id="7caba-253">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="7caba-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="7caba-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-255">Boolean</span></span>|<span data-ttu-id="7caba-256">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="7caba-257">deviceBlockNameModification</span></span>|<span data-ttu-id="7caba-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-258">Boolean</span></span>|<span data-ttu-id="7caba-259">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7caba-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="7caba-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="7caba-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-261">Boolean</span></span>|<span data-ttu-id="7caba-262">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7caba-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="7caba-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="7caba-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="7caba-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-264">Boolean</span></span>|<span data-ttu-id="7caba-265">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="7caba-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="7caba-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="7caba-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-267">Boolean</span></span>|<span data-ttu-id="7caba-268">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="7caba-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="7caba-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="7caba-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="7caba-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-270">Boolean</span></span>|<span data-ttu-id="7caba-271">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="7caba-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="7caba-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="7caba-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="7caba-273">String collection</span><span class="sxs-lookup"><span data-stu-id="7caba-273">String collection</span></span>|<span data-ttu-id="7caba-274">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="7caba-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="7caba-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="7caba-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="7caba-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-276">Boolean</span></span>|<span data-ttu-id="7caba-277">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="7caba-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="7caba-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="7caba-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="7caba-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-279">Boolean</span></span>|<span data-ttu-id="7caba-280">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="7caba-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="7caba-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-281">faceTimeBlocked</span></span>|<span data-ttu-id="7caba-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-282">Boolean</span></span>|<span data-ttu-id="7caba-283">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="7caba-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="7caba-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="7caba-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-285">Boolean</span></span>|<span data-ttu-id="7caba-286">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="7caba-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="7caba-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-288">Boolean</span></span>|<span data-ttu-id="7caba-289">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="7caba-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="7caba-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="7caba-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="7caba-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-291">Boolean</span></span>|<span data-ttu-id="7caba-292">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="7caba-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="7caba-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-293">gameCenterBlocked</span></span>|<span data-ttu-id="7caba-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-294">Boolean</span></span>|<span data-ttu-id="7caba-295">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-296">hostPairingBlocked</span></span>|<span data-ttu-id="7caba-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-297">Boolean</span></span>|<span data-ttu-id="7caba-298">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="7caba-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-300">Boolean</span></span>|<span data-ttu-id="7caba-301">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="7caba-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="7caba-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-303">Boolean</span></span>|<span data-ttu-id="7caba-304">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="7caba-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="7caba-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="7caba-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="7caba-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-306">Boolean</span></span>|<span data-ttu-id="7caba-307">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="7caba-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="7caba-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="7caba-308">iCloudBlockBackup</span></span>|<span data-ttu-id="7caba-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-309">Boolean</span></span>|<span data-ttu-id="7caba-310">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7caba-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="7caba-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="7caba-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="7caba-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-312">Boolean</span></span>|<span data-ttu-id="7caba-313">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7caba-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="7caba-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="7caba-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="7caba-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-315">Boolean</span></span>|<span data-ttu-id="7caba-316">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7caba-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="7caba-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="7caba-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="7caba-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-318">Boolean</span></span>|<span data-ttu-id="7caba-319">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7caba-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="7caba-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="7caba-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="7caba-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-321">Boolean</span></span>|<span data-ttu-id="7caba-322">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7caba-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="7caba-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="7caba-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="7caba-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-324">Boolean</span></span>|<span data-ttu-id="7caba-325">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7caba-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="7caba-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="7caba-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="7caba-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-327">Boolean</span></span>|<span data-ttu-id="7caba-328">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="7caba-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="7caba-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="7caba-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="7caba-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-330">Boolean</span></span>|<span data-ttu-id="7caba-331">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="7caba-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="7caba-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="7caba-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="7caba-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-333">Boolean</span></span>|<span data-ttu-id="7caba-334">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="7caba-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="7caba-335">iTunesBlockRadio</span></span>|<span data-ttu-id="7caba-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-336">Boolean</span></span>|<span data-ttu-id="7caba-337">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="7caba-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="7caba-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="7caba-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-339">Boolean</span></span>|<span data-ttu-id="7caba-340">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="7caba-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="7caba-341">keyboardBlockDictation</span></span>|<span data-ttu-id="7caba-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-342">Boolean</span></span>|<span data-ttu-id="7caba-343">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7caba-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="7caba-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="7caba-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-345">Boolean</span></span>|<span data-ttu-id="7caba-346">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="7caba-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="7caba-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="7caba-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-348">Boolean</span></span>|<span data-ttu-id="7caba-349">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7caba-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="7caba-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="7caba-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-351">Boolean</span></span>|<span data-ttu-id="7caba-352">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="7caba-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="7caba-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="7caba-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-354">Boolean</span></span>|<span data-ttu-id="7caba-355">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="7caba-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="7caba-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-357">Boolean</span></span>|<span data-ttu-id="7caba-358">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="7caba-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="7caba-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-360">Boolean</span></span>|<span data-ttu-id="7caba-361">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="7caba-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="7caba-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-363">Boolean</span></span>|<span data-ttu-id="7caba-364">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="7caba-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="7caba-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-366">Boolean</span></span>|<span data-ttu-id="7caba-367">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="7caba-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="7caba-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-369">Boolean</span></span>|<span data-ttu-id="7caba-370">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="7caba-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="7caba-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-372">Boolean</span></span>|<span data-ttu-id="7caba-373">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="7caba-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="7caba-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-375">Boolean</span></span>|<span data-ttu-id="7caba-376">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="7caba-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="7caba-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-378">Boolean</span></span>|<span data-ttu-id="7caba-379">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="7caba-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="7caba-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-381">Boolean</span></span>|<span data-ttu-id="7caba-382">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="7caba-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="7caba-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="7caba-384">Boolean</span></span>|<span data-ttu-id="7caba-385">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7caba-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="7caba-387">String</span><span class="sxs-lookup"><span data-stu-id="7caba-387">String</span></span>|<span data-ttu-id="7caba-388">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="7caba-389">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="7caba-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="7caba-390">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="7caba-390">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="7caba-391">String</span><span class="sxs-lookup"><span data-stu-id="7caba-391">String</span></span>|<span data-ttu-id="7caba-392">ID para aplicativos internos a ser usado para o modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-392">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="7caba-393">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidas.</span><span class="sxs-lookup"><span data-stu-id="7caba-393">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="7caba-394">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="7caba-394">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="7caba-395">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-395">Boolean</span></span>|<span data-ttu-id="7caba-396">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-396">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-397">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="7caba-397">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="7caba-398">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-398">Boolean</span></span>|<span data-ttu-id="7caba-399">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-399">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-400">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="7caba-400">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="7caba-401">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-401">Boolean</span></span>|<span data-ttu-id="7caba-402">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-402">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-403">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="7caba-403">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="7caba-404">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-404">Boolean</span></span>|<span data-ttu-id="7caba-405">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-405">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-406">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="7caba-406">kioskModeRequireZoom</span></span>|<span data-ttu-id="7caba-407">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-407">Boolean</span></span>|<span data-ttu-id="7caba-408">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-408">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="7caba-409">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="7caba-409">kioskModeManagedAppId</span></span>|<span data-ttu-id="7caba-410">String</span><span class="sxs-lookup"><span data-stu-id="7caba-410">String</span></span>|<span data-ttu-id="7caba-411">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7caba-411">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="7caba-412">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="7caba-412">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="7caba-413">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="7caba-413">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="7caba-414">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-414">Boolean</span></span>|<span data-ttu-id="7caba-415">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="7caba-415">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="7caba-416">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="7caba-416">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="7caba-417">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-417">Boolean</span></span>|<span data-ttu-id="7caba-418">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="7caba-418">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="7caba-419">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="7caba-419">lockScreenBlockPassbook</span></span>|<span data-ttu-id="7caba-420">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-420">Boolean</span></span>|<span data-ttu-id="7caba-421">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="7caba-421">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="7caba-422">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="7caba-422">lockScreenBlockTodayView</span></span>|<span data-ttu-id="7caba-423">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-423">Boolean</span></span>|<span data-ttu-id="7caba-424">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="7caba-424">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="7caba-425">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="7caba-425">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="7caba-426">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="7caba-426">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="7caba-427">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="7caba-427">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="7caba-428">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="7caba-428">mediaContentRatingCanada</span></span>|[<span data-ttu-id="7caba-429">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="7caba-429">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="7caba-430">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="7caba-430">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="7caba-431">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="7caba-431">mediaContentRatingFrance</span></span>|[<span data-ttu-id="7caba-432">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="7caba-432">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="7caba-433">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="7caba-433">Media content rating settings for France</span></span>|
|<span data-ttu-id="7caba-434">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="7caba-434">mediaContentRatingGermany</span></span>|[<span data-ttu-id="7caba-435">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="7caba-435">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="7caba-436">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="7caba-436">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="7caba-437">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="7caba-437">mediaContentRatingIreland</span></span>|[<span data-ttu-id="7caba-438">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="7caba-438">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="7caba-439">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="7caba-439">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="7caba-440">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="7caba-440">mediaContentRatingJapan</span></span>|[<span data-ttu-id="7caba-441">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="7caba-441">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="7caba-442">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="7caba-442">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="7caba-443">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="7caba-443">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="7caba-444">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="7caba-444">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="7caba-445">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="7caba-445">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="7caba-446">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="7caba-446">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="7caba-447">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="7caba-447">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="7caba-448">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="7caba-448">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="7caba-449">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="7caba-449">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="7caba-450">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="7caba-450">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="7caba-451">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="7caba-451">Media content rating settings for United States</span></span>|
|<span data-ttu-id="7caba-452">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="7caba-452">networkUsageRules</span></span>|<span data-ttu-id="7caba-453">Coleção [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="7caba-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="7caba-454">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="7caba-454">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="7caba-455">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="7caba-455">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="7caba-456">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="7caba-456">mediaContentRatingApps</span></span>|[<span data-ttu-id="7caba-457">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="7caba-457">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="7caba-458">As configurações de classificação para aplicativos de conteúdo de mídia.</span><span class="sxs-lookup"><span data-stu-id="7caba-458">Media content rating settings for Apps.</span></span> <span data-ttu-id="7caba-459">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="7caba-459">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="7caba-460">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-460">messagesBlocked</span></span>|<span data-ttu-id="7caba-461">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-461">Boolean</span></span>|<span data-ttu-id="7caba-462">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-462">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="7caba-463">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="7caba-463">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="7caba-464">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-464">Boolean</span></span>|<span data-ttu-id="7caba-465">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-465">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="7caba-466">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="7caba-466">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="7caba-467">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-467">Boolean</span></span>|<span data-ttu-id="7caba-468">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7caba-468">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="7caba-469">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="7caba-469">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="7caba-470">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-470">Boolean</span></span>|<span data-ttu-id="7caba-471">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-471">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="7caba-472">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="7caba-472">passcodeBlockModification</span></span>|<span data-ttu-id="7caba-473">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-473">Boolean</span></span>|<span data-ttu-id="7caba-474">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-474">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7caba-475">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7caba-475">passcodeBlockSimple</span></span>|<span data-ttu-id="7caba-476">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-476">Boolean</span></span>|<span data-ttu-id="7caba-477">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="7caba-477">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="7caba-478">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7caba-478">passcodeExpirationDays</span></span>|<span data-ttu-id="7caba-479">Int32</span><span class="sxs-lookup"><span data-stu-id="7caba-479">Int32</span></span>|<span data-ttu-id="7caba-480">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="7caba-480">Number of days before the passcode expires.</span></span> <span data-ttu-id="7caba-481">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="7caba-481">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="7caba-482">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7caba-482">passcodeMinimumLength</span></span>|<span data-ttu-id="7caba-483">Int32</span><span class="sxs-lookup"><span data-stu-id="7caba-483">Int32</span></span>|<span data-ttu-id="7caba-484">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="7caba-484">Minimum length of passcode.</span></span> <span data-ttu-id="7caba-485">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="7caba-485">Valid values 4 to 14</span></span>|
|<span data-ttu-id="7caba-486">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7caba-486">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7caba-487">Int32</span><span class="sxs-lookup"><span data-stu-id="7caba-487">Int32</span></span>|<span data-ttu-id="7caba-488">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="7caba-488">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="7caba-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7caba-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7caba-490">Int32</span><span class="sxs-lookup"><span data-stu-id="7caba-490">Int32</span></span>|<span data-ttu-id="7caba-491">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="7caba-491">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7caba-492">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7caba-492">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="7caba-493">Int32</span><span class="sxs-lookup"><span data-stu-id="7caba-493">Int32</span></span>|<span data-ttu-id="7caba-494">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="7caba-494">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="7caba-495">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="7caba-495">Valid values 0 to 4</span></span>|
|<span data-ttu-id="7caba-496">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="7caba-496">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="7caba-497">Int32</span><span class="sxs-lookup"><span data-stu-id="7caba-497">Int32</span></span>|<span data-ttu-id="7caba-498">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="7caba-498">Number of previous passcodes to block.</span></span> <span data-ttu-id="7caba-499">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="7caba-499">Valid values 1 to 24</span></span>|
|<span data-ttu-id="7caba-500">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="7caba-500">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="7caba-501">Int32</span><span class="sxs-lookup"><span data-stu-id="7caba-501">Int32</span></span>|<span data-ttu-id="7caba-502">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7caba-502">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="7caba-503">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="7caba-503">Valid values 4 to 11</span></span>|
|<span data-ttu-id="7caba-504">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="7caba-504">passcodeRequiredType</span></span>|[<span data-ttu-id="7caba-505">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7caba-505">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="7caba-506">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="7caba-506">Type of passcode that is required.</span></span> <span data-ttu-id="7caba-507">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7caba-507">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7caba-508">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="7caba-508">passcodeRequired</span></span>|<span data-ttu-id="7caba-509">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-509">Boolean</span></span>|<span data-ttu-id="7caba-510">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="7caba-510">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="7caba-511">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-511">podcastsBlocked</span></span>|<span data-ttu-id="7caba-512">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-512">Boolean</span></span>|<span data-ttu-id="7caba-513">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-513">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="7caba-514">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="7caba-514">safariBlockAutofill</span></span>|<span data-ttu-id="7caba-515">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-515">Boolean</span></span>|<span data-ttu-id="7caba-516">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="7caba-516">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="7caba-517">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="7caba-517">safariBlockJavaScript</span></span>|<span data-ttu-id="7caba-518">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-518">Boolean</span></span>|<span data-ttu-id="7caba-519">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="7caba-519">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="7caba-520">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="7caba-520">safariBlockPopups</span></span>|<span data-ttu-id="7caba-521">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-521">Boolean</span></span>|<span data-ttu-id="7caba-522">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="7caba-522">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="7caba-523">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-523">safariBlocked</span></span>|<span data-ttu-id="7caba-524">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-524">Boolean</span></span>|<span data-ttu-id="7caba-525">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="7caba-525">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="7caba-526">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="7caba-526">safariCookieSettings</span></span>|[<span data-ttu-id="7caba-527">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="7caba-527">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="7caba-528">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="7caba-528">Cookie settings for Safari.</span></span> <span data-ttu-id="7caba-529">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="7caba-529">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="7caba-530">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="7caba-530">safariManagedDomains</span></span>|<span data-ttu-id="7caba-531">String collection</span><span class="sxs-lookup"><span data-stu-id="7caba-531">String collection</span></span>|<span data-ttu-id="7caba-532">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="7caba-532">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="7caba-533">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="7caba-533">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="7caba-534">String collection</span><span class="sxs-lookup"><span data-stu-id="7caba-534">String collection</span></span>|<span data-ttu-id="7caba-535">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="7caba-535">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="7caba-536">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-536">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="7caba-537">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="7caba-537">safariRequireFraudWarning</span></span>|<span data-ttu-id="7caba-538">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-538">Boolean</span></span>|<span data-ttu-id="7caba-539">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="7caba-539">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="7caba-540">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-540">screenCaptureBlocked</span></span>|<span data-ttu-id="7caba-541">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-541">Boolean</span></span>|<span data-ttu-id="7caba-542">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="7caba-542">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="7caba-543">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-543">siriBlocked</span></span>|<span data-ttu-id="7caba-544">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-544">Boolean</span></span>|<span data-ttu-id="7caba-545">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="7caba-545">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="7caba-546">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="7caba-546">siriBlockedWhenLocked</span></span>|<span data-ttu-id="7caba-547">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-547">Boolean</span></span>|<span data-ttu-id="7caba-548">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7caba-548">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="7caba-549">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="7caba-549">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="7caba-550">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-550">Boolean</span></span>|<span data-ttu-id="7caba-551">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-551">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="7caba-552">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="7caba-552">siriRequireProfanityFilter</span></span>|<span data-ttu-id="7caba-553">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-553">Boolean</span></span>|<span data-ttu-id="7caba-554">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-554">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="7caba-555">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="7caba-555">spotlightBlockInternetResults</span></span>|<span data-ttu-id="7caba-556">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-556">Boolean</span></span>|<span data-ttu-id="7caba-557">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-557">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="7caba-558">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="7caba-558">voiceDialingBlocked</span></span>|<span data-ttu-id="7caba-559">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-559">Boolean</span></span>|<span data-ttu-id="7caba-560">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7caba-560">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="7caba-561">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="7caba-561">wallpaperBlockModification</span></span>|<span data-ttu-id="7caba-562">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-562">Boolean</span></span>|<span data-ttu-id="7caba-563">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7caba-563">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="7caba-564">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="7caba-564">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="7caba-565">Booliano</span><span class="sxs-lookup"><span data-stu-id="7caba-565">Boolean</span></span>|<span data-ttu-id="7caba-566">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7caba-566">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="7caba-567">Resposta</span><span class="sxs-lookup"><span data-stu-id="7caba-567">Response</span></span>
<span data-ttu-id="7caba-568">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7caba-568">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7caba-569">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7caba-569">Example</span></span>
### <a name="request"></a><span data-ttu-id="7caba-570">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7caba-570">Request</span></span>
<span data-ttu-id="7caba-571">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7caba-571">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="7caba-572">Resposta</span><span class="sxs-lookup"><span data-stu-id="7caba-572">Response</span></span>
<span data-ttu-id="7caba-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7caba-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```



