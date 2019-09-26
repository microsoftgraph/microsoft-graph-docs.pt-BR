---
title: Obter deviceManagementAutopilotEvent
description: Leia as propriedades e as relações do objeto deviceManagementAutopilotEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5be34653793069083f156928ec4ed3d52f68daf3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199487"
---
# <a name="get-devicemanagementautopilotevent"></a><span data-ttu-id="74b45-103">Obter deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="74b45-103">Get deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="74b45-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74b45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74b45-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74b45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74b45-106">Leia as propriedades e as relações do objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .</span><span class="sxs-lookup"><span data-stu-id="74b45-106">Read properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74b45-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74b45-107">Prerequisites</span></span>
<span data-ttu-id="74b45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74b45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74b45-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74b45-110">Permission type</span></span>|<span data-ttu-id="74b45-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74b45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74b45-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74b45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74b45-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="74b45-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="74b45-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74b45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74b45-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74b45-115">Not supported.</span></span>|
|<span data-ttu-id="74b45-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74b45-116">Application</span></span>|<span data-ttu-id="74b45-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="74b45-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74b45-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74b45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74b45-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="74b45-119">Optional query parameters</span></span>
<span data-ttu-id="74b45-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="74b45-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74b45-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74b45-121">Request headers</span></span>
|<span data-ttu-id="74b45-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74b45-122">Header</span></span>|<span data-ttu-id="74b45-123">Valor</span><span class="sxs-lookup"><span data-stu-id="74b45-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74b45-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="74b45-124">Authorization</span></span>|<span data-ttu-id="74b45-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74b45-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74b45-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74b45-126">Accept</span></span>|<span data-ttu-id="74b45-127">application/json</span><span class="sxs-lookup"><span data-stu-id="74b45-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74b45-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74b45-128">Request body</span></span>
<span data-ttu-id="74b45-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74b45-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74b45-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="74b45-130">Response</span></span>
<span data-ttu-id="74b45-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74b45-131">If successful, this method returns a `200 OK` response code and [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74b45-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74b45-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="74b45-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74b45-133">Request</span></span>
<span data-ttu-id="74b45-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74b45-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

### <a name="response"></a><span data-ttu-id="74b45-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="74b45-135">Response</span></span>
<span data-ttu-id="74b45-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74b45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "value": {
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
}
```




