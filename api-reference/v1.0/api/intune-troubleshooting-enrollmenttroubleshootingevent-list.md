---
title: Listar enrollmentTroubleshootingEvents
description: Lista propriedades e relações dos objetos enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 13e2c88f68eddd35a97dfb3c9573da6308743a98
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732302"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="d3edf-103">Listar enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="d3edf-103">List enrollmentTroubleshootingEvents</span></span>

<span data-ttu-id="d3edf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3edf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3edf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3edf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3edf-106">Lista propriedades e relações dos objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d3edf-106">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3edf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3edf-107">Prerequisites</span></span>
<span data-ttu-id="d3edf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3edf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3edf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3edf-110">Permission type</span></span>|<span data-ttu-id="d3edf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3edf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3edf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3edf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3edf-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3edf-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d3edf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3edf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3edf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3edf-115">Not supported.</span></span>|
|<span data-ttu-id="d3edf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3edf-116">Application</span></span>|<span data-ttu-id="d3edf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3edf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3edf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3edf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="d3edf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3edf-119">Request headers</span></span>
|<span data-ttu-id="d3edf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3edf-120">Header</span></span>|<span data-ttu-id="d3edf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d3edf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3edf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3edf-122">Authorization</span></span>|<span data-ttu-id="d3edf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3edf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3edf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3edf-124">Accept</span></span>|<span data-ttu-id="d3edf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3edf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3edf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3edf-126">Request body</span></span>
<span data-ttu-id="d3edf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3edf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3edf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3edf-128">Response</span></span>
<span data-ttu-id="d3edf-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3edf-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3edf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3edf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3edf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3edf-131">Request</span></span>
<span data-ttu-id="d3edf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3edf-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="d3edf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3edf-133">Response</span></span>
<span data-ttu-id="d3edf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3edf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









