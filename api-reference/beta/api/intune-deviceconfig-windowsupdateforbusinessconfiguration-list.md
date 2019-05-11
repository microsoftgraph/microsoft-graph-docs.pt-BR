---
title: Listar windowsUpdateForBusinessConfigurations
description: Listar propriedades e relações dos objetos windowsUpdateForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41e8f334ac9da841df572944f0274c6ccf528362
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917355"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="90c0e-103">Listar windowsUpdateForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="90c0e-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="90c0e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90c0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90c0e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90c0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90c0e-106">Listar propriedades e relações dos objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90c0e-106">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90c0e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90c0e-107">Prerequisites</span></span>
<span data-ttu-id="90c0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c0e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90c0e-110">Permission type</span></span>|<span data-ttu-id="90c0e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90c0e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90c0e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90c0e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90c0e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90c0e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90c0e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90c0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90c0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90c0e-115">Not supported.</span></span>|
|<span data-ttu-id="90c0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90c0e-116">Application</span></span>|<span data-ttu-id="90c0e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90c0e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90c0e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90c0e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90c0e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90c0e-119">Request headers</span></span>
|<span data-ttu-id="90c0e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90c0e-120">Header</span></span>|<span data-ttu-id="90c0e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90c0e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90c0e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90c0e-122">Authorization</span></span>|<span data-ttu-id="90c0e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90c0e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90c0e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90c0e-124">Accept</span></span>|<span data-ttu-id="90c0e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90c0e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90c0e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90c0e-126">Request body</span></span>
<span data-ttu-id="90c0e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90c0e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90c0e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="90c0e-128">Response</span></span>
<span data-ttu-id="90c0e-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90c0e-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90c0e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90c0e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90c0e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90c0e-131">Request</span></span>
<span data-ttu-id="90c0e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90c0e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="90c0e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="90c0e-133">Response</span></span>
<span data-ttu-id="90c0e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90c0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2292

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




