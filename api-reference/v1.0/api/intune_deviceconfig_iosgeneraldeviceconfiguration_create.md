# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="d6849-101">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6849-101">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="d6849-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d6849-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6849-103">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6849-103">Create a new [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6849-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6849-104">Prerequisites</span></span>
<span data-ttu-id="d6849-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d6849-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6849-107">Permission type</span></span>|<span data-ttu-id="d6849-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6849-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6849-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6849-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d6849-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6849-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6849-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6849-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6849-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6849-112">Not supported.</span></span>|
|<span data-ttu-id="d6849-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6849-113">Application</span></span>|<span data-ttu-id="d6849-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6849-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6849-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6849-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6849-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6849-116">Request headers</span></span>
|<span data-ttu-id="d6849-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6849-117">Header</span></span>|<span data-ttu-id="d6849-118">Valor</span><span class="sxs-lookup"><span data-stu-id="d6849-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6849-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6849-119">Authorization</span></span>|<span data-ttu-id="d6849-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="d6849-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6849-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6849-121">Accept</span></span>|<span data-ttu-id="d6849-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="d6849-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6849-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6849-123">Request body</span></span>
<span data-ttu-id="d6849-124">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6849-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="d6849-125">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6849-125">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="d6849-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6849-126">Property</span></span>|<span data-ttu-id="d6849-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6849-127">Type</span></span>|<span data-ttu-id="d6849-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6849-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6849-129">id</span><span class="sxs-lookup"><span data-stu-id="d6849-129">id</span></span>|<span data-ttu-id="d6849-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6849-130">String</span></span>|<span data-ttu-id="d6849-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d6849-131">Key of the entity.</span></span> <span data-ttu-id="d6849-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6849-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6849-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d6849-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6849-134">DateTimeOffset</span></span>|<span data-ttu-id="d6849-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d6849-135">DateTime the object was last modified.</span></span> <span data-ttu-id="d6849-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6849-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6849-137">createdDateTime</span></span>|<span data-ttu-id="d6849-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6849-138">DateTimeOffset</span></span>|<span data-ttu-id="d6849-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d6849-139">DateTime the object was created.</span></span> <span data-ttu-id="d6849-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6849-141">description</span><span class="sxs-lookup"><span data-stu-id="d6849-141">description</span></span>|<span data-ttu-id="d6849-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6849-142">String</span></span>|<span data-ttu-id="d6849-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6849-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6849-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6849-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d6849-145">displayName</span></span>|<span data-ttu-id="d6849-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6849-146">String</span></span>|<span data-ttu-id="d6849-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6849-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6849-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6849-149">version</span><span class="sxs-lookup"><span data-stu-id="d6849-149">version</span></span>|<span data-ttu-id="d6849-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d6849-150">Int32</span></span>|<span data-ttu-id="d6849-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6849-151">Version of the device configuration.</span></span> <span data-ttu-id="d6849-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6849-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="d6849-153">accountBlockModification</span></span>|<span data-ttu-id="d6849-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-154">Boolean</span></span>|<span data-ttu-id="d6849-155">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="d6849-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="d6849-157">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-157">Boolean</span></span>|<span data-ttu-id="d6849-158">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="d6849-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-159">airDropBlocked</span></span>|<span data-ttu-id="d6849-160">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-160">Boolean</span></span>|<span data-ttu-id="d6849-161">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="d6849-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="d6849-163">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-163">Boolean</span></span>|<span data-ttu-id="d6849-164">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d6849-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="d6849-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="d6849-166">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-166">Boolean</span></span>|<span data-ttu-id="d6849-167">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="d6849-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="d6849-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="d6849-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="d6849-169">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-169">Boolean</span></span>|<span data-ttu-id="d6849-170">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d6849-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="d6849-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="d6849-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-172">Boolean</span></span>|<span data-ttu-id="d6849-173">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="d6849-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-174">appleNewsBlocked</span></span>|<span data-ttu-id="d6849-175">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-175">Boolean</span></span>|<span data-ttu-id="d6849-176">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d6849-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="d6849-177">appsSingleAppModeList</span></span>|<span data-ttu-id="d6849-178">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="d6849-179">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="d6849-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="d6849-180">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-180">Supervised only.</span></span> <span data-ttu-id="d6849-181">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d6849-181">iOS 7.0 and later.</span></span> <span data-ttu-id="d6849-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d6849-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d6849-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="d6849-183">appsVisibilityList</span></span>|<span data-ttu-id="d6849-184">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="d6849-185">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="d6849-186">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d6849-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d6849-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="d6849-187">appsVisibilityListType</span></span>|[<span data-ttu-id="d6849-188">appListType</span><span class="sxs-lookup"><span data-stu-id="d6849-188">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="d6849-189">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="d6849-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="d6849-190">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d6849-190">The possible values are:</span></span>|
|<span data-ttu-id="d6849-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="d6849-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="d6849-192">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-192">Boolean</span></span>|<span data-ttu-id="d6849-193">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d6849-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-194">appStoreBlocked</span></span>|<span data-ttu-id="d6849-195">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-195">Boolean</span></span>|<span data-ttu-id="d6849-196">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="d6849-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="d6849-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="d6849-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="d6849-198">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-198">Boolean</span></span>|<span data-ttu-id="d6849-199">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d6849-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="d6849-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d6849-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="d6849-201">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-201">Boolean</span></span>|<span data-ttu-id="d6849-202">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="d6849-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="d6849-203">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d6849-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d6849-204">appStoreRequirePassword</span></span>|<span data-ttu-id="d6849-205">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-205">Boolean</span></span>|<span data-ttu-id="d6849-206">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d6849-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="d6849-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="d6849-207">bluetoothBlockModification</span></span>|<span data-ttu-id="d6849-208">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-208">Boolean</span></span>|<span data-ttu-id="d6849-209">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="d6849-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-210">cameraBlocked</span></span>|<span data-ttu-id="d6849-211">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-211">Boolean</span></span>|<span data-ttu-id="d6849-212">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6849-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="d6849-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="d6849-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="d6849-214">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-214">Boolean</span></span>|<span data-ttu-id="d6849-215">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d6849-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="d6849-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="d6849-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="d6849-217">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-217">Boolean</span></span>|<span data-ttu-id="d6849-218">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="d6849-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="d6849-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="d6849-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="d6849-220">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-220">Boolean</span></span>|<span data-ttu-id="d6849-221">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="d6849-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="d6849-223">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-223">Boolean</span></span>|<span data-ttu-id="d6849-224">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d6849-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="d6849-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="d6849-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="d6849-226">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-226">Boolean</span></span>|<span data-ttu-id="d6849-227">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d6849-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="d6849-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="d6849-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="d6849-229">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-229">Boolean</span></span>|<span data-ttu-id="d6849-230">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d6849-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="d6849-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d6849-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="d6849-232">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-232">Boolean</span></span>|<span data-ttu-id="d6849-233">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d6849-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d6849-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="d6849-235">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-235">Boolean</span></span>|<span data-ttu-id="d6849-236">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d6849-237">compliantAppsList</span></span>|<span data-ttu-id="d6849-238">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="d6849-239">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="d6849-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d6849-240">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d6849-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d6849-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d6849-241">compliantAppListType</span></span>|[<span data-ttu-id="d6849-242">appListType</span><span class="sxs-lookup"><span data-stu-id="d6849-242">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="d6849-243">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="d6849-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="d6849-244">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d6849-244">The possible values are:</span></span>|
|<span data-ttu-id="d6849-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="d6849-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="d6849-246">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-246">Boolean</span></span>|<span data-ttu-id="d6849-247">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-248">definitionLookupBlocked</span></span>|<span data-ttu-id="d6849-249">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-249">Boolean</span></span>|<span data-ttu-id="d6849-250">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="d6849-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="d6849-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="d6849-252">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-252">Boolean</span></span>|<span data-ttu-id="d6849-253">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="d6849-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="d6849-255">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-255">Boolean</span></span>|<span data-ttu-id="d6849-256">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="d6849-257">deviceBlockNameModification</span></span>|<span data-ttu-id="d6849-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-258">Boolean</span></span>|<span data-ttu-id="d6849-259">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d6849-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="d6849-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="d6849-261">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-261">Boolean</span></span>|<span data-ttu-id="d6849-262">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d6849-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d6849-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="d6849-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="d6849-264">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-264">Boolean</span></span>|<span data-ttu-id="d6849-265">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="d6849-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="d6849-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="d6849-267">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-267">Boolean</span></span>|<span data-ttu-id="d6849-268">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="d6849-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="d6849-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="d6849-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="d6849-270">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-270">Boolean</span></span>|<span data-ttu-id="d6849-271">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="d6849-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="d6849-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="d6849-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="d6849-273">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6849-273">String collection</span></span>|<span data-ttu-id="d6849-274">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="d6849-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="d6849-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="d6849-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="d6849-276">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-276">Boolean</span></span>|<span data-ttu-id="d6849-277">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="d6849-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="d6849-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="d6849-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="d6849-279">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-279">Boolean</span></span>|<span data-ttu-id="d6849-280">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="d6849-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="d6849-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-281">faceTimeBlocked</span></span>|<span data-ttu-id="d6849-282">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-282">Boolean</span></span>|<span data-ttu-id="d6849-283">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="d6849-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="d6849-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="d6849-285">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-285">Boolean</span></span>|<span data-ttu-id="d6849-286">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="d6849-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="d6849-288">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-288">Boolean</span></span>|<span data-ttu-id="d6849-289">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="d6849-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="d6849-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="d6849-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="d6849-291">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-291">Boolean</span></span>|<span data-ttu-id="d6849-292">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="d6849-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="d6849-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-293">gameCenterBlocked</span></span>|<span data-ttu-id="d6849-294">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-294">Boolean</span></span>|<span data-ttu-id="d6849-295">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-296">hostPairingBlocked</span></span>|<span data-ttu-id="d6849-297">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-297">Boolean</span></span>|<span data-ttu-id="d6849-298">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="d6849-300">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-300">Boolean</span></span>|<span data-ttu-id="d6849-301">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="d6849-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="d6849-303">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-303">Boolean</span></span>|<span data-ttu-id="d6849-304">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="d6849-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="d6849-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="d6849-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="d6849-306">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-306">Boolean</span></span>|<span data-ttu-id="d6849-307">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="d6849-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="d6849-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d6849-308">iCloudBlockBackup</span></span>|<span data-ttu-id="d6849-309">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-309">Boolean</span></span>|<span data-ttu-id="d6849-310">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d6849-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="d6849-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="d6849-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="d6849-312">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-312">Boolean</span></span>|<span data-ttu-id="d6849-313">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d6849-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="d6849-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="d6849-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="d6849-315">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-315">Boolean</span></span>|<span data-ttu-id="d6849-316">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d6849-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="d6849-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="d6849-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="d6849-318">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-318">Boolean</span></span>|<span data-ttu-id="d6849-319">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d6849-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="d6849-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="d6849-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="d6849-321">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-321">Boolean</span></span>|<span data-ttu-id="d6849-322">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d6849-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="d6849-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="d6849-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="d6849-324">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-324">Boolean</span></span>|<span data-ttu-id="d6849-325">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d6849-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="d6849-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="d6849-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="d6849-327">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-327">Boolean</span></span>|<span data-ttu-id="d6849-328">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="d6849-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="d6849-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="d6849-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="d6849-330">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-330">Boolean</span></span>|<span data-ttu-id="d6849-331">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="d6849-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="d6849-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="d6849-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="d6849-333">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-333">Boolean</span></span>|<span data-ttu-id="d6849-334">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="d6849-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="d6849-335">iTunesBlockRadio</span></span>|<span data-ttu-id="d6849-336">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-336">Boolean</span></span>|<span data-ttu-id="d6849-337">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d6849-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="d6849-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="d6849-339">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-339">Boolean</span></span>|<span data-ttu-id="d6849-340">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d6849-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="d6849-341">keyboardBlockDictation</span></span>|<span data-ttu-id="d6849-342">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-342">Boolean</span></span>|<span data-ttu-id="d6849-343">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d6849-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="d6849-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="d6849-345">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-345">Boolean</span></span>|<span data-ttu-id="d6849-346">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d6849-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="d6849-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="d6849-348">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-348">Boolean</span></span>|<span data-ttu-id="d6849-349">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d6849-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="d6849-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="d6849-351">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-351">Boolean</span></span>|<span data-ttu-id="d6849-352">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d6849-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="d6849-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="d6849-354">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-354">Boolean</span></span>|<span data-ttu-id="d6849-355">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="d6849-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="d6849-357">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-357">Boolean</span></span>|<span data-ttu-id="d6849-358">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="d6849-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="d6849-360">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-360">Boolean</span></span>|<span data-ttu-id="d6849-361">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="d6849-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="d6849-363">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-363">Boolean</span></span>|<span data-ttu-id="d6849-364">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="d6849-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="d6849-366">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-366">Boolean</span></span>|<span data-ttu-id="d6849-367">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="d6849-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="d6849-369">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-369">Boolean</span></span>|<span data-ttu-id="d6849-370">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="d6849-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="d6849-372">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-372">Boolean</span></span>|<span data-ttu-id="d6849-373">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="d6849-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="d6849-375">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-375">Boolean</span></span>|<span data-ttu-id="d6849-376">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="d6849-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="d6849-378">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-378">Boolean</span></span>|<span data-ttu-id="d6849-379">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d6849-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="d6849-381">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-381">Boolean</span></span>|<span data-ttu-id="d6849-382">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="d6849-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="d6849-384">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-384">Boolean</span></span>|<span data-ttu-id="d6849-385">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d6849-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="d6849-387">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6849-387">String</span></span>|<span data-ttu-id="d6849-388">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="d6849-389">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="d6849-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="d6849-390">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="d6849-390">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="d6849-391">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-391">Boolean</span></span>|<span data-ttu-id="d6849-392">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-392">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-393">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="d6849-393">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="d6849-394">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-394">Boolean</span></span>|<span data-ttu-id="d6849-395">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-395">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-396">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="d6849-396">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="d6849-397">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-397">Boolean</span></span>|<span data-ttu-id="d6849-398">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-398">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-399">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="d6849-399">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="d6849-400">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-400">Boolean</span></span>|<span data-ttu-id="d6849-401">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-401">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-402">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="d6849-402">kioskModeRequireZoom</span></span>|<span data-ttu-id="d6849-403">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-403">Boolean</span></span>|<span data-ttu-id="d6849-404">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-404">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="d6849-405">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="d6849-405">kioskModeManagedAppId</span></span>|<span data-ttu-id="d6849-406">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6849-406">String</span></span>|<span data-ttu-id="d6849-407">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="d6849-407">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="d6849-408">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="d6849-408">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="d6849-409">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="d6849-409">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="d6849-410">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-410">Boolean</span></span>|<span data-ttu-id="d6849-411">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d6849-411">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="d6849-412">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="d6849-412">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="d6849-413">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-413">Boolean</span></span>|<span data-ttu-id="d6849-414">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d6849-414">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="d6849-415">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="d6849-415">lockScreenBlockPassbook</span></span>|<span data-ttu-id="d6849-416">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-416">Boolean</span></span>|<span data-ttu-id="d6849-417">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="d6849-417">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="d6849-418">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="d6849-418">lockScreenBlockTodayView</span></span>|<span data-ttu-id="d6849-419">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-419">Boolean</span></span>|<span data-ttu-id="d6849-420">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d6849-420">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="d6849-421">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d6849-421">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="d6849-422">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d6849-422">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="d6849-423">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="d6849-423">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="d6849-424">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d6849-424">mediaContentRatingCanada</span></span>|[<span data-ttu-id="d6849-425">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d6849-425">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="d6849-426">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="d6849-426">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="d6849-427">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d6849-427">mediaContentRatingFrance</span></span>|[<span data-ttu-id="d6849-428">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d6849-428">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="d6849-429">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="d6849-429">Media content rating settings for France</span></span>|
|<span data-ttu-id="d6849-430">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d6849-430">mediaContentRatingGermany</span></span>|[<span data-ttu-id="d6849-431">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d6849-431">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="d6849-432">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="d6849-432">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="d6849-433">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d6849-433">mediaContentRatingIreland</span></span>|[<span data-ttu-id="d6849-434">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d6849-434">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="d6849-435">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="d6849-435">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="d6849-436">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d6849-436">mediaContentRatingJapan</span></span>|[<span data-ttu-id="d6849-437">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d6849-437">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="d6849-438">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="d6849-438">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="d6849-439">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d6849-439">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="d6849-440">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d6849-440">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="d6849-441">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="d6849-441">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="d6849-442">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d6849-442">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="d6849-443">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d6849-443">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="d6849-444">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="d6849-444">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="d6849-445">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d6849-445">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="d6849-446">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d6849-446">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="d6849-447">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="d6849-447">Media content rating settings for United States</span></span>|
|<span data-ttu-id="d6849-448">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="d6849-448">networkUsageRules</span></span>|<span data-ttu-id="d6849-449">Coleção [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="d6849-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="d6849-450">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="d6849-450">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="d6849-451">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d6849-451">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d6849-452">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="d6849-452">mediaContentRatingApps</span></span>|[<span data-ttu-id="d6849-453">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="d6849-453">ratingAppsType</span></span>](../resources/intune_deviceconfig_ratingappstype.md)|<span data-ttu-id="d6849-454">As configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d6849-454">Media content rating settings for Germany</span></span> <span data-ttu-id="d6849-455">Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="d6849-455">The possible values are `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`, , , , , , or .</span></span>|
|<span data-ttu-id="d6849-456">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-456">messagesBlocked</span></span>|<span data-ttu-id="d6849-457">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-457">Boolean</span></span>|<span data-ttu-id="d6849-458">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-458">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="d6849-459">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="d6849-459">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="d6849-460">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-460">Boolean</span></span>|<span data-ttu-id="d6849-461">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-461">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d6849-462">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d6849-462">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="d6849-463">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-463">Boolean</span></span>|<span data-ttu-id="d6849-464">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d6849-464">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d6849-465">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="d6849-465">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="d6849-466">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-466">Boolean</span></span>|<span data-ttu-id="d6849-467">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-467">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="d6849-468">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="d6849-468">passcodeBlockModification</span></span>|<span data-ttu-id="d6849-469">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-469">Boolean</span></span>|<span data-ttu-id="d6849-470">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-470">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d6849-471">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d6849-471">passcodeBlockSimple</span></span>|<span data-ttu-id="d6849-472">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-472">Boolean</span></span>|<span data-ttu-id="d6849-473">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d6849-473">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="d6849-474">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d6849-474">passcodeExpirationDays</span></span>|<span data-ttu-id="d6849-475">Int32</span><span class="sxs-lookup"><span data-stu-id="d6849-475">Int32</span></span>|<span data-ttu-id="d6849-476">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="d6849-476">Number of days before the passcode expires.</span></span> <span data-ttu-id="d6849-477">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="d6849-477">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="d6849-478">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d6849-478">passcodeMinimumLength</span></span>|<span data-ttu-id="d6849-479">Int32</span><span class="sxs-lookup"><span data-stu-id="d6849-479">Int32</span></span>|<span data-ttu-id="d6849-480">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="d6849-480">Minimum length of passcode.</span></span> <span data-ttu-id="d6849-481">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="d6849-481">Valid values 4 to 14</span></span>|
|<span data-ttu-id="d6849-482">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d6849-482">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d6849-483">Int32</span><span class="sxs-lookup"><span data-stu-id="d6849-483">Int32</span></span>|<span data-ttu-id="d6849-484">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="d6849-484">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="d6849-485">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d6849-485">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d6849-486">Int32</span><span class="sxs-lookup"><span data-stu-id="d6849-486">Int32</span></span>|<span data-ttu-id="d6849-487">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="d6849-487">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d6849-488">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d6849-488">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="d6849-489">Int32</span><span class="sxs-lookup"><span data-stu-id="d6849-489">Int32</span></span>|<span data-ttu-id="d6849-490">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="d6849-490">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="d6849-491">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="d6849-491">Valid values 0 to 4</span></span>|
|<span data-ttu-id="d6849-492">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="d6849-492">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="d6849-493">Int32</span><span class="sxs-lookup"><span data-stu-id="d6849-493">Int32</span></span>|<span data-ttu-id="d6849-494">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="d6849-494">Number of previous passcodes to block.</span></span> <span data-ttu-id="d6849-495">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="d6849-495">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d6849-496">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="d6849-496">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="d6849-497">Int32</span><span class="sxs-lookup"><span data-stu-id="d6849-497">Int32</span></span>|<span data-ttu-id="d6849-498">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6849-498">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="d6849-499">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="d6849-499">Valid values 4 to 11</span></span>|
|<span data-ttu-id="d6849-500">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="d6849-500">passcodeRequiredType</span></span>|[<span data-ttu-id="d6849-501">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d6849-501">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="d6849-502">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="d6849-502">Type of passcode that is required.</span></span> <span data-ttu-id="d6849-503">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d6849-503">The possible values are:</span></span>|
|<span data-ttu-id="d6849-504">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="d6849-504">passcodeRequired</span></span>|<span data-ttu-id="d6849-505">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-505">Boolean</span></span>|<span data-ttu-id="d6849-506">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="d6849-506">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="d6849-507">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-507">podcastsBlocked</span></span>|<span data-ttu-id="d6849-508">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-508">Boolean</span></span>|<span data-ttu-id="d6849-509">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-509">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="d6849-510">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d6849-510">safariBlockAutofill</span></span>|<span data-ttu-id="d6849-511">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-511">Boolean</span></span>|<span data-ttu-id="d6849-512">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="d6849-512">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="d6849-513">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="d6849-513">safariBlockJavaScript</span></span>|<span data-ttu-id="d6849-514">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-514">Boolean</span></span>|<span data-ttu-id="d6849-515">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="d6849-515">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="d6849-516">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="d6849-516">safariBlockPopups</span></span>|<span data-ttu-id="d6849-517">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-517">Boolean</span></span>|<span data-ttu-id="d6849-518">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="d6849-518">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="d6849-519">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-519">safariBlocked</span></span>|<span data-ttu-id="d6849-520">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-520">Boolean</span></span>|<span data-ttu-id="d6849-521">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="d6849-521">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="d6849-522">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d6849-522">safariCookieSettings</span></span>|[<span data-ttu-id="d6849-523">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d6849-523">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="d6849-524">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="d6849-524">Cookie settings for Safari.</span></span> <span data-ttu-id="d6849-525">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="d6849-525">The possible values are `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`, , , , , , , or .</span></span>|
|<span data-ttu-id="d6849-526">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="d6849-526">safariManagedDomains</span></span>|<span data-ttu-id="d6849-527">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6849-527">String collection</span></span>|<span data-ttu-id="d6849-528">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="d6849-528">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="d6849-529">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="d6849-529">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="d6849-530">Coleção de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6849-530">String collection</span></span>|<span data-ttu-id="d6849-531">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="d6849-531">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="d6849-532">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-532">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d6849-533">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="d6849-533">safariRequireFraudWarning</span></span>|<span data-ttu-id="d6849-534">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-534">Boolean</span></span>|<span data-ttu-id="d6849-535">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="d6849-535">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="d6849-536">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-536">screenCaptureBlocked</span></span>|<span data-ttu-id="d6849-537">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-537">Boolean</span></span>|<span data-ttu-id="d6849-538">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="d6849-538">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="d6849-539">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-539">siriBlocked</span></span>|<span data-ttu-id="d6849-540">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-540">Boolean</span></span>|<span data-ttu-id="d6849-541">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="d6849-541">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="d6849-542">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="d6849-542">siriBlockedWhenLocked</span></span>|<span data-ttu-id="d6849-543">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-543">Boolean</span></span>|<span data-ttu-id="d6849-544">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d6849-544">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="d6849-545">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="d6849-545">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="d6849-546">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-546">Boolean</span></span>|<span data-ttu-id="d6849-547">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-547">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="d6849-548">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="d6849-548">siriRequireProfanityFilter</span></span>|<span data-ttu-id="d6849-549">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-549">Boolean</span></span>|<span data-ttu-id="d6849-550">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-550">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="d6849-551">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="d6849-551">spotlightBlockInternetResults</span></span>|<span data-ttu-id="d6849-552">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-552">Boolean</span></span>|<span data-ttu-id="d6849-553">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-553">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="d6849-554">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="d6849-554">voiceDialingBlocked</span></span>|<span data-ttu-id="d6849-555">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-555">Boolean</span></span>|<span data-ttu-id="d6849-556">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d6849-556">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="d6849-557">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="d6849-557">wallpaperBlockModification</span></span>|<span data-ttu-id="d6849-558">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-558">Boolean</span></span>|<span data-ttu-id="d6849-559">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d6849-559">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="d6849-560">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="d6849-560">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="d6849-561">Booleano</span><span class="sxs-lookup"><span data-stu-id="d6849-561">Boolean</span></span>|<span data-ttu-id="d6849-562">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d6849-562">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="d6849-563">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6849-563">Response</span></span>
<span data-ttu-id="d6849-564">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6849-564">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6849-565">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6849-565">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6849-566">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6849-566">Request</span></span>
<span data-ttu-id="d6849-567">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6849-567">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="d6849-568">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6849-568">Response</span></span>
<span data-ttu-id="d6849-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6849-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7949

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



