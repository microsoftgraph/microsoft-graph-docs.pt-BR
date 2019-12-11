---
title: Listar iosUpdateDeviceStatuses
description: Listar propriedades e relações dos objetos iosUpdateDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b65ed64a9449f09207a9493c3971a47b00e10ce2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948624"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="22cf2-103">Listar iosUpdateDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="22cf2-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="22cf2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22cf2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22cf2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22cf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22cf2-106">Listar propriedades e relações dos objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="22cf2-106">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22cf2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22cf2-107">Prerequisites</span></span>
<span data-ttu-id="22cf2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22cf2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22cf2-110">Permission type</span></span>|<span data-ttu-id="22cf2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22cf2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22cf2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22cf2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22cf2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22cf2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22cf2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22cf2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22cf2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22cf2-115">Not supported.</span></span>|
|<span data-ttu-id="22cf2-116">Application</span><span class="sxs-lookup"><span data-stu-id="22cf2-116">Application</span></span>|<span data-ttu-id="22cf2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22cf2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22cf2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22cf2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="22cf2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22cf2-119">Request headers</span></span>
|<span data-ttu-id="22cf2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22cf2-120">Header</span></span>|<span data-ttu-id="22cf2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="22cf2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22cf2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="22cf2-122">Authorization</span></span>|<span data-ttu-id="22cf2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22cf2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22cf2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22cf2-124">Accept</span></span>|<span data-ttu-id="22cf2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22cf2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22cf2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22cf2-126">Request body</span></span>
<span data-ttu-id="22cf2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22cf2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22cf2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="22cf2-128">Response</span></span>
<span data-ttu-id="22cf2-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22cf2-129">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22cf2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22cf2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="22cf2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22cf2-131">Request</span></span>
<span data-ttu-id="22cf2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22cf2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="22cf2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="22cf2-133">Response</span></span>
<span data-ttu-id="22cf2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22cf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

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
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





