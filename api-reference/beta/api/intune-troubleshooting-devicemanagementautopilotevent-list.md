---
title: Listar deviceManagementAutopilotEvents
description: Listar Propriedades e relações dos objetos deviceManagementAutopilotEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f21f7ea7359e9503d1f2f03863536ffcb19b92f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457703"
---
# <a name="list-devicemanagementautopilotevents"></a><span data-ttu-id="6f4ed-103">Listar deviceManagementAutopilotEvents</span><span class="sxs-lookup"><span data-stu-id="6f4ed-103">List deviceManagementAutopilotEvents</span></span>

<span data-ttu-id="6f4ed-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f4ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f4ed-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f4ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f4ed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f4ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f4ed-107">Listar Propriedades e relações dos objetos [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="6f4ed-107">List properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f4ed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f4ed-108">Prerequisites</span></span>
<span data-ttu-id="6f4ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f4ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f4ed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f4ed-111">Permission type</span></span>|<span data-ttu-id="6f4ed-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f4ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f4ed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f4ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f4ed-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f4ed-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6f4ed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f4ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f4ed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f4ed-116">Not supported.</span></span>|
|<span data-ttu-id="6f4ed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f4ed-117">Application</span></span>|<span data-ttu-id="6f4ed-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f4ed-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f4ed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f4ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="6f4ed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f4ed-120">Request headers</span></span>
|<span data-ttu-id="6f4ed-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f4ed-121">Header</span></span>|<span data-ttu-id="6f4ed-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6f4ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f4ed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f4ed-123">Authorization</span></span>|<span data-ttu-id="6f4ed-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f4ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f4ed-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f4ed-125">Accept</span></span>|<span data-ttu-id="6f4ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f4ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f4ed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f4ed-127">Request body</span></span>
<span data-ttu-id="6f4ed-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f4ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f4ed-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f4ed-129">Response</span></span>
<span data-ttu-id="6f4ed-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f4ed-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f4ed-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f4ed-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f4ed-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f4ed-132">Request</span></span>
<span data-ttu-id="6f4ed-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f4ed-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
```

### <a name="response"></a><span data-ttu-id="6f4ed-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f4ed-134">Response</span></span>
<span data-ttu-id="6f4ed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f4ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1501

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
      "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
      "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
      "enrollmentType": "azureADJoinedWithAutopilotProfile",
      "deviceSerialNumber": "Device Serial Number value",
      "managedDeviceName": "Managed Device Name value",
      "userPrincipalName": "User Principal Name value",
      "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
      "enrollmentState": "enrolled",
      "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
      "deploymentState": "success",
      "osVersion": "Os Version value",
      "deploymentDuration": "PT3M21.5549443S",
      "deploymentTotalDuration": "PT1M43.5284261S",
      "devicePreparationDuration": "-PT1M32.1347897S",
      "deviceSetupDuration": "-PT2M57.2190107S",
      "accountSetupDuration": "-PT2M32.0507894S",
      "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
      "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
      "targetedAppCount": 0,
      "targetedPolicyCount": 3,
      "enrollmentFailureDetails": "Enrollment Failure Details value"
    }
  ]
}
```





