---
title: Obter deviceManagementAutopilotEvent
description: Leia propriedades e relações do objeto deviceManagementAutopilotEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91a416fda4fd45730f3c117a3cb65aa24da07b40
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148257"
---
# <a name="get-devicemanagementautopilotevent"></a><span data-ttu-id="f6d56-103">Obter deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="f6d56-103">Get deviceManagementAutopilotEvent</span></span>

<span data-ttu-id="f6d56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6d56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6d56-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6d56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6d56-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6d56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d56-107">Leia propriedades e relações do [objeto deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)</span><span class="sxs-lookup"><span data-stu-id="f6d56-107">Read properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6d56-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f6d56-108">Prerequisites</span></span>
<span data-ttu-id="f6d56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6d56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6d56-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6d56-111">Permission type</span></span>|<span data-ttu-id="f6d56-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6d56-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6d56-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6d56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6d56-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d56-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f6d56-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6d56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6d56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6d56-116">Not supported.</span></span>|
|<span data-ttu-id="f6d56-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6d56-117">Application</span></span>|<span data-ttu-id="f6d56-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d56-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6d56-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6d56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6d56-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6d56-120">Optional query parameters</span></span>
<span data-ttu-id="f6d56-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f6d56-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6d56-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6d56-122">Request headers</span></span>
|<span data-ttu-id="f6d56-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f6d56-123">Header</span></span>|<span data-ttu-id="f6d56-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f6d56-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6d56-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6d56-125">Authorization</span></span>|<span data-ttu-id="f6d56-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6d56-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6d56-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f6d56-127">Accept</span></span>|<span data-ttu-id="f6d56-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f6d56-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6d56-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6d56-129">Request body</span></span>
<span data-ttu-id="f6d56-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6d56-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6d56-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6d56-131">Response</span></span>
<span data-ttu-id="f6d56-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6d56-132">If successful, this method returns a `200 OK` response code and [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6d56-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6d56-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6d56-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6d56-134">Request</span></span>
<span data-ttu-id="f6d56-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6d56-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

### <a name="response"></a><span data-ttu-id="f6d56-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6d56-136">Response</span></span>
<span data-ttu-id="f6d56-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6d56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1669

{
  "value": {
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
    "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
    "deploymentState": "success",
    "deviceSetupStatus": "success",
    "accountSetupStatus": "success",
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




