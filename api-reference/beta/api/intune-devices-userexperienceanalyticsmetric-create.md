---
title: Criar userExperienceAnalyticsMetric
description: Criar um novo objeto userExperienceAnalyticsMetric.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb5e1af4c527f671a23c6e08dfd437ef9385d87c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311596"
---
# <a name="create-userexperienceanalyticsmetric"></a><span data-ttu-id="9634c-103">Criar userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="9634c-103">Create userExperienceAnalyticsMetric</span></span>

> <span data-ttu-id="9634c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9634c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9634c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9634c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9634c-106">Criar um novo objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="9634c-106">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9634c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9634c-107">Prerequisites</span></span>
<span data-ttu-id="9634c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9634c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9634c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9634c-110">Permission type</span></span>|<span data-ttu-id="9634c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9634c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9634c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9634c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9634c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9634c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9634c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9634c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9634c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9634c-115">Not supported.</span></span>|
|<span data-ttu-id="9634c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9634c-116">Application</span></span>|<span data-ttu-id="9634c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9634c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9634c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9634c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="9634c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9634c-119">Request headers</span></span>
|<span data-ttu-id="9634c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9634c-120">Header</span></span>|<span data-ttu-id="9634c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9634c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9634c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9634c-122">Authorization</span></span>|<span data-ttu-id="9634c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9634c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9634c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9634c-124">Accept</span></span>|<span data-ttu-id="9634c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9634c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9634c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9634c-126">Request body</span></span>
<span data-ttu-id="9634c-127">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="9634c-127">In the request body, supply a JSON representation for the userExperienceAnalyticsMetric object.</span></span>

<span data-ttu-id="9634c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="9634c-128">The following table shows the properties that are required when you create the userExperienceAnalyticsMetric.</span></span>

|<span data-ttu-id="9634c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9634c-129">Property</span></span>|<span data-ttu-id="9634c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9634c-130">Type</span></span>|<span data-ttu-id="9634c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9634c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9634c-132">id</span><span class="sxs-lookup"><span data-stu-id="9634c-132">id</span></span>|<span data-ttu-id="9634c-133">String</span><span class="sxs-lookup"><span data-stu-id="9634c-133">String</span></span>|<span data-ttu-id="9634c-134">O identificador exclusivo da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9634c-134">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="9634c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9634c-135">displayName</span></span>|<span data-ttu-id="9634c-136">String</span><span class="sxs-lookup"><span data-stu-id="9634c-136">String</span></span>|<span data-ttu-id="9634c-137">O nome da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9634c-137">The name of the user experience analytics metric.</span></span>|
|<span data-ttu-id="9634c-138">valor</span><span class="sxs-lookup"><span data-stu-id="9634c-138">value</span></span>|<span data-ttu-id="9634c-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="9634c-139">Double</span></span>|<span data-ttu-id="9634c-140">O valor da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9634c-140">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="9634c-141">unidade</span><span class="sxs-lookup"><span data-stu-id="9634c-141">unit</span></span>|<span data-ttu-id="9634c-142">String</span><span class="sxs-lookup"><span data-stu-id="9634c-142">String</span></span>|<span data-ttu-id="9634c-143">A unidade da métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9634c-143">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="9634c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9634c-144">Response</span></span>
<span data-ttu-id="9634c-145">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9634c-145">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9634c-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9634c-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="9634c-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9634c-147">Request</span></span>
<span data-ttu-id="9634c-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9634c-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
Content-type: application/json
Content-length: 187

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "displayName": "Display Name value",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="9634c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9634c-149">Response</span></span>
<span data-ttu-id="9634c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9634c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 236

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "displayName": "Display Name value",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```






