---
title: Listar windowsDeliveryOptimizationConfigurations
description: Listar Propriedades e relações dos objetos windowsDeliveryOptimizationConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07cd6e87859d2d57982e4658e17a56c1fe07bf61
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962012"
---
# <a name="list-windowsdeliveryoptimizationconfigurations"></a><span data-ttu-id="85dc2-103">Listar windowsDeliveryOptimizationConfigurations</span><span class="sxs-lookup"><span data-stu-id="85dc2-103">List windowsDeliveryOptimizationConfigurations</span></span>

> <span data-ttu-id="85dc2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85dc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85dc2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85dc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85dc2-106">Listar Propriedades e relações dos objetos [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="85dc2-106">List properties and relationships of the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85dc2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85dc2-107">Prerequisites</span></span>
<span data-ttu-id="85dc2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85dc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85dc2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85dc2-110">Permission type</span></span>|<span data-ttu-id="85dc2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85dc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85dc2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85dc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85dc2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="85dc2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="85dc2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85dc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85dc2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85dc2-115">Not supported.</span></span>|
|<span data-ttu-id="85dc2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85dc2-116">Application</span></span>|<span data-ttu-id="85dc2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85dc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85dc2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85dc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="85dc2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85dc2-119">Request headers</span></span>
|<span data-ttu-id="85dc2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85dc2-120">Header</span></span>|<span data-ttu-id="85dc2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="85dc2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85dc2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="85dc2-122">Authorization</span></span>|<span data-ttu-id="85dc2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85dc2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85dc2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85dc2-124">Accept</span></span>|<span data-ttu-id="85dc2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85dc2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85dc2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85dc2-126">Request body</span></span>
<span data-ttu-id="85dc2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85dc2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85dc2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="85dc2-128">Response</span></span>
<span data-ttu-id="85dc2-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85dc2-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85dc2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85dc2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="85dc2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85dc2-131">Request</span></span>
<span data-ttu-id="85dc2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85dc2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="85dc2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="85dc2-133">Response</span></span>
<span data-ttu-id="85dc2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85dc2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1389

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
      "vpnPeerCaching": "enabled"
    }
  ]
}
```




