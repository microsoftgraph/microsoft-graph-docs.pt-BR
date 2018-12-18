---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: tfitzmac
ms.openlocfilehash: c3d76e1b07e46245a3e4d391d5f44d04a84399a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359784"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="fe1e1-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fe1e1-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="fe1e1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe1e1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe1e1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe1e1-107">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="fe1e1-107">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe1e1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe1e1-108">Prerequisites</span></span>
<span data-ttu-id="fe1e1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe1e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe1e1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe1e1-111">Permission type</span></span>|<span data-ttu-id="fe1e1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe1e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe1e1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe1e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe1e1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe1e1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fe1e1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe1e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe1e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-116">Not supported.</span></span>|
|<span data-ttu-id="fe1e1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe1e1-117">Application</span></span>|<span data-ttu-id="fe1e1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe1e1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe1e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe1e1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe1e1-120">Optional query parameters</span></span>
<span data-ttu-id="fe1e1-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fe1e1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1e1-122">Request headers</span></span>
|<span data-ttu-id="fe1e1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe1e1-123">Header</span></span>|<span data-ttu-id="fe1e1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fe1e1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe1e1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe1e1-125">Authorization</span></span>|<span data-ttu-id="fe1e1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe1e1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fe1e1-127">Accept</span></span>|<span data-ttu-id="fe1e1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fe1e1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe1e1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1e1-129">Request body</span></span>
<span data-ttu-id="fe1e1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe1e1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe1e1-131">Response</span></span>
<span data-ttu-id="fe1e1-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-132">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe1e1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe1e1-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe1e1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1e1-134">Request</span></span>
<span data-ttu-id="fe1e1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="fe1e1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe1e1-136">Response</span></span>
<span data-ttu-id="fe1e1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe1e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





