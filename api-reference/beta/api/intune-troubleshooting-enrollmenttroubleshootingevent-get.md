---
title: Get enrollmentTroubleshootingEvent
description: Propriedades de leitura e relações do objeto enrollmentTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7d890cd0397a643eba6b727a6b82e6d06e848b3
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088004"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="22b18-103">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="22b18-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="22b18-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22b18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22b18-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22b18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22b18-106">Propriedades de leitura e relações do objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="22b18-106">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22b18-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22b18-107">Prerequisites</span></span>
<span data-ttu-id="22b18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22b18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22b18-110">Permission type</span></span>|<span data-ttu-id="22b18-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22b18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22b18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22b18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22b18-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="22b18-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="22b18-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22b18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22b18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22b18-115">Not supported.</span></span>|
|<span data-ttu-id="22b18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22b18-116">Application</span></span>|<span data-ttu-id="22b18-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="22b18-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22b18-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22b18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22b18-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22b18-119">Optional query parameters</span></span>
<span data-ttu-id="22b18-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22b18-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22b18-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22b18-121">Request headers</span></span>
|<span data-ttu-id="22b18-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22b18-122">Header</span></span>|<span data-ttu-id="22b18-123">Valor</span><span class="sxs-lookup"><span data-stu-id="22b18-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22b18-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="22b18-124">Authorization</span></span>|<span data-ttu-id="22b18-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22b18-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22b18-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22b18-126">Accept</span></span>|<span data-ttu-id="22b18-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22b18-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22b18-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22b18-128">Request body</span></span>
<span data-ttu-id="22b18-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22b18-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22b18-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="22b18-130">Response</span></span>
<span data-ttu-id="22b18-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22b18-131">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22b18-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22b18-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="22b18-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22b18-133">Request</span></span>
<span data-ttu-id="22b18-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22b18-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="22b18-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="22b18-135">Response</span></span>
<span data-ttu-id="22b18-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22b18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1318

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
    "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "troubleshootingErrorDetails": {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
      "context": "Context value",
      "failure": "Failure value",
      "failureDetails": "Failure Details value",
      "remediation": "Remediation value",
      "resources": [
        {
          "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
          "text": "Text value",
          "link": "Link value"
        }
      ]
    },
    "eventName": "Event Name value",
    "additionalInformation": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
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






