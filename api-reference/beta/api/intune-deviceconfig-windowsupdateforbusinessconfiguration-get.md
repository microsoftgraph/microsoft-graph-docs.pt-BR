---
title: Get windowsUpdateForBusinessConfiguration
description: Ler propriedades e relações do objeto windowsUpdateForBusinessConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6533189dc72f4a5e922ba575d6e44b56b88339de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393715"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="f426c-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="f426c-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="f426c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f426c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f426c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f426c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f426c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f426c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f426c-107">Ler propriedades e relações do objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f426c-107">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f426c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f426c-108">Prerequisites</span></span>
<span data-ttu-id="f426c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f426c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f426c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f426c-111">Permission type</span></span>|<span data-ttu-id="f426c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f426c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f426c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f426c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f426c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f426c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f426c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f426c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f426c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f426c-116">Not supported.</span></span>|
|<span data-ttu-id="f426c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f426c-117">Application</span></span>|<span data-ttu-id="f426c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f426c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f426c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f426c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f426c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f426c-120">Optional query parameters</span></span>
<span data-ttu-id="f426c-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f426c-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f426c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f426c-122">Request headers</span></span>
|<span data-ttu-id="f426c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f426c-123">Header</span></span>|<span data-ttu-id="f426c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f426c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f426c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f426c-125">Authorization</span></span>|<span data-ttu-id="f426c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f426c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f426c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f426c-127">Accept</span></span>|<span data-ttu-id="f426c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f426c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f426c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f426c-129">Request body</span></span>
<span data-ttu-id="f426c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f426c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f426c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f426c-131">Response</span></span>
<span data-ttu-id="f426c-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f426c-132">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f426c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f426c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f426c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f426c-134">Request</span></span>
<span data-ttu-id="f426c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f426c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f426c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f426c-136">Response</span></span>
<span data-ttu-id="f426c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f426c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2083

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
    "userPauseAccess": "enabled"
  }
}
```




