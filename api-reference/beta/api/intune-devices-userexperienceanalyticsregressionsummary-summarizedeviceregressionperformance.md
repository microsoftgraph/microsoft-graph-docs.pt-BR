---
title: função summarizeDeviceRegressionPerformance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3616cbf3e20a05f675159314a1085350942b6909
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233912"
---
# <a name="summarizedeviceregressionperformance-function"></a><span data-ttu-id="554c9-103">função summarizeDeviceRegressionPerformance</span><span class="sxs-lookup"><span data-stu-id="554c9-103">summarizeDeviceRegressionPerformance function</span></span>

<span data-ttu-id="554c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="554c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="554c9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="554c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="554c9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="554c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="554c9-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="554c9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="554c9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="554c9-108">Prerequisites</span></span>
<span data-ttu-id="554c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="554c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="554c9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="554c9-111">Permission type</span></span>|<span data-ttu-id="554c9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="554c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="554c9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="554c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="554c9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="554c9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="554c9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="554c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="554c9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="554c9-116">Not supported.</span></span>|
|<span data-ttu-id="554c9-117">Application</span><span class="sxs-lookup"><span data-stu-id="554c9-117">Application</span></span>|<span data-ttu-id="554c9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="554c9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="554c9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="554c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="554c9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="554c9-120">Request headers</span></span>
|<span data-ttu-id="554c9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="554c9-121">Header</span></span>|<span data-ttu-id="554c9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="554c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="554c9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="554c9-123">Authorization</span></span>|<span data-ttu-id="554c9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="554c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="554c9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="554c9-125">Accept</span></span>|<span data-ttu-id="554c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="554c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="554c9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="554c9-127">Request body</span></span>
<span data-ttu-id="554c9-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="554c9-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="554c9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="554c9-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="554c9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="554c9-130">Property</span></span>|<span data-ttu-id="554c9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="554c9-131">Type</span></span>|<span data-ttu-id="554c9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="554c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="554c9-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="554c9-133">summarizeBy</span></span>|[<span data-ttu-id="554c9-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="554c9-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="554c9-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="554c9-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="554c9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="554c9-136">Response</span></span>
<span data-ttu-id="554c9-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="554c9-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="554c9-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="554c9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="554c9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="554c9-139">Request</span></span>
<span data-ttu-id="554c9-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="554c9-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="554c9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="554c9-141">Response</span></span>
<span data-ttu-id="554c9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="554c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 154

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
    "id": "41683327-3327-4168-2733-684127336841"
  }
}
```




