---
title: Listar userExperienceAnalyticsMetrics
description: Listar propriedades e relações dos objetos userExperienceAnalyticsMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfe3a63b8618ba5e888271b510587832bcefe7c2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157874"
---
# <a name="list-userexperienceanalyticsmetrics"></a><span data-ttu-id="82035-103">Listar userExperienceAnalyticsMetrics</span><span class="sxs-lookup"><span data-stu-id="82035-103">List userExperienceAnalyticsMetrics</span></span>

<span data-ttu-id="82035-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82035-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82035-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82035-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82035-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82035-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82035-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="82035-107">List properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82035-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82035-108">Prerequisites</span></span>
<span data-ttu-id="82035-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82035-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82035-111">Permission type</span></span>|<span data-ttu-id="82035-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82035-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82035-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82035-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82035-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82035-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="82035-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82035-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82035-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82035-116">Not supported.</span></span>|
|<span data-ttu-id="82035-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82035-117">Application</span></span>|<span data-ttu-id="82035-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82035-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82035-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82035-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="82035-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82035-120">Request headers</span></span>
|<span data-ttu-id="82035-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82035-121">Header</span></span>|<span data-ttu-id="82035-122">Valor</span><span class="sxs-lookup"><span data-stu-id="82035-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82035-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82035-123">Authorization</span></span>|<span data-ttu-id="82035-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82035-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82035-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82035-125">Accept</span></span>|<span data-ttu-id="82035-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82035-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82035-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82035-127">Request body</span></span>
<span data-ttu-id="82035-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="82035-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82035-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="82035-129">Response</span></span>
<span data-ttu-id="82035-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82035-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82035-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82035-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="82035-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82035-132">Request</span></span>
<span data-ttu-id="82035-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82035-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
```

### <a name="response"></a><span data-ttu-id="82035-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="82035-134">Response</span></span>
<span data-ttu-id="82035-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82035-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 226

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
      "id": "1371822e-822e-1371-2e82-71132e827113",
      "value": 1.6666666666666667,
      "unit": "Unit value"
    }
  ]
}
```




