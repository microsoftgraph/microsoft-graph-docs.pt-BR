---
title: Listar windowsUpdateForBusinessConfigurations
description: Listar propriedades e relações dos objetos windowsUpdateForBusinessConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03264c9085190e62cea570219956c7f77b4c3b77
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42732143"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="5167b-103">Listar windowsUpdateForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="5167b-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="5167b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5167b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5167b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5167b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5167b-106">Listar propriedades e relações dos objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5167b-106">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5167b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5167b-107">Prerequisites</span></span>
<span data-ttu-id="5167b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5167b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5167b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5167b-110">Permission type</span></span>|<span data-ttu-id="5167b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5167b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5167b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5167b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5167b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5167b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5167b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5167b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5167b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5167b-115">Not supported.</span></span>|
|<span data-ttu-id="5167b-116">Application</span><span class="sxs-lookup"><span data-stu-id="5167b-116">Application</span></span>|<span data-ttu-id="5167b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5167b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5167b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5167b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5167b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5167b-119">Request headers</span></span>
|<span data-ttu-id="5167b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5167b-120">Header</span></span>|<span data-ttu-id="5167b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5167b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5167b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5167b-122">Authorization</span></span>|<span data-ttu-id="5167b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5167b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5167b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5167b-124">Accept</span></span>|<span data-ttu-id="5167b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5167b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5167b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5167b-126">Request body</span></span>
<span data-ttu-id="5167b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5167b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5167b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5167b-128">Response</span></span>
<span data-ttu-id="5167b-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5167b-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5167b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5167b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5167b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5167b-131">Request</span></span>
<span data-ttu-id="5167b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5167b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5167b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5167b-133">Response</span></span>
<span data-ttu-id="5167b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5167b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3329

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
      "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
      "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
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




