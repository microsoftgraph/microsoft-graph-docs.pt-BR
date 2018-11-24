# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="87f21-101">Criar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="87f21-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="87f21-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="87f21-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87f21-103">Cria um novo objeto [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87f21-103">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87f21-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87f21-104">Prerequisites</span></span>
<span data-ttu-id="87f21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87f21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87f21-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87f21-107">Permission type</span></span>|<span data-ttu-id="87f21-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87f21-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87f21-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87f21-109">Delegated (work or school account)</span></span>|<span data-ttu-id="87f21-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87f21-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87f21-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87f21-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87f21-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87f21-112">Not supported.</span></span>|
|<span data-ttu-id="87f21-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87f21-113">Application</span></span>|<span data-ttu-id="87f21-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87f21-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87f21-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87f21-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="87f21-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87f21-116">Request headers</span></span>
|<span data-ttu-id="87f21-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87f21-117">Header</span></span>|<span data-ttu-id="87f21-118">Valor</span><span class="sxs-lookup"><span data-stu-id="87f21-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87f21-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="87f21-119">Authorization</span></span>|<span data-ttu-id="87f21-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87f21-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87f21-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87f21-121">Accept</span></span>|<span data-ttu-id="87f21-122">application/json</span><span class="sxs-lookup"><span data-stu-id="87f21-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87f21-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87f21-123">Request body</span></span>
<span data-ttu-id="87f21-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="87f21-124">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="87f21-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="87f21-125">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="87f21-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87f21-126">Property</span></span>|<span data-ttu-id="87f21-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="87f21-127">Type</span></span>|<span data-ttu-id="87f21-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="87f21-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87f21-129">id</span><span class="sxs-lookup"><span data-stu-id="87f21-129">id</span></span>|<span data-ttu-id="87f21-130">String</span><span class="sxs-lookup"><span data-stu-id="87f21-130">String</span></span>|<span data-ttu-id="87f21-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="87f21-131">Key of the entity.</span></span> <span data-ttu-id="87f21-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f21-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f21-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87f21-133">lastModifiedDateTime</span></span>|<span data-ttu-id="87f21-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87f21-134">DateTimeOffset</span></span>|<span data-ttu-id="87f21-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="87f21-135">DateTime the object was last modified.</span></span> <span data-ttu-id="87f21-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f21-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f21-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87f21-137">createdDateTime</span></span>|<span data-ttu-id="87f21-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87f21-138">DateTimeOffset</span></span>|<span data-ttu-id="87f21-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="87f21-139">DateTime the object was created.</span></span> <span data-ttu-id="87f21-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f21-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f21-141">descrição</span><span class="sxs-lookup"><span data-stu-id="87f21-141">description</span></span>|<span data-ttu-id="87f21-142">String</span><span class="sxs-lookup"><span data-stu-id="87f21-142">String</span></span>|<span data-ttu-id="87f21-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87f21-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87f21-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f21-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f21-145">displayName</span><span class="sxs-lookup"><span data-stu-id="87f21-145">displayName</span></span>|<span data-ttu-id="87f21-146">String</span><span class="sxs-lookup"><span data-stu-id="87f21-146">String</span></span>|<span data-ttu-id="87f21-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87f21-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87f21-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f21-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f21-149">version</span><span class="sxs-lookup"><span data-stu-id="87f21-149">version</span></span>|<span data-ttu-id="87f21-150">Int32</span><span class="sxs-lookup"><span data-stu-id="87f21-150">Int32</span></span>|<span data-ttu-id="87f21-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87f21-151">Version of the device configuration.</span></span> <span data-ttu-id="87f21-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f21-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f21-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="87f21-153">deliveryOptimizationMode</span></span>|[<span data-ttu-id="87f21-154">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="87f21-154">windowsDeliveryOptimizationMode</span></span>](../resources/intune_deviceconfig_windowsdeliveryoptimizationmode.md)|<span data-ttu-id="87f21-155">Modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="87f21-155">Delivery Optimization Mode.</span></span> <span data-ttu-id="87f21-156">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="87f21-156">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="87f21-157">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="87f21-157">prereleaseFeatures</span></span>|[<span data-ttu-id="87f21-158">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="87f21-158">prereleaseFeatures</span></span>](../resources/intune_deviceconfig_prereleasefeatures.md)|<span data-ttu-id="87f21-159">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="87f21-159">The pre-release features.</span></span> <span data-ttu-id="87f21-160">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="87f21-160">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="87f21-161">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="87f21-161">automaticUpdateMode</span></span>|[<span data-ttu-id="87f21-162">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="87f21-162">automaticUpdateMode</span></span>](../resources/intune_deviceconfig_automaticupdatemode.md)|<span data-ttu-id="87f21-163">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="87f21-163">Automatic update mode.</span></span> <span data-ttu-id="87f21-164">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="87f21-164">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="87f21-165">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="87f21-165">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="87f21-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="87f21-166">Boolean</span></span>|<span data-ttu-id="87f21-167">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="87f21-167">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="87f21-168">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="87f21-168">driversExcluded</span></span>|<span data-ttu-id="87f21-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="87f21-169">Boolean</span></span>|<span data-ttu-id="87f21-170">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="87f21-170">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="87f21-171">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="87f21-171">installationSchedule</span></span>|[<span data-ttu-id="87f21-172">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="87f21-172">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="87f21-173">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="87f21-173">Installation schedule</span></span>|
|<span data-ttu-id="87f21-174">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="87f21-174">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="87f21-175">Int32</span><span class="sxs-lookup"><span data-stu-id="87f21-175">Int32</span></span>|<span data-ttu-id="87f21-176">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="87f21-176">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="87f21-177">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="87f21-177">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="87f21-178">Int32</span><span class="sxs-lookup"><span data-stu-id="87f21-178">Int32</span></span>|<span data-ttu-id="87f21-179">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="87f21-179">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="87f21-180">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="87f21-180">qualityUpdatesPaused</span></span>|<span data-ttu-id="87f21-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="87f21-181">Boolean</span></span>|<span data-ttu-id="87f21-182">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="87f21-182">Pause Quality Updates</span></span>|
|<span data-ttu-id="87f21-183">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="87f21-183">featureUpdatesPaused</span></span>|<span data-ttu-id="87f21-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="87f21-184">Boolean</span></span>|<span data-ttu-id="87f21-185">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="87f21-185">Pause Feature Updates</span></span>|
|<span data-ttu-id="87f21-186">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="87f21-186">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="87f21-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87f21-187">DateTimeOffset</span></span>|<span data-ttu-id="87f21-188">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="87f21-188">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="87f21-189">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="87f21-189">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="87f21-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87f21-190">DateTimeOffset</span></span>|<span data-ttu-id="87f21-191">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="87f21-191">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="87f21-192">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="87f21-192">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="87f21-193">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="87f21-193">windowsUpdateType</span></span>](../resources/intune_deviceconfig_windowsupdatetype.md)|<span data-ttu-id="87f21-194">Determina quais dispositivos de filial receberão suas atualizações de.</span><span class="sxs-lookup"><span data-stu-id="87f21-194">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="87f21-195">Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="87f21-195">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="87f21-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="87f21-196">Response</span></span>
<span data-ttu-id="87f21-197">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87f21-197">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87f21-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87f21-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="87f21-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87f21-199">Request</span></span>
<span data-ttu-id="87f21-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87f21-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 910

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```

### <a name="response"></a><span data-ttu-id="87f21-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="87f21-201">Response</span></span>
<span data-ttu-id="87f21-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87f21-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```



