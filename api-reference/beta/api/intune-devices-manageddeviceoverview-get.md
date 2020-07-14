---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35b91b36bfaf190a69c8f4d78d717e5c71cb312a
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122704"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="30147-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="30147-103">Get managedDeviceOverview</span></span>

<span data-ttu-id="30147-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30147-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30147-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30147-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30147-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30147-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30147-107">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="30147-107">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30147-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30147-108">Prerequisites</span></span>
<span data-ttu-id="30147-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="30147-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="30147-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30147-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30147-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30147-111">Permission type</span></span>|<span data-ttu-id="30147-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30147-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30147-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30147-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30147-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="30147-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="30147-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30147-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30147-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30147-116">Not supported.</span></span>|
|<span data-ttu-id="30147-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30147-117">Application</span></span>|<span data-ttu-id="30147-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="30147-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30147-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30147-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30147-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30147-120">Optional query parameters</span></span>
<span data-ttu-id="30147-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30147-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30147-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30147-122">Request headers</span></span>
|<span data-ttu-id="30147-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30147-123">Header</span></span>|<span data-ttu-id="30147-124">Valor</span><span class="sxs-lookup"><span data-stu-id="30147-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30147-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="30147-125">Authorization</span></span>|<span data-ttu-id="30147-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30147-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30147-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30147-127">Accept</span></span>|<span data-ttu-id="30147-128">application/json</span><span class="sxs-lookup"><span data-stu-id="30147-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30147-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30147-129">Request body</span></span>
<span data-ttu-id="30147-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30147-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30147-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="30147-131">Response</span></span>
<span data-ttu-id="30147-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30147-132">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30147-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30147-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="30147-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30147-134">Request</span></span>
<span data-ttu-id="30147-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30147-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="30147-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="30147-136">Response</span></span>
<span data-ttu-id="30147-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="30147-137">Here is an example of the response.</span></span> <span data-ttu-id="30147-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="30147-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="30147-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="30147-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1366

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
      "androidCorporateWorkProfileCount": 0,
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



