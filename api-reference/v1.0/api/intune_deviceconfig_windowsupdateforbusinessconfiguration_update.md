# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="5c0ba-101">Atualizar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c0ba-101">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="5c0ba-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c0ba-103">Atualizar as propriedades de um objeto [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c0ba-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c0ba-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c0ba-104">Prerequisites</span></span>
<span data-ttu-id="5c0ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c0ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5c0ba-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c0ba-107">Permission type</span></span>|<span data-ttu-id="5c0ba-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c0ba-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5c0ba-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c0ba-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c0ba-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c0ba-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-112">Not supported.</span></span>|
|<span data-ttu-id="5c0ba-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c0ba-113">Application</span></span>|<span data-ttu-id="5c0ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c0ba-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c0ba-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5c0ba-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0ba-116">Request headers</span></span>
|<span data-ttu-id="5c0ba-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c0ba-117">Header</span></span>|<span data-ttu-id="5c0ba-118">Valor</span><span class="sxs-lookup"><span data-stu-id="5c0ba-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c0ba-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c0ba-119">Authorization</span></span>|<span data-ttu-id="5c0ba-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5c0ba-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c0ba-121">Accept</span></span>|<span data-ttu-id="5c0ba-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5c0ba-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c0ba-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0ba-123">Request body</span></span>
<span data-ttu-id="5c0ba-124">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c0ba-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="5c0ba-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c0ba-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="5c0ba-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c0ba-126">Property</span></span>|<span data-ttu-id="5c0ba-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c0ba-127">Type</span></span>|<span data-ttu-id="5c0ba-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c0ba-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c0ba-129">id</span><span class="sxs-lookup"><span data-stu-id="5c0ba-129">id</span></span>|<span data-ttu-id="5c0ba-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c0ba-130">String</span></span>|<span data-ttu-id="5c0ba-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-131">Key of the setting.</span></span> <span data-ttu-id="5c0ba-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c0ba-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c0ba-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5c0ba-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c0ba-134">DateTimeOffset</span></span>|<span data-ttu-id="5c0ba-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="5c0ba-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c0ba-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c0ba-137">createdDateTime</span></span>|<span data-ttu-id="5c0ba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c0ba-138">DateTimeOffset</span></span>|<span data-ttu-id="5c0ba-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-139">DateTime the object was created.</span></span> <span data-ttu-id="5c0ba-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c0ba-141">descrição</span><span class="sxs-lookup"><span data-stu-id="5c0ba-141">description</span></span>|<span data-ttu-id="5c0ba-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c0ba-142">String</span></span>|<span data-ttu-id="5c0ba-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c0ba-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c0ba-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5c0ba-145">displayName</span></span>|<span data-ttu-id="5c0ba-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c0ba-146">String</span></span>|<span data-ttu-id="5c0ba-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c0ba-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c0ba-149">version</span><span class="sxs-lookup"><span data-stu-id="5c0ba-149">version</span></span>|<span data-ttu-id="5c0ba-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5c0ba-150">Int32</span></span>|<span data-ttu-id="5c0ba-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-151">Version of the device configuration.</span></span> <span data-ttu-id="5c0ba-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c0ba-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c0ba-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="5c0ba-153">deliveryOptimizationMode</span></span>|<span data-ttu-id="5c0ba-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c0ba-154">String</span></span>|<span data-ttu-id="5c0ba-155">Os valores possíveis do modo de Otimização de Entrega são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-155">Delivery Optimization Mode Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="5c0ba-156">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="5c0ba-156">prereleaseFeatures</span></span>|<span data-ttu-id="5c0ba-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c0ba-157">String</span></span>|<span data-ttu-id="5c0ba-158">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-158">The pre-release features.</span></span> <span data-ttu-id="5c0ba-159">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-159">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="5c0ba-160">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="5c0ba-160">automaticUpdateMode</span></span>|<span data-ttu-id="5c0ba-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c0ba-161">String</span></span>|<span data-ttu-id="5c0ba-162">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-162">Automatic update mode.</span></span> <span data-ttu-id="5c0ba-163">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-163">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="5c0ba-164">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="5c0ba-164">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="5c0ba-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c0ba-165">Boolean</span></span>|<span data-ttu-id="5c0ba-166">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="5c0ba-166">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="5c0ba-167">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="5c0ba-167">driversExcluded</span></span>|<span data-ttu-id="5c0ba-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c0ba-168">Boolean</span></span>|<span data-ttu-id="5c0ba-169">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="5c0ba-169">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="5c0ba-170">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="5c0ba-170">installationSchedule</span></span>|[<span data-ttu-id="5c0ba-171">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="5c0ba-171">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="5c0ba-172">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="5c0ba-172">Installation schedule</span></span>|
|<span data-ttu-id="5c0ba-173">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="5c0ba-173">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="5c0ba-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5c0ba-174">Int32</span></span>|<span data-ttu-id="5c0ba-175">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="5c0ba-175">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="5c0ba-176">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="5c0ba-176">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="5c0ba-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5c0ba-177">Int32</span></span>|<span data-ttu-id="5c0ba-178">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="5c0ba-178">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="5c0ba-179">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="5c0ba-179">qualityUpdatesPaused</span></span>|<span data-ttu-id="5c0ba-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c0ba-180">Boolean</span></span>|<span data-ttu-id="5c0ba-181">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="5c0ba-181">Pause Quality Updates</span></span>|
|<span data-ttu-id="5c0ba-182">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="5c0ba-182">featureUpdatesPaused</span></span>|<span data-ttu-id="5c0ba-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c0ba-183">Boolean</span></span>|<span data-ttu-id="5c0ba-184">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="5c0ba-184">Pause Feature Updates</span></span>|
|<span data-ttu-id="5c0ba-185">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="5c0ba-185">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="5c0ba-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c0ba-186">DateTimeOffset</span></span>|<span data-ttu-id="5c0ba-187">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="5c0ba-187">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="5c0ba-188">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="5c0ba-188">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="5c0ba-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c0ba-189">DateTimeOffset</span></span>|<span data-ttu-id="5c0ba-190">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="5c0ba-190">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="5c0ba-191">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="5c0ba-191">businessReadyUpdatesOnly</span></span>|<span data-ttu-id="5c0ba-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c0ba-192">String</span></span>|<span data-ttu-id="5c0ba-193">Determina de qual ramificação os dispositivos receberão suas atualizações. Os valores possíveis são: `userDefined`, `all`, `businessReadyOnly`.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-193">Determines which branch devices will receive their updates from Possible values are: `userDefined`, `all`, `businessReadyOnly`.</span></span>|



## <a name="response"></a><span data-ttu-id="5c0ba-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c0ba-194">Response</span></span>
<span data-ttu-id="5c0ba-195">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-195">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c0ba-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c0ba-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c0ba-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0ba-197">Request</span></span>
<span data-ttu-id="5c0ba-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c0ba-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c0ba-199">Response</span></span>
<span data-ttu-id="5c0ba-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c0ba-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



