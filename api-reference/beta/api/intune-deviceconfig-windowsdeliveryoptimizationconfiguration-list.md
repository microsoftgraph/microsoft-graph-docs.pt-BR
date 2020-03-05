---
title: Listar windowsDeliveryOptimizationConfigurations
description: Listar Propriedades e relações dos objetos windowsDeliveryOptimizationConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8bbf72c115077bea5d6670021ef684663ea5be08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42476178"
---
# <a name="list-windowsdeliveryoptimizationconfigurations"></a><span data-ttu-id="64f12-103">Listar windowsDeliveryOptimizationConfigurations</span><span class="sxs-lookup"><span data-stu-id="64f12-103">List windowsDeliveryOptimizationConfigurations</span></span>

<span data-ttu-id="64f12-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64f12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64f12-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64f12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64f12-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64f12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f12-107">Listar Propriedades e relações dos objetos [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64f12-107">List properties and relationships of the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64f12-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64f12-108">Prerequisites</span></span>
<span data-ttu-id="64f12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64f12-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64f12-111">Permission type</span></span>|<span data-ttu-id="64f12-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="64f12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64f12-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64f12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64f12-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64f12-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="64f12-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64f12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64f12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64f12-116">Not supported.</span></span>|
|<span data-ttu-id="64f12-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64f12-117">Application</span></span>|<span data-ttu-id="64f12-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="64f12-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64f12-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64f12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64f12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64f12-120">Request headers</span></span>
|<span data-ttu-id="64f12-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64f12-121">Header</span></span>|<span data-ttu-id="64f12-122">Valor</span><span class="sxs-lookup"><span data-stu-id="64f12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64f12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64f12-123">Authorization</span></span>|<span data-ttu-id="64f12-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64f12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64f12-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64f12-125">Accept</span></span>|<span data-ttu-id="64f12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64f12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64f12-127">Request body</span></span>
<span data-ttu-id="64f12-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64f12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64f12-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f12-129">Response</span></span>
<span data-ttu-id="64f12-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64f12-130">If successful, this method returns a `200 OK` response code and a collection of [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f12-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64f12-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="64f12-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64f12-132">Request</span></span>
<span data-ttu-id="64f12-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64f12-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="64f12-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f12-134">Response</span></span>
<span data-ttu-id="64f12-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64f12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2472

{
  "value": [
    {
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
  ]
}
```





