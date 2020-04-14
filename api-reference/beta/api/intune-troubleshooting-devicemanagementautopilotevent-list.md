---
title: Listar deviceManagementAutopilotEvents
description: Listar Propriedades e relações dos objetos deviceManagementAutopilotEvent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf121e8763005d96bc4b1d65dd6b1e6cb7cec65f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448148"
---
# <a name="list-devicemanagementautopilotevents"></a><span data-ttu-id="75710-103">Listar deviceManagementAutopilotEvents</span><span class="sxs-lookup"><span data-stu-id="75710-103">List deviceManagementAutopilotEvents</span></span>

<span data-ttu-id="75710-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75710-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75710-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75710-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75710-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75710-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75710-107">Listar Propriedades e relações dos objetos [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="75710-107">List properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75710-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75710-108">Prerequisites</span></span>
<span data-ttu-id="75710-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75710-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75710-111">Permission type</span></span>|<span data-ttu-id="75710-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75710-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75710-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75710-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75710-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="75710-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="75710-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75710-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75710-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75710-116">Not supported.</span></span>|
|<span data-ttu-id="75710-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75710-117">Application</span></span>|<span data-ttu-id="75710-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="75710-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75710-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75710-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="75710-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75710-120">Request headers</span></span>
|<span data-ttu-id="75710-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75710-121">Header</span></span>|<span data-ttu-id="75710-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75710-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75710-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75710-123">Authorization</span></span>|<span data-ttu-id="75710-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75710-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75710-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75710-125">Accept</span></span>|<span data-ttu-id="75710-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75710-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75710-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75710-127">Request body</span></span>
<span data-ttu-id="75710-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75710-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75710-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="75710-129">Response</span></span>
<span data-ttu-id="75710-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75710-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75710-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75710-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="75710-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75710-132">Request</span></span>
<span data-ttu-id="75710-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75710-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
```

### <a name="response"></a><span data-ttu-id="75710-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="75710-134">Response</span></span>
<span data-ttu-id="75710-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75710-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1539

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
      "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
      "deviceId": "Device Id value",
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



