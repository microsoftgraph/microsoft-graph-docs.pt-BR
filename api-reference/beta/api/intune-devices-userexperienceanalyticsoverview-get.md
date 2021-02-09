---
title: Obter userExperienceAnalyticsOverview
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92e1efcd6533cf9f35aa65157442581773c723b8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159966"
---
# <a name="get-userexperienceanalyticsoverview"></a><span data-ttu-id="5b18d-103">Obter userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="5b18d-103">Get userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="5b18d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b18d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b18d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b18d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b18d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b18d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b18d-107">Leia as propriedades e as relações do [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="5b18d-107">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b18d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b18d-108">Prerequisites</span></span>
<span data-ttu-id="5b18d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b18d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b18d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b18d-111">Permission type</span></span>|<span data-ttu-id="5b18d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b18d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b18d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b18d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b18d-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b18d-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5b18d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b18d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b18d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b18d-116">Not supported.</span></span>|
|<span data-ttu-id="5b18d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b18d-117">Application</span></span>|<span data-ttu-id="5b18d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b18d-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b18d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b18d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b18d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b18d-120">Optional query parameters</span></span>
<span data-ttu-id="5b18d-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b18d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b18d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b18d-122">Request headers</span></span>
|<span data-ttu-id="5b18d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b18d-123">Header</span></span>|<span data-ttu-id="5b18d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5b18d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b18d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b18d-125">Authorization</span></span>|<span data-ttu-id="5b18d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b18d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b18d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b18d-127">Accept</span></span>|<span data-ttu-id="5b18d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b18d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b18d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b18d-129">Request body</span></span>
<span data-ttu-id="5b18d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b18d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b18d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b18d-131">Response</span></span>
<span data-ttu-id="5b18d-132">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b18d-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b18d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b18d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b18d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b18d-134">Request</span></span>
<span data-ttu-id="5b18d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b18d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
```

### <a name="response"></a><span data-ttu-id="5b18d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b18d-136">Response</span></span>
<span data-ttu-id="5b18d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b18d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 929

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
    "id": "8228da2b-da2b-8228-2bda-28822bda2882",
    "overallScore": 12,
    "deviceBootPerformanceOverallScore": 1,
    "bestPracticesOverallScore": 9,
    "appHealthOverallScore": 5,
    "insights": [
      {
        "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
        "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
        "insightId": "Insight Id value",
        "values": [
          {
            "@odata.type": "microsoft.graph.insightValueDouble",
            "value": 1.6666666666666667
          }
        ],
        "severity": "informational"
      }
    ],
    "state": "insufficientData",
    "deviceBootPerformanceHealthState": "insufficientData",
    "bestPracticesHealthState": "insufficientData",
    "appHealthState": "insufficientData"
  }
}
```




