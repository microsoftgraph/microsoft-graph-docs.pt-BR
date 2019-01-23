---
title: Listar enrollmentTroubleshootingEvents
description: Lista propriedades e relações dos objetos enrollmentTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62a2718408ef1c90c92136cbf2faf87ad2eec63e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404320"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="8a03f-103">Listar enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="8a03f-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="8a03f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a03f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8a03f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a03f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a03f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="8a03f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a03f-107">Lista propriedades e relações dos objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8a03f-107">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a03f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a03f-108">Prerequisites</span></span>
<span data-ttu-id="8a03f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a03f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8a03f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a03f-111">Permission type</span></span>|<span data-ttu-id="8a03f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a03f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a03f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a03f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a03f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a03f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8a03f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a03f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a03f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a03f-116">Not supported.</span></span>|
|<span data-ttu-id="8a03f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a03f-117">Application</span></span>|<span data-ttu-id="8a03f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a03f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a03f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a03f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8a03f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a03f-120">Request headers</span></span>
|<span data-ttu-id="8a03f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a03f-121">Header</span></span>|<span data-ttu-id="8a03f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8a03f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a03f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a03f-123">Authorization</span></span>|<span data-ttu-id="8a03f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a03f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a03f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a03f-125">Accept</span></span>|<span data-ttu-id="8a03f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a03f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a03f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a03f-127">Request body</span></span>
<span data-ttu-id="8a03f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a03f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a03f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a03f-129">Response</span></span>
<span data-ttu-id="8a03f-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a03f-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a03f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a03f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a03f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a03f-132">Request</span></span>
<span data-ttu-id="8a03f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a03f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="8a03f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a03f-134">Response</span></span>
<span data-ttu-id="8a03f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a03f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




