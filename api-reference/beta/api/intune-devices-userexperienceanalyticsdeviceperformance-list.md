---
title: Listar userExperienceAnalyticsDevicePerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsDevicePerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 963e5972e0c2b8900feef0163695492e78692b2a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468450"
---
# <a name="list-userexperienceanalyticsdeviceperformances"></a><span data-ttu-id="ed0bd-103">Listar userExperienceAnalyticsDevicePerformances</span><span class="sxs-lookup"><span data-stu-id="ed0bd-103">List userExperienceAnalyticsDevicePerformances</span></span>

<span data-ttu-id="ed0bd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ed0bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed0bd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed0bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed0bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed0bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed0bd-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="ed0bd-107">List properties and relationships of the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed0bd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed0bd-108">Prerequisites</span></span>
<span data-ttu-id="ed0bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed0bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed0bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed0bd-111">Permission type</span></span>|<span data-ttu-id="ed0bd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed0bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed0bd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed0bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed0bd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed0bd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ed0bd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed0bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed0bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed0bd-116">Not supported.</span></span>|
|<span data-ttu-id="ed0bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed0bd-117">Application</span></span>|<span data-ttu-id="ed0bd-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed0bd-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed0bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed0bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="ed0bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0bd-120">Request headers</span></span>
|<span data-ttu-id="ed0bd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed0bd-121">Header</span></span>|<span data-ttu-id="ed0bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed0bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed0bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed0bd-123">Authorization</span></span>|<span data-ttu-id="ed0bd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed0bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed0bd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed0bd-125">Accept</span></span>|<span data-ttu-id="ed0bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed0bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed0bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0bd-127">Request body</span></span>
<span data-ttu-id="ed0bd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed0bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed0bd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed0bd-129">Response</span></span>
<span data-ttu-id="ed0bd-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed0bd-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed0bd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed0bd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed0bd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0bd-132">Request</span></span>
<span data-ttu-id="ed0bd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed0bd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
```

### <a name="response"></a><span data-ttu-id="ed0bd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed0bd-134">Response</span></span>
<span data-ttu-id="ed0bd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed0bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
      "id": "852ae826-e826-852a-26e8-2a8526e82a85",
      "deviceName": "Device Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "diskType": "hdd",
      "operatingSystemVersion": "Operating System Version value",
      "bootScore": 9,
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "healthStatus": "insufficientData",
      "loginScore": 10,
      "coreLoginTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "deviceCount": 11,
      "responsiveDesktopTimeInMs": 9
    }
  ]
}
```





