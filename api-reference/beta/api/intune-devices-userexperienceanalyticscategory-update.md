---
title: Atualizar userExperienceAnalyticsCategory
description: Atualiza as propriedades de um objeto userExperienceAnalyticsCategory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 550aea2dce1fb11c6888f8652ef39b9d0a6d84cb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43322588"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="a9c5c-103">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="a9c5c-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="a9c5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9c5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9c5c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9c5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9c5c-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="a9c5c-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9c5c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9c5c-108">Prerequisites</span></span>
<span data-ttu-id="a9c5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9c5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9c5c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9c5c-111">Permission type</span></span>|<span data-ttu-id="a9c5c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9c5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9c5c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9c5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9c5c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9c5c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a9c5c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9c5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9c5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-116">Not supported.</span></span>|
|<span data-ttu-id="a9c5c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9c5c-117">Application</span></span>|<span data-ttu-id="a9c5c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9c5c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9c5c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9c5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="a9c5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c5c-120">Request headers</span></span>
|<span data-ttu-id="a9c5c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9c5c-121">Header</span></span>|<span data-ttu-id="a9c5c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9c5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9c5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9c5c-123">Authorization</span></span>|<span data-ttu-id="a9c5c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9c5c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9c5c-125">Accept</span></span>|<span data-ttu-id="a9c5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9c5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9c5c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c5c-127">Request body</span></span>
<span data-ttu-id="a9c5c-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="a9c5c-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="a9c5c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="a9c5c-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="a9c5c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9c5c-130">Property</span></span>|<span data-ttu-id="a9c5c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9c5c-131">Type</span></span>|<span data-ttu-id="a9c5c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9c5c-133">id</span><span class="sxs-lookup"><span data-stu-id="a9c5c-133">id</span></span>|<span data-ttu-id="a9c5c-134">String</span><span class="sxs-lookup"><span data-stu-id="a9c5c-134">String</span></span>|<span data-ttu-id="a9c5c-135">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="a9c5c-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="a9c5c-136">overallScore</span></span>|<span data-ttu-id="a9c5c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a9c5c-137">Int32</span></span>|<span data-ttu-id="a9c5c-138">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="a9c5c-139">insights</span><span class="sxs-lookup"><span data-stu-id="a9c5c-139">insights</span></span>|<span data-ttu-id="a9c5c-140">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="a9c5c-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="a9c5c-141">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-141">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="a9c5c-142">state</span><span class="sxs-lookup"><span data-stu-id="a9c5c-142">state</span></span>|[<span data-ttu-id="a9c5c-143">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a9c5c-143">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a9c5c-144">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-144">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="a9c5c-145">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-145">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="a9c5c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9c5c-146">Response</span></span>
<span data-ttu-id="a9c5c-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-147">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9c5c-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9c5c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9c5c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c5c-149">Request</span></span>
<span data-ttu-id="a9c5c-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9c5c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9c5c-151">Response</span></span>
<span data-ttu-id="a9c5c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9c5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



