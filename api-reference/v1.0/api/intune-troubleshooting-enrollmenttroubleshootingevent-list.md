---
title: Listar enrollmentTroubleshootingEvents
description: Lista propriedades e relações dos objetos enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8dd03acd651a4a54891a2f5245cff32e1ae308fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023234"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="d1487-103">Listar enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="d1487-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="d1487-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1487-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1487-105">Lista propriedades e relações dos objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d1487-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1487-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1487-106">Prerequisites</span></span>
<span data-ttu-id="d1487-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1487-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1487-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1487-109">Permission type</span></span>|<span data-ttu-id="d1487-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1487-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1487-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1487-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1487-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1487-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d1487-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1487-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1487-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1487-114">Not supported.</span></span>|
|<span data-ttu-id="d1487-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1487-115">Application</span></span>|<span data-ttu-id="d1487-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1487-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1487-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1487-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="d1487-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1487-118">Request headers</span></span>
|<span data-ttu-id="d1487-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1487-119">Header</span></span>|<span data-ttu-id="d1487-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d1487-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1487-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1487-121">Authorization</span></span>|<span data-ttu-id="d1487-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1487-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1487-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1487-123">Accept</span></span>|<span data-ttu-id="d1487-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d1487-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1487-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1487-125">Request body</span></span>
<span data-ttu-id="d1487-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1487-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1487-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1487-127">Response</span></span>
<span data-ttu-id="d1487-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1487-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1487-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1487-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1487-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1487-130">Request</span></span>
<span data-ttu-id="d1487-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1487-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="d1487-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1487-132">Response</span></span>
<span data-ttu-id="d1487-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1487-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
      "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "operatingSystem": "Operating System value",
      "osVersion": "Os Version value",
      "userId": "User Id value",
      "deviceId": "Device Id value",
      "enrollmentType": "userEnrollment",
      "failureCategory": "authentication",
      "failureReason": "Failure Reason value"
    }
  ]
}
```



