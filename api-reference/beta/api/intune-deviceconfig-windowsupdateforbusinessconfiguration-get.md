---
title: Get windowsUpdateForBusinessConfiguration
description: Ler propriedades e relações do objeto windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64c8158cf69e6a763cf062067f81077d27c24fb5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991094"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="da7b3-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="da7b3-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="da7b3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da7b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da7b3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da7b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da7b3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="da7b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da7b3-107">Ler propriedades e relações do objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da7b3-107">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da7b3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da7b3-108">Prerequisites</span></span>
<span data-ttu-id="da7b3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da7b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da7b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da7b3-111">Permission type</span></span>|<span data-ttu-id="da7b3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da7b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da7b3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da7b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da7b3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="da7b3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="da7b3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da7b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da7b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da7b3-116">Not supported.</span></span>|
|<span data-ttu-id="da7b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da7b3-117">Application</span></span>|<span data-ttu-id="da7b3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da7b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da7b3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da7b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da7b3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da7b3-120">Optional query parameters</span></span>
<span data-ttu-id="da7b3-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da7b3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da7b3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da7b3-122">Request headers</span></span>
|<span data-ttu-id="da7b3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da7b3-123">Header</span></span>|<span data-ttu-id="da7b3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="da7b3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da7b3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="da7b3-125">Authorization</span></span>|<span data-ttu-id="da7b3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da7b3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da7b3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da7b3-127">Accept</span></span>|<span data-ttu-id="da7b3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da7b3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da7b3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da7b3-129">Request body</span></span>
<span data-ttu-id="da7b3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da7b3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da7b3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="da7b3-131">Response</span></span>
<span data-ttu-id="da7b3-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da7b3-132">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da7b3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da7b3-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="da7b3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da7b3-134">Request</span></span>
<span data-ttu-id="da7b3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da7b3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="da7b3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="da7b3-136">Response</span></span>
<span data-ttu-id="da7b3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da7b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2076

{
  "value": {
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
    "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
    "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
    "scheduleImminentRestartWarningInMinutes": 7
  }
}
```





