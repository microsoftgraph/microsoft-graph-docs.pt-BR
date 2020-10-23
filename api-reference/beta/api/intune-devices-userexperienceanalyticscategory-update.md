---
title: Atualizar userExperienceAnalyticsCategory
description: Atualiza as propriedades de um objeto userExperienceAnalyticsCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81bab6e15c422ea1f3142f97c7943cb80ef66a9f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726077"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="0b421-103">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="0b421-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="0b421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b421-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b421-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b421-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b421-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b421-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="0b421-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b421-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b421-108">Prerequisites</span></span>
<span data-ttu-id="0b421-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b421-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b421-111">Permission type</span></span>|<span data-ttu-id="0b421-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b421-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b421-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b421-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b421-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b421-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0b421-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b421-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b421-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b421-116">Not supported.</span></span>|
|<span data-ttu-id="0b421-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b421-117">Application</span></span>|<span data-ttu-id="0b421-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b421-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b421-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b421-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthOverview
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/rebootAnalyticsMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="0b421-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b421-120">Request headers</span></span>
|<span data-ttu-id="0b421-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b421-121">Header</span></span>|<span data-ttu-id="0b421-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0b421-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b421-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b421-123">Authorization</span></span>|<span data-ttu-id="0b421-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b421-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b421-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b421-125">Accept</span></span>|<span data-ttu-id="0b421-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b421-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b421-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b421-127">Request body</span></span>
<span data-ttu-id="0b421-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="0b421-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="0b421-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="0b421-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="0b421-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b421-130">Property</span></span>|<span data-ttu-id="0b421-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b421-131">Type</span></span>|<span data-ttu-id="0b421-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b421-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b421-133">id</span><span class="sxs-lookup"><span data-stu-id="0b421-133">id</span></span>|<span data-ttu-id="0b421-134">String</span><span class="sxs-lookup"><span data-stu-id="0b421-134">String</span></span>|<span data-ttu-id="0b421-135">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="0b421-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="0b421-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="0b421-136">overallScore</span></span>|<span data-ttu-id="0b421-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0b421-137">Int32</span></span>|<span data-ttu-id="0b421-138">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="0b421-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="0b421-139">insights</span><span class="sxs-lookup"><span data-stu-id="0b421-139">insights</span></span>|<span data-ttu-id="0b421-140">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="0b421-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="0b421-141">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="0b421-141">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="0b421-142">state</span><span class="sxs-lookup"><span data-stu-id="0b421-142">state</span></span>|[<span data-ttu-id="0b421-143">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="0b421-143">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="0b421-144">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="0b421-144">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="0b421-145">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="0b421-145">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="0b421-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b421-146">Response</span></span>
<span data-ttu-id="0b421-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b421-147">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b421-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b421-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b421-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b421-149">Request</span></span>
<span data-ttu-id="0b421-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b421-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b421-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b421-151">Response</span></span>
<span data-ttu-id="0b421-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b421-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





