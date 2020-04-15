---
title: Listar iosUpdateDeviceStatuses
description: Listar propriedades e relações dos objetos iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1daed1064108f37df74eb2312251a905078691dd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446095"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="aa421-103">Listar iosUpdateDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="aa421-103">List iosUpdateDeviceStatuses</span></span>

<span data-ttu-id="aa421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa421-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa421-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa421-106">Listar propriedades e relações dos objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="aa421-106">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa421-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa421-107">Prerequisites</span></span>
<span data-ttu-id="aa421-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa421-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa421-110">Permission type</span></span>|<span data-ttu-id="aa421-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa421-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa421-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa421-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa421-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa421-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aa421-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa421-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa421-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa421-115">Not supported.</span></span>|
|<span data-ttu-id="aa421-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa421-116">Application</span></span>|<span data-ttu-id="aa421-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa421-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa421-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa421-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="aa421-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa421-119">Request headers</span></span>
|<span data-ttu-id="aa421-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa421-120">Header</span></span>|<span data-ttu-id="aa421-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aa421-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa421-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa421-122">Authorization</span></span>|<span data-ttu-id="aa421-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa421-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa421-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa421-124">Accept</span></span>|<span data-ttu-id="aa421-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa421-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa421-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa421-126">Request body</span></span>
<span data-ttu-id="aa421-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa421-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa421-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa421-128">Response</span></span>
<span data-ttu-id="aa421-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa421-129">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa421-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa421-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa421-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa421-131">Request</span></span>
<span data-ttu-id="aa421-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa421-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="aa421-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa421-133">Response</span></span>
<span data-ttu-id="aa421-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa421-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






