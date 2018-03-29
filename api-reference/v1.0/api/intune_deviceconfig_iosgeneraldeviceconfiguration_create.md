# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="6f0b3-101">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f0b3-101">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6f0b3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f0b3-103">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-103">Create a new [plannerBucket](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f0b3-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f0b3-104">Prerequisites</span></span>
<span data-ttu-id="6f0b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6f0b3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f0b3-107">Permission type</span></span>|<span data-ttu-id="6f0b3-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f0b3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6f0b3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f0b3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f0b3-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f0b3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-112">Not supported.</span></span>|
|<span data-ttu-id="6f0b3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f0b3-113">Application</span></span>|<span data-ttu-id="6f0b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f0b3-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f0b3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6f0b3-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f0b3-116">Request headers</span></span>
|<span data-ttu-id="6f0b3-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f0b3-117">Header</span></span>|<span data-ttu-id="6f0b3-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6f0b3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f0b3-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f0b3-119">Authorization</span></span>|<span data-ttu-id="6f0b3-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6f0b3-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f0b3-121">Accept</span></span>|<span data-ttu-id="6f0b3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6f0b3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f0b3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f0b3-123">Request body</span></span>
<span data-ttu-id="6f0b3-124">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="6f0b3-125">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="6f0b3-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f0b3-126">Property</span></span>|<span data-ttu-id="6f0b3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f0b3-127">Type</span></span>|<span data-ttu-id="6f0b3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f0b3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f0b3-129">id</span><span class="sxs-lookup"><span data-stu-id="6f0b3-129">id</span></span>|<span data-ttu-id="6f0b3-130">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-130">String</span></span>|<span data-ttu-id="6f0b3-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-131">Key of the setting.</span></span> <span data-ttu-id="6f0b3-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0b3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f0b3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6f0b3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f0b3-134">DateTimeOffset</span></span>|<span data-ttu-id="6f0b3-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="6f0b3-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0b3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f0b3-137">createdDateTime</span></span>|<span data-ttu-id="6f0b3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f0b3-138">DateTimeOffset</span></span>|<span data-ttu-id="6f0b3-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-139">DateTime the object was created.</span></span> <span data-ttu-id="6f0b3-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0b3-141">descrição</span><span class="sxs-lookup"><span data-stu-id="6f0b3-141">description</span></span>|<span data-ttu-id="6f0b3-142">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-142">String</span></span>|<span data-ttu-id="6f0b3-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f0b3-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0b3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6f0b3-145">displayName</span></span>|<span data-ttu-id="6f0b3-146">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-146">String</span></span>|<span data-ttu-id="6f0b3-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f0b3-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0b3-149">version</span><span class="sxs-lookup"><span data-stu-id="6f0b3-149">version</span></span>|<span data-ttu-id="6f0b3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0b3-150">Int32</span></span>|<span data-ttu-id="6f0b3-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-151">Version of the device configuration.</span></span> <span data-ttu-id="6f0b3-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f0b3-153">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-153">accountBlockModification</span></span>|<span data-ttu-id="6f0b3-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-154">Boolean</span></span>|<span data-ttu-id="6f0b3-155">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-155">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-156">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="6f0b3-156">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="6f0b3-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-157">Boolean</span></span>|<span data-ttu-id="6f0b3-158">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-158">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-159">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-159">airDropBlocked</span></span>|<span data-ttu-id="6f0b3-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-160">Boolean</span></span>|<span data-ttu-id="6f0b3-161">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-161">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-162">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="6f0b3-162">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="6f0b3-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-163">Boolean</span></span>|<span data-ttu-id="6f0b3-164">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-164">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-165">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="6f0b3-165">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="6f0b3-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-166">Boolean</span></span>|<span data-ttu-id="6f0b3-167">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-167">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="6f0b3-168">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="6f0b3-168">appleWatchBlockPairing</span></span>|<span data-ttu-id="6f0b3-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-169">Boolean</span></span>|<span data-ttu-id="6f0b3-170">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-170">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-171">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="6f0b3-171">appleWatchForceWristDetection</span></span>|<span data-ttu-id="6f0b3-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-172">Boolean</span></span>|<span data-ttu-id="6f0b3-173">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-173">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="6f0b3-174">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-174">appleNewsBlocked</span></span>|<span data-ttu-id="6f0b3-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-175">Boolean</span></span>|<span data-ttu-id="6f0b3-176">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-176">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-177">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="6f0b3-177">appsSingleAppModeList</span></span>|<span data-ttu-id="6f0b3-178">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-178">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="6f0b3-179">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-179">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="6f0b3-180">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-180">Supervised only.</span></span> <span data-ttu-id="6f0b3-181">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-181">iOS 7.0 and later.</span></span> <span data-ttu-id="6f0b3-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-182">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6f0b3-183">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="6f0b3-183">appsVisibilityList</span></span>|<span data-ttu-id="6f0b3-184">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-184">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="6f0b3-185">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-185">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="6f0b3-186">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6f0b3-187">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="6f0b3-187">appsVisibilityListType</span></span>|<span data-ttu-id="6f0b3-188">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-188">String</span></span>|<span data-ttu-id="6f0b3-189">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-189">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="6f0b3-190">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6f0b3-191">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="6f0b3-191">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="6f0b3-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-192">Boolean</span></span>|<span data-ttu-id="6f0b3-193">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-193">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-194">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-194">appStoreBlocked</span></span>|<span data-ttu-id="6f0b3-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-195">Boolean</span></span>|<span data-ttu-id="6f0b3-196">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-196">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="6f0b3-197">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="6f0b3-197">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="6f0b3-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-198">Boolean</span></span>|<span data-ttu-id="6f0b3-199">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-199">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="6f0b3-200">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="6f0b3-200">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="6f0b3-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-201">Boolean</span></span>|<span data-ttu-id="6f0b3-202">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-202">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="6f0b3-203">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-203">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-204">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="6f0b3-204">appStoreRequirePassword</span></span>|<span data-ttu-id="6f0b3-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-205">Boolean</span></span>|<span data-ttu-id="6f0b3-206">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-206">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="6f0b3-207">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-207">bluetoothBlockModification</span></span>|<span data-ttu-id="6f0b3-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-208">Boolean</span></span>|<span data-ttu-id="6f0b3-209">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-209">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-210">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-210">cameraBlocked</span></span>|<span data-ttu-id="6f0b3-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-211">Boolean</span></span>|<span data-ttu-id="6f0b3-212">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-212">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="6f0b3-213">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="6f0b3-213">cellularBlockDataRoaming</span></span>|<span data-ttu-id="6f0b3-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-214">Boolean</span></span>|<span data-ttu-id="6f0b3-215">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-215">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="6f0b3-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="6f0b3-216">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="6f0b3-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-217">Boolean</span></span>|<span data-ttu-id="6f0b3-218">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-218">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="6f0b3-219">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-219">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="6f0b3-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-220">Boolean</span></span>|<span data-ttu-id="6f0b3-221">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-221">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-222">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="6f0b3-222">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="6f0b3-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-223">Boolean</span></span>|<span data-ttu-id="6f0b3-224">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-224">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="6f0b3-225">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="6f0b3-225">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="6f0b3-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-226">Boolean</span></span>|<span data-ttu-id="6f0b3-227">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-227">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="6f0b3-228">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="6f0b3-228">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="6f0b3-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-229">Boolean</span></span>|<span data-ttu-id="6f0b3-230">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-230">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="6f0b3-231">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6f0b3-231">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="6f0b3-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-232">Boolean</span></span>|<span data-ttu-id="6f0b3-233">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-233">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6f0b3-234">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6f0b3-234">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="6f0b3-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-235">Boolean</span></span>|<span data-ttu-id="6f0b3-236">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-236">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-237">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="6f0b3-237">compliantAppsList</span></span>|<span data-ttu-id="6f0b3-238">Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-238">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="6f0b3-239">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-239">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="6f0b3-240">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-240">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6f0b3-241">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="6f0b3-241">compliantAppListType</span></span>|<span data-ttu-id="6f0b3-242">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-242">String</span></span>|<span data-ttu-id="6f0b3-243">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-243">List that is in the AppComplianceList.</span></span> <span data-ttu-id="6f0b3-244">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-244">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6f0b3-245">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="6f0b3-245">configurationProfileBlockChanges</span></span>|<span data-ttu-id="6f0b3-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-246">Boolean</span></span>|<span data-ttu-id="6f0b3-247">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-247">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-248">definitionLookupBlocked</span></span>|<span data-ttu-id="6f0b3-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-249">Boolean</span></span>|<span data-ttu-id="6f0b3-250">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-250">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="6f0b3-251">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="6f0b3-251">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="6f0b3-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-252">Boolean</span></span>|<span data-ttu-id="6f0b3-253">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-253">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-254">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="6f0b3-254">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="6f0b3-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-255">Boolean</span></span>|<span data-ttu-id="6f0b3-256">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-256">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-257">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-257">deviceBlockNameModification</span></span>|<span data-ttu-id="6f0b3-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-258">Boolean</span></span>|<span data-ttu-id="6f0b3-259">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-259">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-260">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="6f0b3-260">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="6f0b3-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-261">Boolean</span></span>|<span data-ttu-id="6f0b3-262">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-262">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="6f0b3-263">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-263">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="6f0b3-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-264">Boolean</span></span>|<span data-ttu-id="6f0b3-265">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-265">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="6f0b3-266">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="6f0b3-266">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="6f0b3-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-267">Boolean</span></span>|<span data-ttu-id="6f0b3-268">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-268">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="6f0b3-269">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="6f0b3-269">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="6f0b3-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-270">Boolean</span></span>|<span data-ttu-id="6f0b3-271">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-271">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="6f0b3-272">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="6f0b3-272">emailInDomainSuffixes</span></span>|<span data-ttu-id="6f0b3-273">String collection</span><span class="sxs-lookup"><span data-stu-id="6f0b3-273">String collection</span></span>|<span data-ttu-id="6f0b3-274">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-274">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="6f0b3-275">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="6f0b3-275">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="6f0b3-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-276">Boolean</span></span>|<span data-ttu-id="6f0b3-277">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-277">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="6f0b3-278">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-278">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="6f0b3-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-279">Boolean</span></span>|<span data-ttu-id="6f0b3-280">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-280">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="6f0b3-281">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-281">faceTimeBlocked</span></span>|<span data-ttu-id="6f0b3-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-282">Boolean</span></span>|<span data-ttu-id="6f0b3-283">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-283">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="6f0b3-284">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-284">findMyFriendsBlocked</span></span>|<span data-ttu-id="6f0b3-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-285">Boolean</span></span>|<span data-ttu-id="6f0b3-286">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-286">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-287">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="6f0b3-287">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="6f0b3-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-288">Boolean</span></span>|<span data-ttu-id="6f0b3-289">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-289">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="6f0b3-290">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="6f0b3-290">gamingBlockMultiplayer</span></span>|<span data-ttu-id="6f0b3-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-291">Boolean</span></span>|<span data-ttu-id="6f0b3-292">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-292">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="6f0b3-293">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-293">gameCenterBlocked</span></span>|<span data-ttu-id="6f0b3-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-294">Boolean</span></span>|<span data-ttu-id="6f0b3-295">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-295">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-296">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-296">hostPairingBlocked</span></span>|<span data-ttu-id="6f0b3-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-297">Boolean</span></span>|<span data-ttu-id="6f0b3-298">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-298">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-299">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-299">iBooksStoreBlocked</span></span>|<span data-ttu-id="6f0b3-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-300">Boolean</span></span>|<span data-ttu-id="6f0b3-301">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-301">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-302">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="6f0b3-302">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="6f0b3-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-303">Boolean</span></span>|<span data-ttu-id="6f0b3-304">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-304">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="6f0b3-305">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="6f0b3-305">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="6f0b3-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-306">Boolean</span></span>|<span data-ttu-id="6f0b3-307">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-307">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="6f0b3-308">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="6f0b3-308">iCloudBlockBackup</span></span>|<span data-ttu-id="6f0b3-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-309">Boolean</span></span>|<span data-ttu-id="6f0b3-310">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-310">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="6f0b3-311">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="6f0b3-311">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="6f0b3-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-312">Boolean</span></span>|<span data-ttu-id="6f0b3-313">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-313">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="6f0b3-314">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="6f0b3-314">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="6f0b3-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-315">Boolean</span></span>|<span data-ttu-id="6f0b3-316">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-316">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="6f0b3-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="6f0b3-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="6f0b3-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-318">Boolean</span></span>|<span data-ttu-id="6f0b3-319">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="6f0b3-320">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="6f0b3-320">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="6f0b3-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-321">Boolean</span></span>|<span data-ttu-id="6f0b3-322">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-322">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="6f0b3-323">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="6f0b3-323">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="6f0b3-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-324">Boolean</span></span>|<span data-ttu-id="6f0b3-325">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-325">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="6f0b3-326">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="6f0b3-326">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="6f0b3-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-327">Boolean</span></span>|<span data-ttu-id="6f0b3-328">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-328">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="6f0b3-329">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="6f0b3-329">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="6f0b3-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-330">Boolean</span></span>|<span data-ttu-id="6f0b3-331">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-331">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="6f0b3-332">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="6f0b3-332">iTunesBlockMusicService</span></span>|<span data-ttu-id="6f0b3-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-333">Boolean</span></span>|<span data-ttu-id="6f0b3-334">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-334">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="6f0b3-335">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="6f0b3-335">iTunesBlockRadio</span></span>|<span data-ttu-id="6f0b3-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-336">Boolean</span></span>|<span data-ttu-id="6f0b3-337">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-337">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6f0b3-338">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="6f0b3-338">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="6f0b3-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-339">Boolean</span></span>|<span data-ttu-id="6f0b3-340">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-340">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6f0b3-341">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="6f0b3-341">keyboardBlockDictation</span></span>|<span data-ttu-id="6f0b3-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-342">Boolean</span></span>|<span data-ttu-id="6f0b3-343">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-343">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-344">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="6f0b3-344">keyboardBlockPredictive</span></span>|<span data-ttu-id="6f0b3-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-345">Boolean</span></span>|<span data-ttu-id="6f0b3-346">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-346">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6f0b3-347">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="6f0b3-347">keyboardBlockShortcuts</span></span>|<span data-ttu-id="6f0b3-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-348">Boolean</span></span>|<span data-ttu-id="6f0b3-349">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-349">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-350">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="6f0b3-350">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="6f0b3-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-351">Boolean</span></span>|<span data-ttu-id="6f0b3-352">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-352">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6f0b3-353">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="6f0b3-353">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="6f0b3-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-354">Boolean</span></span>|<span data-ttu-id="6f0b3-355">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-355">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-356">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="6f0b3-356">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="6f0b3-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-357">Boolean</span></span>|<span data-ttu-id="6f0b3-358">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-358">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-359">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="6f0b3-359">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="6f0b3-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-360">Boolean</span></span>|<span data-ttu-id="6f0b3-361">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-361">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-362">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="6f0b3-362">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="6f0b3-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-363">Boolean</span></span>|<span data-ttu-id="6f0b3-364">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-364">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-365">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="6f0b3-365">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="6f0b3-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-366">Boolean</span></span>|<span data-ttu-id="6f0b3-367">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-367">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-368">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="6f0b3-368">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="6f0b3-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-369">Boolean</span></span>|<span data-ttu-id="6f0b3-370">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-370">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-371">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="6f0b3-371">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="6f0b3-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-372">Boolean</span></span>|<span data-ttu-id="6f0b3-373">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-373">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-374">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="6f0b3-374">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="6f0b3-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-375">Boolean</span></span>|<span data-ttu-id="6f0b3-376">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-376">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-377">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="6f0b3-377">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="6f0b3-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-378">Boolean</span></span>|<span data-ttu-id="6f0b3-379">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-379">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-380">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="6f0b3-380">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="6f0b3-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-381">Boolean</span></span>|<span data-ttu-id="6f0b3-382">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-382">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-383">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="6f0b3-383">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="6f0b3-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-384">Boolean</span></span>|<span data-ttu-id="6f0b3-385">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-385">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-386">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6f0b3-386">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="6f0b3-387">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-387">String</span></span>|<span data-ttu-id="6f0b3-388">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-388">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="6f0b3-389">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-389">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="6f0b3-390">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="6f0b3-390">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="6f0b3-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-391">Boolean</span></span>|<span data-ttu-id="6f0b3-392">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-392">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-393">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="6f0b3-393">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="6f0b3-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-394">Boolean</span></span>|<span data-ttu-id="6f0b3-395">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-395">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-396">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="6f0b3-396">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="6f0b3-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-397">Boolean</span></span>|<span data-ttu-id="6f0b3-398">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-398">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-399">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="6f0b3-399">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="6f0b3-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-400">Boolean</span></span>|<span data-ttu-id="6f0b3-401">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-401">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-402">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="6f0b3-402">kioskModeRequireZoom</span></span>|<span data-ttu-id="6f0b3-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-403">Boolean</span></span>|<span data-ttu-id="6f0b3-404">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-404">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="6f0b3-405">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="6f0b3-405">kioskModeManagedAppId</span></span>|<span data-ttu-id="6f0b3-406">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-406">String</span></span>|<span data-ttu-id="6f0b3-407">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-407">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="6f0b3-408">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-408">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="6f0b3-409">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="6f0b3-409">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="6f0b3-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-410">Boolean</span></span>|<span data-ttu-id="6f0b3-411">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-411">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="6f0b3-412">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="6f0b3-412">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="6f0b3-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-413">Boolean</span></span>|<span data-ttu-id="6f0b3-414">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-414">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="6f0b3-415">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="6f0b3-415">lockScreenBlockPassbook</span></span>|<span data-ttu-id="6f0b3-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-416">Boolean</span></span>|<span data-ttu-id="6f0b3-417">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="6f0b3-417">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="6f0b3-418">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="6f0b3-418">lockScreenBlockTodayView</span></span>|<span data-ttu-id="6f0b3-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-419">Boolean</span></span>|<span data-ttu-id="6f0b3-420">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-420">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="6f0b3-421">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6f0b3-421">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="6f0b3-422">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6f0b3-422">mediaContentRatingAustralia</span></span>](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|<span data-ttu-id="6f0b3-423">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="6f0b3-423">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="6f0b3-424">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6f0b3-424">mediaContentRatingCanada</span></span>|[<span data-ttu-id="6f0b3-425">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6f0b3-425">mediaContentRatingCanada</span></span>](../resources/intune_deviceconfig_mediacontentratingcanada.md)|<span data-ttu-id="6f0b3-426">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="6f0b3-426">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="6f0b3-427">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="6f0b3-427">mediaContentRatingFrance</span></span>|[<span data-ttu-id="6f0b3-428">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="6f0b3-428">mediaContentRatingFrance</span></span>](../resources/intune_deviceconfig_mediacontentratingfrance.md)|<span data-ttu-id="6f0b3-429">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="6f0b3-429">Media content rating settings for France</span></span>|
|<span data-ttu-id="6f0b3-430">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6f0b3-430">mediaContentRatingGermany</span></span>|[<span data-ttu-id="6f0b3-431">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6f0b3-431">mediaContentRatingGermany</span></span>](../resources/intune_deviceconfig_mediacontentratinggermany.md)|<span data-ttu-id="6f0b3-432">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="6f0b3-432">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="6f0b3-433">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="6f0b3-433">mediaContentRatingIreland</span></span>|[<span data-ttu-id="6f0b3-434">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="6f0b3-434">mediaContentRatingIreland</span></span>](../resources/intune_deviceconfig_mediacontentratingireland.md)|<span data-ttu-id="6f0b3-435">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="6f0b3-435">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="6f0b3-436">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6f0b3-436">mediaContentRatingJapan</span></span>|[<span data-ttu-id="6f0b3-437">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6f0b3-437">mediaContentRatingJapan</span></span>](../resources/intune_deviceconfig_mediacontentratingjapan.md)|<span data-ttu-id="6f0b3-438">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="6f0b3-438">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="6f0b3-439">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6f0b3-439">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="6f0b3-440">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6f0b3-440">mediaContentRatingNewZealand</span></span>](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|<span data-ttu-id="6f0b3-441">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="6f0b3-441">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="6f0b3-442">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6f0b3-442">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="6f0b3-443">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6f0b3-443">mediaContentRatingUnitedKingdom</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|<span data-ttu-id="6f0b3-444">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="6f0b3-444">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="6f0b3-445">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6f0b3-445">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="6f0b3-446">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6f0b3-446">mediaContentRatingUnitedStates</span></span>](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|<span data-ttu-id="6f0b3-447">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="6f0b3-447">Media content rating settings for United States</span></span>|
|<span data-ttu-id="6f0b3-448">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="6f0b3-448">networkUsageRules</span></span>|<span data-ttu-id="6f0b3-449">Coleção [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="6f0b3-449">[iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="6f0b3-450">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-450">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="6f0b3-451">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-451">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6f0b3-452">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="6f0b3-452">mediaContentRatingApps</span></span>|<span data-ttu-id="6f0b3-453">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-453">String</span></span>|<span data-ttu-id="6f0b3-454">Configurações de classificação de conteúdo de mídia Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-454">Media content rating settings for Apps Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="6f0b3-455">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-455">messagesBlocked</span></span>|<span data-ttu-id="6f0b3-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-456">Boolean</span></span>|<span data-ttu-id="6f0b3-457">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-457">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="6f0b3-458">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-458">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="6f0b3-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-459">Boolean</span></span>|<span data-ttu-id="6f0b3-460">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-460">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6f0b3-461">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6f0b3-461">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="6f0b3-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-462">Boolean</span></span>|<span data-ttu-id="6f0b3-463">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-463">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6f0b3-464">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-464">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="6f0b3-465">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-465">Boolean</span></span>|<span data-ttu-id="6f0b3-466">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-466">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="6f0b3-467">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-467">passcodeBlockModification</span></span>|<span data-ttu-id="6f0b3-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-468">Boolean</span></span>|<span data-ttu-id="6f0b3-469">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-469">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-470">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6f0b3-470">passcodeBlockSimple</span></span>|<span data-ttu-id="6f0b3-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-471">Boolean</span></span>|<span data-ttu-id="6f0b3-472">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-472">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6f0b3-473">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6f0b3-473">passcodeExpirationDays</span></span>|<span data-ttu-id="6f0b3-474">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0b3-474">Int32</span></span>|<span data-ttu-id="6f0b3-475">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-475">Number of days before the passcode expires.</span></span> <span data-ttu-id="6f0b3-476">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="6f0b3-476">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6f0b3-477">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6f0b3-477">passcodeMinimumLength</span></span>|<span data-ttu-id="6f0b3-478">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0b3-478">Int32</span></span>|<span data-ttu-id="6f0b3-479">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-479">Minimum length of passcode.</span></span> <span data-ttu-id="6f0b3-480">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="6f0b3-480">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6f0b3-481">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6f0b3-481">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6f0b3-482">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0b3-482">Int32</span></span>|<span data-ttu-id="6f0b3-483">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-483">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6f0b3-484">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6f0b3-484">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6f0b3-485">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0b3-485">Int32</span></span>|<span data-ttu-id="6f0b3-486">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-486">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6f0b3-487">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6f0b3-487">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6f0b3-488">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0b3-488">Int32</span></span>|<span data-ttu-id="6f0b3-489">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-489">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="6f0b3-490">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="6f0b3-490">Valid values 0 to 4</span></span>|
|<span data-ttu-id="6f0b3-491">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6f0b3-491">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6f0b3-492">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0b3-492">Int32</span></span>|<span data-ttu-id="6f0b3-493">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-493">Number of previous passcodes to block.</span></span> <span data-ttu-id="6f0b3-494">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="6f0b3-494">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6f0b3-495">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="6f0b3-495">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="6f0b3-496">Int32</span><span class="sxs-lookup"><span data-stu-id="6f0b3-496">Int32</span></span>|<span data-ttu-id="6f0b3-497">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-497">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="6f0b3-498">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="6f0b3-498">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6f0b3-499">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6f0b3-499">passcodeRequiredType</span></span>|<span data-ttu-id="6f0b3-500">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-500">String</span></span>|<span data-ttu-id="6f0b3-501">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-501">Type of passcode that is required.</span></span> <span data-ttu-id="6f0b3-502">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-502">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6f0b3-503">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6f0b3-503">passcodeRequired</span></span>|<span data-ttu-id="6f0b3-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-504">Boolean</span></span>|<span data-ttu-id="6f0b3-505">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-505">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6f0b3-506">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-506">podcastsBlocked</span></span>|<span data-ttu-id="6f0b3-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-507">Boolean</span></span>|<span data-ttu-id="6f0b3-508">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-508">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="6f0b3-509">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="6f0b3-509">safariBlockAutofill</span></span>|<span data-ttu-id="6f0b3-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-510">Boolean</span></span>|<span data-ttu-id="6f0b3-511">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-511">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="6f0b3-512">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="6f0b3-512">safariBlockJavaScript</span></span>|<span data-ttu-id="6f0b3-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-513">Boolean</span></span>|<span data-ttu-id="6f0b3-514">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-514">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="6f0b3-515">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="6f0b3-515">safariBlockPopups</span></span>|<span data-ttu-id="6f0b3-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-516">Boolean</span></span>|<span data-ttu-id="6f0b3-517">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-517">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="6f0b3-518">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-518">safariBlocked</span></span>|<span data-ttu-id="6f0b3-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-519">Boolean</span></span>|<span data-ttu-id="6f0b3-520">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-520">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="6f0b3-521">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="6f0b3-521">safariCookieSettings</span></span>|<span data-ttu-id="6f0b3-522">String</span><span class="sxs-lookup"><span data-stu-id="6f0b3-522">String</span></span>|<span data-ttu-id="6f0b3-523">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-523">Cookie settings for Safari.</span></span> <span data-ttu-id="6f0b3-524">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-524">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="6f0b3-525">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="6f0b3-525">safariManagedDomains</span></span>|<span data-ttu-id="6f0b3-526">String collection</span><span class="sxs-lookup"><span data-stu-id="6f0b3-526">String collection</span></span>|<span data-ttu-id="6f0b3-527">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-527">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="6f0b3-528">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="6f0b3-528">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="6f0b3-529">String collection</span><span class="sxs-lookup"><span data-stu-id="6f0b3-529">String collection</span></span>|<span data-ttu-id="6f0b3-530">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-530">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="6f0b3-531">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-531">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6f0b3-532">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="6f0b3-532">safariRequireFraudWarning</span></span>|<span data-ttu-id="6f0b3-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-533">Boolean</span></span>|<span data-ttu-id="6f0b3-534">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-534">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="6f0b3-535">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-535">screenCaptureBlocked</span></span>|<span data-ttu-id="6f0b3-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-536">Boolean</span></span>|<span data-ttu-id="6f0b3-537">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-537">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="6f0b3-538">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-538">siriBlocked</span></span>|<span data-ttu-id="6f0b3-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-539">Boolean</span></span>|<span data-ttu-id="6f0b3-540">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-540">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="6f0b3-541">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-541">siriBlockedWhenLocked</span></span>|<span data-ttu-id="6f0b3-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-542">Boolean</span></span>|<span data-ttu-id="6f0b3-543">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-543">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="6f0b3-544">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="6f0b3-544">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="6f0b3-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-545">Boolean</span></span>|<span data-ttu-id="6f0b3-546">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-546">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="6f0b3-547">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="6f0b3-547">siriRequireProfanityFilter</span></span>|<span data-ttu-id="6f0b3-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-548">Boolean</span></span>|<span data-ttu-id="6f0b3-549">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-549">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="6f0b3-550">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="6f0b3-550">spotlightBlockInternetResults</span></span>|<span data-ttu-id="6f0b3-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-551">Boolean</span></span>|<span data-ttu-id="6f0b3-552">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-552">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="6f0b3-553">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="6f0b3-553">voiceDialingBlocked</span></span>|<span data-ttu-id="6f0b3-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-554">Boolean</span></span>|<span data-ttu-id="6f0b3-555">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-555">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="6f0b3-556">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="6f0b3-556">wallpaperBlockModification</span></span>|<span data-ttu-id="6f0b3-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-557">Boolean</span></span>|<span data-ttu-id="6f0b3-558">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="6f0b3-558">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="6f0b3-559">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="6f0b3-559">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="6f0b3-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f0b3-560">Boolean</span></span>|<span data-ttu-id="6f0b3-561">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-561">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="6f0b3-562">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f0b3-562">Response</span></span>
<span data-ttu-id="6f0b3-563">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-563">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f0b3-564">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f0b3-564">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f0b3-565">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f0b3-565">Request</span></span>
<span data-ttu-id="6f0b3-566">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-566">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f0b3-567">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f0b3-567">Response</span></span>
<span data-ttu-id="6f0b3-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f0b3-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



