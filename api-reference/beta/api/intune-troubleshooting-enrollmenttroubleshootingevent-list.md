---
title: Listar enrollmentTroubleshootingEvents
description: Lista propriedades e relações dos objetos enrollmentTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82d40704ddbaaef1be7bbe509f4463a971a84f39
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457640"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="04d4b-103">Listar enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="04d4b-103">List enrollmentTroubleshootingEvents</span></span>

<span data-ttu-id="04d4b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04d4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04d4b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04d4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04d4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04d4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04d4b-107">Lista propriedades e relações dos objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="04d4b-107">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04d4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04d4b-108">Prerequisites</span></span>
<span data-ttu-id="04d4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04d4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04d4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04d4b-111">Permission type</span></span>|<span data-ttu-id="04d4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04d4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04d4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04d4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04d4b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="04d4b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="04d4b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04d4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04d4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04d4b-116">Not supported.</span></span>|
|<span data-ttu-id="04d4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04d4b-117">Application</span></span>|<span data-ttu-id="04d4b-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="04d4b-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04d4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04d4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="04d4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04d4b-120">Request headers</span></span>
|<span data-ttu-id="04d4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04d4b-121">Header</span></span>|<span data-ttu-id="04d4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04d4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04d4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04d4b-123">Authorization</span></span>|<span data-ttu-id="04d4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04d4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04d4b-125">Accept</span></span>|<span data-ttu-id="04d4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04d4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04d4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04d4b-127">Request body</span></span>
<span data-ttu-id="04d4b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04d4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04d4b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="04d4b-129">Response</span></span>
<span data-ttu-id="04d4b-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04d4b-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04d4b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04d4b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="04d4b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04d4b-132">Request</span></span>
<span data-ttu-id="04d4b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04d4b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="04d4b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="04d4b-134">Response</span></span>
<span data-ttu-id="04d4b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04d4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1400

{
  "value": [
    {
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
  ]
}
```





