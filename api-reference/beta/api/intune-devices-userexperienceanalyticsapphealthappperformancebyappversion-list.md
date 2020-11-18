---
title: Listar userExperienceAnalyticsAppHealthAppPerformanceByAppVersions
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef13a94160063a798e4514c7c4721e332da9eaf2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203169"
---
# <a name="list-userexperienceanalyticsapphealthappperformancebyappversions"></a><span data-ttu-id="5cd12-103">Listar userExperienceAnalyticsAppHealthAppPerformanceByAppVersions</span><span class="sxs-lookup"><span data-stu-id="5cd12-103">List userExperienceAnalyticsAppHealthAppPerformanceByAppVersions</span></span>

<span data-ttu-id="5cd12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cd12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cd12-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5cd12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cd12-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cd12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd12-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .</span><span class="sxs-lookup"><span data-stu-id="5cd12-107">List properties and relationships of the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cd12-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5cd12-108">Prerequisites</span></span>
<span data-ttu-id="5cd12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cd12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cd12-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cd12-111">Permission type</span></span>|<span data-ttu-id="5cd12-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5cd12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cd12-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cd12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cd12-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cd12-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5cd12-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cd12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cd12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cd12-116">Not supported.</span></span>|
|<span data-ttu-id="5cd12-117">Application</span><span class="sxs-lookup"><span data-stu-id="5cd12-117">Application</span></span>|<span data-ttu-id="5cd12-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cd12-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cd12-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cd12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
```

## <a name="request-headers"></a><span data-ttu-id="5cd12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd12-120">Request headers</span></span>
|<span data-ttu-id="5cd12-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cd12-121">Header</span></span>|<span data-ttu-id="5cd12-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5cd12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cd12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cd12-123">Authorization</span></span>|<span data-ttu-id="5cd12-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cd12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cd12-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5cd12-125">Accept</span></span>|<span data-ttu-id="5cd12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cd12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cd12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd12-127">Request body</span></span>
<span data-ttu-id="5cd12-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5cd12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cd12-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cd12-129">Response</span></span>
<span data-ttu-id="5cd12-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cd12-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cd12-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cd12-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cd12-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd12-132">Request</span></span>
<span data-ttu-id="5cd12-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cd12-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
```

### <a name="response"></a><span data-ttu-id="5cd12-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cd12-134">Response</span></span>
<span data-ttu-id="5cd12-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cd12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 464

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
      "id": "257804c8-04c8-2578-c804-7825c8047825",
      "appVersion": "App Version value",
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




