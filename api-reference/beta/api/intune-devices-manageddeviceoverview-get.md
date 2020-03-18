---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6efbc640c14c31d3e9de308aa4b58d7d698d067d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773879"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="60480-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="60480-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="60480-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60480-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60480-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60480-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60480-106">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="60480-106">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60480-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60480-107">Prerequisites</span></span>
<span data-ttu-id="60480-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60480-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60480-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60480-110">Permission type</span></span>|<span data-ttu-id="60480-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60480-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60480-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60480-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60480-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="60480-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="60480-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60480-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60480-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60480-115">Not supported.</span></span>|
|<span data-ttu-id="60480-116">Application</span><span class="sxs-lookup"><span data-stu-id="60480-116">Application</span></span>|<span data-ttu-id="60480-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="60480-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60480-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60480-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60480-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="60480-119">Optional query parameters</span></span>
<span data-ttu-id="60480-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60480-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60480-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60480-121">Request headers</span></span>
|<span data-ttu-id="60480-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60480-122">Header</span></span>|<span data-ttu-id="60480-123">Valor</span><span class="sxs-lookup"><span data-stu-id="60480-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60480-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="60480-124">Authorization</span></span>|<span data-ttu-id="60480-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60480-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60480-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60480-126">Accept</span></span>|<span data-ttu-id="60480-127">application/json</span><span class="sxs-lookup"><span data-stu-id="60480-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60480-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60480-128">Request body</span></span>
<span data-ttu-id="60480-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60480-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60480-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="60480-130">Response</span></span>
<span data-ttu-id="60480-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60480-131">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60480-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60480-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="60480-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60480-133">Request</span></span>
<span data-ttu-id="60480-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60480-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="60480-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="60480-135">Response</span></span>
<span data-ttu-id="60480-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60480-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1320

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12,
      "androidDedicatedCount": 5,
      "androidDeviceAdminCount": 7,
      "androidFullyManagedCount": 8,
      "androidWorkProfileCount": 7,
      "configMgrDeviceCount": 4
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    },
    "managedDeviceModelsAndManufacturers": {
      "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
      "deviceModels": [
        "Device Models value"
      ],
      "deviceManufacturers": [
        "Device Manufacturers value"
      ]
    },
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




