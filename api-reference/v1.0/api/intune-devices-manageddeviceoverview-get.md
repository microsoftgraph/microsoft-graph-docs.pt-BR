---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4515c143de30007104c7addfb148a9965118caad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826380"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="c62a9-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c62a9-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="c62a9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c62a9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c62a9-105">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="c62a9-105">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c62a9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c62a9-106">Prerequisites</span></span>
<span data-ttu-id="c62a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c62a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c62a9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c62a9-109">Permission type</span></span>|<span data-ttu-id="c62a9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c62a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c62a9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c62a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c62a9-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62a9-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c62a9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c62a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c62a9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c62a9-114">Not supported.</span></span>|
|<span data-ttu-id="c62a9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c62a9-115">Application</span></span>|<span data-ttu-id="c62a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c62a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c62a9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c62a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c62a9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c62a9-118">Optional query parameters</span></span>
<span data-ttu-id="c62a9-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c62a9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c62a9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c62a9-120">Request headers</span></span>
|<span data-ttu-id="c62a9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c62a9-121">Header</span></span>|<span data-ttu-id="c62a9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c62a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c62a9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c62a9-123">Authorization</span></span>|<span data-ttu-id="c62a9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c62a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c62a9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c62a9-125">Accept</span></span>|<span data-ttu-id="c62a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c62a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c62a9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c62a9-127">Request body</span></span>
<span data-ttu-id="c62a9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c62a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c62a9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c62a9-129">Response</span></span>
<span data-ttu-id="c62a9-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c62a9-130">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c62a9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c62a9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c62a9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c62a9-132">Request</span></span>
<span data-ttu-id="c62a9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c62a9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="c62a9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c62a9-134">Response</span></span>
<span data-ttu-id="c62a9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c62a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

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
    }
  }
}
```



