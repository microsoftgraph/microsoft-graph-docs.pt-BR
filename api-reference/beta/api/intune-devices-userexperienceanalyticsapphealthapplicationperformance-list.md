---
title: Listar userExperienceAnalyticsAppHealthApplicationPerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e11fdd2b2635dc2f042b7355e64f5c804e3a0b42
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017581"
---
# <a name="list-userexperienceanalyticsapphealthapplicationperformances"></a><span data-ttu-id="201ae-103">Listar userExperienceAnalyticsAppHealthApplicationPerformances</span><span class="sxs-lookup"><span data-stu-id="201ae-103">List userExperienceAnalyticsAppHealthApplicationPerformances</span></span>

<span data-ttu-id="201ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="201ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="201ae-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="201ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="201ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="201ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="201ae-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="201ae-107">List properties and relationships of the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="201ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="201ae-108">Prerequisites</span></span>
<span data-ttu-id="201ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="201ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="201ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="201ae-111">Permission type</span></span>|<span data-ttu-id="201ae-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="201ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="201ae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="201ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="201ae-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="201ae-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="201ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="201ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="201ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="201ae-116">Not supported.</span></span>|
|<span data-ttu-id="201ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="201ae-117">Application</span></span>|<span data-ttu-id="201ae-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="201ae-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="201ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="201ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="201ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="201ae-120">Request headers</span></span>
|<span data-ttu-id="201ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="201ae-121">Header</span></span>|<span data-ttu-id="201ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="201ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="201ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="201ae-123">Authorization</span></span>|<span data-ttu-id="201ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="201ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="201ae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="201ae-125">Accept</span></span>|<span data-ttu-id="201ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="201ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="201ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="201ae-127">Request body</span></span>
<span data-ttu-id="201ae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="201ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="201ae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="201ae-129">Response</span></span>
<span data-ttu-id="201ae-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="201ae-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="201ae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="201ae-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="201ae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="201ae-132">Request</span></span>
<span data-ttu-id="201ae-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="201ae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

### <a name="response"></a><span data-ttu-id="201ae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="201ae-134">Response</span></span>
<span data-ttu-id="201ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="201ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 607

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
      "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
      "appHangCount": 12,
      "appHealthScore": 4.666666666666667,
      "appHealthStatus": "App Health Status value",
      "allOrgsHealthScore": 6.0,
      "activeDeviceCount": 1,
      "appName": "App Name value",
      "appDisplayName": "App Display Name value",
      "appPublisher": "App Publisher value",
      "appUsageDuration": 0,
      "appCrashCount": 13,
      "meanTimeToFailureInMinutes": 10
    }
  ]
}
```






