---
title: Criar userExperienceAnalyticsMetric
description: Criar um novo objeto userExperienceAnalyticsMetric.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be303d476524af2711937dd73d8f93d244e05d24
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188196"
---
# <a name="create-userexperienceanalyticsmetric"></a><span data-ttu-id="51e0f-103">Criar userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="51e0f-103">Create userExperienceAnalyticsMetric</span></span>

> <span data-ttu-id="51e0f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51e0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51e0f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51e0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51e0f-106">Criar um novo objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="51e0f-106">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51e0f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51e0f-107">Prerequisites</span></span>
<span data-ttu-id="51e0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51e0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51e0f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51e0f-110">Permission type</span></span>|<span data-ttu-id="51e0f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51e0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51e0f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51e0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51e0f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e0f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="51e0f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51e0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51e0f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51e0f-115">Not supported.</span></span>|
|<span data-ttu-id="51e0f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51e0f-116">Application</span></span>|<span data-ttu-id="51e0f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e0f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51e0f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51e0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="51e0f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51e0f-119">Request headers</span></span>
|<span data-ttu-id="51e0f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51e0f-120">Header</span></span>|<span data-ttu-id="51e0f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="51e0f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51e0f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="51e0f-122">Authorization</span></span>|<span data-ttu-id="51e0f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51e0f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51e0f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51e0f-124">Accept</span></span>|<span data-ttu-id="51e0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51e0f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51e0f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51e0f-126">Request body</span></span>
<span data-ttu-id="51e0f-127">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="51e0f-127">In the request body, supply a JSON representation for the userExperienceAnalyticsMetric object.</span></span>

<span data-ttu-id="51e0f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="51e0f-128">The following table shows the properties that are required when you create the userExperienceAnalyticsMetric.</span></span>

|<span data-ttu-id="51e0f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51e0f-129">Property</span></span>|<span data-ttu-id="51e0f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="51e0f-130">Type</span></span>|<span data-ttu-id="51e0f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e0f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e0f-132">id</span><span class="sxs-lookup"><span data-stu-id="51e0f-132">id</span></span>|<span data-ttu-id="51e0f-133">String</span><span class="sxs-lookup"><span data-stu-id="51e0f-133">String</span></span>|<span data-ttu-id="51e0f-134">O identificador exclusivo da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="51e0f-134">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="51e0f-135">valor</span><span class="sxs-lookup"><span data-stu-id="51e0f-135">value</span></span>|<span data-ttu-id="51e0f-136">Duplo</span><span class="sxs-lookup"><span data-stu-id="51e0f-136">Double</span></span>|<span data-ttu-id="51e0f-137">O valor da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="51e0f-137">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="51e0f-138">unidade</span><span class="sxs-lookup"><span data-stu-id="51e0f-138">unit</span></span>|<span data-ttu-id="51e0f-139">String</span><span class="sxs-lookup"><span data-stu-id="51e0f-139">String</span></span>|<span data-ttu-id="51e0f-140">A unidade da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="51e0f-140">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="51e0f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e0f-141">Response</span></span>
<span data-ttu-id="51e0f-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51e0f-142">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51e0f-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51e0f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="51e0f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51e0f-144">Request</span></span>
<span data-ttu-id="51e0f-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51e0f-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="51e0f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e0f-146">Response</span></span>
<span data-ttu-id="51e0f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51e0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




