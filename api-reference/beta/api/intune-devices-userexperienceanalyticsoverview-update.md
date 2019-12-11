---
title: Atualizar userExperienceAnalyticsOverview
description: Atualiza as propriedades de um objeto userExperienceAnalyticsOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2140a8955b49f0f792058dffd6c743d75b8bd97
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944390"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="542f0-103">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="542f0-103">Update userExperienceAnalyticsOverview</span></span>

> <span data-ttu-id="542f0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="542f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="542f0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="542f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="542f0-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="542f0-106">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="542f0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="542f0-107">Prerequisites</span></span>
<span data-ttu-id="542f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="542f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="542f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="542f0-110">Permission type</span></span>|<span data-ttu-id="542f0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="542f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="542f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="542f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="542f0-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542f0-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="542f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="542f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="542f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="542f0-115">Not supported.</span></span>|
|<span data-ttu-id="542f0-116">Application</span><span class="sxs-lookup"><span data-stu-id="542f0-116">Application</span></span>|<span data-ttu-id="542f0-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542f0-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="542f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="542f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="542f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="542f0-119">Request headers</span></span>
|<span data-ttu-id="542f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="542f0-120">Header</span></span>|<span data-ttu-id="542f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="542f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="542f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="542f0-122">Authorization</span></span>|<span data-ttu-id="542f0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="542f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="542f0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="542f0-124">Accept</span></span>|<span data-ttu-id="542f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="542f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="542f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="542f0-126">Request body</span></span>
<span data-ttu-id="542f0-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="542f0-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="542f0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="542f0-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="542f0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="542f0-129">Property</span></span>|<span data-ttu-id="542f0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="542f0-130">Type</span></span>|<span data-ttu-id="542f0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="542f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="542f0-132">id</span><span class="sxs-lookup"><span data-stu-id="542f0-132">id</span></span>|<span data-ttu-id="542f0-133">String</span><span class="sxs-lookup"><span data-stu-id="542f0-133">String</span></span>|<span data-ttu-id="542f0-134">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="542f0-134">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="542f0-135">overallScore</span><span class="sxs-lookup"><span data-stu-id="542f0-135">overallScore</span></span>|<span data-ttu-id="542f0-136">Int32</span><span class="sxs-lookup"><span data-stu-id="542f0-136">Int32</span></span>|<span data-ttu-id="542f0-137">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="542f0-137">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="542f0-138">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="542f0-138">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="542f0-139">Int32</span><span class="sxs-lookup"><span data-stu-id="542f0-139">Int32</span></span>|<span data-ttu-id="542f0-140">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="542f0-140">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="542f0-141">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="542f0-141">bestPracticesOverallScore</span></span>|<span data-ttu-id="542f0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="542f0-142">Int32</span></span>|<span data-ttu-id="542f0-143">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="542f0-143">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="542f0-144">insights</span><span class="sxs-lookup"><span data-stu-id="542f0-144">insights</span></span>|<span data-ttu-id="542f0-145">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="542f0-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="542f0-146">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="542f0-146">The user experience analytics insights.</span></span>|
|<span data-ttu-id="542f0-147">state</span><span class="sxs-lookup"><span data-stu-id="542f0-147">state</span></span>|[<span data-ttu-id="542f0-148">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="542f0-148">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="542f0-149">O estado de integridade atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="542f0-149">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="542f0-150">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="542f0-150">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="542f0-151">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="542f0-151">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="542f0-152">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="542f0-152">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="542f0-153">O estado de integridade atual da categoria "BootPerformance" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="542f0-153">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="542f0-154">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="542f0-154">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="542f0-155">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="542f0-155">bestPracticesHealthState</span></span>|[<span data-ttu-id="542f0-156">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="542f0-156">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="542f0-157">O estado de integridade atual da categoria "BestPractices" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="542f0-157">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="542f0-158">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="542f0-158">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="542f0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="542f0-159">Response</span></span>
<span data-ttu-id="542f0-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="542f0-160">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="542f0-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="542f0-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="542f0-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="542f0-162">Request</span></span>
<span data-ttu-id="542f0-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="542f0-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 760

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
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="542f0-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="542f0-164">Response</span></span>
<span data-ttu-id="542f0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="542f0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 809

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
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```





