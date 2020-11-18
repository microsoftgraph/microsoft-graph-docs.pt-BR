---
title: Listar userExperienceAnalyticsAppHealthDevicePerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10843547afbfb0ab9840cf6af04681054ff8ad00
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202814"
---
# <a name="list-userexperienceanalyticsapphealthdeviceperformances"></a><span data-ttu-id="757a5-103">Listar userExperienceAnalyticsAppHealthDevicePerformances</span><span class="sxs-lookup"><span data-stu-id="757a5-103">List userExperienceAnalyticsAppHealthDevicePerformances</span></span>

<span data-ttu-id="757a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="757a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="757a5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="757a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="757a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="757a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="757a5-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="757a5-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="757a5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="757a5-108">Prerequisites</span></span>
<span data-ttu-id="757a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="757a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="757a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="757a5-111">Permission type</span></span>|<span data-ttu-id="757a5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="757a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="757a5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="757a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="757a5-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="757a5-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="757a5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="757a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="757a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="757a5-116">Not supported.</span></span>|
|<span data-ttu-id="757a5-117">Application</span><span class="sxs-lookup"><span data-stu-id="757a5-117">Application</span></span>|<span data-ttu-id="757a5-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="757a5-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="757a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="757a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="757a5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="757a5-120">Request headers</span></span>
|<span data-ttu-id="757a5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="757a5-121">Header</span></span>|<span data-ttu-id="757a5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="757a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="757a5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="757a5-123">Authorization</span></span>|<span data-ttu-id="757a5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="757a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="757a5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="757a5-125">Accept</span></span>|<span data-ttu-id="757a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="757a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="757a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="757a5-127">Request body</span></span>
<span data-ttu-id="757a5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="757a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="757a5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="757a5-129">Response</span></span>
<span data-ttu-id="757a5-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="757a5-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="757a5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="757a5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="757a5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="757a5-132">Request</span></span>
<span data-ttu-id="757a5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="757a5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

### <a name="response"></a><span data-ttu-id="757a5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="757a5-134">Response</span></span>
<span data-ttu-id="757a5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="757a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": [
    {
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
  ]
}
```




