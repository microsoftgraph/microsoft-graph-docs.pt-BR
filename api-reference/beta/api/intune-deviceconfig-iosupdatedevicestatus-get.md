---
title: Get iosUpdateDeviceStatus
description: Ler propriedades e relações do objeto iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61e4f7f9fdd6faf2fb6f2b9f5b75646cdf82b9f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155073"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="9e2af-103">Get iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="9e2af-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="9e2af-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e2af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e2af-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e2af-106">Ler propriedades e relações do objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9e2af-106">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e2af-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e2af-107">Prerequisites</span></span>
<span data-ttu-id="9e2af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9e2af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e2af-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e2af-110">Permission type</span></span>|<span data-ttu-id="9e2af-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e2af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e2af-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e2af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e2af-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e2af-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e2af-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e2af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e2af-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e2af-115">Not supported.</span></span>|
|<span data-ttu-id="9e2af-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e2af-116">Application</span></span>|<span data-ttu-id="9e2af-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e2af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e2af-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e2af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e2af-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e2af-119">Optional query parameters</span></span>
<span data-ttu-id="9e2af-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e2af-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e2af-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e2af-121">Request headers</span></span>
|<span data-ttu-id="9e2af-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e2af-122">Header</span></span>|<span data-ttu-id="9e2af-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9e2af-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e2af-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e2af-124">Authorization</span></span>|<span data-ttu-id="9e2af-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e2af-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e2af-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e2af-126">Accept</span></span>|<span data-ttu-id="9e2af-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9e2af-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e2af-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e2af-128">Request body</span></span>
<span data-ttu-id="9e2af-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e2af-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e2af-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e2af-130">Response</span></span>
<span data-ttu-id="9e2af-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e2af-131">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e2af-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e2af-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e2af-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e2af-133">Request</span></span>
<span data-ttu-id="9e2af-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e2af-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="9e2af-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e2af-135">Response</span></span>
<span data-ttu-id="9e2af-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e2af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
    "id": "63a79499-9499-63a7-9994-a7639994a763",
    "installStatus": "available",
    "osVersion": "Os Version value",
    "deviceId": "Device Id value",
    "userId": "User Id value",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




