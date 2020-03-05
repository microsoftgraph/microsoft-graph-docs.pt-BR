---
title: Atualizar userExperienceAnalyticsCategory
description: Atualiza as propriedades de um objeto userExperienceAnalyticsCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7309621128d2adfd41cdc7869bcfaea995ba500
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468457"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="cc403-103">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="cc403-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="cc403-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cc403-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc403-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc403-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc403-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc403-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc403-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="cc403-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc403-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc403-108">Prerequisites</span></span>
<span data-ttu-id="cc403-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc403-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc403-111">Permission type</span></span>|<span data-ttu-id="cc403-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc403-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc403-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc403-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc403-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc403-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cc403-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc403-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc403-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc403-116">Not supported.</span></span>|
|<span data-ttu-id="cc403-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc403-117">Application</span></span>|<span data-ttu-id="cc403-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc403-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc403-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc403-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="cc403-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc403-120">Request headers</span></span>
|<span data-ttu-id="cc403-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc403-121">Header</span></span>|<span data-ttu-id="cc403-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cc403-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc403-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc403-123">Authorization</span></span>|<span data-ttu-id="cc403-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc403-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc403-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc403-125">Accept</span></span>|<span data-ttu-id="cc403-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc403-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc403-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc403-127">Request body</span></span>
<span data-ttu-id="cc403-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="cc403-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="cc403-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="cc403-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="cc403-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc403-130">Property</span></span>|<span data-ttu-id="cc403-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc403-131">Type</span></span>|<span data-ttu-id="cc403-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc403-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc403-133">id</span><span class="sxs-lookup"><span data-stu-id="cc403-133">id</span></span>|<span data-ttu-id="cc403-134">String</span><span class="sxs-lookup"><span data-stu-id="cc403-134">String</span></span>|<span data-ttu-id="cc403-135">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cc403-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="cc403-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="cc403-136">overallScore</span></span>|<span data-ttu-id="cc403-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cc403-137">Int32</span></span>|<span data-ttu-id="cc403-138">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cc403-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="cc403-139">insights</span><span class="sxs-lookup"><span data-stu-id="cc403-139">insights</span></span>|<span data-ttu-id="cc403-140">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="cc403-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="cc403-141">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cc403-141">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="cc403-142">state</span><span class="sxs-lookup"><span data-stu-id="cc403-142">state</span></span>|[<span data-ttu-id="cc403-143">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="cc403-143">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="cc403-144">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cc403-144">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="cc403-145">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="cc403-145">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="cc403-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc403-146">Response</span></span>
<span data-ttu-id="cc403-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc403-147">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc403-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc403-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc403-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc403-149">Request</span></span>
<span data-ttu-id="cc403-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc403-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc403-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc403-151">Response</span></span>
<span data-ttu-id="cc403-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc403-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





