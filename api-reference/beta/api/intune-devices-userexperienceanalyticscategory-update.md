---
title: Atualizar userExperienceAnalyticsCategory
description: Atualize as propriedades de um objeto userExperienceAnalyticsCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23f89e530972e3510efc8051d065c28a5cef7c89
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154235"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="806b3-103">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="806b3-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="806b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="806b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="806b3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="806b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="806b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="806b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="806b3-107">Atualize as propriedades de [um objeto userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="806b3-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="806b3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="806b3-108">Prerequisites</span></span>
<span data-ttu-id="806b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="806b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="806b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="806b3-111">Permission type</span></span>|<span data-ttu-id="806b3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="806b3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="806b3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="806b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="806b3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="806b3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="806b3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="806b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="806b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="806b3-116">Not supported.</span></span>|
|<span data-ttu-id="806b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="806b3-117">Application</span></span>|<span data-ttu-id="806b3-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="806b3-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="806b3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="806b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthOverview
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/appHealthMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/rebootAnalyticsMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/workFromAnywhereMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="806b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="806b3-120">Request headers</span></span>
|<span data-ttu-id="806b3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="806b3-121">Header</span></span>|<span data-ttu-id="806b3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="806b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="806b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="806b3-123">Authorization</span></span>|<span data-ttu-id="806b3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="806b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="806b3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="806b3-125">Accept</span></span>|<span data-ttu-id="806b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="806b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="806b3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="806b3-127">Request body</span></span>
<span data-ttu-id="806b3-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="806b3-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="806b3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="806b3-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="806b3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="806b3-130">Property</span></span>|<span data-ttu-id="806b3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="806b3-131">Type</span></span>|<span data-ttu-id="806b3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="806b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="806b3-133">id</span><span class="sxs-lookup"><span data-stu-id="806b3-133">id</span></span>|<span data-ttu-id="806b3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="806b3-134">String</span></span>|<span data-ttu-id="806b3-135">O identificador exclusivo da categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="806b3-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="806b3-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="806b3-136">overallScore</span></span>|<span data-ttu-id="806b3-137">Int32</span><span class="sxs-lookup"><span data-stu-id="806b3-137">Int32</span></span>|<span data-ttu-id="806b3-138">A pontuação geral da categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="806b3-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="806b3-139">totalDevices</span><span class="sxs-lookup"><span data-stu-id="806b3-139">totalDevices</span></span>|<span data-ttu-id="806b3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="806b3-140">Int32</span></span>|<span data-ttu-id="806b3-141">A contagem total de dispositivos da categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="806b3-141">The total device count of the user experience analytics category.</span></span>|
|<span data-ttu-id="806b3-142">insights</span><span class="sxs-lookup"><span data-stu-id="806b3-142">insights</span></span>|<span data-ttu-id="806b3-143">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="806b3-143">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="806b3-144">Os insights para a categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="806b3-144">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="806b3-145">state</span><span class="sxs-lookup"><span data-stu-id="806b3-145">state</span></span>|[<span data-ttu-id="806b3-146">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="806b3-146">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="806b3-147">O estado de saúde atual da categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="806b3-147">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="806b3-148">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="806b3-148">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="806b3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="806b3-149">Response</span></span>
<span data-ttu-id="806b3-150">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="806b3-150">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="806b3-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="806b3-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="806b3-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="806b3-152">Request</span></span>
<span data-ttu-id="806b3-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="806b3-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOverview
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "overallScore": 12,
  "totalDevices": 12,
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
```

### <a name="response"></a><span data-ttu-id="806b3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="806b3-154">Response</span></span>
<span data-ttu-id="806b3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="806b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 625

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "overallScore": 12,
  "totalDevices": 12,
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
```




