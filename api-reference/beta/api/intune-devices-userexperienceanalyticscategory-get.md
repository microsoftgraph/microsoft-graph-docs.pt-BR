---
title: Obter userExperienceAnalyticsCategory
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba9d2ef8618a3b409884ae630ae5b81bc922b97a
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087465"
---
# <a name="get-userexperienceanalyticscategory"></a><span data-ttu-id="91e31-103">Obter userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="91e31-103">Get userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="91e31-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91e31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91e31-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91e31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91e31-106">Leia as propriedades e as relações do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="91e31-106">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91e31-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91e31-107">Prerequisites</span></span>
<span data-ttu-id="91e31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91e31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91e31-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91e31-110">Permission type</span></span>|<span data-ttu-id="91e31-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91e31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91e31-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91e31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91e31-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="91e31-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="91e31-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91e31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91e31-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91e31-115">Not supported.</span></span>|
|<span data-ttu-id="91e31-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91e31-116">Application</span></span>|<span data-ttu-id="91e31-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="91e31-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91e31-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91e31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91e31-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91e31-119">Optional query parameters</span></span>
<span data-ttu-id="91e31-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="91e31-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91e31-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91e31-121">Request headers</span></span>
|<span data-ttu-id="91e31-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91e31-122">Header</span></span>|<span data-ttu-id="91e31-123">Valor</span><span class="sxs-lookup"><span data-stu-id="91e31-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91e31-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="91e31-124">Authorization</span></span>|<span data-ttu-id="91e31-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91e31-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91e31-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91e31-126">Accept</span></span>|<span data-ttu-id="91e31-127">application/json</span><span class="sxs-lookup"><span data-stu-id="91e31-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91e31-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91e31-128">Request body</span></span>
<span data-ttu-id="91e31-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91e31-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91e31-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="91e31-130">Response</span></span>
<span data-ttu-id="91e31-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91e31-131">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91e31-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91e31-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="91e31-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91e31-133">Request</span></span>
<span data-ttu-id="91e31-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91e31-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
```

### <a name="response"></a><span data-ttu-id="91e31-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="91e31-135">Response</span></span>
<span data-ttu-id="91e31-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91e31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 676

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
            "value": "<Unknown Primitive Type Edm.Double>"
          }
        ],
        "severity": "informational"
      }
    ],
    "state": "insufficientData"
  }
}
```






