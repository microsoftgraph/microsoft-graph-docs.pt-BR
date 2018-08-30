# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="e0dd3-101">Atualizar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0dd3-101">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="e0dd3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0dd3-103">Atualizar as propriedades de um objeto [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0dd3-103">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0dd3-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0dd3-104">Prerequisites</span></span>
<span data-ttu-id="e0dd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e0dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e0dd3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0dd3-107">Permission type</span></span>|<span data-ttu-id="e0dd3-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0dd3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e0dd3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0dd3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0dd3-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0dd3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-112">Not supported.</span></span>|
|<span data-ttu-id="e0dd3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0dd3-113">Application</span></span>|<span data-ttu-id="e0dd3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0dd3-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0dd3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0dd3-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0dd3-116">Request headers</span></span>
|<span data-ttu-id="e0dd3-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0dd3-117">Header</span></span>|<span data-ttu-id="e0dd3-118">Valor</span><span class="sxs-lookup"><span data-stu-id="e0dd3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0dd3-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0dd3-119">Authorization</span></span>|<span data-ttu-id="e0dd3-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="e0dd3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0dd3-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0dd3-121">Accept</span></span>|<span data-ttu-id="e0dd3-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="e0dd3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0dd3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0dd3-123">Request body</span></span>
<span data-ttu-id="e0dd3-124">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0dd3-124">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="e0dd3-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0dd3-125">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="e0dd3-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0dd3-126">Property</span></span>|<span data-ttu-id="e0dd3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0dd3-127">Type</span></span>|<span data-ttu-id="e0dd3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0dd3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0dd3-129">id</span><span class="sxs-lookup"><span data-stu-id="e0dd3-129">id</span></span>|<span data-ttu-id="e0dd3-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0dd3-130">String</span></span>|<span data-ttu-id="e0dd3-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-131">Key of the entity.</span></span> <span data-ttu-id="e0dd3-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0dd3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0dd3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e0dd3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0dd3-134">DateTimeOffset</span></span>|<span data-ttu-id="e0dd3-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-135">DateTime the object was last modified.</span></span> <span data-ttu-id="e0dd3-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0dd3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0dd3-137">createdDateTime</span></span>|<span data-ttu-id="e0dd3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0dd3-138">DateTimeOffset</span></span>|<span data-ttu-id="e0dd3-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-139">DateTime the object was created.</span></span> <span data-ttu-id="e0dd3-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0dd3-141">description</span><span class="sxs-lookup"><span data-stu-id="e0dd3-141">description</span></span>|<span data-ttu-id="e0dd3-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0dd3-142">String</span></span>|<span data-ttu-id="e0dd3-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0dd3-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0dd3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e0dd3-145">displayName</span></span>|<span data-ttu-id="e0dd3-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0dd3-146">String</span></span>|<span data-ttu-id="e0dd3-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0dd3-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0dd3-149">version</span><span class="sxs-lookup"><span data-stu-id="e0dd3-149">version</span></span>|<span data-ttu-id="e0dd3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e0dd3-150">Int32</span></span>|<span data-ttu-id="e0dd3-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-151">Version of the device configuration.</span></span> <span data-ttu-id="e0dd3-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0dd3-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0dd3-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e0dd3-153">deliveryOptimizationMode</span></span>|[<span data-ttu-id="e0dd3-154">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e0dd3-154">windowsDeliveryOptimizationMode</span></span>](../resources/intune_deviceconfig_windowsdeliveryoptimizationmode.md)|<span data-ttu-id="e0dd3-155">Modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-155">Delivery Optimization Mode Possible values are: , , , , , , .</span></span> <span data-ttu-id="e0dd3-156">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-156">The possible values are `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`, , , , , or .</span></span>|
|<span data-ttu-id="e0dd3-157">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="e0dd3-157">prereleaseFeatures</span></span>|[<span data-ttu-id="e0dd3-158">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="e0dd3-158">prereleaseFeatures</span></span>](../resources/intune_deviceconfig_prereleasefeatures.md)|<span data-ttu-id="e0dd3-159">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-159">The pre-release features.</span></span> <span data-ttu-id="e0dd3-160">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-160">The possible values are `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`, , , , , , , , or .</span></span>|
|<span data-ttu-id="e0dd3-161">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="e0dd3-161">automaticUpdateMode</span></span>|[<span data-ttu-id="e0dd3-162">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="e0dd3-162">automaticUpdateMode</span></span>](../resources/intune_deviceconfig_automaticupdatemode.md)|<span data-ttu-id="e0dd3-163">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-163">Automatic update mode.</span></span> <span data-ttu-id="e0dd3-164">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-164">The possible values are `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, , , , , , or .</span></span>|
|<span data-ttu-id="e0dd3-165">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="e0dd3-165">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="e0dd3-166">Booleano</span><span class="sxs-lookup"><span data-stu-id="e0dd3-166">Boolean</span></span>|<span data-ttu-id="e0dd3-167">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="e0dd3-167">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="e0dd3-168">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="e0dd3-168">driversExcluded</span></span>|<span data-ttu-id="e0dd3-169">Booleano</span><span class="sxs-lookup"><span data-stu-id="e0dd3-169">Boolean</span></span>|<span data-ttu-id="e0dd3-170">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="e0dd3-170">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="e0dd3-171">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="e0dd3-171">installationSchedule</span></span>|[<span data-ttu-id="e0dd3-172">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="e0dd3-172">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="e0dd3-173">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="e0dd3-173">Installation schedule</span></span>|
|<span data-ttu-id="e0dd3-174">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="e0dd3-174">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="e0dd3-175">Int32</span><span class="sxs-lookup"><span data-stu-id="e0dd3-175">Int32</span></span>|<span data-ttu-id="e0dd3-176">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="e0dd3-176">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="e0dd3-177">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="e0dd3-177">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="e0dd3-178">Int32</span><span class="sxs-lookup"><span data-stu-id="e0dd3-178">Int32</span></span>|<span data-ttu-id="e0dd3-179">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="e0dd3-179">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="e0dd3-180">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="e0dd3-180">qualityUpdatesPaused</span></span>|<span data-ttu-id="e0dd3-181">Booleano</span><span class="sxs-lookup"><span data-stu-id="e0dd3-181">Boolean</span></span>|<span data-ttu-id="e0dd3-182">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="e0dd3-182">Pause Quality Updates</span></span>|
|<span data-ttu-id="e0dd3-183">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="e0dd3-183">featureUpdatesPaused</span></span>|<span data-ttu-id="e0dd3-184">Booleano</span><span class="sxs-lookup"><span data-stu-id="e0dd3-184">Boolean</span></span>|<span data-ttu-id="e0dd3-185">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="e0dd3-185">Pause Feature Updates</span></span>|
|<span data-ttu-id="e0dd3-186">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="e0dd3-186">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="e0dd3-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0dd3-187">DateTimeOffset</span></span>|<span data-ttu-id="e0dd3-188">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="e0dd3-188">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="e0dd3-189">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="e0dd3-189">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="e0dd3-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0dd3-190">DateTimeOffset</span></span>|<span data-ttu-id="e0dd3-191">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="e0dd3-191">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="e0dd3-192">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="e0dd3-192">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="e0dd3-193">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="e0dd3-193">windowsUpdateType</span></span>](../resources/intune_deviceconfig_windowsupdatetype.md)|<span data-ttu-id="e0dd3-194">Determina de qual branch os dispositivos receberão suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-194">Determines which branch devices will receive their updates from Possible values are: , , .</span></span> <span data-ttu-id="e0dd3-195">Os valores possíveis são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-195">The possible values are `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`, , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="e0dd3-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0dd3-196">Response</span></span>
<span data-ttu-id="e0dd3-197">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-197">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0dd3-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0dd3-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0dd3-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0dd3-199">Request</span></span>
<span data-ttu-id="e0dd3-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 898

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="e0dd3-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0dd3-201">Response</span></span>
<span data-ttu-id="e0dd3-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0dd3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



