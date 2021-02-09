---
title: Criar userExperienceAnalyticsMetricHistory
description: Crie um novo objeto userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 070c34b225ab49eb7625c313544a785d7cc3e518
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155052"
---
# <a name="create-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="e922b-103">Criar userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="e922b-103">Create userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="e922b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e922b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e922b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e922b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e922b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e922b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e922b-107">Crie um novo [objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="e922b-107">Create a new [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e922b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e922b-108">Prerequisites</span></span>
<span data-ttu-id="e922b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e922b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e922b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e922b-111">Permission type</span></span>|<span data-ttu-id="e922b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e922b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e922b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e922b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e922b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e922b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e922b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e922b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e922b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e922b-116">Not supported.</span></span>|
|<span data-ttu-id="e922b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e922b-117">Application</span></span>|<span data-ttu-id="e922b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e922b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e922b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e922b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="e922b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e922b-120">Request headers</span></span>
|<span data-ttu-id="e922b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e922b-121">Header</span></span>|<span data-ttu-id="e922b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e922b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e922b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e922b-123">Authorization</span></span>|<span data-ttu-id="e922b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e922b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e922b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e922b-125">Accept</span></span>|<span data-ttu-id="e922b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e922b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e922b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e922b-127">Request body</span></span>
<span data-ttu-id="e922b-128">No corpo da solicitação, fornece uma representação JSON do objeto userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="e922b-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetricHistory object.</span></span>

<span data-ttu-id="e922b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="e922b-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetricHistory.</span></span>

|<span data-ttu-id="e922b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e922b-130">Property</span></span>|<span data-ttu-id="e922b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e922b-131">Type</span></span>|<span data-ttu-id="e922b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e922b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e922b-133">id</span><span class="sxs-lookup"><span data-stu-id="e922b-133">id</span></span>|<span data-ttu-id="e922b-134">String</span><span class="sxs-lookup"><span data-stu-id="e922b-134">String</span></span>|<span data-ttu-id="e922b-135">O identificador exclusivo do histórico de métricas da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e922b-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="e922b-136">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="e922b-136">metricDateTime</span></span>|<span data-ttu-id="e922b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e922b-137">DateTimeOffset</span></span>|<span data-ttu-id="e922b-138">A data e a hora da métrica da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e922b-138">The user experience analytics metric date time.</span></span>|
|<span data-ttu-id="e922b-139">metricType</span><span class="sxs-lookup"><span data-stu-id="e922b-139">metricType</span></span>|<span data-ttu-id="e922b-140">String</span><span class="sxs-lookup"><span data-stu-id="e922b-140">String</span></span>|<span data-ttu-id="e922b-141">O tipo de métrica de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e922b-141">The user experience analytics metric type.</span></span>|



## <a name="response"></a><span data-ttu-id="e922b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e922b-142">Response</span></span>
<span data-ttu-id="e922b-143">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e922b-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e922b-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e922b-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e922b-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e922b-145">Request</span></span>
<span data-ttu-id="e922b-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e922b-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```

### <a name="response"></a><span data-ttu-id="e922b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e922b-147">Response</span></span>
<span data-ttu-id="e922b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e922b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```




