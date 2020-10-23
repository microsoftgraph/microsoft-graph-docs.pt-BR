---
title: Criar userExperienceAnalyticsMetric
description: Criar um novo objeto userExperienceAnalyticsMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1fbdb73cf1db5769e7319002923cf7466c80f9e1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731229"
---
# <a name="create-userexperienceanalyticsmetric"></a><span data-ttu-id="b8688-103">Criar userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="b8688-103">Create userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="b8688-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8688-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8688-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8688-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8688-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8688-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8688-107">Criar um novo objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="b8688-107">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8688-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8688-108">Prerequisites</span></span>
<span data-ttu-id="b8688-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8688-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8688-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8688-111">Permission type</span></span>|<span data-ttu-id="b8688-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8688-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8688-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8688-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8688-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8688-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b8688-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8688-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8688-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8688-116">Not supported.</span></span>|
|<span data-ttu-id="b8688-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8688-117">Application</span></span>|<span data-ttu-id="b8688-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8688-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8688-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8688-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b8688-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8688-120">Request headers</span></span>
|<span data-ttu-id="b8688-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8688-121">Header</span></span>|<span data-ttu-id="b8688-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8688-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8688-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8688-123">Authorization</span></span>|<span data-ttu-id="b8688-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8688-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8688-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8688-125">Accept</span></span>|<span data-ttu-id="b8688-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8688-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8688-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8688-127">Request body</span></span>
<span data-ttu-id="b8688-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="b8688-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetric object.</span></span>

<span data-ttu-id="b8688-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="b8688-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetric.</span></span>

|<span data-ttu-id="b8688-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8688-130">Property</span></span>|<span data-ttu-id="b8688-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8688-131">Type</span></span>|<span data-ttu-id="b8688-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8688-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8688-133">id</span><span class="sxs-lookup"><span data-stu-id="b8688-133">id</span></span>|<span data-ttu-id="b8688-134">String</span><span class="sxs-lookup"><span data-stu-id="b8688-134">String</span></span>|<span data-ttu-id="b8688-135">O identificador exclusivo da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8688-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="b8688-136">valor</span><span class="sxs-lookup"><span data-stu-id="b8688-136">value</span></span>|<span data-ttu-id="b8688-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="b8688-137">Double</span></span>|<span data-ttu-id="b8688-138">O valor da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8688-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="b8688-139">unidade</span><span class="sxs-lookup"><span data-stu-id="b8688-139">unit</span></span>|<span data-ttu-id="b8688-140">String</span><span class="sxs-lookup"><span data-stu-id="b8688-140">String</span></span>|<span data-ttu-id="b8688-141">A unidade da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8688-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="b8688-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8688-142">Response</span></span>
<span data-ttu-id="b8688-143">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8688-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8688-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8688-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8688-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8688-145">Request</span></span>
<span data-ttu-id="b8688-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8688-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="b8688-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8688-147">Response</span></span>
<span data-ttu-id="b8688-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8688-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```





