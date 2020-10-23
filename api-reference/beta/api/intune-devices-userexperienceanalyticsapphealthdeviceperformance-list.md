---
title: Listar userExperienceAnalyticsAppHealthDevicePerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 918b889a73ee5455e9829b05836e0d6966bb0bae
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729963"
---
# <a name="list-userexperienceanalyticsapphealthdeviceperformances"></a><span data-ttu-id="7eddf-103">Listar userExperienceAnalyticsAppHealthDevicePerformances</span><span class="sxs-lookup"><span data-stu-id="7eddf-103">List userExperienceAnalyticsAppHealthDevicePerformances</span></span>

<span data-ttu-id="7eddf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eddf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7eddf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7eddf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7eddf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7eddf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7eddf-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="7eddf-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7eddf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7eddf-108">Prerequisites</span></span>
<span data-ttu-id="7eddf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eddf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eddf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7eddf-111">Permission type</span></span>|<span data-ttu-id="7eddf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7eddf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7eddf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7eddf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7eddf-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7eddf-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7eddf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7eddf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7eddf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7eddf-116">Not supported.</span></span>|
|<span data-ttu-id="7eddf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7eddf-117">Application</span></span>|<span data-ttu-id="7eddf-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7eddf-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7eddf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7eddf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="7eddf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7eddf-120">Request headers</span></span>
|<span data-ttu-id="7eddf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7eddf-121">Header</span></span>|<span data-ttu-id="7eddf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7eddf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7eddf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7eddf-123">Authorization</span></span>|<span data-ttu-id="7eddf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7eddf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7eddf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7eddf-125">Accept</span></span>|<span data-ttu-id="7eddf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7eddf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7eddf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7eddf-127">Request body</span></span>
<span data-ttu-id="7eddf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7eddf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eddf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eddf-129">Response</span></span>
<span data-ttu-id="7eddf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7eddf-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7eddf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7eddf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7eddf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7eddf-132">Request</span></span>
<span data-ttu-id="7eddf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7eddf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

### <a name="response"></a><span data-ttu-id="7eddf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eddf-134">Response</span></span>
<span data-ttu-id="7eddf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7eddf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





