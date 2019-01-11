---
title: Atualizar windowsUpdateForBusinessConfiguration
description: Atualizar as propriedades de um objeto windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 55166d68f8f9f3044c89e798a650ce34fc00bb5e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867393"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="4072b-103">Atualizar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="4072b-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="4072b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4072b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4072b-105">Atualizar as propriedades de um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4072b-105">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4072b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4072b-106">Prerequisites</span></span>
<span data-ttu-id="4072b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4072b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4072b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4072b-109">Permission type</span></span>|<span data-ttu-id="4072b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4072b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4072b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4072b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4072b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4072b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4072b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4072b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4072b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4072b-114">Not supported.</span></span>|
|<span data-ttu-id="4072b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4072b-115">Application</span></span>|<span data-ttu-id="4072b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4072b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4072b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4072b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4072b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4072b-118">Request headers</span></span>
|<span data-ttu-id="4072b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4072b-119">Header</span></span>|<span data-ttu-id="4072b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4072b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4072b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4072b-121">Authorization</span></span>|<span data-ttu-id="4072b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4072b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4072b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4072b-123">Accept</span></span>|<span data-ttu-id="4072b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4072b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4072b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4072b-125">Request body</span></span>
<span data-ttu-id="4072b-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4072b-126">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="4072b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4072b-127">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="4072b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4072b-128">Property</span></span>|<span data-ttu-id="4072b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4072b-129">Type</span></span>|<span data-ttu-id="4072b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4072b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4072b-131">id</span><span class="sxs-lookup"><span data-stu-id="4072b-131">id</span></span>|<span data-ttu-id="4072b-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4072b-132">String</span></span>|<span data-ttu-id="4072b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4072b-133">Key of the entity.</span></span> <span data-ttu-id="4072b-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4072b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4072b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4072b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4072b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4072b-136">DateTimeOffset</span></span>|<span data-ttu-id="4072b-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4072b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4072b-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4072b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4072b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4072b-139">createdDateTime</span></span>|<span data-ttu-id="4072b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4072b-140">DateTimeOffset</span></span>|<span data-ttu-id="4072b-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4072b-141">DateTime the object was created.</span></span> <span data-ttu-id="4072b-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4072b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4072b-143">description</span><span class="sxs-lookup"><span data-stu-id="4072b-143">description</span></span>|<span data-ttu-id="4072b-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4072b-144">String</span></span>|<span data-ttu-id="4072b-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4072b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4072b-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4072b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4072b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4072b-147">displayName</span></span>|<span data-ttu-id="4072b-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4072b-148">String</span></span>|<span data-ttu-id="4072b-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4072b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4072b-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4072b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4072b-151">version</span><span class="sxs-lookup"><span data-stu-id="4072b-151">version</span></span>|<span data-ttu-id="4072b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4072b-152">Int32</span></span>|<span data-ttu-id="4072b-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4072b-153">Version of the device configuration.</span></span> <span data-ttu-id="4072b-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4072b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4072b-155">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4072b-155">deliveryOptimizationMode</span></span>|[<span data-ttu-id="4072b-156">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4072b-156">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="4072b-157">Modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="4072b-157">Delivery Optimization Mode.</span></span> <span data-ttu-id="4072b-158">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="4072b-158">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="4072b-159">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="4072b-159">prereleaseFeatures</span></span>|[<span data-ttu-id="4072b-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="4072b-160">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="4072b-161">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="4072b-161">The pre-release features.</span></span> <span data-ttu-id="4072b-162">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="4072b-162">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="4072b-163">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="4072b-163">automaticUpdateMode</span></span>|[<span data-ttu-id="4072b-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="4072b-164">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="4072b-165">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="4072b-165">Automatic update mode.</span></span> <span data-ttu-id="4072b-166">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="4072b-166">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="4072b-167">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="4072b-167">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="4072b-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="4072b-168">Boolean</span></span>|<span data-ttu-id="4072b-169">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="4072b-169">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="4072b-170">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="4072b-170">driversExcluded</span></span>|<span data-ttu-id="4072b-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="4072b-171">Boolean</span></span>|<span data-ttu-id="4072b-172">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="4072b-172">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="4072b-173">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="4072b-173">installationSchedule</span></span>|[<span data-ttu-id="4072b-174">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="4072b-174">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="4072b-175">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="4072b-175">Installation schedule</span></span>|
|<span data-ttu-id="4072b-176">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="4072b-176">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="4072b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4072b-177">Int32</span></span>|<span data-ttu-id="4072b-178">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="4072b-178">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="4072b-179">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="4072b-179">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="4072b-180">Int32</span><span class="sxs-lookup"><span data-stu-id="4072b-180">Int32</span></span>|<span data-ttu-id="4072b-181">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="4072b-181">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="4072b-182">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="4072b-182">qualityUpdatesPaused</span></span>|<span data-ttu-id="4072b-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="4072b-183">Boolean</span></span>|<span data-ttu-id="4072b-184">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="4072b-184">Pause Quality Updates</span></span>|
|<span data-ttu-id="4072b-185">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="4072b-185">featureUpdatesPaused</span></span>|<span data-ttu-id="4072b-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="4072b-186">Boolean</span></span>|<span data-ttu-id="4072b-187">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="4072b-187">Pause Feature Updates</span></span>|
|<span data-ttu-id="4072b-188">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="4072b-188">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="4072b-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4072b-189">DateTimeOffset</span></span>|<span data-ttu-id="4072b-190">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="4072b-190">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="4072b-191">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="4072b-191">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="4072b-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4072b-192">DateTimeOffset</span></span>|<span data-ttu-id="4072b-193">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="4072b-193">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="4072b-194">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="4072b-194">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="4072b-195">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="4072b-195">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="4072b-196">Determina quais dispositivos de filial receberão suas atualizações de.</span><span class="sxs-lookup"><span data-stu-id="4072b-196">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="4072b-197">Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="4072b-197">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="4072b-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="4072b-198">Response</span></span>
<span data-ttu-id="4072b-199">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4072b-199">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4072b-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4072b-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="4072b-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4072b-201">Request</span></span>
<span data-ttu-id="4072b-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4072b-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="4072b-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="4072b-203">Response</span></span>
<span data-ttu-id="4072b-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4072b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



