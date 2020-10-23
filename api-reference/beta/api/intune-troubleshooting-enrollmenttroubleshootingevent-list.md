---
title: Listar enrollmentTroubleshootingEvents
description: Lista propriedades e relações dos objetos enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d0791a3d0652ad1a559ef2f25884cb7dc018f85
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692727"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="af798-103">Listar enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="af798-103">List enrollmentTroubleshootingEvents</span></span>

<span data-ttu-id="af798-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af798-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af798-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="af798-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af798-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af798-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af798-107">Lista propriedades e relações dos objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="af798-107">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af798-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af798-108">Prerequisites</span></span>
<span data-ttu-id="af798-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af798-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af798-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af798-111">Permission type</span></span>|<span data-ttu-id="af798-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af798-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af798-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af798-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af798-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="af798-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="af798-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af798-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af798-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af798-116">Not supported.</span></span>|
|<span data-ttu-id="af798-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af798-117">Application</span></span>|<span data-ttu-id="af798-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="af798-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af798-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af798-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="af798-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af798-120">Request headers</span></span>
|<span data-ttu-id="af798-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af798-121">Header</span></span>|<span data-ttu-id="af798-122">Valor</span><span class="sxs-lookup"><span data-stu-id="af798-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af798-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="af798-123">Authorization</span></span>|<span data-ttu-id="af798-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af798-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af798-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af798-125">Accept</span></span>|<span data-ttu-id="af798-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af798-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af798-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af798-127">Request body</span></span>
<span data-ttu-id="af798-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af798-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af798-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="af798-129">Response</span></span>
<span data-ttu-id="af798-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af798-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af798-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af798-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="af798-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af798-132">Request</span></span>
<span data-ttu-id="af798-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af798-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="af798-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="af798-134">Response</span></span>
<span data-ttu-id="af798-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af798-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





