---
title: Criar windowsUpdateForBusinessConfiguration
description: Cria um novo objeto windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c95b51348f839d0ff19c8cc17d8516c6fd38620
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388920"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="22f94-103">Criar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="22f94-103">Create windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="22f94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22f94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22f94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22f94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f94-106">Cria um novo objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22f94-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22f94-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22f94-107">Prerequisites</span></span>
<span data-ttu-id="22f94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22f94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22f94-110">Permission type</span></span>|<span data-ttu-id="22f94-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22f94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22f94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22f94-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22f94-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22f94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22f94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22f94-115">Not supported.</span></span>|
|<span data-ttu-id="22f94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22f94-116">Application</span></span>|<span data-ttu-id="22f94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22f94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22f94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22f94-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22f94-119">Request headers</span></span>
|<span data-ttu-id="22f94-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22f94-120">Header</span></span>|<span data-ttu-id="22f94-121">Valor</span><span class="sxs-lookup"><span data-stu-id="22f94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f94-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="22f94-122">Authorization</span></span>|<span data-ttu-id="22f94-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22f94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f94-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22f94-124">Accept</span></span>|<span data-ttu-id="22f94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22f94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f94-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22f94-126">Request body</span></span>
<span data-ttu-id="22f94-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22f94-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="22f94-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22f94-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="22f94-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22f94-129">Property</span></span>|<span data-ttu-id="22f94-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="22f94-130">Type</span></span>|<span data-ttu-id="22f94-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="22f94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22f94-132">id</span><span class="sxs-lookup"><span data-stu-id="22f94-132">id</span></span>|<span data-ttu-id="22f94-133">String</span><span class="sxs-lookup"><span data-stu-id="22f94-133">String</span></span>|<span data-ttu-id="22f94-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22f94-134">Key of the entity.</span></span> <span data-ttu-id="22f94-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f94-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f94-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22f94-136">lastModifiedDateTime</span></span>|<span data-ttu-id="22f94-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f94-137">DateTimeOffset</span></span>|<span data-ttu-id="22f94-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="22f94-138">DateTime the object was last modified.</span></span> <span data-ttu-id="22f94-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f94-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f94-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22f94-140">createdDateTime</span></span>|<span data-ttu-id="22f94-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f94-141">DateTimeOffset</span></span>|<span data-ttu-id="22f94-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="22f94-142">DateTime the object was created.</span></span> <span data-ttu-id="22f94-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f94-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f94-144">description</span><span class="sxs-lookup"><span data-stu-id="22f94-144">description</span></span>|<span data-ttu-id="22f94-145">String</span><span class="sxs-lookup"><span data-stu-id="22f94-145">String</span></span>|<span data-ttu-id="22f94-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22f94-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22f94-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f94-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f94-148">displayName</span><span class="sxs-lookup"><span data-stu-id="22f94-148">displayName</span></span>|<span data-ttu-id="22f94-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22f94-149">String</span></span>|<span data-ttu-id="22f94-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22f94-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22f94-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f94-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f94-152">versão</span><span class="sxs-lookup"><span data-stu-id="22f94-152">version</span></span>|<span data-ttu-id="22f94-153">Int32</span><span class="sxs-lookup"><span data-stu-id="22f94-153">Int32</span></span>|<span data-ttu-id="22f94-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22f94-154">Version of the device configuration.</span></span> <span data-ttu-id="22f94-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22f94-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22f94-156">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="22f94-156">deliveryOptimizationMode</span></span>|[<span data-ttu-id="22f94-157">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="22f94-157">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="22f94-158">Modo de otimização de entrega.</span><span class="sxs-lookup"><span data-stu-id="22f94-158">Delivery Optimization Mode.</span></span> <span data-ttu-id="22f94-159">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="22f94-159">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="22f94-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="22f94-160">prereleaseFeatures</span></span>|[<span data-ttu-id="22f94-161">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="22f94-161">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="22f94-162">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="22f94-162">The pre-release features.</span></span> <span data-ttu-id="22f94-163">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="22f94-163">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="22f94-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="22f94-164">automaticUpdateMode</span></span>|[<span data-ttu-id="22f94-165">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="22f94-165">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="22f94-166">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="22f94-166">Automatic update mode.</span></span> <span data-ttu-id="22f94-167">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="22f94-167">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="22f94-168">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="22f94-168">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="22f94-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="22f94-169">Boolean</span></span>|<span data-ttu-id="22f94-170">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="22f94-170">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="22f94-171">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="22f94-171">driversExcluded</span></span>|<span data-ttu-id="22f94-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="22f94-172">Boolean</span></span>|<span data-ttu-id="22f94-173">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="22f94-173">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="22f94-174">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="22f94-174">installationSchedule</span></span>|[<span data-ttu-id="22f94-175">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="22f94-175">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="22f94-176">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="22f94-176">Installation schedule</span></span>|
|<span data-ttu-id="22f94-177">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="22f94-177">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="22f94-178">Int32</span><span class="sxs-lookup"><span data-stu-id="22f94-178">Int32</span></span>|<span data-ttu-id="22f94-179">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="22f94-179">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="22f94-180">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="22f94-180">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="22f94-181">Int32</span><span class="sxs-lookup"><span data-stu-id="22f94-181">Int32</span></span>|<span data-ttu-id="22f94-182">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="22f94-182">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="22f94-183">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="22f94-183">qualityUpdatesPaused</span></span>|<span data-ttu-id="22f94-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="22f94-184">Boolean</span></span>|<span data-ttu-id="22f94-185">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="22f94-185">Pause Quality Updates</span></span>|
|<span data-ttu-id="22f94-186">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="22f94-186">featureUpdatesPaused</span></span>|<span data-ttu-id="22f94-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="22f94-187">Boolean</span></span>|<span data-ttu-id="22f94-188">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="22f94-188">Pause Feature Updates</span></span>|
|<span data-ttu-id="22f94-189">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="22f94-189">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="22f94-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f94-190">DateTimeOffset</span></span>|<span data-ttu-id="22f94-191">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="22f94-191">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="22f94-192">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="22f94-192">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="22f94-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22f94-193">DateTimeOffset</span></span>|<span data-ttu-id="22f94-194">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="22f94-194">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="22f94-195">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="22f94-195">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="22f94-196">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="22f94-196">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="22f94-197">Determina quais dispositivos de filial receberão suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="22f94-197">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="22f94-198">Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="22f94-198">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="22f94-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f94-199">Response</span></span>
<span data-ttu-id="22f94-200">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22f94-200">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f94-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22f94-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="22f94-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22f94-202">Request</span></span>
<span data-ttu-id="22f94-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22f94-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22f94-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f94-204">Response</span></span>
<span data-ttu-id="22f94-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22f94-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






