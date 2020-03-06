---
title: Listar iosUpdateDeviceStatuses
description: Listar propriedades e relações dos objetos iosUpdateDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4650f1e9c8e89334e144b9d945f5e922b1a9c469
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514442"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="ed64d-103">Listar iosUpdateDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ed64d-103">List iosUpdateDeviceStatuses</span></span>

<span data-ttu-id="ed64d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed64d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed64d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed64d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed64d-106">Listar propriedades e relações dos objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ed64d-106">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed64d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed64d-107">Prerequisites</span></span>
<span data-ttu-id="ed64d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed64d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed64d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed64d-110">Permission type</span></span>|<span data-ttu-id="ed64d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed64d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed64d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed64d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed64d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed64d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ed64d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed64d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed64d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed64d-115">Not supported.</span></span>|
|<span data-ttu-id="ed64d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed64d-116">Application</span></span>|<span data-ttu-id="ed64d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed64d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed64d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed64d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ed64d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed64d-119">Request headers</span></span>
|<span data-ttu-id="ed64d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed64d-120">Header</span></span>|<span data-ttu-id="ed64d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ed64d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed64d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed64d-122">Authorization</span></span>|<span data-ttu-id="ed64d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed64d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed64d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed64d-124">Accept</span></span>|<span data-ttu-id="ed64d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed64d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed64d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed64d-126">Request body</span></span>
<span data-ttu-id="ed64d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed64d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed64d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed64d-128">Response</span></span>
<span data-ttu-id="ed64d-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed64d-129">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed64d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed64d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed64d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed64d-131">Request</span></span>
<span data-ttu-id="ed64d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed64d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="ed64d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed64d-133">Response</span></span>
<span data-ttu-id="ed64d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed64d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
    {
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
  ]
}
```




