---
title: função summarizeDeviceRegressionPerformance
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6cb9d9e5e7a5fbb80e89e50e0283587aa8d4f57e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944376"
---
# <a name="summarizedeviceregressionperformance-function"></a><span data-ttu-id="d27cd-103">função summarizeDeviceRegressionPerformance</span><span class="sxs-lookup"><span data-stu-id="d27cd-103">summarizeDeviceRegressionPerformance function</span></span>

> <span data-ttu-id="d27cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d27cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d27cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d27cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d27cd-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d27cd-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d27cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d27cd-107">Prerequisites</span></span>
<span data-ttu-id="d27cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d27cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d27cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d27cd-110">Permission type</span></span>|<span data-ttu-id="d27cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d27cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d27cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d27cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d27cd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d27cd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d27cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d27cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d27cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d27cd-115">Not supported.</span></span>|
|<span data-ttu-id="d27cd-116">Application</span><span class="sxs-lookup"><span data-stu-id="d27cd-116">Application</span></span>|<span data-ttu-id="d27cd-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d27cd-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d27cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d27cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="d27cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d27cd-119">Request headers</span></span>
|<span data-ttu-id="d27cd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d27cd-120">Header</span></span>|<span data-ttu-id="d27cd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d27cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d27cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d27cd-122">Authorization</span></span>|<span data-ttu-id="d27cd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d27cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d27cd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d27cd-124">Accept</span></span>|<span data-ttu-id="d27cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d27cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d27cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d27cd-126">Request body</span></span>
<span data-ttu-id="d27cd-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="d27cd-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d27cd-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="d27cd-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d27cd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d27cd-129">Property</span></span>|<span data-ttu-id="d27cd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d27cd-130">Type</span></span>|<span data-ttu-id="d27cd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d27cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d27cd-132">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="d27cd-132">summarizeBy</span></span>|[<span data-ttu-id="d27cd-133">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="d27cd-133">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="d27cd-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d27cd-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d27cd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d27cd-135">Response</span></span>
<span data-ttu-id="d27cd-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d27cd-136">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d27cd-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d27cd-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d27cd-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d27cd-138">Request</span></span>
<span data-ttu-id="d27cd-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d27cd-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d27cd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d27cd-140">Response</span></span>
<span data-ttu-id="d27cd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d27cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





