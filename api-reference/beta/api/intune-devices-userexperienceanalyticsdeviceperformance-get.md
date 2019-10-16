---
title: Obter userExperienceAnalyticsDevicePerformance
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsDevicePerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30ac11f412a533d12532520c2f7953f1a843eb69
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529246"
---
# <a name="get-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="a9a26-103">Obter userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="a9a26-103">Get userExperienceAnalyticsDevicePerformance</span></span>

> <span data-ttu-id="a9a26-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9a26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9a26-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9a26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9a26-106">Leia as propriedades e as relações do objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="a9a26-106">Read properties and relationships of the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9a26-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9a26-107">Prerequisites</span></span>
<span data-ttu-id="a9a26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9a26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9a26-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9a26-110">Permission type</span></span>|<span data-ttu-id="a9a26-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9a26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9a26-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9a26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9a26-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9a26-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a9a26-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9a26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9a26-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9a26-115">Not supported.</span></span>|
|<span data-ttu-id="a9a26-116">Application</span><span class="sxs-lookup"><span data-stu-id="a9a26-116">Application</span></span>|<span data-ttu-id="a9a26-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9a26-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9a26-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9a26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9a26-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9a26-119">Optional query parameters</span></span>
<span data-ttu-id="a9a26-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9a26-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9a26-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9a26-121">Request headers</span></span>
|<span data-ttu-id="a9a26-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9a26-122">Header</span></span>|<span data-ttu-id="a9a26-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a9a26-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9a26-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9a26-124">Authorization</span></span>|<span data-ttu-id="a9a26-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9a26-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9a26-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9a26-126">Accept</span></span>|<span data-ttu-id="a9a26-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a9a26-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9a26-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9a26-128">Request body</span></span>
<span data-ttu-id="a9a26-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9a26-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9a26-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9a26-130">Response</span></span>
<span data-ttu-id="a9a26-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9a26-131">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9a26-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9a26-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9a26-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9a26-133">Request</span></span>
<span data-ttu-id="a9a26-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9a26-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

### <a name="response"></a><span data-ttu-id="a9a26-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9a26-135">Response</span></span>
<span data-ttu-id="a9a26-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9a26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": {
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
    "deviceCount": 11
  }
}
```






