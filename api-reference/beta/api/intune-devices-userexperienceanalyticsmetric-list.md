---
title: Listar userExperienceAnalyticsMetrics
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsMetric.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30a72de1206d99d7bfd3a82e8ae57bf034810156
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176005"
---
# <a name="list-userexperienceanalyticsmetrics"></a><span data-ttu-id="e7ce6-103">Listar userExperienceAnalyticsMetrics</span><span class="sxs-lookup"><span data-stu-id="e7ce6-103">List userExperienceAnalyticsMetrics</span></span>

<span data-ttu-id="e7ce6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7ce6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7ce6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7ce6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7ce6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7ce6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7ce6-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="e7ce6-107">List properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7ce6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7ce6-108">Prerequisites</span></span>
<span data-ttu-id="e7ce6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7ce6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7ce6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7ce6-111">Permission type</span></span>|<span data-ttu-id="e7ce6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7ce6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7ce6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7ce6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7ce6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7ce6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e7ce6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7ce6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7ce6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7ce6-116">Not supported.</span></span>|
|<span data-ttu-id="e7ce6-117">Application</span><span class="sxs-lookup"><span data-stu-id="e7ce6-117">Application</span></span>|<span data-ttu-id="e7ce6-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7ce6-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7ce6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7ce6-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e7ce6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7ce6-120">Request headers</span></span>
|<span data-ttu-id="e7ce6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7ce6-121">Header</span></span>|<span data-ttu-id="e7ce6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e7ce6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7ce6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7ce6-123">Authorization</span></span>|<span data-ttu-id="e7ce6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7ce6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7ce6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7ce6-125">Accept</span></span>|<span data-ttu-id="e7ce6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7ce6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7ce6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7ce6-127">Request body</span></span>
<span data-ttu-id="e7ce6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7ce6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7ce6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7ce6-129">Response</span></span>
<span data-ttu-id="e7ce6-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7ce6-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7ce6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7ce6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7ce6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7ce6-132">Request</span></span>
<span data-ttu-id="e7ce6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7ce6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
```

### <a name="response"></a><span data-ttu-id="e7ce6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7ce6-134">Response</span></span>
<span data-ttu-id="e7ce6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7ce6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



