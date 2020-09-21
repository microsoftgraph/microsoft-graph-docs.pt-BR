---
title: Atualizar userExperienceAnalyticsMetric
description: Atualiza as propriedades de um objeto userExperienceAnalyticsMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7daf4c416d3664baed18f7299135e05a422de9bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970128"
---
# <a name="update-userexperienceanalyticsmetric"></a><span data-ttu-id="ef2ee-103">Atualizar userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="ef2ee-103">Update userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="ef2ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef2ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef2ee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef2ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef2ee-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="ef2ee-107">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef2ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef2ee-108">Prerequisites</span></span>
<span data-ttu-id="ef2ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef2ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef2ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef2ee-111">Permission type</span></span>|<span data-ttu-id="ef2ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef2ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef2ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef2ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef2ee-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2ee-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ef2ee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef2ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef2ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-116">Not supported.</span></span>|
|<span data-ttu-id="ef2ee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef2ee-117">Application</span></span>|<span data-ttu-id="ef2ee-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2ee-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef2ee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef2ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}/userExperienceAnalyticsMetric
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="ef2ee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef2ee-120">Request headers</span></span>
|<span data-ttu-id="ef2ee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef2ee-121">Header</span></span>|<span data-ttu-id="ef2ee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef2ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef2ee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef2ee-123">Authorization</span></span>|<span data-ttu-id="ef2ee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef2ee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef2ee-125">Accept</span></span>|<span data-ttu-id="ef2ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef2ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef2ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef2ee-127">Request body</span></span>
<span data-ttu-id="ef2ee-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="ef2ee-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

<span data-ttu-id="ef2ee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span><span class="sxs-lookup"><span data-stu-id="ef2ee-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>

|<span data-ttu-id="ef2ee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef2ee-130">Property</span></span>|<span data-ttu-id="ef2ee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef2ee-131">Type</span></span>|<span data-ttu-id="ef2ee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef2ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef2ee-133">id</span><span class="sxs-lookup"><span data-stu-id="ef2ee-133">id</span></span>|<span data-ttu-id="ef2ee-134">String</span><span class="sxs-lookup"><span data-stu-id="ef2ee-134">String</span></span>|<span data-ttu-id="ef2ee-135">O identificador exclusivo da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="ef2ee-136">valor</span><span class="sxs-lookup"><span data-stu-id="ef2ee-136">value</span></span>|<span data-ttu-id="ef2ee-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="ef2ee-137">Double</span></span>|<span data-ttu-id="ef2ee-138">O valor da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="ef2ee-139">unidade</span><span class="sxs-lookup"><span data-stu-id="ef2ee-139">unit</span></span>|<span data-ttu-id="ef2ee-140">String</span><span class="sxs-lookup"><span data-stu-id="ef2ee-140">String</span></span>|<span data-ttu-id="ef2ee-141">A unidade da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="ef2ee-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef2ee-142">Response</span></span>
<span data-ttu-id="ef2ee-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-143">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef2ee-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef2ee-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef2ee-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef2ee-145">Request</span></span>
<span data-ttu-id="ef2ee-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="ef2ee-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef2ee-147">Response</span></span>
<span data-ttu-id="ef2ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef2ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```






