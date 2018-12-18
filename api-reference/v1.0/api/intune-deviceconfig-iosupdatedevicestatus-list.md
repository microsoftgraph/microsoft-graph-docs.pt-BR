---
title: Listar iosUpdateDeviceStatuses
description: Listar propriedades e relações dos objetos iosUpdateDeviceStatus.
author: tfitzmac
ms.openlocfilehash: a708fe9a8e27cafd3ffe96123b0cc88ce12c0a2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357929"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="0b40f-103">Listar iosUpdateDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0b40f-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="0b40f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0b40f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b40f-105">Listar propriedades e relações dos objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="0b40f-105">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b40f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b40f-106">Prerequisites</span></span>
<span data-ttu-id="0b40f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b40f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b40f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b40f-109">Permission type</span></span>|<span data-ttu-id="0b40f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b40f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b40f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b40f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b40f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b40f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0b40f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b40f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b40f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b40f-114">Not supported.</span></span>|
|<span data-ttu-id="0b40f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b40f-115">Application</span></span>|<span data-ttu-id="0b40f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b40f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b40f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b40f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0b40f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b40f-118">Request headers</span></span>
|<span data-ttu-id="0b40f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b40f-119">Header</span></span>|<span data-ttu-id="0b40f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0b40f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b40f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b40f-121">Authorization</span></span>|<span data-ttu-id="0b40f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b40f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b40f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0b40f-123">Accept</span></span>|<span data-ttu-id="0b40f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0b40f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b40f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b40f-125">Request body</span></span>
<span data-ttu-id="0b40f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b40f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b40f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b40f-127">Response</span></span>
<span data-ttu-id="0b40f-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b40f-128">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b40f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b40f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b40f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b40f-130">Request</span></span>
<span data-ttu-id="0b40f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b40f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="0b40f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b40f-132">Response</span></span>
<span data-ttu-id="0b40f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b40f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



