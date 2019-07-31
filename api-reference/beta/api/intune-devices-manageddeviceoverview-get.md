---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 36ca13e182e5a7e1a8e84b2d4af15a4090e15835
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987086"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="330b5-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="330b5-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="330b5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="330b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="330b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="330b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="330b5-106">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="330b5-106">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="330b5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="330b5-107">Prerequisites</span></span>
<span data-ttu-id="330b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="330b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="330b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="330b5-110">Permission type</span></span>|<span data-ttu-id="330b5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="330b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="330b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="330b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="330b5-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="330b5-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="330b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="330b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="330b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="330b5-115">Not supported.</span></span>|
|<span data-ttu-id="330b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="330b5-116">Application</span></span>|<span data-ttu-id="330b5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="330b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="330b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="330b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="330b5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="330b5-119">Optional query parameters</span></span>
<span data-ttu-id="330b5-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="330b5-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="330b5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="330b5-121">Request headers</span></span>
|<span data-ttu-id="330b5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="330b5-122">Header</span></span>|<span data-ttu-id="330b5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="330b5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="330b5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="330b5-124">Authorization</span></span>|<span data-ttu-id="330b5-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="330b5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="330b5-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="330b5-126">Accept</span></span>|<span data-ttu-id="330b5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="330b5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="330b5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="330b5-128">Request body</span></span>
<span data-ttu-id="330b5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="330b5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="330b5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="330b5-130">Response</span></span>
<span data-ttu-id="330b5-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="330b5-131">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="330b5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="330b5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="330b5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330b5-133">Request</span></span>
<span data-ttu-id="330b5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="330b5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="330b5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="330b5-135">Response</span></span>
<span data-ttu-id="330b5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="330b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1139

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
      "unknownCount": 12
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





