---
title: Criar userExperienceAnalyticsMetric
description: Criar um novo objeto userExperienceAnalyticsMetric.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9e8ca95bcb11d26212f0248fcced244d6edbc9d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468233"
---
# <a name="create-userexperienceanalyticsmetric"></a><span data-ttu-id="56981-103">Criar userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="56981-103">Create userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="56981-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="56981-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56981-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56981-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56981-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56981-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56981-107">Criar um novo objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="56981-107">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56981-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56981-108">Prerequisites</span></span>
<span data-ttu-id="56981-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56981-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56981-111">Permission type</span></span>|<span data-ttu-id="56981-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56981-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56981-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56981-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56981-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56981-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="56981-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56981-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56981-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56981-116">Not supported.</span></span>|
|<span data-ttu-id="56981-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56981-117">Application</span></span>|<span data-ttu-id="56981-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56981-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56981-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56981-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression
POST /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="56981-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56981-120">Request headers</span></span>
|<span data-ttu-id="56981-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56981-121">Header</span></span>|<span data-ttu-id="56981-122">Valor</span><span class="sxs-lookup"><span data-stu-id="56981-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56981-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56981-123">Authorization</span></span>|<span data-ttu-id="56981-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56981-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56981-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56981-125">Accept</span></span>|<span data-ttu-id="56981-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56981-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56981-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56981-127">Request body</span></span>
<span data-ttu-id="56981-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="56981-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetric object.</span></span>

<span data-ttu-id="56981-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="56981-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetric.</span></span>

|<span data-ttu-id="56981-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56981-130">Property</span></span>|<span data-ttu-id="56981-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="56981-131">Type</span></span>|<span data-ttu-id="56981-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="56981-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56981-133">id</span><span class="sxs-lookup"><span data-stu-id="56981-133">id</span></span>|<span data-ttu-id="56981-134">String</span><span class="sxs-lookup"><span data-stu-id="56981-134">String</span></span>|<span data-ttu-id="56981-135">O identificador exclusivo da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="56981-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="56981-136">valor</span><span class="sxs-lookup"><span data-stu-id="56981-136">value</span></span>|<span data-ttu-id="56981-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="56981-137">Double</span></span>|<span data-ttu-id="56981-138">O valor da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="56981-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="56981-139">unidade</span><span class="sxs-lookup"><span data-stu-id="56981-139">unit</span></span>|<span data-ttu-id="56981-140">String</span><span class="sxs-lookup"><span data-stu-id="56981-140">String</span></span>|<span data-ttu-id="56981-141">A unidade da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="56981-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="56981-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="56981-142">Response</span></span>
<span data-ttu-id="56981-143">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56981-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56981-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56981-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="56981-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56981-145">Request</span></span>
<span data-ttu-id="56981-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56981-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="56981-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="56981-147">Response</span></span>
<span data-ttu-id="56981-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56981-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 196

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```





