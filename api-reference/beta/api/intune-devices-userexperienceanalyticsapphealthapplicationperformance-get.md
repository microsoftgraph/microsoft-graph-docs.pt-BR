---
title: Obter userExperienceAnalyticsAppHealthApplicationPerformance
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b565e811103e21b5f70884107e71d11b28f7a45e
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790251"
---
# <a name="get-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="7f952-103">Obter userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="7f952-103">Get userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="7f952-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f952-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f952-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f952-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f952-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f952-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f952-107">Leia as propriedades e as relações do objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="7f952-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f952-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f952-108">Prerequisites</span></span>
<span data-ttu-id="7f952-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f952-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f952-111">Permission type</span></span>|<span data-ttu-id="7f952-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7f952-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f952-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f952-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f952-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f952-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7f952-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f952-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f952-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f952-116">Not supported.</span></span>|
|<span data-ttu-id="7f952-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f952-117">Application</span></span>|<span data-ttu-id="7f952-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f952-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f952-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f952-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f952-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f952-120">Optional query parameters</span></span>
<span data-ttu-id="7f952-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f952-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f952-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f952-122">Request headers</span></span>
|<span data-ttu-id="7f952-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f952-123">Header</span></span>|<span data-ttu-id="7f952-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7f952-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f952-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f952-125">Authorization</span></span>|<span data-ttu-id="7f952-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f952-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f952-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f952-127">Accept</span></span>|<span data-ttu-id="7f952-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7f952-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f952-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f952-129">Request body</span></span>
<span data-ttu-id="7f952-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f952-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f952-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f952-131">Response</span></span>
<span data-ttu-id="7f952-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f952-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f952-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f952-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f952-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f952-134">Request</span></span>
<span data-ttu-id="7f952-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f952-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

### <a name="response"></a><span data-ttu-id="7f952-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f952-136">Response</span></span>
<span data-ttu-id="7f952-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f952-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 691

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
    "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
    "appName": "App Name value",
    "appFriendlyName": "App Friendly Name value",
    "appPublisher": "App Publisher value",
    "activeDevices": 13,
    "totalAppUsageDuration": 5,
    "totalAppCrashes": 15,
    "totalAppHangs": 13,
    "meanTimeToFailure": 1,
    "appHealthScore": 4.666666666666667,
    "appHealthStatus": "App Health Status value",
    "allOrgsHealthScore": 6.0,
    "allOrgsMeanTimeToFailure": 8,
    "tenantId": "Tenant Id value",
    "memaTimeGenerated": "Mema Time Generated value"
  }
}
```



