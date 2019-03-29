---
title: Get managedDeviceOverview
description: Ler propriedades e relações do objeto managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b249899a5169ed181e017aef16c909998422f7e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977510"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="b8591-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b8591-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="b8591-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8591-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8591-105">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b8591-105">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8591-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8591-106">Prerequisites</span></span>
<span data-ttu-id="b8591-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8591-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8591-109">Permission type</span></span>|<span data-ttu-id="b8591-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8591-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8591-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8591-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8591-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8591-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b8591-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8591-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8591-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8591-114">Not supported.</span></span>|
|<span data-ttu-id="b8591-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8591-115">Application</span></span>|<span data-ttu-id="b8591-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8591-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8591-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8591-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8591-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8591-118">Optional query parameters</span></span>
<span data-ttu-id="b8591-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8591-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8591-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8591-120">Request headers</span></span>
|<span data-ttu-id="b8591-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8591-121">Header</span></span>|<span data-ttu-id="b8591-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8591-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8591-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8591-123">Authorization</span></span>|<span data-ttu-id="b8591-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8591-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8591-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8591-125">Accept</span></span>|<span data-ttu-id="b8591-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8591-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8591-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8591-127">Request body</span></span>
<span data-ttu-id="b8591-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8591-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8591-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8591-129">Response</span></span>
<span data-ttu-id="b8591-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8591-130">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8591-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8591-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8591-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8591-132">Request</span></span>
<span data-ttu-id="b8591-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8591-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="b8591-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8591-134">Response</span></span>
<span data-ttu-id="b8591-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8591-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



