---
title: Listar userExperienceAnalyticsDeviceStartupHistories
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b5563bcdfcdf78f16f931ddec99c20037c45d23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082592"
---
# <a name="list-userexperienceanalyticsdevicestartuphistories"></a><span data-ttu-id="7e322-103">Listar userExperienceAnalyticsDeviceStartupHistories</span><span class="sxs-lookup"><span data-stu-id="7e322-103">List userExperienceAnalyticsDeviceStartupHistories</span></span>

<span data-ttu-id="7e322-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e322-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e322-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e322-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e322-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e322-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="7e322-107">List properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e322-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e322-108">Prerequisites</span></span>
<span data-ttu-id="7e322-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e322-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e322-111">Permission type</span></span>|<span data-ttu-id="7e322-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e322-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e322-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e322-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e322-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e322-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7e322-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e322-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e322-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e322-116">Not supported.</span></span>|
|<span data-ttu-id="7e322-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e322-117">Application</span></span>|<span data-ttu-id="7e322-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e322-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e322-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e322-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="7e322-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e322-120">Request headers</span></span>
|<span data-ttu-id="7e322-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e322-121">Header</span></span>|<span data-ttu-id="7e322-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7e322-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e322-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e322-123">Authorization</span></span>|<span data-ttu-id="7e322-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e322-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e322-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e322-125">Accept</span></span>|<span data-ttu-id="7e322-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e322-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e322-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e322-127">Request body</span></span>
<span data-ttu-id="7e322-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e322-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e322-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e322-129">Response</span></span>
<span data-ttu-id="7e322-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e322-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e322-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e322-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e322-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e322-132">Request</span></span>
<span data-ttu-id="7e322-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e322-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

### <a name="response"></a><span data-ttu-id="7e322-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e322-134">Response</span></span>
<span data-ttu-id="7e322-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e322-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
      "id": "13357123-7123-1335-2371-351323713513",
      "deviceId": "Device Id value",
      "startTime": "2017-01-01T00:03:29.2730865-08:00",
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "featureUpdateBootTimeInMs": 9,
      "totalBootTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "coreLoginTimeInMs": 1,
      "responsiveDesktopTimeInMs": 9,
      "totalLoginTimeInMs": 2,
      "isFirstLogin": true,
      "isFeatureUpdate": true,
      "operatingSystemVersion": "Operating System Version value",
      "restartCategory": "restartWithUpdate",
      "restartStopCode": "Restart Stop Code value",
      "restartFaultBucket": "Restart Fault Bucket value"
    }
  ]
}
```






