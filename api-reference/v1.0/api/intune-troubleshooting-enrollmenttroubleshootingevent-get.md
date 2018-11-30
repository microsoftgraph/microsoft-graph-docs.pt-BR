---
title: Get enrollmentTroubleshootingEvent
description: Propriedades de leitura e relações do objeto enrollmentTroubleshootingEvent.
ms.openlocfilehash: c35f0b41c7c79abcba0c38025535805b50c917bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003387"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="e1442-103">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e1442-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="e1442-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1442-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1442-105">Propriedades de leitura e relações do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e1442-105">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1442-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1442-106">Prerequisites</span></span>
<span data-ttu-id="e1442-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1442-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1442-109">Permission type</span></span>|<span data-ttu-id="e1442-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1442-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1442-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1442-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1442-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1442-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e1442-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1442-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1442-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1442-114">Not supported.</span></span>|
|<span data-ttu-id="e1442-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1442-115">Application</span></span>|<span data-ttu-id="e1442-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1442-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1442-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1442-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1442-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1442-118">Optional query parameters</span></span>
<span data-ttu-id="e1442-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1442-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e1442-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1442-120">Request headers</span></span>
|<span data-ttu-id="e1442-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1442-121">Header</span></span>|<span data-ttu-id="e1442-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1442-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1442-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1442-123">Authorization</span></span>|<span data-ttu-id="e1442-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1442-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1442-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1442-125">Accept</span></span>|<span data-ttu-id="e1442-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1442-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1442-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1442-127">Request body</span></span>
<span data-ttu-id="e1442-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1442-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1442-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1442-129">Response</span></span>
<span data-ttu-id="e1442-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1442-130">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1442-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1442-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1442-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1442-132">Request</span></span>
<span data-ttu-id="e1442-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1442-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="e1442-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1442-134">Response</span></span>
<span data-ttu-id="e1442-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1442-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



