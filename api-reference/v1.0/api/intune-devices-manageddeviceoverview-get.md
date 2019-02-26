---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6284ab765df2bfc6060c9b95a76964cfbffa68a5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252417"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="e7f71-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e7f71-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="e7f71-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7f71-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7f71-105">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="e7f71-105">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7f71-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7f71-106">Prerequisites</span></span>
<span data-ttu-id="e7f71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7f71-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7f71-109">Permission type</span></span>|<span data-ttu-id="e7f71-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7f71-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7f71-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7f71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7f71-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7f71-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e7f71-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7f71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7f71-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7f71-114">Not supported.</span></span>|
|<span data-ttu-id="e7f71-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7f71-115">Application</span></span>|<span data-ttu-id="e7f71-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7f71-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7f71-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7f71-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7f71-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7f71-118">Optional query parameters</span></span>
<span data-ttu-id="e7f71-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7f71-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7f71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7f71-120">Request headers</span></span>
|<span data-ttu-id="e7f71-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7f71-121">Header</span></span>|<span data-ttu-id="e7f71-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e7f71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7f71-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7f71-123">Authorization</span></span>|<span data-ttu-id="e7f71-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7f71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7f71-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7f71-125">Accept</span></span>|<span data-ttu-id="e7f71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7f71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7f71-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7f71-127">Request body</span></span>
<span data-ttu-id="e7f71-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7f71-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7f71-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7f71-129">Response</span></span>
<span data-ttu-id="e7f71-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7f71-130">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7f71-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7f71-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7f71-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7f71-132">Request</span></span>
<span data-ttu-id="e7f71-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7f71-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="e7f71-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7f71-134">Response</span></span>
<span data-ttu-id="e7f71-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7f71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



