# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="314e2-101">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="314e2-101">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="314e2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="314e2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="314e2-103">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="314e2-103">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="314e2-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="314e2-104">Prerequisites</span></span>
<span data-ttu-id="314e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="314e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="314e2-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="314e2-107">Permission type</span></span>|<span data-ttu-id="314e2-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="314e2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="314e2-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="314e2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="314e2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="314e2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="314e2-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="314e2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="314e2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="314e2-112">Not supported.</span></span>|
|<span data-ttu-id="314e2-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="314e2-113">Application</span></span>|<span data-ttu-id="314e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="314e2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="314e2-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="314e2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="314e2-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="314e2-116">Request headers</span></span>
|<span data-ttu-id="314e2-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="314e2-117">Header</span></span>|<span data-ttu-id="314e2-118">Valor</span><span class="sxs-lookup"><span data-stu-id="314e2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="314e2-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="314e2-119">Authorization</span></span>|<span data-ttu-id="314e2-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="314e2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="314e2-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="314e2-121">Accept</span></span>|<span data-ttu-id="314e2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="314e2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="314e2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="314e2-123">Request body</span></span>
<span data-ttu-id="314e2-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="314e2-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="314e2-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="314e2-125">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="314e2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="314e2-126">Property</span></span>|<span data-ttu-id="314e2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="314e2-127">Type</span></span>|<span data-ttu-id="314e2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="314e2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="314e2-129">id</span><span class="sxs-lookup"><span data-stu-id="314e2-129">id</span></span>|<span data-ttu-id="314e2-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-130">String</span></span>|<span data-ttu-id="314e2-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="314e2-131">Key of the entity.</span></span> <span data-ttu-id="314e2-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="314e2-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="314e2-133">lastModifiedDateTime</span></span>|<span data-ttu-id="314e2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="314e2-134">DateTimeOffset</span></span>|<span data-ttu-id="314e2-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="314e2-135">DateTime the object was last modified.</span></span> <span data-ttu-id="314e2-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="314e2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="314e2-137">createdDateTime</span></span>|<span data-ttu-id="314e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="314e2-138">DateTimeOffset</span></span>|<span data-ttu-id="314e2-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="314e2-139">DateTime the object was created.</span></span> <span data-ttu-id="314e2-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="314e2-141">descrição</span><span class="sxs-lookup"><span data-stu-id="314e2-141">description</span></span>|<span data-ttu-id="314e2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-142">String</span></span>|<span data-ttu-id="314e2-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="314e2-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="314e2-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="314e2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="314e2-145">displayName</span></span>|<span data-ttu-id="314e2-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-146">String</span></span>|<span data-ttu-id="314e2-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="314e2-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="314e2-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="314e2-149">version</span><span class="sxs-lookup"><span data-stu-id="314e2-149">version</span></span>|<span data-ttu-id="314e2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="314e2-150">Int32</span></span>|<span data-ttu-id="314e2-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="314e2-151">Version of the device configuration.</span></span> <span data-ttu-id="314e2-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="314e2-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="314e2-153">accountBlockModification</span></span>|<span data-ttu-id="314e2-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-154">Boolean</span></span>|<span data-ttu-id="314e2-155">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="314e2-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="314e2-157">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-157">Boolean</span></span>|<span data-ttu-id="314e2-158">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="314e2-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-159">airDropBlocked</span></span>|<span data-ttu-id="314e2-160">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-160">Boolean</span></span>|<span data-ttu-id="314e2-161">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="314e2-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="314e2-163">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-163">Boolean</span></span>|<span data-ttu-id="314e2-164">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="314e2-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="314e2-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="314e2-166">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-166">Boolean</span></span>|<span data-ttu-id="314e2-167">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="314e2-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="314e2-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="314e2-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="314e2-169">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-169">Boolean</span></span>|<span data-ttu-id="314e2-170">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="314e2-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="314e2-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="314e2-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-172">Boolean</span></span>|<span data-ttu-id="314e2-173">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="314e2-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-174">appleNewsBlocked</span></span>|<span data-ttu-id="314e2-175">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-175">Boolean</span></span>|<span data-ttu-id="314e2-176">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="314e2-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="314e2-177">appsSingleAppModeList</span></span>|<span data-ttu-id="314e2-178">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="314e2-179">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="314e2-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="314e2-180">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-180">Supervised only.</span></span> <span data-ttu-id="314e2-181">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="314e2-181">iOS 7.0 and later.</span></span> <span data-ttu-id="314e2-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="314e2-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="314e2-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="314e2-183">appsVisibilityList</span></span>|<span data-ttu-id="314e2-184">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="314e2-185">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="314e2-186">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="314e2-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="314e2-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="314e2-187">appsVisibilityListType</span></span>|[<span data-ttu-id="314e2-188">appListType</span><span class="sxs-lookup"><span data-stu-id="314e2-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="314e2-189">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="314e2-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="314e2-190">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="314e2-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="314e2-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="314e2-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="314e2-192">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-192">Boolean</span></span>|<span data-ttu-id="314e2-193">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="314e2-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-194">appStoreBlocked</span></span>|<span data-ttu-id="314e2-195">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-195">Boolean</span></span>|<span data-ttu-id="314e2-196">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="314e2-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="314e2-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="314e2-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="314e2-198">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-198">Boolean</span></span>|<span data-ttu-id="314e2-199">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="314e2-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="314e2-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="314e2-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="314e2-201">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-201">Boolean</span></span>|<span data-ttu-id="314e2-202">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="314e2-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="314e2-203">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="314e2-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="314e2-204">appStoreRequirePassword</span></span>|<span data-ttu-id="314e2-205">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-205">Boolean</span></span>|<span data-ttu-id="314e2-206">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="314e2-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="314e2-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="314e2-207">bluetoothBlockModification</span></span>|<span data-ttu-id="314e2-208">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-208">Boolean</span></span>|<span data-ttu-id="314e2-209">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="314e2-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-210">cameraBlocked</span></span>|<span data-ttu-id="314e2-211">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-211">Boolean</span></span>|<span data-ttu-id="314e2-212">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="314e2-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="314e2-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="314e2-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="314e2-214">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-214">Boolean</span></span>|<span data-ttu-id="314e2-215">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="314e2-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="314e2-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="314e2-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="314e2-217">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-217">Boolean</span></span>|<span data-ttu-id="314e2-218">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="314e2-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="314e2-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="314e2-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="314e2-220">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-220">Boolean</span></span>|<span data-ttu-id="314e2-221">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="314e2-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="314e2-223">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-223">Boolean</span></span>|<span data-ttu-id="314e2-224">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="314e2-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="314e2-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="314e2-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="314e2-226">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-226">Boolean</span></span>|<span data-ttu-id="314e2-227">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="314e2-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="314e2-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="314e2-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="314e2-229">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-229">Boolean</span></span>|<span data-ttu-id="314e2-230">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="314e2-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="314e2-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="314e2-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="314e2-232">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-232">Boolean</span></span>|<span data-ttu-id="314e2-233">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="314e2-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="314e2-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="314e2-235">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-235">Boolean</span></span>|<span data-ttu-id="314e2-236">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="314e2-237">compliantAppsList</span></span>|<span data-ttu-id="314e2-238">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="314e2-239">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="314e2-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="314e2-240">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="314e2-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="314e2-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="314e2-241">compliantAppListType</span></span>|[<span data-ttu-id="314e2-242">appListType</span><span class="sxs-lookup"><span data-stu-id="314e2-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="314e2-243">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="314e2-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="314e2-244">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="314e2-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="314e2-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="314e2-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="314e2-246">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-246">Boolean</span></span>|<span data-ttu-id="314e2-247">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-248">definitionLookupBlocked</span></span>|<span data-ttu-id="314e2-249">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-249">Boolean</span></span>|<span data-ttu-id="314e2-250">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="314e2-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="314e2-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="314e2-252">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-252">Boolean</span></span>|<span data-ttu-id="314e2-253">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="314e2-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="314e2-255">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-255">Boolean</span></span>|<span data-ttu-id="314e2-256">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="314e2-257">deviceBlockNameModification</span></span>|<span data-ttu-id="314e2-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-258">Boolean</span></span>|<span data-ttu-id="314e2-259">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="314e2-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="314e2-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="314e2-261">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-261">Boolean</span></span>|<span data-ttu-id="314e2-262">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="314e2-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="314e2-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="314e2-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="314e2-264">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-264">Boolean</span></span>|<span data-ttu-id="314e2-265">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="314e2-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="314e2-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="314e2-267">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-267">Boolean</span></span>|<span data-ttu-id="314e2-268">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="314e2-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="314e2-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="314e2-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="314e2-270">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-270">Boolean</span></span>|<span data-ttu-id="314e2-271">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="314e2-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="314e2-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="314e2-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="314e2-273">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-273">String collection</span></span>|<span data-ttu-id="314e2-274">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="314e2-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="314e2-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="314e2-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="314e2-276">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-276">Boolean</span></span>|<span data-ttu-id="314e2-277">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="314e2-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="314e2-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="314e2-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="314e2-279">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-279">Boolean</span></span>|<span data-ttu-id="314e2-280">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="314e2-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="314e2-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-281">faceTimeBlocked</span></span>|<span data-ttu-id="314e2-282">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-282">Boolean</span></span>|<span data-ttu-id="314e2-283">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="314e2-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="314e2-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="314e2-285">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-285">Boolean</span></span>|<span data-ttu-id="314e2-286">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="314e2-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="314e2-288">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-288">Boolean</span></span>|<span data-ttu-id="314e2-289">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="314e2-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="314e2-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="314e2-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="314e2-291">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-291">Boolean</span></span>|<span data-ttu-id="314e2-292">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="314e2-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="314e2-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-293">gameCenterBlocked</span></span>|<span data-ttu-id="314e2-294">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-294">Boolean</span></span>|<span data-ttu-id="314e2-295">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-296">hostPairingBlocked</span></span>|<span data-ttu-id="314e2-297">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-297">Boolean</span></span>|<span data-ttu-id="314e2-298">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="314e2-300">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-300">Boolean</span></span>|<span data-ttu-id="314e2-301">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="314e2-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="314e2-303">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-303">Boolean</span></span>|<span data-ttu-id="314e2-304">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="314e2-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="314e2-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="314e2-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="314e2-306">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-306">Boolean</span></span>|<span data-ttu-id="314e2-307">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="314e2-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="314e2-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="314e2-308">iCloudBlockBackup</span></span>|<span data-ttu-id="314e2-309">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-309">Boolean</span></span>|<span data-ttu-id="314e2-310">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="314e2-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="314e2-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="314e2-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="314e2-312">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-312">Boolean</span></span>|<span data-ttu-id="314e2-313">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="314e2-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="314e2-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="314e2-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="314e2-315">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-315">Boolean</span></span>|<span data-ttu-id="314e2-316">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="314e2-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="314e2-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="314e2-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="314e2-318">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-318">Boolean</span></span>|<span data-ttu-id="314e2-319">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="314e2-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="314e2-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="314e2-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="314e2-321">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-321">Boolean</span></span>|<span data-ttu-id="314e2-322">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="314e2-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="314e2-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="314e2-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="314e2-324">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-324">Boolean</span></span>|<span data-ttu-id="314e2-325">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="314e2-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="314e2-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="314e2-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="314e2-327">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-327">Boolean</span></span>|<span data-ttu-id="314e2-328">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="314e2-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="314e2-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="314e2-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="314e2-330">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-330">Boolean</span></span>|<span data-ttu-id="314e2-331">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="314e2-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="314e2-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="314e2-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="314e2-333">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-333">Boolean</span></span>|<span data-ttu-id="314e2-334">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="314e2-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="314e2-335">iTunesBlockRadio</span></span>|<span data-ttu-id="314e2-336">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-336">Boolean</span></span>|<span data-ttu-id="314e2-337">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="314e2-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="314e2-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="314e2-339">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-339">Boolean</span></span>|<span data-ttu-id="314e2-340">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="314e2-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="314e2-341">keyboardBlockDictation</span></span>|<span data-ttu-id="314e2-342">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-342">Boolean</span></span>|<span data-ttu-id="314e2-343">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="314e2-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="314e2-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="314e2-345">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-345">Boolean</span></span>|<span data-ttu-id="314e2-346">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="314e2-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="314e2-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="314e2-348">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-348">Boolean</span></span>|<span data-ttu-id="314e2-349">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="314e2-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="314e2-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="314e2-351">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-351">Boolean</span></span>|<span data-ttu-id="314e2-352">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="314e2-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="314e2-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="314e2-354">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-354">Boolean</span></span>|<span data-ttu-id="314e2-355">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="314e2-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="314e2-357">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-357">Boolean</span></span>|<span data-ttu-id="314e2-358">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="314e2-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="314e2-360">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-360">Boolean</span></span>|<span data-ttu-id="314e2-361">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="314e2-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="314e2-363">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-363">Boolean</span></span>|<span data-ttu-id="314e2-364">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="314e2-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="314e2-366">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-366">Boolean</span></span>|<span data-ttu-id="314e2-367">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="314e2-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="314e2-369">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-369">Boolean</span></span>|<span data-ttu-id="314e2-370">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="314e2-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="314e2-372">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-372">Boolean</span></span>|<span data-ttu-id="314e2-373">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="314e2-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="314e2-375">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-375">Boolean</span></span>|<span data-ttu-id="314e2-376">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="314e2-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="314e2-378">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-378">Boolean</span></span>|<span data-ttu-id="314e2-379">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="314e2-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="314e2-381">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-381">Boolean</span></span>|<span data-ttu-id="314e2-382">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="314e2-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="314e2-384">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-384">Boolean</span></span>|<span data-ttu-id="314e2-385">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="314e2-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="314e2-387">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-387">String</span></span>|<span data-ttu-id="314e2-388">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="314e2-389">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="314e2-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="314e2-390">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="314e2-390">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="314e2-391">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-391">String</span></span>|<span data-ttu-id="314e2-392">ID para aplicativos internos a ser usado para o modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-392">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="314e2-393">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidas.</span><span class="sxs-lookup"><span data-stu-id="314e2-393">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="314e2-394">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="314e2-394">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="314e2-395">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-395">Boolean</span></span>|<span data-ttu-id="314e2-396">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-396">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-397">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="314e2-397">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="314e2-398">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-398">Boolean</span></span>|<span data-ttu-id="314e2-399">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-399">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-400">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="314e2-400">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="314e2-401">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-401">Boolean</span></span>|<span data-ttu-id="314e2-402">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-402">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-403">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="314e2-403">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="314e2-404">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-404">Boolean</span></span>|<span data-ttu-id="314e2-405">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-405">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-406">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="314e2-406">kioskModeRequireZoom</span></span>|<span data-ttu-id="314e2-407">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-407">Boolean</span></span>|<span data-ttu-id="314e2-408">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-408">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="314e2-409">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="314e2-409">kioskModeManagedAppId</span></span>|<span data-ttu-id="314e2-410">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-410">String</span></span>|<span data-ttu-id="314e2-411">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="314e2-411">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="314e2-412">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="314e2-412">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="314e2-413">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="314e2-413">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="314e2-414">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-414">Boolean</span></span>|<span data-ttu-id="314e2-415">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="314e2-415">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="314e2-416">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="314e2-416">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="314e2-417">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-417">Boolean</span></span>|<span data-ttu-id="314e2-418">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="314e2-418">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="314e2-419">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="314e2-419">lockScreenBlockPassbook</span></span>|<span data-ttu-id="314e2-420">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-420">Boolean</span></span>|<span data-ttu-id="314e2-421">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="314e2-421">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="314e2-422">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="314e2-422">lockScreenBlockTodayView</span></span>|<span data-ttu-id="314e2-423">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-423">Boolean</span></span>|<span data-ttu-id="314e2-424">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="314e2-424">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="314e2-425">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="314e2-425">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="314e2-426">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="314e2-426">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="314e2-427">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="314e2-427">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="314e2-428">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="314e2-428">mediaContentRatingCanada</span></span>|[<span data-ttu-id="314e2-429">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="314e2-429">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="314e2-430">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="314e2-430">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="314e2-431">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="314e2-431">mediaContentRatingFrance</span></span>|[<span data-ttu-id="314e2-432">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="314e2-432">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="314e2-433">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="314e2-433">Media content rating settings for France</span></span>|
|<span data-ttu-id="314e2-434">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="314e2-434">mediaContentRatingGermany</span></span>|[<span data-ttu-id="314e2-435">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="314e2-435">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="314e2-436">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="314e2-436">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="314e2-437">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="314e2-437">mediaContentRatingIreland</span></span>|[<span data-ttu-id="314e2-438">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="314e2-438">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="314e2-439">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="314e2-439">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="314e2-440">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="314e2-440">mediaContentRatingJapan</span></span>|[<span data-ttu-id="314e2-441">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="314e2-441">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="314e2-442">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="314e2-442">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="314e2-443">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="314e2-443">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="314e2-444">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="314e2-444">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="314e2-445">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="314e2-445">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="314e2-446">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="314e2-446">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="314e2-447">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="314e2-447">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="314e2-448">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="314e2-448">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="314e2-449">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="314e2-449">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="314e2-450">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="314e2-450">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="314e2-451">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="314e2-451">Media content rating settings for United States</span></span>|
|<span data-ttu-id="314e2-452">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="314e2-452">networkUsageRules</span></span>|<span data-ttu-id="314e2-453">Coleção [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="314e2-453">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="314e2-454">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="314e2-454">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="314e2-455">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="314e2-455">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="314e2-456">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="314e2-456">mediaContentRatingApps</span></span>|[<span data-ttu-id="314e2-457">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="314e2-457">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="314e2-458">As configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="314e2-458">Media content rating settings for Canada</span></span> <span data-ttu-id="314e2-459">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="314e2-459">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="314e2-460">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-460">messagesBlocked</span></span>|<span data-ttu-id="314e2-461">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-461">Boolean</span></span>|<span data-ttu-id="314e2-462">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-462">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="314e2-463">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="314e2-463">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="314e2-464">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-464">Boolean</span></span>|<span data-ttu-id="314e2-465">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-465">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="314e2-466">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="314e2-466">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="314e2-467">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-467">Boolean</span></span>|<span data-ttu-id="314e2-468">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="314e2-468">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="314e2-469">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="314e2-469">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="314e2-470">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-470">Boolean</span></span>|<span data-ttu-id="314e2-471">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-471">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="314e2-472">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="314e2-472">passcodeBlockModification</span></span>|<span data-ttu-id="314e2-473">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-473">Boolean</span></span>|<span data-ttu-id="314e2-474">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-474">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="314e2-475">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="314e2-475">passcodeBlockSimple</span></span>|<span data-ttu-id="314e2-476">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-476">Boolean</span></span>|<span data-ttu-id="314e2-477">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="314e2-477">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="314e2-478">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="314e2-478">passcodeExpirationDays</span></span>|<span data-ttu-id="314e2-479">Int32</span><span class="sxs-lookup"><span data-stu-id="314e2-479">Int32</span></span>|<span data-ttu-id="314e2-480">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="314e2-480">Number of days before the passcode expires.</span></span> <span data-ttu-id="314e2-481">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="314e2-481">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="314e2-482">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="314e2-482">passcodeMinimumLength</span></span>|<span data-ttu-id="314e2-483">Int32</span><span class="sxs-lookup"><span data-stu-id="314e2-483">Int32</span></span>|<span data-ttu-id="314e2-484">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="314e2-484">Minimum length of passcode.</span></span> <span data-ttu-id="314e2-485">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="314e2-485">Valid values 4 to 14</span></span>|
|<span data-ttu-id="314e2-486">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="314e2-486">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="314e2-487">Int32</span><span class="sxs-lookup"><span data-stu-id="314e2-487">Int32</span></span>|<span data-ttu-id="314e2-488">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="314e2-488">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="314e2-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="314e2-489">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="314e2-490">Int32</span><span class="sxs-lookup"><span data-stu-id="314e2-490">Int32</span></span>|<span data-ttu-id="314e2-491">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="314e2-491">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="314e2-492">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="314e2-492">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="314e2-493">Int32</span><span class="sxs-lookup"><span data-stu-id="314e2-493">Int32</span></span>|<span data-ttu-id="314e2-494">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="314e2-494">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="314e2-495">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="314e2-495">Valid values 0 to 4</span></span>|
|<span data-ttu-id="314e2-496">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="314e2-496">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="314e2-497">Int32</span><span class="sxs-lookup"><span data-stu-id="314e2-497">Int32</span></span>|<span data-ttu-id="314e2-498">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="314e2-498">Number of previous passcodes to block.</span></span> <span data-ttu-id="314e2-499">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="314e2-499">Valid values 1 to 24</span></span>|
|<span data-ttu-id="314e2-500">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="314e2-500">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="314e2-501">Int32</span><span class="sxs-lookup"><span data-stu-id="314e2-501">Int32</span></span>|<span data-ttu-id="314e2-502">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="314e2-502">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="314e2-503">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="314e2-503">Valid values 4 to 11</span></span>|
|<span data-ttu-id="314e2-504">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="314e2-504">passcodeRequiredType</span></span>|[<span data-ttu-id="314e2-505">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="314e2-505">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="314e2-506">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="314e2-506">Type of passcode that is required.</span></span> <span data-ttu-id="314e2-507">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="314e2-507">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="314e2-508">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="314e2-508">passcodeRequired</span></span>|<span data-ttu-id="314e2-509">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-509">Boolean</span></span>|<span data-ttu-id="314e2-510">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="314e2-510">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="314e2-511">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-511">podcastsBlocked</span></span>|<span data-ttu-id="314e2-512">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-512">Boolean</span></span>|<span data-ttu-id="314e2-513">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-513">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="314e2-514">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="314e2-514">safariBlockAutofill</span></span>|<span data-ttu-id="314e2-515">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-515">Boolean</span></span>|<span data-ttu-id="314e2-516">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="314e2-516">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="314e2-517">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="314e2-517">safariBlockJavaScript</span></span>|<span data-ttu-id="314e2-518">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-518">Boolean</span></span>|<span data-ttu-id="314e2-519">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="314e2-519">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="314e2-520">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="314e2-520">safariBlockPopups</span></span>|<span data-ttu-id="314e2-521">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-521">Boolean</span></span>|<span data-ttu-id="314e2-522">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="314e2-522">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="314e2-523">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-523">safariBlocked</span></span>|<span data-ttu-id="314e2-524">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-524">Boolean</span></span>|<span data-ttu-id="314e2-525">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="314e2-525">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="314e2-526">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="314e2-526">safariCookieSettings</span></span>|[<span data-ttu-id="314e2-527">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="314e2-527">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="314e2-528">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="314e2-528">Cookie settings for Safari.</span></span> <span data-ttu-id="314e2-529">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="314e2-529">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="314e2-530">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="314e2-530">safariManagedDomains</span></span>|<span data-ttu-id="314e2-531">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-531">String collection</span></span>|<span data-ttu-id="314e2-532">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="314e2-532">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="314e2-533">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="314e2-533">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="314e2-534">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="314e2-534">String collection</span></span>|<span data-ttu-id="314e2-535">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="314e2-535">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="314e2-536">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-536">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="314e2-537">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="314e2-537">safariRequireFraudWarning</span></span>|<span data-ttu-id="314e2-538">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-538">Boolean</span></span>|<span data-ttu-id="314e2-539">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="314e2-539">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="314e2-540">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-540">screenCaptureBlocked</span></span>|<span data-ttu-id="314e2-541">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-541">Boolean</span></span>|<span data-ttu-id="314e2-542">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="314e2-542">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="314e2-543">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-543">siriBlocked</span></span>|<span data-ttu-id="314e2-544">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-544">Boolean</span></span>|<span data-ttu-id="314e2-545">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="314e2-545">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="314e2-546">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="314e2-546">siriBlockedWhenLocked</span></span>|<span data-ttu-id="314e2-547">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-547">Boolean</span></span>|<span data-ttu-id="314e2-548">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="314e2-548">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="314e2-549">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="314e2-549">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="314e2-550">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-550">Boolean</span></span>|<span data-ttu-id="314e2-551">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-551">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="314e2-552">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="314e2-552">siriRequireProfanityFilter</span></span>|<span data-ttu-id="314e2-553">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-553">Boolean</span></span>|<span data-ttu-id="314e2-554">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-554">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="314e2-555">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="314e2-555">spotlightBlockInternetResults</span></span>|<span data-ttu-id="314e2-556">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-556">Boolean</span></span>|<span data-ttu-id="314e2-557">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-557">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="314e2-558">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="314e2-558">voiceDialingBlocked</span></span>|<span data-ttu-id="314e2-559">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-559">Boolean</span></span>|<span data-ttu-id="314e2-560">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="314e2-560">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="314e2-561">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="314e2-561">wallpaperBlockModification</span></span>|<span data-ttu-id="314e2-562">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-562">Boolean</span></span>|<span data-ttu-id="314e2-563">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="314e2-563">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="314e2-564">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="314e2-564">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="314e2-565">Booleano</span><span class="sxs-lookup"><span data-stu-id="314e2-565">Boolean</span></span>|<span data-ttu-id="314e2-566">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="314e2-566">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="314e2-567">Resposta</span><span class="sxs-lookup"><span data-stu-id="314e2-567">Response</span></span>
<span data-ttu-id="314e2-568">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="314e2-568">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="314e2-569">Exemplo</span><span class="sxs-lookup"><span data-stu-id="314e2-569">Example</span></span>
### <a name="request"></a><span data-ttu-id="314e2-570">Solicitação</span><span class="sxs-lookup"><span data-stu-id="314e2-570">Request</span></span>
<span data-ttu-id="314e2-571">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="314e2-571">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7837

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="314e2-572">Resposta</span><span class="sxs-lookup"><span data-stu-id="314e2-572">Response</span></span>
<span data-ttu-id="314e2-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="314e2-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








