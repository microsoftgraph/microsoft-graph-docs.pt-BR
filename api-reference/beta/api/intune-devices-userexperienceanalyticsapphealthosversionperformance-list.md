---
title: Listar userExperienceAnalyticsAppHealthOSVersionPerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsAppHealthOSVersionPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d208ba2390df76f9c635cce61c903fd49cc3f390
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691677"
---
# <a name="list-userexperienceanalyticsapphealthosversionperformances"></a><span data-ttu-id="c4818-103">Listar userExperienceAnalyticsAppHealthOSVersionPerformances</span><span class="sxs-lookup"><span data-stu-id="c4818-103">List userExperienceAnalyticsAppHealthOSVersionPerformances</span></span>

<span data-ttu-id="c4818-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4818-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4818-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4818-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4818-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4818-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4818-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="c4818-107">List properties and relationships of the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4818-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4818-108">Prerequisites</span></span>
<span data-ttu-id="c4818-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4818-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4818-111">Permission type</span></span>|<span data-ttu-id="c4818-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4818-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4818-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4818-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4818-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4818-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c4818-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4818-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4818-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4818-116">Not supported.</span></span>|
|<span data-ttu-id="c4818-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4818-117">Application</span></span>|<span data-ttu-id="c4818-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4818-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4818-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4818-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="c4818-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4818-120">Request headers</span></span>
|<span data-ttu-id="c4818-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4818-121">Header</span></span>|<span data-ttu-id="c4818-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4818-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4818-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4818-123">Authorization</span></span>|<span data-ttu-id="c4818-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4818-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4818-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4818-125">Accept</span></span>|<span data-ttu-id="c4818-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4818-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4818-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4818-127">Request body</span></span>
<span data-ttu-id="c4818-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4818-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4818-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4818-129">Response</span></span>
<span data-ttu-id="c4818-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4818-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4818-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4818-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4818-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4818-132">Request</span></span>
<span data-ttu-id="c4818-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4818-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

### <a name="response"></a><span data-ttu-id="c4818-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4818-134">Response</span></span>
<span data-ttu-id="c4818-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4818-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
      "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
      "osVersion": "Os Version value",
      "osBuildNumber": "Os Build Number value",
      "activeDeviceCount": 1,
      "meanTimeToFailureInMinutes": 10,
      "osVersionAppHealthScore": 7.666666666666667,
      "osVersionAppHealthStatus": "Os Version App Health Status value"
    }
  ]
}
```





