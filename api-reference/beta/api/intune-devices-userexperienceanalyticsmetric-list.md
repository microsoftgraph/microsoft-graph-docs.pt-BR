---
title: Listar userExperienceAnalyticsMetrics
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsMetric.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1ea9b5aef45661be6cd24a1a02347ad9f40c216
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180108"
---
# <a name="list-userexperienceanalyticsmetrics"></a><span data-ttu-id="837be-103">Listar userExperienceAnalyticsMetrics</span><span class="sxs-lookup"><span data-stu-id="837be-103">List userExperienceAnalyticsMetrics</span></span>

> <span data-ttu-id="837be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="837be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="837be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="837be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="837be-106">Listar Propriedades e relações dos objetos [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="837be-106">List properties and relationships of the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="837be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="837be-107">Prerequisites</span></span>
<span data-ttu-id="837be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="837be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="837be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="837be-110">Permission type</span></span>|<span data-ttu-id="837be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="837be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="837be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="837be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="837be-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="837be-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="837be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="837be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="837be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="837be-115">Not supported.</span></span>|
|<span data-ttu-id="837be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="837be-116">Application</span></span>|<span data-ttu-id="837be-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="837be-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="837be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="837be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="837be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="837be-119">Request headers</span></span>
|<span data-ttu-id="837be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="837be-120">Header</span></span>|<span data-ttu-id="837be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="837be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="837be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="837be-122">Authorization</span></span>|<span data-ttu-id="837be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="837be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="837be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="837be-124">Accept</span></span>|<span data-ttu-id="837be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="837be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="837be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="837be-126">Request body</span></span>
<span data-ttu-id="837be-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="837be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="837be-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="837be-128">Response</span></span>
<span data-ttu-id="837be-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="837be-129">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="837be-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="837be-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="837be-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="837be-131">Request</span></span>
<span data-ttu-id="837be-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="837be-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

### <a name="response"></a><span data-ttu-id="837be-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="837be-133">Response</span></span>
<span data-ttu-id="837be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="837be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 245

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
      "id": "1371822e-822e-1371-2e82-71132e827113",
      "value": "<Unknown Primitive Type Edm.Double>",
      "unit": "Unit value"
    }
  ]
}
```




