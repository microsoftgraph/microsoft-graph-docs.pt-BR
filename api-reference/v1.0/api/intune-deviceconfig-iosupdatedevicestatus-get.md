---
title: Get iosUpdateDeviceStatus
description: Ler propriedades e relações do objeto iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ec6ef635955b0a2124dcc900a4c2c3131572410
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997579"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="e6499-103">Get iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="e6499-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="e6499-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6499-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6499-105">Ler propriedades e relações do objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="e6499-105">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6499-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6499-106">Prerequisites</span></span>
<span data-ttu-id="e6499-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6499-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6499-109">Permission type</span></span>|<span data-ttu-id="e6499-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6499-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6499-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6499-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6499-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6499-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e6499-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6499-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6499-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6499-114">Not supported.</span></span>|
|<span data-ttu-id="e6499-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6499-115">Application</span></span>|<span data-ttu-id="e6499-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6499-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6499-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6499-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6499-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e6499-118">Optional query parameters</span></span>
<span data-ttu-id="e6499-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e6499-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6499-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6499-120">Request headers</span></span>
|<span data-ttu-id="e6499-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6499-121">Header</span></span>|<span data-ttu-id="e6499-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e6499-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6499-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6499-123">Authorization</span></span>|<span data-ttu-id="e6499-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6499-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6499-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6499-125">Accept</span></span>|<span data-ttu-id="e6499-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6499-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6499-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6499-127">Request body</span></span>
<span data-ttu-id="e6499-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6499-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6499-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6499-129">Response</span></span>
<span data-ttu-id="e6499-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6499-130">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6499-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6499-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6499-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6499-132">Request</span></span>
<span data-ttu-id="e6499-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6499-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="e6499-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6499-134">Response</span></span>
<span data-ttu-id="e6499-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6499-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 646

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
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



