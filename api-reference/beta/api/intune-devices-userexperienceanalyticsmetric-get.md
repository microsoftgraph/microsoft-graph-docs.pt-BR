---
title: Obter userExperienceAnalyticsMetric
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsMetric.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19f4fc6ffa4fec8af5b559297b1e2600211bf94c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43379315"
---
# <a name="get-userexperienceanalyticsmetric"></a><span data-ttu-id="707bb-103">Obter userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="707bb-103">Get userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="707bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="707bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="707bb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="707bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="707bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="707bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="707bb-107">Leia as propriedades e as relações do objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="707bb-107">Read properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="707bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="707bb-108">Prerequisites</span></span>
<span data-ttu-id="707bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="707bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="707bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="707bb-111">Permission type</span></span>|<span data-ttu-id="707bb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="707bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="707bb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="707bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="707bb-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="707bb-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="707bb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="707bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="707bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="707bb-116">Not supported.</span></span>|
|<span data-ttu-id="707bb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="707bb-117">Application</span></span>|<span data-ttu-id="707bb-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="707bb-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="707bb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="707bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="707bb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="707bb-120">Optional query parameters</span></span>
<span data-ttu-id="707bb-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="707bb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="707bb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="707bb-122">Request headers</span></span>
|<span data-ttu-id="707bb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="707bb-123">Header</span></span>|<span data-ttu-id="707bb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="707bb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="707bb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="707bb-125">Authorization</span></span>|<span data-ttu-id="707bb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="707bb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="707bb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="707bb-127">Accept</span></span>|<span data-ttu-id="707bb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="707bb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="707bb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="707bb-129">Request body</span></span>
<span data-ttu-id="707bb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="707bb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="707bb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="707bb-131">Response</span></span>
<span data-ttu-id="707bb-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="707bb-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="707bb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="707bb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="707bb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="707bb-134">Request</span></span>
<span data-ttu-id="707bb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="707bb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
```

### <a name="response"></a><span data-ttu-id="707bb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="707bb-136">Response</span></span>
<span data-ttu-id="707bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="707bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
    "id": "1371822e-822e-1371-2e82-71132e827113",
    "value": "<Unknown Primitive Type Edm.Double>",
    "unit": "Unit value"
  }
}
```



