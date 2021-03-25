---
title: Criar userExperienceAnalyticsMetricHistory
description: Crie um novo objeto userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f5160db6d8a589eaef946e52675e2cb9d2d3e943
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159239"
---
# <a name="create-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="7f439-103">Criar userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="7f439-103">Create userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="7f439-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f439-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f439-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f439-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f439-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f439-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f439-107">Crie um novo [objeto userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="7f439-107">Create a new [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f439-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f439-108">Prerequisites</span></span>
<span data-ttu-id="7f439-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f439-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f439-111">Permission type</span></span>|<span data-ttu-id="7f439-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f439-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f439-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f439-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f439-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f439-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7f439-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f439-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f439-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f439-116">Not supported.</span></span>|
|<span data-ttu-id="7f439-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f439-117">Application</span></span>|<span data-ttu-id="7f439-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f439-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f439-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f439-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsMetricHistory
POST /deviceManagement/userExperienceAnalyticsDeviceMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="7f439-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f439-120">Request headers</span></span>
|<span data-ttu-id="7f439-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f439-121">Header</span></span>|<span data-ttu-id="7f439-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7f439-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f439-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f439-123">Authorization</span></span>|<span data-ttu-id="7f439-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f439-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f439-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f439-125">Accept</span></span>|<span data-ttu-id="7f439-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f439-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f439-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f439-127">Request body</span></span>
<span data-ttu-id="7f439-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="7f439-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetricHistory object.</span></span>

<span data-ttu-id="7f439-129">A tabela a seguir mostra as propriedades necessárias ao criar o userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="7f439-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetricHistory.</span></span>

|<span data-ttu-id="7f439-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f439-130">Property</span></span>|<span data-ttu-id="7f439-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f439-131">Type</span></span>|<span data-ttu-id="7f439-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f439-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f439-133">id</span><span class="sxs-lookup"><span data-stu-id="7f439-133">id</span></span>|<span data-ttu-id="7f439-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f439-134">String</span></span>|<span data-ttu-id="7f439-135">O identificador exclusivo do histórico métrico de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="7f439-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="7f439-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="7f439-136">deviceId</span></span>|<span data-ttu-id="7f439-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f439-137">String</span></span>|<span data-ttu-id="7f439-138">A ID do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="7f439-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="7f439-139">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="7f439-139">metricDateTime</span></span>|<span data-ttu-id="7f439-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f439-140">DateTimeOffset</span></span>|<span data-ttu-id="7f439-141">A data de data métrica da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="7f439-141">The user experience analytics metric date time.</span></span>|
|<span data-ttu-id="7f439-142">metricType</span><span class="sxs-lookup"><span data-stu-id="7f439-142">metricType</span></span>|<span data-ttu-id="7f439-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f439-143">String</span></span>|<span data-ttu-id="7f439-144">O tipo métrico de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="7f439-144">The user experience analytics metric type.</span></span>|



## <a name="response"></a><span data-ttu-id="7f439-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f439-145">Response</span></span>
<span data-ttu-id="7f439-146">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f439-146">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f439-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f439-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f439-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f439-148">Request</span></span>
<span data-ttu-id="7f439-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f439-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```

### <a name="response"></a><span data-ttu-id="7f439-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f439-150">Response</span></span>
<span data-ttu-id="7f439-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f439-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```




