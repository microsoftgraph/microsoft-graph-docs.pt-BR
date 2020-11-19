---
title: Obter windowsDeliveryOptimizationConfiguration
description: Leia as propriedades e as relações do objeto windowsDeliveryOptimizationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 195f1c292c6db5cada6d8623c31b456e1f85b8ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49204135"
---
# <a name="get-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="0fbe9-103">Obter windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fbe9-103">Get windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="0fbe9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fbe9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fbe9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fbe9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fbe9-107">Leia as propriedades e as relações do objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0fbe9-107">Read properties and relationships of the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fbe9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0fbe9-108">Prerequisites</span></span>
<span data-ttu-id="0fbe9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fbe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fbe9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fbe9-111">Permission type</span></span>|<span data-ttu-id="0fbe9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0fbe9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fbe9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fbe9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fbe9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fbe9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0fbe9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fbe9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fbe9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-116">Not supported.</span></span>|
|<span data-ttu-id="0fbe9-117">Application</span><span class="sxs-lookup"><span data-stu-id="0fbe9-117">Application</span></span>|<span data-ttu-id="0fbe9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fbe9-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fbe9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fbe9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fbe9-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0fbe9-120">Optional query parameters</span></span>
<span data-ttu-id="0fbe9-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fbe9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fbe9-122">Request headers</span></span>
|<span data-ttu-id="0fbe9-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fbe9-123">Header</span></span>|<span data-ttu-id="0fbe9-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0fbe9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fbe9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fbe9-125">Authorization</span></span>|<span data-ttu-id="0fbe9-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fbe9-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0fbe9-127">Accept</span></span>|<span data-ttu-id="0fbe9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0fbe9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fbe9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fbe9-129">Request body</span></span>
<span data-ttu-id="0fbe9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fbe9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fbe9-131">Response</span></span>
<span data-ttu-id="0fbe9-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-132">If successful, this method returns a `200 OK` response code and [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fbe9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fbe9-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fbe9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fbe9-134">Request</span></span>
<span data-ttu-id="0fbe9-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0fbe9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fbe9-136">Response</span></span>
<span data-ttu-id="0fbe9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fbe9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2344

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
    "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
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
    "restrictPeerSelectionBy": "subnetMask",
    "groupIdSource": {
      "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
    },
    "bandwidthMode": {
      "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
    },
    "backgroundDownloadFromHttpDelayInSeconds": 8,
    "foregroundDownloadFromHttpDelayInSeconds": 8,
    "minimumRamAllowedToPeerInGigabytes": 2,
    "minimumDiskSizeAllowedToPeerInGigabytes": 7,
    "minimumFileSizeToCacheInMegabytes": 1,
    "minimumBatteryPercentageAllowedToUpload": 7,
    "modifyCacheLocation": "Modify Cache Location value",
    "maximumCacheAgeInDays": 5,
    "maximumCacheSize": {
      "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
    },
    "vpnPeerCaching": "enabled",
    "cacheServerHostNames": [
      "Cache Server Host Names value"
    ],
    "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
    "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
  }
}
```




