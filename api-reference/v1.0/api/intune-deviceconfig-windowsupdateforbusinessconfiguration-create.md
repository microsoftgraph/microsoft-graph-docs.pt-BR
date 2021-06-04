---
title: Criar windowsUpdateForBusinessConfiguration
description: Cria um novo objeto windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e47aa6db924d18e1c6f84bedf877722ec4e6521
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753787"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="5dacd-103">Criar windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="5dacd-103">Create windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="5dacd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dacd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5dacd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5dacd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dacd-106">Cria um novo objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5dacd-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dacd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5dacd-107">Prerequisites</span></span>
<span data-ttu-id="5dacd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dacd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dacd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dacd-110">Permission type</span></span>|<span data-ttu-id="5dacd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dacd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dacd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dacd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5dacd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dacd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5dacd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dacd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dacd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dacd-115">Not supported.</span></span>|
|<span data-ttu-id="5dacd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dacd-116">Application</span></span>|<span data-ttu-id="5dacd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dacd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dacd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dacd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5dacd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dacd-119">Request headers</span></span>
|<span data-ttu-id="5dacd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5dacd-120">Header</span></span>|<span data-ttu-id="5dacd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5dacd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dacd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dacd-122">Authorization</span></span>|<span data-ttu-id="5dacd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dacd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dacd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5dacd-124">Accept</span></span>|<span data-ttu-id="5dacd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5dacd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dacd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dacd-126">Request body</span></span>
<span data-ttu-id="5dacd-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5dacd-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="5dacd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5dacd-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="5dacd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dacd-129">Property</span></span>|<span data-ttu-id="5dacd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dacd-130">Type</span></span>|<span data-ttu-id="5dacd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dacd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dacd-132">id</span><span class="sxs-lookup"><span data-stu-id="5dacd-132">id</span></span>|<span data-ttu-id="5dacd-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dacd-133">String</span></span>|<span data-ttu-id="5dacd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5dacd-134">Key of the entity.</span></span> <span data-ttu-id="5dacd-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dacd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dacd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dacd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5dacd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dacd-137">DateTimeOffset</span></span>|<span data-ttu-id="5dacd-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5dacd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5dacd-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dacd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dacd-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5dacd-140">createdDateTime</span></span>|<span data-ttu-id="5dacd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dacd-141">DateTimeOffset</span></span>|<span data-ttu-id="5dacd-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5dacd-142">DateTime the object was created.</span></span> <span data-ttu-id="5dacd-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dacd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dacd-144">descrição</span><span class="sxs-lookup"><span data-stu-id="5dacd-144">description</span></span>|<span data-ttu-id="5dacd-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dacd-145">String</span></span>|<span data-ttu-id="5dacd-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5dacd-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5dacd-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dacd-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dacd-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5dacd-148">displayName</span></span>|<span data-ttu-id="5dacd-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dacd-149">String</span></span>|<span data-ttu-id="5dacd-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5dacd-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5dacd-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dacd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dacd-152">versão</span><span class="sxs-lookup"><span data-stu-id="5dacd-152">version</span></span>|<span data-ttu-id="5dacd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5dacd-153">Int32</span></span>|<span data-ttu-id="5dacd-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5dacd-154">Version of the device configuration.</span></span> <span data-ttu-id="5dacd-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dacd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dacd-156">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="5dacd-156">deliveryOptimizationMode</span></span>|[<span data-ttu-id="5dacd-157">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="5dacd-157">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="5dacd-158">Modo de Otimização de Entrega.</span><span class="sxs-lookup"><span data-stu-id="5dacd-158">Delivery Optimization Mode.</span></span> <span data-ttu-id="5dacd-159">Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="5dacd-159">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="5dacd-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="5dacd-160">prereleaseFeatures</span></span>|[<span data-ttu-id="5dacd-161">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="5dacd-161">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="5dacd-162">Os recursos de pré-lançamento.</span><span class="sxs-lookup"><span data-stu-id="5dacd-162">The pre-release features.</span></span> <span data-ttu-id="5dacd-163">Os valores possíveis são: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="5dacd-163">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="5dacd-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="5dacd-164">automaticUpdateMode</span></span>|[<span data-ttu-id="5dacd-165">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="5dacd-165">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="5dacd-166">Modo de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="5dacd-166">Automatic update mode.</span></span> <span data-ttu-id="5dacd-167">Os valores possíveis são: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="5dacd-167">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="5dacd-168">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="5dacd-168">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="5dacd-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dacd-169">Boolean</span></span>|<span data-ttu-id="5dacd-170">Permitir serviço Microsoft Update</span><span class="sxs-lookup"><span data-stu-id="5dacd-170">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="5dacd-171">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="5dacd-171">driversExcluded</span></span>|<span data-ttu-id="5dacd-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dacd-172">Boolean</span></span>|<span data-ttu-id="5dacd-173">Excluir drivers de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="5dacd-173">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="5dacd-174">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="5dacd-174">installationSchedule</span></span>|[<span data-ttu-id="5dacd-175">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="5dacd-175">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="5dacd-176">Cronograma de instalação</span><span class="sxs-lookup"><span data-stu-id="5dacd-176">Installation schedule</span></span>|
|<span data-ttu-id="5dacd-177">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="5dacd-177">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="5dacd-178">Int32</span><span class="sxs-lookup"><span data-stu-id="5dacd-178">Int32</span></span>|<span data-ttu-id="5dacd-179">Aditar atualizações de qualidade por este número de dias</span><span class="sxs-lookup"><span data-stu-id="5dacd-179">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="5dacd-180">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="5dacd-180">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="5dacd-181">Int32</span><span class="sxs-lookup"><span data-stu-id="5dacd-181">Int32</span></span>|<span data-ttu-id="5dacd-182">Aditar atualizações de recursos por este número de dias</span><span class="sxs-lookup"><span data-stu-id="5dacd-182">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="5dacd-183">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="5dacd-183">qualityUpdatesPaused</span></span>|<span data-ttu-id="5dacd-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dacd-184">Boolean</span></span>|<span data-ttu-id="5dacd-185">Pausar atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="5dacd-185">Pause Quality Updates</span></span>|
|<span data-ttu-id="5dacd-186">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="5dacd-186">featureUpdatesPaused</span></span>|<span data-ttu-id="5dacd-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dacd-187">Boolean</span></span>|<span data-ttu-id="5dacd-188">Pausar atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="5dacd-188">Pause Feature Updates</span></span>|
|<span data-ttu-id="5dacd-189">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="5dacd-189">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="5dacd-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dacd-190">DateTimeOffset</span></span>|<span data-ttu-id="5dacd-191">Data e hora de expiração da pausa de atualizações de qualidade</span><span class="sxs-lookup"><span data-stu-id="5dacd-191">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="5dacd-192">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="5dacd-192">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="5dacd-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dacd-193">DateTimeOffset</span></span>|<span data-ttu-id="5dacd-194">Data e hora de expiração da pausa de atualizações de recursos</span><span class="sxs-lookup"><span data-stu-id="5dacd-194">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="5dacd-195">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="5dacd-195">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="5dacd-196">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="5dacd-196">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="5dacd-197">Determina de quais dispositivos de filial receberão suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="5dacd-197">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="5dacd-198">Os possíveis valores são: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="5dacd-198">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="5dacd-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dacd-199">Response</span></span>
<span data-ttu-id="5dacd-200">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dacd-200">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dacd-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dacd-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dacd-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dacd-202">Request</span></span>
<span data-ttu-id="5dacd-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dacd-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5dacd-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dacd-204">Response</span></span>
<span data-ttu-id="5dacd-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dacd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




