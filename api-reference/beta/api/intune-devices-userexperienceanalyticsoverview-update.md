---
title: Atualizar userExperienceAnalyticsOverview
description: Atualiza as propriedades de um objeto userExperienceAnalyticsOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb00499ea103b89dc45e1b5028858b0747f5163e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350416"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="059fb-103">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="059fb-103">Update userExperienceAnalyticsOverview</span></span>

> <span data-ttu-id="059fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="059fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="059fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="059fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="059fb-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="059fb-106">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="059fb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="059fb-107">Prerequisites</span></span>
<span data-ttu-id="059fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="059fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="059fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="059fb-110">Permission type</span></span>|<span data-ttu-id="059fb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="059fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="059fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="059fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="059fb-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="059fb-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="059fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="059fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="059fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="059fb-115">Not supported.</span></span>|
|<span data-ttu-id="059fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="059fb-116">Application</span></span>|<span data-ttu-id="059fb-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="059fb-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="059fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="059fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="059fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="059fb-119">Request headers</span></span>
|<span data-ttu-id="059fb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="059fb-120">Header</span></span>|<span data-ttu-id="059fb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="059fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="059fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="059fb-122">Authorization</span></span>|<span data-ttu-id="059fb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="059fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="059fb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="059fb-124">Accept</span></span>|<span data-ttu-id="059fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="059fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="059fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="059fb-126">Request body</span></span>
<span data-ttu-id="059fb-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="059fb-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="059fb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="059fb-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="059fb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="059fb-129">Property</span></span>|<span data-ttu-id="059fb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="059fb-130">Type</span></span>|<span data-ttu-id="059fb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="059fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="059fb-132">id</span><span class="sxs-lookup"><span data-stu-id="059fb-132">id</span></span>|<span data-ttu-id="059fb-133">String</span><span class="sxs-lookup"><span data-stu-id="059fb-133">String</span></span>|<span data-ttu-id="059fb-134">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="059fb-134">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="059fb-135">overallScore</span><span class="sxs-lookup"><span data-stu-id="059fb-135">overallScore</span></span>|<span data-ttu-id="059fb-136">Int32</span><span class="sxs-lookup"><span data-stu-id="059fb-136">Int32</span></span>|<span data-ttu-id="059fb-137">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="059fb-137">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="059fb-138">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="059fb-138">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="059fb-139">Int32</span><span class="sxs-lookup"><span data-stu-id="059fb-139">Int32</span></span>|<span data-ttu-id="059fb-140">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="059fb-140">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="059fb-141">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="059fb-141">bestPracticesOverallScore</span></span>|<span data-ttu-id="059fb-142">Int32</span><span class="sxs-lookup"><span data-stu-id="059fb-142">Int32</span></span>|<span data-ttu-id="059fb-143">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="059fb-143">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="059fb-144">insights</span><span class="sxs-lookup"><span data-stu-id="059fb-144">insights</span></span>|<span data-ttu-id="059fb-145">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="059fb-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="059fb-146">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="059fb-146">The user experience analytics insights.</span></span>|



## <a name="response"></a><span data-ttu-id="059fb-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="059fb-147">Response</span></span>
<span data-ttu-id="059fb-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="059fb-148">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="059fb-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="059fb-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="059fb-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="059fb-150">Request</span></span>
<span data-ttu-id="059fb-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="059fb-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
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

### <a name="response"></a><span data-ttu-id="059fb-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="059fb-152">Response</span></span>
<span data-ttu-id="059fb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="059fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 571

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
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






