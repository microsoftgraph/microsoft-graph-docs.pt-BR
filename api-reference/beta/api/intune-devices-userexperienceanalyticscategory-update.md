---
title: Atualizar userExperienceAnalyticsCategory
description: Atualiza as propriedades de um objeto userExperienceAnalyticsCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f99c4bd2090f751b0a54df6ad408cda463266605
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350420"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="36aa1-103">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="36aa1-103">Update userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="36aa1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="36aa1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36aa1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36aa1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36aa1-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="36aa1-106">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36aa1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36aa1-107">Prerequisites</span></span>
<span data-ttu-id="36aa1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36aa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36aa1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36aa1-110">Permission type</span></span>|<span data-ttu-id="36aa1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36aa1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36aa1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36aa1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36aa1-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36aa1-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="36aa1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36aa1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36aa1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36aa1-115">Not supported.</span></span>|
|<span data-ttu-id="36aa1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36aa1-116">Application</span></span>|<span data-ttu-id="36aa1-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36aa1-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36aa1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36aa1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="36aa1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36aa1-119">Request headers</span></span>
|<span data-ttu-id="36aa1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36aa1-120">Header</span></span>|<span data-ttu-id="36aa1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="36aa1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36aa1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="36aa1-122">Authorization</span></span>|<span data-ttu-id="36aa1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36aa1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36aa1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36aa1-124">Accept</span></span>|<span data-ttu-id="36aa1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36aa1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36aa1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36aa1-126">Request body</span></span>
<span data-ttu-id="36aa1-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="36aa1-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="36aa1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="36aa1-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="36aa1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36aa1-129">Property</span></span>|<span data-ttu-id="36aa1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="36aa1-130">Type</span></span>|<span data-ttu-id="36aa1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="36aa1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36aa1-132">id</span><span class="sxs-lookup"><span data-stu-id="36aa1-132">id</span></span>|<span data-ttu-id="36aa1-133">String</span><span class="sxs-lookup"><span data-stu-id="36aa1-133">String</span></span>|<span data-ttu-id="36aa1-134">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="36aa1-134">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="36aa1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="36aa1-135">displayName</span></span>|<span data-ttu-id="36aa1-136">String</span><span class="sxs-lookup"><span data-stu-id="36aa1-136">String</span></span>|<span data-ttu-id="36aa1-137">O nome da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="36aa1-137">The name of the user experience analytics category.</span></span>|
|<span data-ttu-id="36aa1-138">overallScore</span><span class="sxs-lookup"><span data-stu-id="36aa1-138">overallScore</span></span>|<span data-ttu-id="36aa1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="36aa1-139">Int32</span></span>|<span data-ttu-id="36aa1-140">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="36aa1-140">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="36aa1-141">insights</span><span class="sxs-lookup"><span data-stu-id="36aa1-141">insights</span></span>|<span data-ttu-id="36aa1-142">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="36aa1-142">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="36aa1-143">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="36aa1-143">The insights for the user experience analytics category.</span></span>|



## <a name="response"></a><span data-ttu-id="36aa1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="36aa1-144">Response</span></span>
<span data-ttu-id="36aa1-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36aa1-145">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36aa1-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36aa1-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="36aa1-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36aa1-147">Request</span></span>
<span data-ttu-id="36aa1-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36aa1-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 484

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "displayName": "Display Name value",
  "overallScore": 12,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="36aa1-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="36aa1-149">Response</span></span>
<span data-ttu-id="36aa1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36aa1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 533

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "displayName": "Display Name value",
  "overallScore": 12,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```






