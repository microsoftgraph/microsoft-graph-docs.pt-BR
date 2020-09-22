---
title: Obter userExperienceAnalyticsAppHealthDevicePerformance
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30bd56ff453776ebd8f4fedf3d03f280c0424467
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992513"
---
# <a name="get-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="670a6-103">Obter userExperienceAnalyticsAppHealthDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="670a6-103">Get userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="670a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="670a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="670a6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="670a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="670a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="670a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="670a6-107">Leia as propriedades e as relações do objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="670a6-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="670a6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="670a6-108">Prerequisites</span></span>
<span data-ttu-id="670a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="670a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="670a6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="670a6-111">Permission type</span></span>|<span data-ttu-id="670a6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="670a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="670a6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="670a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="670a6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="670a6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="670a6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="670a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="670a6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="670a6-116">Not supported.</span></span>|
|<span data-ttu-id="670a6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="670a6-117">Application</span></span>|<span data-ttu-id="670a6-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="670a6-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="670a6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="670a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="670a6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="670a6-120">Optional query parameters</span></span>
<span data-ttu-id="670a6-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="670a6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="670a6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="670a6-122">Request headers</span></span>
|<span data-ttu-id="670a6-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="670a6-123">Header</span></span>|<span data-ttu-id="670a6-124">Valor</span><span class="sxs-lookup"><span data-stu-id="670a6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="670a6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="670a6-125">Authorization</span></span>|<span data-ttu-id="670a6-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="670a6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="670a6-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="670a6-127">Accept</span></span>|<span data-ttu-id="670a6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="670a6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="670a6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="670a6-129">Request body</span></span>
<span data-ttu-id="670a6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="670a6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="670a6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="670a6-131">Response</span></span>
<span data-ttu-id="670a6-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="670a6-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="670a6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="670a6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="670a6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="670a6-134">Request</span></span>
<span data-ttu-id="670a6-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="670a6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

### <a name="response"></a><span data-ttu-id="670a6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="670a6-136">Response</span></span>
<span data-ttu-id="670a6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="670a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
    "id": "2c651499-1499-2c65-9914-652c9914652c",
    "deviceModel": "Device Model value",
    "deviceManufacturer": "Device Manufacturer value",
    "appCrashCount": 13,
    "crashedAppCount": 15,
    "appHangCount": 12,
    "meanTimeToFailureInMinutes": 10,
    "deviceAppHealthScore": 6.666666666666667,
    "deviceAppHealthStatus": "Device App Health Status value",
    "deviceId": "Device Id value",
    "deviceDisplayName": "Device Display Name value"
  }
}
```





