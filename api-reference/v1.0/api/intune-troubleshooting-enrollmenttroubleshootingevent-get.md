---
title: Get enrollmentTroubleshootingEvent
description: Propriedades de leitura e relações do objeto enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3931d9753eb48c20b462cc239aac162edb1dddc8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43368641"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="61275-103">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="61275-103">Get enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="61275-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61275-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61275-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61275-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61275-106">Propriedades de leitura e relações do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="61275-106">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61275-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61275-107">Prerequisites</span></span>
<span data-ttu-id="61275-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61275-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61275-110">Permission type</span></span>|<span data-ttu-id="61275-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61275-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61275-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61275-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61275-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="61275-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="61275-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61275-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61275-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61275-115">Not supported.</span></span>|
|<span data-ttu-id="61275-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61275-116">Application</span></span>|<span data-ttu-id="61275-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61275-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61275-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61275-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61275-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61275-119">Optional query parameters</span></span>
<span data-ttu-id="61275-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61275-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61275-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61275-121">Request headers</span></span>
|<span data-ttu-id="61275-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61275-122">Header</span></span>|<span data-ttu-id="61275-123">Valor</span><span class="sxs-lookup"><span data-stu-id="61275-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61275-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="61275-124">Authorization</span></span>|<span data-ttu-id="61275-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61275-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61275-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61275-126">Accept</span></span>|<span data-ttu-id="61275-127">application/json</span><span class="sxs-lookup"><span data-stu-id="61275-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61275-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61275-128">Request body</span></span>
<span data-ttu-id="61275-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61275-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61275-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="61275-130">Response</span></span>
<span data-ttu-id="61275-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61275-131">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61275-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61275-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="61275-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61275-133">Request</span></span>
<span data-ttu-id="61275-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61275-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="61275-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="61275-135">Response</span></span>
<span data-ttu-id="61275-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61275-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": {
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
}
```






