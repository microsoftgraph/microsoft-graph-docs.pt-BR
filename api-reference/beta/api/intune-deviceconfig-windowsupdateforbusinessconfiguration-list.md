---
title: Listar windowsUpdateForBusinessConfigurations
description: Listar propriedades e relações dos objetos windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21968a002c6677e001744d29699e31f4662b8576
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154634"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="ece34-103">Listar windowsUpdateForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="ece34-103">List windowsUpdateForBusinessConfigurations</span></span>

<span data-ttu-id="ece34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ece34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ece34-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ece34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ece34-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ece34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ece34-107">Listar propriedades e relações dos objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ece34-107">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ece34-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ece34-108">Prerequisites</span></span>
<span data-ttu-id="ece34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ece34-111">Permission type</span></span>|<span data-ttu-id="ece34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ece34-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ece34-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ece34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ece34-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece34-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ece34-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ece34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ece34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ece34-116">Not supported.</span></span>|
|<span data-ttu-id="ece34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ece34-117">Application</span></span>|<span data-ttu-id="ece34-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece34-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ece34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ece34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ece34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ece34-120">Request headers</span></span>
|<span data-ttu-id="ece34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ece34-121">Header</span></span>|<span data-ttu-id="ece34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ece34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ece34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ece34-123">Authorization</span></span>|<span data-ttu-id="ece34-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ece34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ece34-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ece34-125">Accept</span></span>|<span data-ttu-id="ece34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ece34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ece34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ece34-127">Request body</span></span>
<span data-ttu-id="ece34-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ece34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ece34-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ece34-129">Response</span></span>
<span data-ttu-id="ece34-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ece34-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ece34-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ece34-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ece34-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ece34-132">Request</span></span>
<span data-ttu-id="ece34-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ece34-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ece34-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ece34-134">Response</span></span>
<span data-ttu-id="ece34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ece34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3283

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
      "id": "4928dd6a-dd6a-4928-6add-28496add2849",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
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
      "businessReadyUpdatesOnly": "all",
      "skipChecksBeforeRestart": true,
      "updateWeeks": "firstWeek",
      "qualityUpdatesPauseStartDate": "2016-12-31",
      "featureUpdatesPauseStartDate": "2016-12-31",
      "featureUpdatesRollbackWindowInDays": 2,
      "qualityUpdatesWillBeRolledBack": true,
      "featureUpdatesWillBeRolledBack": true,
      "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
      "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
      "engagedRestartDeadlineInDays": 12,
      "engagedRestartSnoozeScheduleInDays": 2,
      "engagedRestartTransitionScheduleInDays": 6,
      "deadlineForFeatureUpdatesInDays": 15,
      "deadlineForQualityUpdatesInDays": 15,
      "deadlineGracePeriodInDays": 9,
      "postponeRebootUntilAfterDeadline": true,
      "autoRestartNotificationDismissal": "automatic",
      "scheduleRestartWarningInHours": 13,
      "scheduleImminentRestartWarningInMinutes": 7,
      "userPauseAccess": "enabled",
      "userWindowsUpdateScanAccess": "enabled",
      "updateNotificationLevel": "defaultNotifications"
    }
  ]
}
```




