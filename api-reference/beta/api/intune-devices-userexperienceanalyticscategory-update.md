---
title: Atualizar userExperienceAnalyticsCategory
description: Atualiza as propriedades de um objeto userExperienceAnalyticsCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 475f6b28ee6f4838feccf496af3d94c76f974f23
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180141"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="14b09-103">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="14b09-103">Update userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="14b09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14b09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14b09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14b09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14b09-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="14b09-106">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14b09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14b09-107">Prerequisites</span></span>
<span data-ttu-id="14b09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14b09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14b09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14b09-110">Permission type</span></span>|<span data-ttu-id="14b09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14b09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14b09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14b09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14b09-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b09-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="14b09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14b09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14b09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14b09-115">Not supported.</span></span>|
|<span data-ttu-id="14b09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14b09-116">Application</span></span>|<span data-ttu-id="14b09-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b09-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14b09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14b09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="14b09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14b09-119">Request headers</span></span>
|<span data-ttu-id="14b09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14b09-120">Header</span></span>|<span data-ttu-id="14b09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="14b09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14b09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14b09-122">Authorization</span></span>|<span data-ttu-id="14b09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14b09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14b09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14b09-124">Accept</span></span>|<span data-ttu-id="14b09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14b09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14b09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14b09-126">Request body</span></span>
<span data-ttu-id="14b09-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="14b09-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="14b09-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="14b09-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="14b09-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14b09-129">Property</span></span>|<span data-ttu-id="14b09-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="14b09-130">Type</span></span>|<span data-ttu-id="14b09-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="14b09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14b09-132">id</span><span class="sxs-lookup"><span data-stu-id="14b09-132">id</span></span>|<span data-ttu-id="14b09-133">String</span><span class="sxs-lookup"><span data-stu-id="14b09-133">String</span></span>|<span data-ttu-id="14b09-134">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="14b09-134">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="14b09-135">overallScore</span><span class="sxs-lookup"><span data-stu-id="14b09-135">overallScore</span></span>|<span data-ttu-id="14b09-136">Int32</span><span class="sxs-lookup"><span data-stu-id="14b09-136">Int32</span></span>|<span data-ttu-id="14b09-137">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="14b09-137">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="14b09-138">insights</span><span class="sxs-lookup"><span data-stu-id="14b09-138">insights</span></span>|<span data-ttu-id="14b09-139">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="14b09-139">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="14b09-140">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="14b09-140">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="14b09-141">estado</span><span class="sxs-lookup"><span data-stu-id="14b09-141">state</span></span>|[<span data-ttu-id="14b09-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="14b09-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="14b09-143">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="14b09-143">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="14b09-144">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="14b09-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="14b09-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="14b09-145">Response</span></span>
<span data-ttu-id="14b09-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14b09-146">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14b09-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14b09-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="14b09-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14b09-148">Request</span></span>
<span data-ttu-id="14b09-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14b09-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 572

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
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
```

### <a name="response"></a><span data-ttu-id="14b09-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="14b09-150">Response</span></span>
<span data-ttu-id="14b09-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14b09-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 621

{
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
```




