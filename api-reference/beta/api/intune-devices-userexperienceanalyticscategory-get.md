---
title: Obter userExperienceAnalyticsCategory
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6a5ae09689d491d1ecb334c3dbbf56f8f239d44
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155080"
---
# <a name="get-userexperienceanalyticscategory"></a><span data-ttu-id="2b6a1-103">Obter userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="2b6a1-103">Get userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="2b6a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b6a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b6a1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b6a1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b6a1-107">Leia as propriedades e as relações do [objeto userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="2b6a1-107">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b6a1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b6a1-108">Prerequisites</span></span>
<span data-ttu-id="2b6a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b6a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b6a1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b6a1-111">Permission type</span></span>|<span data-ttu-id="2b6a1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b6a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b6a1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b6a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b6a1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b6a1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2b6a1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b6a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b6a1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-116">Not supported.</span></span>|
|<span data-ttu-id="2b6a1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b6a1-117">Application</span></span>|<span data-ttu-id="2b6a1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b6a1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b6a1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b6a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthOverview
GET /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/appHealthMetrics
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/rebootAnalyticsMetrics
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b6a1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2b6a1-120">Optional query parameters</span></span>
<span data-ttu-id="2b6a1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b6a1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b6a1-122">Request headers</span></span>
|<span data-ttu-id="2b6a1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b6a1-123">Header</span></span>|<span data-ttu-id="2b6a1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2b6a1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b6a1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b6a1-125">Authorization</span></span>|<span data-ttu-id="2b6a1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b6a1-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b6a1-127">Accept</span></span>|<span data-ttu-id="2b6a1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2b6a1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6a1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b6a1-129">Request body</span></span>
<span data-ttu-id="2b6a1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b6a1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b6a1-131">Response</span></span>
<span data-ttu-id="2b6a1-132">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b6a1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b6a1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b6a1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b6a1-134">Request</span></span>
<span data-ttu-id="2b6a1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOverview
```

### <a name="response"></a><span data-ttu-id="2b6a1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b6a1-136">Response</span></span>
<span data-ttu-id="2b6a1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b6a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 657

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
    "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
    "overallScore": 12,
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
    "state": "insufficientData"
  }
}
```




