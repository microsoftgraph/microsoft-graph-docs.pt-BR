---
title: Atualizar userExperienceAnalyticsCategory
description: Atualizar as propriedades de um objeto userExperienceAnalyticsCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d2529e8bb6d07ec45dc7bee675594b10a02d696
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155073"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="b4f14-103">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="b4f14-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="b4f14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4f14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4f14-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4f14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4f14-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4f14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4f14-107">Atualizar as propriedades de [um objeto userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="b4f14-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4f14-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4f14-108">Prerequisites</span></span>
<span data-ttu-id="b4f14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4f14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4f14-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4f14-111">Permission type</span></span>|<span data-ttu-id="b4f14-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4f14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4f14-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4f14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4f14-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f14-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b4f14-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4f14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4f14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4f14-116">Not supported.</span></span>|
|<span data-ttu-id="b4f14-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4f14-117">Application</span></span>|<span data-ttu-id="b4f14-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f14-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4f14-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4f14-119">HTTP Request</span></span>
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
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="b4f14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4f14-120">Request headers</span></span>
|<span data-ttu-id="b4f14-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4f14-121">Header</span></span>|<span data-ttu-id="b4f14-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b4f14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4f14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4f14-123">Authorization</span></span>|<span data-ttu-id="b4f14-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4f14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4f14-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4f14-125">Accept</span></span>|<span data-ttu-id="b4f14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4f14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4f14-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4f14-127">Request body</span></span>
<span data-ttu-id="b4f14-128">No corpo da solicitação, fornece uma representação JSON do [objeto userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="b4f14-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="b4f14-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="b4f14-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="b4f14-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4f14-130">Property</span></span>|<span data-ttu-id="b4f14-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4f14-131">Type</span></span>|<span data-ttu-id="b4f14-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4f14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4f14-133">id</span><span class="sxs-lookup"><span data-stu-id="b4f14-133">id</span></span>|<span data-ttu-id="b4f14-134">String</span><span class="sxs-lookup"><span data-stu-id="b4f14-134">String</span></span>|<span data-ttu-id="b4f14-135">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b4f14-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="b4f14-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="b4f14-136">overallScore</span></span>|<span data-ttu-id="b4f14-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b4f14-137">Int32</span></span>|<span data-ttu-id="b4f14-138">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b4f14-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="b4f14-139">insights</span><span class="sxs-lookup"><span data-stu-id="b4f14-139">insights</span></span>|<span data-ttu-id="b4f14-140">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="b4f14-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="b4f14-141">As informações para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b4f14-141">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="b4f14-142">estado</span><span class="sxs-lookup"><span data-stu-id="b4f14-142">state</span></span>|[<span data-ttu-id="b4f14-143">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="b4f14-143">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="b4f14-144">O estado de saúde atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b4f14-144">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="b4f14-145">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="b4f14-145">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="b4f14-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4f14-146">Response</span></span>
<span data-ttu-id="b4f14-147">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4f14-147">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4f14-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4f14-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4f14-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4f14-149">Request</span></span>
<span data-ttu-id="b4f14-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4f14-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOverview
Content-type: application/json
Content-length: 553

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
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="b4f14-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4f14-151">Response</span></span>
<span data-ttu-id="b4f14-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4f14-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

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
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```




