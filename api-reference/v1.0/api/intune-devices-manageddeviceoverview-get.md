---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75e96b633a43d8ba95ab4792c089c3549be1d981
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513438"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="cc0b0-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="cc0b0-103">Get managedDeviceOverview</span></span>

<span data-ttu-id="cc0b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc0b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc0b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc0b0-106">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="cc0b0-106">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc0b0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc0b0-107">Prerequisites</span></span>
<span data-ttu-id="cc0b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc0b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc0b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc0b0-110">Permission type</span></span>|<span data-ttu-id="cc0b0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc0b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc0b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc0b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc0b0-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc0b0-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cc0b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc0b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc0b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-115">Not supported.</span></span>|
|<span data-ttu-id="cc0b0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc0b0-116">Application</span></span>|<span data-ttu-id="cc0b0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc0b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc0b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc0b0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc0b0-119">Optional query parameters</span></span>
<span data-ttu-id="cc0b0-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc0b0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0b0-121">Request headers</span></span>
|<span data-ttu-id="cc0b0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc0b0-122">Header</span></span>|<span data-ttu-id="cc0b0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cc0b0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc0b0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc0b0-124">Authorization</span></span>|<span data-ttu-id="cc0b0-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc0b0-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc0b0-126">Accept</span></span>|<span data-ttu-id="cc0b0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cc0b0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc0b0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0b0-128">Request body</span></span>
<span data-ttu-id="cc0b0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc0b0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc0b0-130">Response</span></span>
<span data-ttu-id="cc0b0-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-131">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc0b0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc0b0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc0b0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0b0-133">Request</span></span>
<span data-ttu-id="cc0b0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="cc0b0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc0b0-135">Response</span></span>
<span data-ttu-id="cc0b0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc0b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




